---
title: Installieren des Az-Moduls von Azure PowerShell mit PowerShellGet
description: Anleitung für die Installation von Azure PowerShell mit PowerShellGet unter Windows, macOS und Linux
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/16/2018
ms.openlocfilehash: 32e96c6459c9db0c4b9eda0cc170c85ba99a22ca
ms.sourcegitcommit: 80a3da199954d0ab78765715fb49793e89a30f12
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2018
ms.locfileid: "52259793"
---
# <a name="install-the-azure-powershell-az-module"></a><span data-ttu-id="e6b2f-103">Installieren des Az-Moduls von Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="e6b2f-103">Install the Azure PowerShell 'Az' module</span></span>

<span data-ttu-id="e6b2f-104">In diesem Artikel erfahren Sie, wie Sie mithilfe von „PowerShellGet“ die Azure PowerShell-Module installieren.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-104">This article tells you how to install the Azure PowerShell modules using PowerShellGet.</span></span> <span data-ttu-id="e6b2f-105">Diese Anweisungen können für Windows-, macOS- und Linux-Plattformen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-105">These instructions work on Windows, macOS, and Linux platforms.</span></span> <span data-ttu-id="e6b2f-106">Für die Vorschauversion von Az werden keine anderen Installationsmethoden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-106">For the preview release of Az, no other install methods are supported.</span></span> 

## <a name="requirements"></a><span data-ttu-id="e6b2f-107">Requirements (Anforderungen)</span><span class="sxs-lookup"><span data-stu-id="e6b2f-107">Requirements</span></span>

<span data-ttu-id="e6b2f-108">Azure PowerShell kann mit PowerShell 5.x unter Windows und mit PowerShell 6.x auf einer beliebigen Plattform verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-108">Azure PowerShell works with either PowerShell 5.x on Windows, or PowerShell 6.x on any platform.</span></span> <span data-ttu-id="e6b2f-109">Führen Sie den folgenden Befehl aus, um die Version von PowerShell zu prüfen, die auf Ihrem Computer ausgeführt wird:</span><span class="sxs-lookup"><span data-stu-id="e6b2f-109">To check the version of PowerShell running on your machine, run the following command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="e6b2f-110">Falls Sie eine veraltete Version verwenden oder PowerShell installieren müssen, lesen Sie den Artikel [Installieren verschiedener Versionen von PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="e6b2f-110">If you have an outdated version or need to install PowerShell, see [Installing various versions of PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6).</span></span> <span data-ttu-id="e6b2f-111">Auf dieser Seite finden Sie einen Link zu den Installationsinformationen für Ihre Plattform.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-111">Install information for your platform is linked from that page.</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="e6b2f-112">Installieren des Azure PowerShell-Moduls</span><span class="sxs-lookup"><span data-stu-id="e6b2f-112">Install the Azure PowerShell module</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="e6b2f-113">Die Module `AzureRM` und `Az` dürfen nicht gleichzeitig auf einem System installiert sein.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-113">You shouldn't have both the `AzureRM` and `Az` modules installed on a system at the same time.</span></span> <span data-ttu-id="e6b2f-114">Um das Modul `Az` installieren zu können, muss `AzureRM` deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-114">In order to install the `Az` module, `AzureRM` must be uninstalled.</span></span> <span data-ttu-id="e6b2f-115">Eine entsprechende Anleitung finden Sie unter [Deinstallieren des Azure PowerShell-Moduls](uninstall-azurerm-ps.md) (AzureRM).</span><span class="sxs-lookup"><span data-stu-id="e6b2f-115">For instructions on how to do that, see [Uninstall the Azure PowerShell module (AzureRM)](uninstall-azurerm-ps.md).</span></span>

<span data-ttu-id="e6b2f-116">Für die globale Installation von Modulen benötigen Sie erhöhte Rechte, um Module aus dem PowerShell-Katalog installieren zu können.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-116">To install modules at a global scope, you need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="e6b2f-117">Führen Sie zum Installieren von Azure PowerShell den folgenden Befehl in einer Sitzung mit erhöhten Rechten aus („Als Administrator ausführen“ unter Windows oder mit Superuser-Berechtigungen unter macOS/Linux):</span><span class="sxs-lookup"><span data-stu-id="e6b2f-117">To install Azure PowerShell, run the following command in an elevated session ("Run as Administrator" on Windows, or with superuser privileges on macOS or Linux):</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

<span data-ttu-id="e6b2f-118">Sollten Sie über keine Administratorrechte verfügen, können Sie die Installation für den aktuellen Benutzer durch Hinzufügen des Arguments `-Scope` ausführen.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-118">If you don't have access to administrator privileges, you can install for the current user by adding the `-Scope` argument.</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

<span data-ttu-id="e6b2f-119">Standardmäßig ist der PowerShell-Katalog nicht als vertrauenswürdiges Repository für PowerShellGet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-119">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="e6b2f-120">Bei der ersten Verwendung des PowerShell-Katalogs wird die folgende Meldung angezeigt:</span><span class="sxs-lookup"><span data-stu-id="e6b2f-120">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="e6b2f-121">Antworten Sie mit `Yes` oder `Yes to All`, um die Installation fortzusetzen.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-121">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="e6b2f-122">Das Modul `Az` ist ein Rollupmodul für die Azure PowerShell-Cmdlets.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-122">The `Az` module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="e6b2f-123">Wenn Sie es installieren, werden alle verfügbaren Azure Resource Manager-Module heruntergeladen und die zugehörigen Cmdlets für die Nutzung zur Verfügung gestellt.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-123">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="e6b2f-124">Anmelden</span><span class="sxs-lookup"><span data-stu-id="e6b2f-124">Sign in</span></span>

