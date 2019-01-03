---
title: Andere Installationsmöglichkeiten für Azure PowerShell
description: Installieren von Azure PowerShell ohne PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/20/2018
ms.openlocfilehash: 30f7a01b941bb2861b1652fa30ea002d40c80a80
ms.sourcegitcommit: 797c18f93aaa495ef005993b2e202d7378588dfa
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/19/2018
ms.locfileid: "53594572"
---
# <a name="install-azure-powershell-on-windows-with-msi-or-web-platform-installer"></a><span data-ttu-id="06194-103">Installieren von Azure PowerShell unter Windows per MSI oder Webplattform-Installer</span><span class="sxs-lookup"><span data-stu-id="06194-103">Install Azure PowerShell on Windows with MSI or Web Platform Installer</span></span>

<span data-ttu-id="06194-104">In diesem Artikel erfahren Sie, wie Sie Azure PowerShell unter Windows mit einem MSI-Paket oder mit dem Webplattform-Installer (WebPI) installieren.</span><span class="sxs-lookup"><span data-stu-id="06194-104">This article explains how to install Azure PowerShell on Windows using an MSI or Web Platform Installer (WebPI).</span></span>  
<span data-ttu-id="06194-105">Verwenden Sie diese Installationsmethoden nur, wenn sie für Ihr System erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="06194-105">Use these installation methods only if they're necessary for your system.</span></span> <span data-ttu-id="06194-106">Die empfohlene Vorgehensweise zum Installieren von Azure PowerShell unter Windows ist die Verwendung von PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="06194-106">The recommended way to install Azure PowerShell on Windows is with PowerShellGet.</span></span> <span data-ttu-id="06194-107">Eine Anleitung für die Installation von Azure PowerShell unter Verwendung von PowerShellGet finden Sie unter [Installieren von Azure PowerShell mit PowerShellGet](install-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="06194-107">For instructions on using PowerShellGet to install Azure PowerShell, see [Install Azure PowerShell with PowerShellGet](install-azurerm-ps.md).</span></span>

[!INCLUDE[az-replacing-azurerm.md](../includes/az-replacing-azurerm.md)]

## <a name="install-or-update-on-windows-using-the-msi-package"></a><span data-ttu-id="06194-108">Installieren oder Aktualisieren unter Windows mithilfe des MSI-Pakets</span><span class="sxs-lookup"><span data-stu-id="06194-108">Install or update on Windows using the MSI Package</span></span>

