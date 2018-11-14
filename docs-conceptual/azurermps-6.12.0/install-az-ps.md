---
title: Installieren von Azure PowerShell mit PowerShellGet
description: Anleitung für die Installation von Azure PowerShell mit PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/29/2018
ms.openlocfilehash: c4af07816aaa6713d67e3349a45880f8cc22c80a
ms.sourcegitcommit: ac4b53bb42a25aae013a9d8cd9ae98ada9397274
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/08/2018
ms.locfileid: "51276039"
---
# <a name="install-azure-powershell-with-powershellget"></a><span data-ttu-id="96eca-103">Installieren von Azure PowerShell mit PowerShellGet</span><span class="sxs-lookup"><span data-stu-id="96eca-103">Install Azure PowerShell with PowerShellGet</span></span>

<span data-ttu-id="96eca-104">In diesem Artikel erfahren Sie, wie Sie mithilfe von „PowerShellGet“ die Azure PowerShell-Module installieren.</span><span class="sxs-lookup"><span data-stu-id="96eca-104">This article tells you how to install the Azure PowerShell modules using PowerShellGet.</span></span> <span data-ttu-id="96eca-105">Für die Vorschauversion von Az werden keine anderen Installationsmethoden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="96eca-105">For the preview release of Az, no other install methods are supported.</span></span> 

## <a name="requirements"></a><span data-ttu-id="96eca-106">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="96eca-106">Requirements</span></span>