<span data-ttu-id="e6b2f-125">Melden Sie sich mit Ihren Azure-Anmeldeinformationen an, um Azure PowerShell zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-125">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> <span data-ttu-id="e6b2f-126">Wenn Sie das automatische Laden von Modulen deaktiviert haben, müssen Sie das Modul manuell mit `Import-Module Az` importieren.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-126">If you've disabled module autoloading, you need to manually import the module with `Import-Module Az`.</span></span> <span data-ttu-id="e6b2f-127">Aufgrund der Modulstruktur kann dieser Vorgang einige Sekunden dauern.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-127">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="e6b2f-128">Sie müssen diese Schritte für jede neue PowerShell-Sitzung wiederholen, die Sie starten.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-128">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="e6b2f-129">Informationen zum sitzungsübergreifenden Speichern der Azure-Anmeldung in PowerShell finden Sie unter [Speichern von Benutzeranmeldeinformationen zwischen PowerShell-Sitzungen](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="e6b2f-129">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="e6b2f-130">Aktualisieren des Azure PowerShell-Moduls</span><span class="sxs-lookup"><span data-stu-id="e6b2f-130">Update the Azure PowerShell module</span></span>

<span data-ttu-id="e6b2f-131">Sie können Ihre Azure PowerShell-Installation aktualisieren, indem Sie [Update-Module](/powershell/module/powershellget/update-module) ausführen.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-131">You can update your Azure PowerShell installation by running [Update-Module](/powershell/module/powershellget/update-module).</span></span> <span data-ttu-id="e6b2f-132">Mit diesem Befehl werden __keine__ früheren Versionen deinstalliert.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-132">This command does __not__ uninstall earlier versions.</span></span>

```powershell-interactive
Update-Module -Name Az
```

<span data-ttu-id="e6b2f-133">Wenn Sie ältere Versionen von Azure PowerShell von Ihrem System entfernen möchten, helfen Ihnen die Informationen unter [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md) (Deinstallieren des Azure PowerShell-Moduls) weiter.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-133">If you want to remove older versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="e6b2f-134">Verwenden von mehreren Versionen von Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="e6b2f-134">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="e6b2f-135">Es ist möglich, mehr als eine Version von Azure PowerShell zu installieren.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-135">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="e6b2f-136">Verwenden Sie den folgenden Befehl zum Überprüfen, ob Sie mehrere Versionen von Azure PowerShell installiert haben:</span><span class="sxs-lookup"><span data-stu-id="e6b2f-136">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-Module -Name Az -List | select Name,Version
```

<span data-ttu-id="e6b2f-137">Anweisungen zum Entfernen einer Version von Azure PowerShell finden Sie unter [Deinstallieren des Azure PowerShell-Moduls](uninstall-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="e6b2f-137">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

<span data-ttu-id="e6b2f-138">Wenn Sie eine bestimmte Version des `Az`-Moduls laden möchten, verwenden Sie das Argument `-RequiredVersion` mit `Install-Module` und `Import-Module`:</span><span class="sxs-lookup"><span data-stu-id="e6b2f-138">You can load a specific version of the `Az` module by using the `-RequiredVersion` argument with `Install-Module` and `Import-Module`:</span></span>

```powershell-interactive
Install-Module -Name Az -RequiredVersion 0.4.0
Import-Module -Name Az -RequiredVersion 0.4.0
```

<span data-ttu-id="e6b2f-139">Sind mehrere Versionen des Moduls installiert, wird standardmäßig die neueste Version geladen.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-139">If you have more than one version of the module installed, the latest version is loaded by default.</span></span>

## <a name="provide-feedback"></a><span data-ttu-id="e6b2f-140">Feedback geben</span><span class="sxs-lookup"><span data-stu-id="e6b2f-140">Provide feedback</span></span>

<span data-ttu-id="e6b2f-141">[Melden Sie auf GitHub ein Problem](https://github.com/Azure/azure-powershell/issues), wenn Sie bei der Nutzung von Azure PowerShell einen Fehler finden.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-141">If you find a bug when using Azure Powershell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="e6b2f-142">Verwenden Sie das [Send-Feedback](/powershell/module/az.profile/send-feedback)-Cmdlet, um über die Befehlszeile Feedback zu senden.</span><span class="sxs-lookup"><span data-stu-id="e6b2f-142">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.profile/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e6b2f-143">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="e6b2f-143">Next Steps</span></span>

<span data-ttu-id="e6b2f-144">Weitere Informationen zum Modul und zu den zugehörigen Features als Einstieg in die Nutzung von Azure PowerShell finden Sie unter [Get started with Azure PowerShell](get-started-azureps.md) (Erste Schritte mit Azure PowerShell).</span><span class="sxs-lookup"><span data-stu-id="e6b2f-144">To get started using Azure PowerShell, see [Get Started with Azure PowerShell](get-started-azureps.md) to learn more about the module and its features.</span></span>
