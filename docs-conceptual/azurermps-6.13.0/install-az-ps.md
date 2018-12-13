---
title: Installieren des Az-Moduls von Azure PowerShell mit PowerShellGet
description: Anleitung für die Installation von Azure PowerShell mit PowerShellGet unter Windows, macOS und Linux
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/26/2018
ms.openlocfilehash: 3d52b18750341f220dc8e10d6bf89796457c5a10
ms.sourcegitcommit: 087c588169786c005a3c177624fb3ac6c8870125
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/13/2018
ms.locfileid: "53216996"
---
# <a name="install-the-azure-powershell-az-module"></a><span data-ttu-id="3028f-103">Installieren des Az-Moduls von Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="3028f-103">Install the Azure PowerShell 'Az' module</span></span>

<span data-ttu-id="3028f-104">In diesem Artikel erfahren Sie, wie Sie mithilfe von „PowerShellGet“ die Azure PowerShell-Module installieren.</span><span class="sxs-lookup"><span data-stu-id="3028f-104">This article tells you how to install the Azure PowerShell modules using PowerShellGet.</span></span> <span data-ttu-id="3028f-105">Diese Anweisungen können für Windows-, macOS- und Linux-Plattformen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="3028f-105">These instructions work on Windows, macOS, and Linux platforms.</span></span> <span data-ttu-id="3028f-106">Für die Vorschauversion von Az werden keine anderen Installationsmethoden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3028f-106">For the preview release of Az, no other install methods are supported.</span></span> 

## <a name="requirements"></a><span data-ttu-id="3028f-107">Requirements (Anforderungen)</span><span class="sxs-lookup"><span data-stu-id="3028f-107">Requirements</span></span>