<span data-ttu-id="06194-109">Azure PowerShell kann mithilfe der bei [GitHub](https://github.com/Azure/azure-powershell/releases/tag/v5.7.0-April2018) verfügbaren MSI-Datei installiert werden.</span><span class="sxs-lookup"><span data-stu-id="06194-109">Azure PowerShell can be installed using the MSI file available from [GitHub](https://github.com/Azure/azure-powershell/releases/tag/v5.7.0-April2018).</span></span> <span data-ttu-id="06194-110">Ältere per MSI installierte Versionen von Azure-Modulen werden vom Installationsprogramm automatisch entfernt.</span><span class="sxs-lookup"><span data-stu-id="06194-110">If you have installed previous versions of Azure modules as an MSI, the installer automatically removes them.</span></span> <span data-ttu-id="06194-111">Mit dem MSI-Paket werden Module unter `${env:ProgramFiles}\WindowsPowerShell\Modules` installiert.</span><span class="sxs-lookup"><span data-stu-id="06194-111">The MSI package installs modules in `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="06194-112">Sowohl das Modul `AzureRM` als auch das Modul `Azure` werden installiert.</span><span class="sxs-lookup"><span data-stu-id="06194-112">Both the `AzureRM` and `Azure` modules are installed.</span></span>

> [!NOTE]
> <span data-ttu-id="06194-113">Verwenden Sie das Modul `Azure` nur, wenn Sie mit dem klassischen Azure-Bereitstellungsmodell arbeiten.</span><span class="sxs-lookup"><span data-stu-id="06194-113">Only use the `Azure` module if you are working with the Azure classic deployment model.</span></span>

<span data-ttu-id="06194-114">Damit Sie Azure PowerShell verwenden können, müssen Sie `AzureRM` mit dem [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module)-Cmdlet in Ihre aktuelle PowerShell-Sitzung laden und sich dann mit Ihren Azure-Anmeldeinformationen anmelden.</span><span class="sxs-lookup"><span data-stu-id="06194-114">To start working with Azure PowerShell, you need to load `AzureRM` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="06194-115">Sie müssen diese Schritte für jede neue PowerShell-Sitzung wiederholen, die Sie starten.</span><span class="sxs-lookup"><span data-stu-id="06194-115">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="06194-116">Für den automatischen Import des Moduls `AzureRM` muss ein PowerShell-Profil eingerichtet werden. Informationen hierzu finden Sie unter [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles) (Informationen zu Profilen).</span><span class="sxs-lookup"><span data-stu-id="06194-116">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="06194-117">Informationen zum sitzungsübergreifenden Speichern der Azure-Anmeldung finden Sie unter [Persisting user credentials across PowerShell sessions](context-persistence.md) (Speichern von Benutzeranmeldeinformationen zwischen PowerShell-Sitzungen).</span><span class="sxs-lookup"><span data-stu-id="06194-117">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="install-or-update-on-windows-using-the-web-platform-installer"></a><span data-ttu-id="06194-118">Installieren oder Aktualisieren unter Windows mit dem Webplattform-Installer</span><span class="sxs-lookup"><span data-stu-id="06194-118">Install or update on Windows using the Web Platform Installer</span></span>

<span data-ttu-id="06194-119">Laden Sie das [Azure PowerShell-WebPI-Paket](http://aka.ms/webpi-azps) herunter, und starten Sie die Installation.</span><span class="sxs-lookup"><span data-stu-id="06194-119">Download the [Azure PowerShell WebPI package](http://aka.ms/webpi-azps) and start the install.</span></span> <span data-ttu-id="06194-120">Ältere per MSI oder WebPI installierte Versionen von Azure-Modulen werden vom Installationsprogramm automatisch entfernt.</span><span class="sxs-lookup"><span data-stu-id="06194-120">If you have installed previous versions of Azure modules from an MSI or with WebPI, the installer automatically removes them.</span></span> <span data-ttu-id="06194-121">Die Module werden unter `${env:ProgramFiles}\WindowsPowerShell\Modules` installiert.</span><span class="sxs-lookup"><span data-stu-id="06194-121">Modules are installed into `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="06194-122">Sowohl das Modul `AzureRM` als auch das Modul `Azure` werden installiert.</span><span class="sxs-lookup"><span data-stu-id="06194-122">Both the `AzureRM` and `Azure` modules are installed.</span></span>

> [!NOTE]
> <span data-ttu-id="06194-123">Verwenden Sie das Modul `Azure` nur, wenn Sie mit dem klassischen Azure-Bereitstellungsmodell arbeiten.</span><span class="sxs-lookup"><span data-stu-id="06194-123">Only use the `Azure` module if you are working with the Azure classic deployment model.</span></span>

<span data-ttu-id="06194-124">Damit Sie Azure PowerShell verwenden können, müssen Sie `AzureRM` mit dem [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module)-Cmdlet in Ihre aktuelle PowerShell-Sitzung laden und sich dann mit Ihren Azure-Anmeldeinformationen anmelden.</span><span class="sxs-lookup"><span data-stu-id="06194-124">To start working with Azure PowerShell, you need to load `AzureRM` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="06194-125">Sie müssen diese Schritte für jede neue PowerShell-Sitzung wiederholen, die Sie starten.</span><span class="sxs-lookup"><span data-stu-id="06194-125">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="06194-126">Für den automatischen Import des Moduls `AzureRM` muss ein PowerShell-Profil eingerichtet werden. Informationen hierzu finden Sie unter [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles) (Informationen zu Profilen).</span><span class="sxs-lookup"><span data-stu-id="06194-126">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="06194-127">Informationen zum sitzungsübergreifenden Speichern der Azure-Anmeldung finden Sie unter [Persisting user credentials across PowerShell sessions](context-persistence.md) (Speichern von Benutzeranmeldeinformationen zwischen PowerShell-Sitzungen).</span><span class="sxs-lookup"><span data-stu-id="06194-127">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>