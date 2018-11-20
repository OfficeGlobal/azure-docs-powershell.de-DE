---
title: Deinstallieren von Azure PowerShell
description: Anleitung zum vollständigen Deinstallieren von Azure PowerShell
ms.date: 09/11/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: bf1f81b4929ec066eeb888da4ba1303430f026b4
ms.sourcegitcommit: 4afdba3cd7e1d348876ce59f3503fdcd258f79ab
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/15/2018
ms.locfileid: "51574701"
---
# <a name="uninstall-the-azure-powershell-module"></a><span data-ttu-id="0e2a3-103">Deinstallieren des Azure PowerShell-Moduls</span><span class="sxs-lookup"><span data-stu-id="0e2a3-103">Uninstall the Azure PowerShell module</span></span>

<span data-ttu-id="0e2a3-104">In diesem Artikel erfahren Sie, wie Sie eine ältere Version von Azure PowerShell deinstallieren bzw. vollständig vom System entfernen.</span><span class="sxs-lookup"><span data-stu-id="0e2a3-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="0e2a3-105">Verwenden Sie das [Send-Feedback](/powershell/module/azurerm.profile/send-feedback)-Cmdlet, um uns Feedback zu senden, falls Sie Azure PowerShell vollständig deinstallieren möchten.</span><span class="sxs-lookup"><span data-stu-id="0e2a3-105">If you've decided to completely uninstall the Azure PowerShell, give us some feedback through the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>
<span data-ttu-id="0e2a3-106">Sollte ein Fehler auftreten, können Sie ein [GitHub-Problem melden](https://github.com/azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="0e2a3-106">If you encounter a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues).</span></span>

## <a name="uninstall-from-powershell"></a><span data-ttu-id="0e2a3-107">Deinstallieren über PowerShell</span><span class="sxs-lookup"><span data-stu-id="0e2a3-107">Uninstall from PowerShell</span></span>

<span data-ttu-id="0e2a3-108">Falls Sie Azure PowerShell mithilfe von PowerShellGet installiert haben, können Sie das Cmdlet [Uninstall-Module](/powershell/module/powershellget/uninstall-module) verwenden.</span><span class="sxs-lookup"><span data-stu-id="0e2a3-108">If you installed Azure PowerShell using PowerShellGet, you can use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="0e2a3-109">Mit `Uninstall-Module` wird jedoch nur ein Modul deinstalliert.</span><span class="sxs-lookup"><span data-stu-id="0e2a3-109">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="0e2a3-110">Wenn Sie Azure PowerShell vollständig entfernen möchten, müssen Sie die Module einzeln deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="0e2a3-110">To remove Azure PowerShell completely, you must uninstall each module individually.</span></span> <span data-ttu-id="0e2a3-111">Die Deinstallation kann kompliziert sein, wenn Sie mehrere Versionen von Azure PowerShell installiert haben.</span><span class="sxs-lookup"><span data-stu-id="0e2a3-111">Uninstallation can be complicated if you have more than one version of Azure PowerShell installed.</span></span>

<span data-ttu-id="0e2a3-112">Das folgende Skript fragt den PowerShell-Katalog ab, um eine Liste mit den abhängigen Submodulen abzurufen.</span><span class="sxs-lookup"><span data-stu-id="0e2a3-112">The following script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="0e2a3-113">Anschließend wird mit dem Skript die richtige Version der einzelnen Submodule deinstalliert.</span><span class="sxs-lookup"><span data-stu-id="0e2a3-113">Then, the script uninstalls the correct version of each submodule.</span></span>

```powershell-interactive
function Uninstall-AllModules {
  param(
    [Parameter(Mandatory=$true)]
    [string]$TargetModule,

    [Parameter(Mandatory=$true)]
    [string]$Version,

    [switch]$Force
  )

  $AllModules = @()

  'Creating list of dependencies...'
  $target = Find-Module $TargetModule -RequiredVersion $version
  $target.Dependencies | ForEach-Object {
    $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$_.minimumVersion}
  }
  $AllModules += New-Object -TypeName psobject -Property @{name=$TargetModule; version=$Version}

  foreach ($module in $AllModules) {
    Write-Host ('Uninstalling {0} version {1}' -f $module.name,$module.version)
    try {
      Uninstall-Module -Name $module.name -RequiredVersion $module.version -Force:$Force -ErrorAction Stop
    } catch {
      Write-Host ("`t" + $_.Exception.Message)
    }
  }
}
```

<span data-ttu-id="0e2a3-114">Kopieren Sie zum Verwenden dieser Funktion den Code, und fügen Sie ihn in Ihre PowerShell-Sitzung ein.</span><span class="sxs-lookup"><span data-stu-id="0e2a3-114">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="0e2a3-115">Das folgende Beispiel zeigt, wie Sie die Funktion ausführen, um eine ältere Version von Azure PowerShell zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="0e2a3-115">The following example shows how to run the function to remove an older version of Azure PowerShell.</span></span>

```powershell-interactive
Uninstall-AllModules -TargetModule AzureRM -Version 4.4.1 -Force
```

<span data-ttu-id="0e2a3-116">Bei der Ausführung des Skripts werden jeweils der Name und die Version des Submoduls angezeigt, das gerade deinstalliert wird.</span><span class="sxs-lookup"><span data-stu-id="0e2a3-116">As the script runs, it will display the name and version of each submodule that is being uninstalled.</span></span>

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

<span data-ttu-id="0e2a3-117">Führen Sie diesen Befehl für jede Azure PowerShell-Version aus, die Sie deinstallieren möchten.</span><span class="sxs-lookup"><span data-stu-id="0e2a3-117">Run this command for every version of Azure PowerShell that you want to uninstall.</span></span> <span data-ttu-id="0e2a3-118">Der Einfachheit halber deinstalliert das folgende Skript alle AzureRM-Versionen __mit Ausnahme__ der aktuellen Version.</span><span class="sxs-lookup"><span data-stu-id="0e2a3-118">For convenience, the following script will uninstall all versions of AzureRM __except__ for the latest.</span></span>

```powershell-interactive
$versions = (get-installedmodule AzureRM -AllVersions | Select-Object Version)
$versions[1..($versions.Length-1)]  | foreach { Uninstall-AllModules -TargetModule AzureRM -Version ($_.Version) -Force }
```

## <a name="uninstall-msi"></a><span data-ttu-id="0e2a3-119">Deinstallieren einer MSI</span><span class="sxs-lookup"><span data-stu-id="0e2a3-119">Uninstall MSI</span></span>

<span data-ttu-id="0e2a3-120">Falls Sie Azure PowerShell mithilfe des MSI-Pakets installiert haben, müssen Sie die Deinstallation nicht über PowerShell, sondern über das Windows-System ausführen.</span><span class="sxs-lookup"><span data-stu-id="0e2a3-120">If you installed Azure PowerShell using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

| <span data-ttu-id="0e2a3-121">Plattform</span><span class="sxs-lookup"><span data-stu-id="0e2a3-121">Platform</span></span> | <span data-ttu-id="0e2a3-122">Anleitung</span><span class="sxs-lookup"><span data-stu-id="0e2a3-122">Instructions</span></span> |
|----------|--------------|
| <span data-ttu-id="0e2a3-123">Windows 10</span><span class="sxs-lookup"><span data-stu-id="0e2a3-123">Windows 10</span></span> | <span data-ttu-id="0e2a3-124">Start > Einstellungen > Apps</span><span class="sxs-lookup"><span data-stu-id="0e2a3-124">Start > Settings > Apps</span></span> |
| <span data-ttu-id="0e2a3-125">Windows 7</span><span class="sxs-lookup"><span data-stu-id="0e2a3-125">Windows 7</span></span> </br><span data-ttu-id="0e2a3-126">Windows 8</span><span class="sxs-lookup"><span data-stu-id="0e2a3-126">Windows 8</span></span> | <span data-ttu-id="0e2a3-127">Start > Systemsteuerung > Programme > Programm deinstallieren</span><span class="sxs-lookup"><span data-stu-id="0e2a3-127">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="0e2a3-128">Auf diesem Bildschirm sollte „Azure PowerShell“ in der Programmliste aufgeführt sein. Sie können die Anwendung dort deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="0e2a3-128">Once on this screen you should see "Azure PowerShell" in the program listing, and can uninstall from there.</span></span>