<span data-ttu-id="3028f-108">Azure PowerShell kann mit PowerShell 5.x unter Windows und mit PowerShell 6.x auf einer beliebigen Plattform verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="3028f-108">Azure PowerShell works with either PowerShell 5.x on Windows, or PowerShell 6.x on any platform.</span></span> <span data-ttu-id="3028f-109">Führen Sie den folgenden Befehl aus, um die Version von PowerShell zu prüfen, die auf Ihrem Computer ausgeführt wird:</span><span class="sxs-lookup"><span data-stu-id="3028f-109">To check the version of PowerShell running on your machine, run the following command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="3028f-110">Falls Sie eine veraltete Version verwenden oder PowerShell installieren müssen, lesen Sie den Artikel [Installieren verschiedener Versionen von PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="3028f-110">If you have an outdated version or need to install PowerShell, see [Installing various versions of PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6).</span></span> <span data-ttu-id="3028f-111">Auf dieser Seite finden Sie einen Link zu den Installationsinformationen für Ihre Plattform.</span><span class="sxs-lookup"><span data-stu-id="3028f-111">Install information for your platform is linked from that page.</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="3028f-112">Installieren des Azure PowerShell-Moduls</span><span class="sxs-lookup"><span data-stu-id="3028f-112">Install the Azure PowerShell module</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="3028f-113">Die Module `AzureRM` und `Az` können gleichzeitig installiert sein.</span><span class="sxs-lookup"><span data-stu-id="3028f-113">You can have both the `AzureRM` and `Az` modules installed at the same time.</span></span> <span data-ttu-id="3028f-114">Wenn Sie beide Module installiert haben, __aktivieren Sie keine Aliase__.</span><span class="sxs-lookup"><span data-stu-id="3028f-114">If you have both modules installed, __don't enable aliases__.</span></span>
> <span data-ttu-id="3028f-115">Die Aktivierung von Aliasen verursacht Konflikte zwischen `AzureRM`-Cmdlets und `Az`-Befehlsaliasen und kann zu unerwartetem Verhalten führen.</span><span class="sxs-lookup"><span data-stu-id="3028f-115">Enabling aliases will cause conflicts between `AzureRM` cmdlets and `Az` command aliases, and could cause unexpected behavior.</span></span>
> <span data-ttu-id="3028f-116">Es wird empfohlen, vor der Installation des `Az`-Moduls `AzureRM` zu deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="3028f-116">It's recommended that before installing the `Az` module, you uninstall `AzureRM`.</span></span> <span data-ttu-id="3028f-117">Sie können jederzeit `AzureRM` deinstallieren bzw. Aliase aktivieren.</span><span class="sxs-lookup"><span data-stu-id="3028f-117">You can always uninstall `AzureRM` or enable aliases at any time.</span></span> <span data-ttu-id="3028f-118">Eine Anleitung zur Deinstallation finden Sie unter [Deinstallieren des Azure PowerShell-Moduls](uninstall-azurerm-ps.md) (AzureRM).</span><span class="sxs-lookup"><span data-stu-id="3028f-118">For uninstall instructions, see [Uninstall the Azure PowerShell module (AzureRM)](uninstall-azurerm-ps.md).</span></span> 

<span data-ttu-id="3028f-119">Für die globale Installation von Modulen benötigen Sie erhöhte Rechte, um Module aus dem PowerShell-Katalog installieren zu können.</span><span class="sxs-lookup"><span data-stu-id="3028f-119">To install modules at a global scope, you need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="3028f-120">Führen Sie zum Installieren von Azure PowerShell den folgenden Befehl in einer Sitzung mit erhöhten Rechten aus („Als Administrator ausführen“ unter Windows oder mit Superuser-Berechtigungen unter macOS/Linux):</span><span class="sxs-lookup"><span data-stu-id="3028f-120">To install Azure PowerShell, run the following command in an elevated session ("Run as Administrator" on Windows, or with superuser privileges on macOS or Linux):</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

<span data-ttu-id="3028f-121">Sollten Sie über keine Administratorrechte verfügen, können Sie die Installation für den aktuellen Benutzer durch Hinzufügen des Arguments `-Scope` ausführen.</span><span class="sxs-lookup"><span data-stu-id="3028f-121">If you don't have access to administrator privileges, you can install for the current user by adding the `-Scope` argument.</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

<span data-ttu-id="3028f-122">Standardmäßig ist der PowerShell-Katalog nicht als vertrauenswürdiges Repository für PowerShellGet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="3028f-122">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="3028f-123">Bei der ersten Verwendung des PowerShell-Katalogs wird die folgende Meldung angezeigt:</span><span class="sxs-lookup"><span data-stu-id="3028f-123">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="3028f-124">Antworten Sie mit `Yes` oder `Yes to All`, um die Installation fortzusetzen.</span><span class="sxs-lookup"><span data-stu-id="3028f-124">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="3028f-125">Das Modul `Az` ist ein Rollupmodul für die Azure PowerShell-Cmdlets.</span><span class="sxs-lookup"><span data-stu-id="3028f-125">The `Az` module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="3028f-126">Wenn Sie es installieren, werden alle verfügbaren Azure Resource Manager-Module heruntergeladen und die zugehörigen Cmdlets für die Nutzung zur Verfügung gestellt.</span><span class="sxs-lookup"><span data-stu-id="3028f-126">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="3028f-127">Anmelden</span><span class="sxs-lookup"><span data-stu-id="3028f-127">Sign in</span></span>

<span data-ttu-id="3028f-128">Melden Sie sich mit Ihren Azure-Anmeldeinformationen an, um Azure PowerShell zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="3028f-128">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> <span data-ttu-id="3028f-129">Wenn Sie das automatische Laden von Modulen deaktiviert haben, müssen Sie das Modul manuell mit `Import-Module Az` importieren.</span><span class="sxs-lookup"><span data-stu-id="3028f-129">If you've disabled module autoloading, you need to manually import the module with `Import-Module Az`.</span></span> <span data-ttu-id="3028f-130">Aufgrund der Modulstruktur kann dieser Vorgang einige Sekunden dauern.</span><span class="sxs-lookup"><span data-stu-id="3028f-130">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="3028f-131">Sie müssen diese Schritte für jede neue PowerShell-Sitzung wiederholen, die Sie starten.</span><span class="sxs-lookup"><span data-stu-id="3028f-131">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="3028f-132">Informationen zum sitzungsübergreifenden Speichern der Azure-Anmeldung in PowerShell finden Sie unter [Speichern von Benutzeranmeldeinformationen zwischen PowerShell-Sitzungen](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="3028f-132">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="3028f-133">Aktualisieren des Azure PowerShell-Moduls</span><span class="sxs-lookup"><span data-stu-id="3028f-133">Update the Azure PowerShell module</span></span>

<span data-ttu-id="3028f-134">Sie können Ihre Azure PowerShell-Installation aktualisieren, indem Sie [Update-Module](/powershell/module/powershellget/update-module) ausführen.</span><span class="sxs-lookup"><span data-stu-id="3028f-134">You can update your Azure PowerShell installation by running [Update-Module](/powershell/module/powershellget/update-module).</span></span> <span data-ttu-id="3028f-135">Mit diesem Befehl werden __keine__ früheren Versionen deinstalliert.</span><span class="sxs-lookup"><span data-stu-id="3028f-135">This command does __not__ uninstall earlier versions.</span></span>

```powershell-interactive
Update-Module -Name Az
```

<span data-ttu-id="3028f-136">Wenn Sie ältere Versionen von Azure PowerShell von Ihrem System entfernen möchten, helfen Ihnen die Informationen unter [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md) (Deinstallieren des Azure PowerShell-Moduls) weiter.</span><span class="sxs-lookup"><span data-stu-id="3028f-136">If you want to remove older versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="3028f-137">Verwenden von mehreren Versionen von Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="3028f-137">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="3028f-138">Es ist möglich, mehr als eine Version von Azure PowerShell zu installieren.</span><span class="sxs-lookup"><span data-stu-id="3028f-138">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="3028f-139">Verwenden Sie den folgenden Befehl zum Überprüfen, ob Sie mehrere Versionen von Azure PowerShell installiert haben:</span><span class="sxs-lookup"><span data-stu-id="3028f-139">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-Module -Name Az -List | select Name,Version
```

<span data-ttu-id="3028f-140">Anweisungen zum Entfernen einer Version von Azure PowerShell finden Sie unter [Deinstallieren des Azure PowerShell-Moduls](uninstall-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="3028f-140">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

<span data-ttu-id="3028f-141">Wenn Sie eine bestimmte Version des `Az`-Moduls laden möchten, verwenden Sie das Argument `-RequiredVersion` mit `Install-Module` und `Import-Module`:</span><span class="sxs-lookup"><span data-stu-id="3028f-141">You can load a specific version of the `Az` module by using the `-RequiredVersion` argument with `Install-Module` and `Import-Module`:</span></span>

```powershell-interactive
Install-Module -Name Az -RequiredVersion 0.4.0
Import-Module -Name Az -RequiredVersion 0.4.0
```

<span data-ttu-id="3028f-142">Sind mehrere Versionen des Moduls installiert, wird standardmäßig die neueste Version geladen.</span><span class="sxs-lookup"><span data-stu-id="3028f-142">If you have more than one version of the module installed, the latest version is loaded by default.</span></span>

## <a name="provide-feedback"></a><span data-ttu-id="3028f-143">Feedback geben</span><span class="sxs-lookup"><span data-stu-id="3028f-143">Provide feedback</span></span>

<span data-ttu-id="3028f-144">[Melden Sie auf GitHub ein Problem](https://github.com/Azure/azure-powershell/issues), wenn Sie bei der Nutzung von Azure PowerShell einen Fehler finden.</span><span class="sxs-lookup"><span data-stu-id="3028f-144">If you find a bug when using Azure Powershell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="3028f-145">Verwenden Sie das [Send-Feedback](/powershell/module/az.profile/send-feedback)-Cmdlet, um über die Befehlszeile Feedback zu senden.</span><span class="sxs-lookup"><span data-stu-id="3028f-145">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.profile/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3028f-146">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="3028f-146">Next Steps</span></span>

<span data-ttu-id="3028f-147">Weitere Informationen zum Modul und zu den zugehörigen Features als Einstieg in die Nutzung von Azure PowerShell finden Sie unter [Get started with Azure PowerShell](get-started-azureps.md) (Erste Schritte mit Azure PowerShell).</span><span class="sxs-lookup"><span data-stu-id="3028f-147">To get started using Azure PowerShell, see [Get Started with Azure PowerShell](get-started-azureps.md) to learn more about the module and its features.</span></span>
