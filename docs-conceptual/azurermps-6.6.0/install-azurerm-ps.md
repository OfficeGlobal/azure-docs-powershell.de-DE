---
title: Installieren von Azure PowerShell unter Windows mit PowerShellGet
description: Anleitung für die Installation von Azure PowerShell mit PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/15/2018
ms.openlocfilehash: 50b05e5f25b6e3e1c815f6b26f1b53b84cd0b7da
ms.sourcegitcommit: afae9f2f091b21ed07d5aec1c249cf859a8b89a4
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/09/2018
ms.locfileid: "39653558"
---
# <a name="install-azure-powershell-on-windows-with-powershellget"></a><span data-ttu-id="fc1e9-103">Installieren von Azure PowerShell unter Windows mit PowerShellGet</span><span class="sxs-lookup"><span data-stu-id="fc1e9-103">Install Azure PowerShell on Windows with PowerShellGet</span></span>

<span data-ttu-id="fc1e9-104">In diesem Artikel erfahren Sie, wie Sie die Azure PowerShell-Module in einer Windows-Umgebung unter Verwendung von PowerShellGet installieren.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-104">This article explains the steps to install the Azure PowerShell modules in a Windows environment using PowerShellGet.</span></span> <span data-ttu-id="fc1e9-105">PowerShellGet und die Modulverwaltung stellen die bevorzugte Installationsmethode für Azure PowerShell dar. Sie können aber auch den Webplattform-Installer oder das MSI-Paket verwenden. Entsprechende Informationen finden Sie unter [Andere Installationsmethoden](other-install.md).</span><span class="sxs-lookup"><span data-stu-id="fc1e9-105">PowerShellGet and module management is the preferred way to install Azure PowerShell but if you would rather install with the Web Platform Installer or MSI package, see [Other installation methods](other-install.md).</span></span>

<span data-ttu-id="fc1e9-106">Eine Anleitung zum Installieren von Azure PowerShell auf anderen Plattformen finden Sie unter [Installieren und Konfigurieren von Azure PowerShell unter macOS und Linux](install-azurermps-maclinux.md).</span><span class="sxs-lookup"><span data-stu-id="fc1e9-106">For instructions to install Azure PowerShell on other platforms, see [Install and configure Azure PowerShell on macOS and Linux](install-azurermps-maclinux.md).</span></span>

