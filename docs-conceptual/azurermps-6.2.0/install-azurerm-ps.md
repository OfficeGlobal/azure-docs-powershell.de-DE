---
title: Installieren von Azure PowerShell mit PowerShellGet
description: Anleitung für die Installation von Azure PowerShell mit PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/31/2018
ms.openlocfilehash: 9b7046157e32a5c8473210e9840f9ae1b2f45902
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323100"
---
# <a name="install-azure-powershell-with-powershellget"></a><span data-ttu-id="445c0-103">Installieren von Azure PowerShell mit PowerShellGet</span><span class="sxs-lookup"><span data-stu-id="445c0-103">Install Azure PowerShell with PowerShellGet</span></span>

<span data-ttu-id="445c0-104">In diesem Artikel erfahren Sie, wie Sie die Azure PowerShell-Module in einer Windows-Umgebung unter Verwendung von PowerShellGet installieren.</span><span class="sxs-lookup"><span data-stu-id="445c0-104">This article explains the steps to install the Azure PowerShell modules in a Windows environment using PowerShellGet.</span></span>  <span data-ttu-id="445c0-105">Dies ist die bevorzugte Installationsmethode für Azure PowerShell. Sie können aber auch den Webplattform-Installer oder das MSI-Paket verwenden. Entsprechende Informationen finden Sie unter [Andere Installationsmethoden](other-install.md).</span><span class="sxs-lookup"><span data-stu-id="445c0-105">This is the preferred way to install Azure PowerShell, but if you would rather install with the Web Platform Installer or MSI package, see [Other installation methods](other-install.md).</span></span>

<span data-ttu-id="445c0-106">Wenn Sie Azure PowerShell unter macOS oder Linux verwenden möchten, lesen Sie den folgenden Artikel: [Installieren und Konfigurieren von Azure PowerShell unter macOS und Linux](install-azurermps-maclinux.md).</span><span class="sxs-lookup"><span data-stu-id="445c0-106">If you want to use Azure PowerShell on macOS or Linux, see the following article: [Install and configure Azure PowerShell on macOS and Linux](install-azurermps-maclinux.md).</span></span>

## <a name="system-requirements"></a><span data-ttu-id="445c0-107">Systemanforderungen</span><span class="sxs-lookup"><span data-stu-id="445c0-107">System requirements</span></span>