<span data-ttu-id="96eca-107">Azure PowerShell kann mit PowerShell 5.x unter Windows und mit PowerShell 6.x auf einer beliebigen Plattform verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="96eca-107">Azure PowerShell works with either PowerShell 5.x on Windows, or PowerShell 6.x on any platform.</span></span> <span data-ttu-id="96eca-108">Führen Sie den folgenden Befehl aus, um die Version von PowerShell zu prüfen, die auf Ihrem Computer ausgeführt wird:</span><span class="sxs-lookup"><span data-stu-id="96eca-108">To check the version of PowerShell running on your machine, run the following command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="96eca-109">Falls Sie eine veraltete Version verwenden oder PowerShell installieren müssen, lesen Sie den Artikel [Installieren verschiedener Versionen von PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="96eca-109">If you have an outdated version or need to install PowerShell, see [Installing various versions of PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6).</span></span> <span data-ttu-id="96eca-110">Auf dieser Seite finden Sie einen Link zu den Installationsinformationen für Ihre Plattform.</span><span class="sxs-lookup"><span data-stu-id="96eca-110">Install information for your platform is linked from that page.</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="96eca-111">Installieren des Azure PowerShell-Moduls</span><span class="sxs-lookup"><span data-stu-id="96eca-111">Install the Azure PowerShell module</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="96eca-112">Die Module `AzureRM` und `Az` dürfen nicht gleichzeitig auf einem System installiert sein.</span><span class="sxs-lookup"><span data-stu-id="96eca-112">You shouldn't have both the `AzureRM` and `Az` modules installed on a system at the same time.</span></span> <span data-ttu-id="96eca-113">Um das Modul `Az` installieren zu können, muss `AzureRM` deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="96eca-113">In order to install the `Az` module, `AzureRM` must be uninstalled.</span></span> <span data-ttu-id="96eca-114">Eine entsprechende Anleitung finden Sie unter [Deinstallieren des Azure PowerShell-Moduls](uninstall-azurerm-ps.md) (AzureRM).</span><span class="sxs-lookup"><span data-stu-id="96eca-114">For instructions on how to do that, see [Uninstall the Azure PowerShell module (AzureRM)](uninstall-azurerm-ps.md).</span></span>

<span data-ttu-id="96eca-115">Für die globale Installation von Modulen benötigen Sie erhöhte Rechte, um Module aus dem PowerShell-Katalog installieren zu können.</span><span class="sxs-lookup"><span data-stu-id="96eca-115">To install modules at a global scope, you need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="96eca-116">Führen Sie zum Installieren von Azure PowerShell den folgenden Befehl in einer Sitzung mit erhöhten Rechten aus („Als Administrator ausführen“ unter Windows oder mit Superuser-Berechtigungen unter macOS/Linux):</span><span class="sxs-lookup"><span data-stu-id="96eca-116">To install Azure PowerShell, run the following command in an elevated session ("Run as Administrator" on Windows, or with superuser privileges on macOS or Linux):</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

<span data-ttu-id="96eca-117">Sollten Sie über keine Administratorrechte verfügen, können Sie die Installation für den aktuellen Benutzer durch Hinzufügen des Arguments `-Scope` ausführen.</span><span class="sxs-lookup"><span data-stu-id="96eca-117">If you don't have access to administrator privileges, you can install for the current user by adding the `-Scope` argument.</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

<span data-ttu-id="96eca-118">Standardmäßig ist der PowerShell-Katalog nicht als vertrauenswürdiges Repository für PowerShellGet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="96eca-118">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="96eca-119">Bei der ersten Verwendung des PowerShell-Katalogs wird die folgende Meldung angezeigt:</span><span class="sxs-lookup"><span data-stu-id="96eca-119">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="96eca-120">Antworten Sie mit `Yes` oder `Yes to All`, um die Installation fortzusetzen.</span><span class="sxs-lookup"><span data-stu-id="96eca-120">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="96eca-121">Das Modul `Az` ist ein Rollupmodul für die Azure PowerShell-Cmdlets.</span><span class="sxs-lookup"><span data-stu-id="96eca-121">The `Az` module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="96eca-122">Wenn Sie es installieren, werden alle verfügbaren Azure Resource Manager-Module heruntergeladen und die zugehörigen Cmdlets für die Nutzung zur Verfügung gestellt.</span><span class="sxs-lookup"><span data-stu-id="96eca-122">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="96eca-123">Anmelden</span><span class="sxs-lookup"><span data-stu-id="96eca-123">Sign in</span></span>

<span data-ttu-id="96eca-124">Damit Sie Azure PowerShell verwenden können, müssen Sie `Az` mit dem [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module)-Cmdlet in Ihre aktuelle PowerShell-Sitzung laden und sich dann mit Ihren Azure-Anmeldeinformationen anmelden.</span><span class="sxs-lookup"><span data-stu-id="96eca-124">To start working with Azure PowerShell, you need to load `Az` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell-interactive
# Import the module into the PowerShell session
Import-Module Az
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

<span data-ttu-id="96eca-125">Sie müssen diese Schritte für jede neue PowerShell-Sitzung wiederholen, die Sie starten.</span><span class="sxs-lookup"><span data-stu-id="96eca-125">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="96eca-126">Für den automatischen Import des Moduls `Az` muss ein PowerShell-Profil eingerichtet werden. Informationen hierzu finden Sie unter [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles) (Informationen zu Profilen).</span><span class="sxs-lookup"><span data-stu-id="96eca-126">Automatically importing the `Az` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="96eca-127">Informationen zum sitzungsübergreifenden Speichern der Azure-Anmeldung finden Sie unter [Persisting user credentials across PowerShell sessions](context-persistence.md) (Speichern von Benutzeranmeldeinformationen zwischen PowerShell-Sitzungen).</span><span class="sxs-lookup"><span data-stu-id="96eca-127">To learn how to persist your Azure sign-in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="96eca-128">Aktualisieren des Azure PowerShell-Moduls</span><span class="sxs-lookup"><span data-stu-id="96eca-128">Update the Azure PowerShell module</span></span>

<span data-ttu-id="96eca-129">Sie können Ihre Azure PowerShell-Installation aktualisieren, indem Sie [Update-Module](/powershell/module/powershellget/update-module) ausführen.</span><span class="sxs-lookup"><span data-stu-id="96eca-129">You can update your Azure PowerShell installation by running [Update-Module](/powershell/module/powershellget/update-module).</span></span> <span data-ttu-id="96eca-130">Mit diesem Befehl werden __keine__ früheren Versionen deinstalliert.</span><span class="sxs-lookup"><span data-stu-id="96eca-130">This command does __not__ uninstall earlier versions.</span></span>

```powershell-interactive
Update-Module -Name Az
```

<span data-ttu-id="96eca-131">Wenn Sie ältere Versionen von Azure PowerShell von Ihrem System entfernen möchten, helfen Ihnen die Informationen unter [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md) (Deinstallieren des Azure PowerShell-Moduls) weiter.</span><span class="sxs-lookup"><span data-stu-id="96eca-131">If you want to remove older versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="96eca-132">Verwenden von mehreren Versionen von Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="96eca-132">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="96eca-133">Es ist möglich, mehr als eine Version von Azure PowerShell zu installieren.</span><span class="sxs-lookup"><span data-stu-id="96eca-133">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="96eca-134">Verwenden Sie den folgenden Befehl zum Überprüfen, ob Sie mehrere Versionen von Azure PowerShell installiert haben:</span><span class="sxs-lookup"><span data-stu-id="96eca-134">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-Module -Name Az -List | select Name,Version
```

<span data-ttu-id="96eca-135">Anweisungen zum Entfernen einer Version von Azure PowerShell finden Sie unter [Deinstallieren des Azure PowerShell-Moduls](uninstall-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="96eca-135">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

<span data-ttu-id="96eca-136">Wenn Sie eine bestimmte Version des `Az`-Moduls laden möchten, verwenden Sie das Argument `-RequiredVersion` mit `Install-Module` oder `Import-Module`:</span><span class="sxs-lookup"><span data-stu-id="96eca-136">You can load a specific version of the `Az` module by using the `-RequiredVersion` argument with `Install-Module` or `Import-Module`:</span></span>

```powershell-interactive
Install-Module -Name Az -RequiredVersion 0.4.0
Import-Module -Name Az -RequiredVersion 0.4.0
```

<span data-ttu-id="96eca-137">Sind mehrere Versionen des Moduls installiert, wird beim Importieren standardmäßig die neueste Version geladen.</span><span class="sxs-lookup"><span data-stu-id="96eca-137">If you have more than one version of the module installed, the latest version is loaded by default when importing.</span></span>

## <a name="provide-feedback"></a><span data-ttu-id="96eca-138">Feedback geben</span><span class="sxs-lookup"><span data-stu-id="96eca-138">Provide feedback</span></span>

<span data-ttu-id="96eca-139">[Melden Sie auf GitHub ein Problem](https://github.com/Azure/azure-powershell/issues), wenn Sie bei der Nutzung von Azure PowerShell einen Fehler finden.</span><span class="sxs-lookup"><span data-stu-id="96eca-139">If you find a bug when using Azure Powershell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="96eca-140">Verwenden Sie das [Send-Feedback](/powershell/module/az.profile/send-feedback)-Cmdlet, um über die Befehlszeile Feedback zu senden.</span><span class="sxs-lookup"><span data-stu-id="96eca-140">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.profile/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="96eca-141">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="96eca-141">Next Steps</span></span>

<span data-ttu-id="96eca-142">Weitere Informationen zum Modul und zu den zugehörigen Features als Einstieg in die Nutzung von Azure PowerShell finden Sie unter [Get started with Azure PowerShell](get-started-azureps.md) (Erste Schritte mit Azure PowerShell).</span><span class="sxs-lookup"><span data-stu-id="96eca-142">To get started using Azure PowerShell, see [Get Started with Azure PowerShell](get-started-azureps.md) to learn more about the module and its features.</span></span>