<span data-ttu-id="fc1e9-107">Das klassische Azure-Bereitstellungsmodell wird von dieser Version von Azure PowerShell nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-107">The Azure classic deployment model is not supported by this version of Azure PowerShell.</span></span> <span data-ttu-id="fc1e9-108">Befolgen Sie die Anleitung unter [Installieren des Azure PowerShell-Dienstverwaltungsmoduls](/powershell/azure/servicemanagement/install-azure-ps), um Unterstützung zu klassischen Bereitstellungen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-108">For support for classic deployments, follow the instructions in [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span>

## <a name="requirements"></a><span data-ttu-id="fc1e9-109">Requirements (Anforderungen)</span><span class="sxs-lookup"><span data-stu-id="fc1e9-109">Requirements</span></span>

<span data-ttu-id="fc1e9-110">Ab Version 6.0 erfordert Azure PowerShell die PowerShell-Version 5.0.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-110">Starting with Azure PowerShell version 6.0, Azure PowerShell requires PowerShell version 5.0.</span></span> <span data-ttu-id="fc1e9-111">Führen Sie den folgenden Befehl aus, um die Version von PowerShell zu prüfen, die auf Ihrem Computer ausgeführt wird:</span><span class="sxs-lookup"><span data-stu-id="fc1e9-111">To check the version of PowerShell running on your machine, run the following command:</span></span>

```powershell
$PSVersionTable.PSVersion
```

<span data-ttu-id="fc1e9-112">Falls Sie über eine veraltete Version verfügen, helfen Ihnen die Informationen unter [Aktualisieren einer vorhandenen Windows PowerShell](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell) weiter.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-112">If you have an outdated version, see [Upgrading existing Windows PowerShell](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="fc1e9-113">Das in diesem Dokument beschriebene Modul „AzureRM“ verwendet .NET Framework.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-113">The module described in this document, AzureRM, uses .NET Framework.</span></span> <span data-ttu-id="fc1e9-114">Dadurch ist es nicht mit PowerShell 6.0 kompatibel, das .NET Core verwendet.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-114">This makes it incompatible with PowerShell 6.0, which uses .NET Core.</span></span> <span data-ttu-id="fc1e9-115">Wenn Sie PowerShell 6.0 verwenden, befolgen Sie die [Installationsanweisungen für macOS und Linux](install-azurermps-maclinux.md).</span><span class="sxs-lookup"><span data-stu-id="fc1e9-115">If you are using PowerShell 6.0, follow the [installation instructions for macOS and Linux](install-azurermps-maclinux.md).</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="fc1e9-116">Installieren des Azure PowerShell-Moduls</span><span class="sxs-lookup"><span data-stu-id="fc1e9-116">Install the Azure PowerShell module</span></span>

<span data-ttu-id="fc1e9-117">Sie benötigen erhöhte Rechte, um Module aus dem PowerShell-Katalog installieren zu können.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-117">You need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="fc1e9-118">Führen Sie den folgenden Befehl in einer Sitzung mit erhöhten Rechten aus, um Azure PowerShell zu installieren:</span><span class="sxs-lookup"><span data-stu-id="fc1e9-118">To install Azure PowerShell, run the following command in an elevated session:</span></span>

```powershell
Install-Module -Name AzureRM
```

> [!NOTE]
> <span data-ttu-id="fc1e9-119">Wenn Sie eine ältere NuGet-Version als 2.8.5.201 haben, werden Sie aufgefordert, die aktuelle NuGet-Version herunterzuladen und zu installieren.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-119">If you have a version older than 2.8.5.201 of NuGet, you are prompted to download and install the latest version of NuGet.</span></span>

<span data-ttu-id="fc1e9-120">Standardmäßig ist der PowerShell-Katalog nicht als vertrauenswürdiges Repository für PowerShellGet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-120">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="fc1e9-121">Bei der ersten Verwendung des PowerShell-Katalogs wird die folgende Meldung angezeigt:</span><span class="sxs-lookup"><span data-stu-id="fc1e9-121">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="fc1e9-122">Antworten Sie mit `Yes` oder `Yes to All`, um die Installation fortzusetzen.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-122">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="fc1e9-123">Das Modul `AzureRM` ist ein Rollupmodul für die Azure PowerShell-Cmdlets.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-123">The `AzureRM` module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="fc1e9-124">Wenn Sie es installieren, werden alle verfügbaren Azure Resource Manager-Module heruntergeladen und die zugehörigen Cmdlets für die Nutzung zur Verfügung gestellt.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-124">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="fc1e9-125">Anmelden</span><span class="sxs-lookup"><span data-stu-id="fc1e9-125">Sign in</span></span>

<span data-ttu-id="fc1e9-126">Damit Sie Azure PowerShell verwenden können, müssen Sie `AzureRM` mit dem [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module)-Cmdlet in Ihre aktuelle PowerShell-Sitzung laden und sich dann mit Ihren Azure-Anmeldeinformationen anmelden.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-126">To start working with Azure PowerShell, you need to load `AzureRM` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="fc1e9-127">Sie müssen diese Schritte für jede neue PowerShell-Sitzung wiederholen, die Sie starten.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-127">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="fc1e9-128">Für den automatischen Import des Moduls `AzureRM` muss ein PowerShell-Profil eingerichtet werden. Informationen hierzu finden Sie unter [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles) (Informationen zu Profilen).</span><span class="sxs-lookup"><span data-stu-id="fc1e9-128">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="fc1e9-129">Informationen zum sitzungsübergreifenden Speichern der Azure-Anmeldung finden Sie unter [Persisting user credentials across PowerShell sessions](context-persistence.md) (Speichern von Benutzeranmeldeinformationen zwischen PowerShell-Sitzungen).</span><span class="sxs-lookup"><span data-stu-id="fc1e9-129">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="fc1e9-130">Aktualisieren des Azure PowerShell-Moduls</span><span class="sxs-lookup"><span data-stu-id="fc1e9-130">Update the Azure PowerShell module</span></span>

<span data-ttu-id="fc1e9-131">Sie können Ihre Azure PowerShell-Installation aktualisieren, indem Sie [Update-Module](/powershell/module/powershellget/update-module) ausführen.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-131">You can update your Azure PowerShell installation by running [Update-Module](/powershell/module/powershellget/update-module).</span></span> <span data-ttu-id="fc1e9-132">Mit diesem Befehl werden __keine__ früheren Versionen deinstalliert.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-132">This command does __not__ uninstall earlier versions.</span></span>

```powershell
Update-Module -Name AzureRM
```

<span data-ttu-id="fc1e9-133">Wenn Sie ältere Versionen von Azure PowerShell von Ihrem System entfernen möchten, helfen Ihnen die Informationen unter [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md) (Deinstallieren des Azure PowerShell-Moduls) weiter.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-133">If you want to remove older versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="fc1e9-134">Verwenden von mehreren Versionen von Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="fc1e9-134">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="fc1e9-135">Es ist möglich, mehrere Versionen von Azure PowerShell zu installieren.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-135">It's possible to install multiple versions of Azure PowerShell.</span></span> <span data-ttu-id="fc1e9-136">Unter Umständen benötigen Sie mehr als eine Version, wenn Sie mit lokalen Azure Stack-Ressourcen arbeiten, eine ältere Version von Windows ausführen, die nicht auf PowerShell 5.0 aktualisiert werden kann, oder das klassische Azure-Bereitstellungsmodell nutzen.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-136">You might need more than one version if you work with on-premises Azure Stack resources, run an older version of Windows that you can't update to PowerShell 5.0, or use the Azure classic deployment model.</span></span> <span data-ttu-id="fc1e9-137">Geben Sie beim Installieren das Argument `-RequiredVersion` an, um eine ältere Version zu installieren.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-137">To install an older version, provide the `-RequiredVersion` argument when installing.</span></span>

```powershell
# Install version 1.2.9 of Azure PowerShell
Install-Module -Name AzureRM -RequiredVersion 1.2.9
```

<span data-ttu-id="fc1e9-138">Beim Laden des Azure PowerShell-Moduls wird standardmäßig die aktuelle Version geladen.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-138">When loading the Azure PowerShell module the latest version is loaded by default.</span></span> <span data-ttu-id="fc1e9-139">Geben Sie das Argument `-RequiredVersion` an, um eine andere Version zu laden.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-139">To load a different version, provide the `-RequiredVersion` argument.</span></span>

```powershell
# Load version 1.2.9 of Azure PowerShell
Import-Module -Name AzureRM -RequiredVersion 1.2.9
```

## <a name="provide-feedback"></a><span data-ttu-id="fc1e9-140">Feedback geben</span><span class="sxs-lookup"><span data-stu-id="fc1e9-140">Provide feedback</span></span>

<span data-ttu-id="fc1e9-141">Bitte [melden Sie auf GitHub ein Problem](https://github.com/Azure/azure-powershell/issues), wenn Sie bei der Nutzung von Azure PowerShell einen Fehler finden.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-141">If you find a bug when using Azure Powershell, please [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="fc1e9-142">Verwenden Sie das [Send-Feedback](/powershell/module/azurerm.profile/send-feedback)-Cmdlet, um über die Befehlszeile Feedback zu senden.</span><span class="sxs-lookup"><span data-stu-id="fc1e9-142">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="fc1e9-143">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="fc1e9-143">Next Steps</span></span>

<span data-ttu-id="fc1e9-144">Weitere Informationen zum Modul und zu den zugehörigen Features als Einstieg in die Nutzung von Azure PowerShell finden Sie unter [Get started with Azure PowerShell](get-started-azureps.md) (Erste Schritte mit Azure PowerShell).</span><span class="sxs-lookup"><span data-stu-id="fc1e9-144">To get started using Azure PowerShell, see [Get Started with Azure PowerShell](get-started-azureps.md) to learn more about the module and its features.</span></span>