<span data-ttu-id="445c0-108">Für die Azure PowerShell-Version 6.1.0 wird mindestens die Version 5.0 von PowerShell benötigt.</span><span class="sxs-lookup"><span data-stu-id="445c0-108">Azure PowerShell version 6.1.0 requires version 5.0 (or higher) of PowerShell.</span></span> <span data-ttu-id="445c0-109">Informationen zum Upgraden auf PowerShell 5.0 finden Sie unter [Aktualisieren einer vorhandenen Windows PowerShell](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="445c0-109">For information on upgrading to PowerShell 5.0, see [Upgrading existing Windows PowerShell](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).</span></span>

<span data-ttu-id="445c0-110">PowerShellGet ist automatisch in PowerShell 5.0 enthalten.</span><span class="sxs-lookup"><span data-stu-id="445c0-110">PowerShellGet is automatically included as part of PowerShell 5.0.</span></span>

## <a name="install-or-update-the-azure-powershell-module"></a><span data-ttu-id="445c0-111">Installieren oder Aktualisieren des Azure PowerShell-Moduls</span><span class="sxs-lookup"><span data-stu-id="445c0-111">Install or update the Azure PowerShell module</span></span>

<span data-ttu-id="445c0-112">Für die Installation von Azure PowerShell aus dem PowerShell-Katalog sind erhöhte Rechte erforderlich.</span><span class="sxs-lookup"><span data-stu-id="445c0-112">Installing Azure PowerShell from the PowerShell Gallery requires elevated privileges.</span></span> <span data-ttu-id="445c0-113">Führen Sie den folgenden Befehl in einer PowerShell-Sitzung mit erhöhten Rechten aus:</span><span class="sxs-lookup"><span data-stu-id="445c0-113">Run the following command from an elevated PowerShell session:</span></span>

```powershell
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

> [!IMPORTANT]
> <span data-ttu-id="445c0-114">Mit diesem Befehl werden alle vorhandenen Installationen von Azure PowerShell in Ihrem System aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="445c0-114">This command will update any existing installation of Azure PowerShell on your system.</span></span> <span data-ttu-id="445c0-115">Sollten Sie mehrere installierte Versionen benötigen, sehen Sie sich die Antwort auf die häufig gestellte Frage [Kann ich mehrere Versionen von Azure PowerShell installieren?](#multiple-versions) an.</span><span class="sxs-lookup"><span data-stu-id="445c0-115">If you need to have more than one version installed, see the FAQ answer for [Can I install multiple versions of Azure PowerShell?](#multiple-versions)</span></span>

<span data-ttu-id="445c0-116">Standardmäßig ist der PowerShell-Katalog nicht als vertrauenswürdiges Repository für PowerShellGet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="445c0-116">By default, the PowerShell gallery is not configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="445c0-117">Bei der ersten Verwendung des PowerShell-Katalogs wird die folgende Meldung angezeigt:</span><span class="sxs-lookup"><span data-stu-id="445c0-117">The first time you use the PSGallery you see the following prompt:</span></span>

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="445c0-118">Antworten Sie mit „Ja“ oder „Ja zu allen“, um die Installation fortzusetzen.</span><span class="sxs-lookup"><span data-stu-id="445c0-118">Answer 'Yes' or 'Yes to All' to continue with the installation.</span></span>

> [!NOTE]
> <span data-ttu-id="445c0-119">Wenn Sie eine ältere NuGet-Version als 2.8.5.201 haben, werden Sie aufgefordert, die aktuelle NuGet-Version herunterzuladen und zu installieren.</span><span class="sxs-lookup"><span data-stu-id="445c0-119">If you have a version older than 2.8.5.201 of NuGet, you are prompted to download and install the latest version of NuGet.</span></span>

<span data-ttu-id="445c0-120">Das AzureRM-Modul ist ein Rollupmodul für die Azure Resource Manager-Cmdlets.</span><span class="sxs-lookup"><span data-stu-id="445c0-120">The AzureRM module is a rollup module for the Azure Resource Manager cmdlets.</span></span> <span data-ttu-id="445c0-121">Bei der Installation des AzureRM-Moduls werden alle noch nicht installierten Azure PowerShell-Module aus dem PowerShell-Katalog heruntergeladen.</span><span class="sxs-lookup"><span data-stu-id="445c0-121">When you install the AzureRM module, any Azure PowerShell module not previously installed is downloaded from the PowerShell Gallery.</span></span>

## <a name="load-the-azure-powershell-module"></a><span data-ttu-id="445c0-122">Laden des Azure PowerShell-Moduls</span><span class="sxs-lookup"><span data-stu-id="445c0-122">Load the Azure PowerShell module</span></span>

<span data-ttu-id="445c0-123">Nach der Installation des Moduls müssen Sie das Modul in der PowerShell-Sitzung laden.</span><span class="sxs-lookup"><span data-stu-id="445c0-123">Once the module is installed, you need to load the module into your PowerShell session.</span></span> <span data-ttu-id="445c0-124">Dies muss in einer normalen PowerShell-Sitzung (ohne erhöhte Rechte) erfolgen.</span><span class="sxs-lookup"><span data-stu-id="445c0-124">You should do this in a normal (non-elevated) PowerShell session.</span></span> <span data-ttu-id="445c0-125">Module werden wie folgt mit dem Cmdlet `Import-Module` geladen:</span><span class="sxs-lookup"><span data-stu-id="445c0-125">Modules are loaded using the `Import-Module` cmdlet, as follows:</span></span>

```powershell
Import-Module -Name AzureRM
```

## <a name="reporting-issues-and-feedback"></a><span data-ttu-id="445c0-126">Melden von Problemen und Bereitstellen von Feedback</span><span class="sxs-lookup"><span data-stu-id="445c0-126">Reporting issues and feedback</span></span>

<span data-ttu-id="445c0-127">Sollten bei Ihnen Probleme mit dem Tool auftreten, können Sie [hier](https://github.com/Azure/azure-powershell/issues) ein Problem auf GitHub melden.</span><span class="sxs-lookup"><span data-stu-id="445c0-127">If you encounter any bugs with the tool, please [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span> <span data-ttu-id="445c0-128">Zum Senden von Feedback zur Befehlszeile verwenden Sie das Cmdlet `Send-Feedback`.</span><span class="sxs-lookup"><span data-stu-id="445c0-128">To provide feedback from the command line, use the `Send-Feedback` cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="445c0-129">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="445c0-129">Next Steps</span></span>

<span data-ttu-id="445c0-130">Weitere Informationen zur Verwendung von Azure PowerShell finden Sie in den folgenden Artikeln:</span><span class="sxs-lookup"><span data-stu-id="445c0-130">For more information about using Azure PowerShell, see the following articles:</span></span>

* [<span data-ttu-id="445c0-131">Erste Schritte mit Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="445c0-131">Get started with Azure PowerShell</span></span>](get-started-azureps.md)

## <a name="frequently-asked-questions"></a><span data-ttu-id="445c0-132">Häufig gestellte Fragen</span><span class="sxs-lookup"><span data-stu-id="445c0-132">Frequently asked questions</span></span>

### <a id="helpmechoose"></a><span data-ttu-id="445c0-133">Wie überprüfe ich die Version von Azure PowerShell?</span><span class="sxs-lookup"><span data-stu-id="445c0-133">How do I check the version of Azure PowerShell?</span></span>

<span data-ttu-id="445c0-134">Obwohl empfohlen wird, möglichst bald ein Upgrade auf die neueste Version auszuführen, werden verschiedene Azure PowerShell-Versionen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="445c0-134">Although we encourage you to upgrade to the latest version as early as possible, several versions of Azure PowerShell are supported.</span></span> <span data-ttu-id="445c0-135">Führen Sie zum Ermitteln der installierten Azure PowerShell-Version `Get-Module AzureRM` in der Befehlszeile aus:</span><span class="sxs-lookup"><span data-stu-id="445c0-135">To determine the version of Azure PowerShell you have installed, run `Get-Module AzureRM` from your command line.</span></span>

```powershell
Get-Module AzureRM -ListAvailable | Select-Object -Property Name,Version,Path
```

### <a name="can-i-use-azure-powershell-for-azure-classic-deployments"></a><span data-ttu-id="445c0-136">Kann ich Azure PowerShell für klassische Azure-Bereitstellungen verwenden?</span><span class="sxs-lookup"><span data-stu-id="445c0-136">Can I use Azure PowerShell for Azure Classic deployments?</span></span>

<span data-ttu-id="445c0-137">Bei Bereitstellungen mit dem klassischen Bereitstellungsmodell können Sie die Dienstverwaltungsversion von Azure PowerShell installieren.</span><span class="sxs-lookup"><span data-stu-id="445c0-137">If you have deployments that use the classic deployment model you can install the Service Management version of Azure PowerShell.</span></span> <span data-ttu-id="445c0-138">Weitere Informationen finden Sie unter [Installing the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps) (Installieren des Azure PowerShell-Dienstverwaltungsmoduls).</span><span class="sxs-lookup"><span data-stu-id="445c0-138">For more information, see [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span> <span data-ttu-id="445c0-139">Das Azure- und das AzureRM-Modul nutzen gemeinsame Abhängigkeiten.</span><span class="sxs-lookup"><span data-stu-id="445c0-139">The Azure and AzureRM modules share common dependencies.</span></span> <span data-ttu-id="445c0-140">Wenn Sie sowohl die Azure- als auch die AzureRM-Module verwenden, müssen Sie die gleiche Version der einzelnen Pakete installieren.</span><span class="sxs-lookup"><span data-stu-id="445c0-140">If you use both the Azure and AzureRM modules, you should install the same version of each package.</span></span>

### <a name="a-namemultiple-versionscan-i-install-multiple-versions-of-azure-powershell"></a><span data-ttu-id="445c0-141"><a name="multiple-versions"/>Kann ich mehrere Versionen von Azure PowerShell installieren?</span><span class="sxs-lookup"><span data-stu-id="445c0-141"><a name="multiple-versions"/>Can I install multiple versions of Azure PowerShell?</span></span>

<span data-ttu-id="445c0-142">PowerShellGet ist die einzige Installationsmethode, die mehrere Versionen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="445c0-142">PowerShellGet the only method of installation that supports multiple versions.</span></span> <span data-ttu-id="445c0-143">Wenn Sie mehrere Versionen installieren möchten, können Sie dem Cmdlet `Install-Module` den Parameter `-RequiredVersion` hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="445c0-143">To install multiple versions, you can add the `-RequiredVersion` parameter to the `Install-Module` cmdlet.</span></span> <span data-ttu-id="445c0-144">Beispiel für die Installation der Versionen 6.1.0 und 1.2.9:</span><span class="sxs-lookup"><span data-stu-id="445c0-144">For example, to install both versions 6.1.0 and 1.2.9:</span></span>

```powershell
Install-Module -Name AzureRM -RequiredVersion 6.1.0
Install-Module -Name AzureRM -RequiredVersion 1.2.9
```

<span data-ttu-id="445c0-145">Nur eine Version des Moduls kann in einer PowerShell-Sitzung geladen werden.</span><span class="sxs-lookup"><span data-stu-id="445c0-145">Only one version of the module can be loaded in a PowerShell session.</span></span> <span data-ttu-id="445c0-146">Sie müssen ein neues PowerShell-Fenster öffnen und `Import-Module` verwenden, um eine bestimmte Version des Azure PowerShell-Moduls zu importieren.</span><span class="sxs-lookup"><span data-stu-id="445c0-146">You must open a new PowerShell window and use `Import-Module` to import a specific version of the Azure PowerShell module.</span></span>

```powershell
Import-Module -Name AzureRM -RequiredVersion 1.2.9
```

> [!NOTE]
> <span data-ttu-id="445c0-147">Version 2.1.0 und Version 1.2.6 sind die ersten Modulversionen, die parallel installiert und genutzt werden können.</span><span class="sxs-lookup"><span data-stu-id="445c0-147">Version 2.1.0 and version 1.2.6 are the first module versions designed to be installed and used side by side.</span></span> <span data-ttu-id="445c0-148">Beim Laden einer früheren Version von Azure PowerShell werden inkompatible Versionen des **AzureRM.Profile**-Moduls geladen.</span><span class="sxs-lookup"><span data-stu-id="445c0-148">When loading an earlier version of the Azure PowerShell, incompatible versions of the **AzureRM.Profile** module are loaded.</span></span> <span data-ttu-id="445c0-149">Dies führt dazu, dass Sie, immer wenn Sie ein Cmdlet ausführen, zum Anmelden aufgefordert werden.</span><span class="sxs-lookup"><span data-stu-id="445c0-149">This results in the cmdlets prompting you to log in whenever you execute a cmdlet.</span></span>
