---
title: Installieren von Azure PowerShell unter macOS oder Linux
description: Anleitung für die Installation von Azure PowerShell unter macOS oder Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: f014d62e898da195a38052db6b7e37a2cd96dfdd
ms.sourcegitcommit: 3a02e0c85c83de873981dd392500bc82c1cf9286
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/24/2018
ms.locfileid: "46560115"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a><span data-ttu-id="dd327-103">Installieren von Azure PowerShell unter macOS oder Linux</span><span class="sxs-lookup"><span data-stu-id="dd327-103">Install Azure PowerShell on macOS or Linux</span></span>

<span data-ttu-id="dd327-104">Bei Windows-fremden Plattformen kann Azure PowerShell in PowerShell Core v6 ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="dd327-104">For non-Windows platforms, it's possible to run Azure PowerShell in PowerShell Core v6.</span></span> <span data-ttu-id="dd327-105">Diese Version von PowerShell ist für die Verwendung auf allen Plattformen konzipiert, die .NET Core unterstützen.</span><span class="sxs-lookup"><span data-stu-id="dd327-105">This version of PowerShell is built for use on any platform that supports .NET Core.</span></span> <span data-ttu-id="dd327-106">Damit Sie diese Plattformen verwenden können, steht eine .NET Standard-Version von Azure PowerShell zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="dd327-106">To work with these platforms, there's a .NET Standard version of Azure PowerShell available.</span></span>

> [!NOTE]
> <span data-ttu-id="dd327-107">PowerShell Core v6 und Azure PowerShell für .NET Core befinden sich derzeit noch in der Betaphase.</span><span class="sxs-lookup"><span data-stu-id="dd327-107">At this time, both PowerShell Core v6 and Azure PowerShell for .NET Core are still in beta.</span></span>
> <span data-ttu-id="dd327-108">Der Support für diese Produkte ist eingeschränkt.</span><span class="sxs-lookup"><span data-stu-id="dd327-108">Support for these products is limited.</span></span> <span data-ttu-id="dd327-109">Sollten bei Ihnen Probleme oder Fehler auftreten, melden Sie dies bitte auf GitHub.</span><span class="sxs-lookup"><span data-stu-id="dd327-109">If you have problems or discover bugs, please file an issue on GitHub.</span></span>
>
> * [<span data-ttu-id="dd327-110">Probleme mit PowerShell Core v6</span><span class="sxs-lookup"><span data-stu-id="dd327-110">Issues for PowerShell Core v6</span></span>](https://github.com/PowerShell/PowerShell/issues)
> * [<span data-ttu-id="dd327-111">Probleme mit Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="dd327-111">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a><span data-ttu-id="dd327-112">Installieren von PowerShell Core</span><span class="sxs-lookup"><span data-stu-id="dd327-112">Install PowerShell Core</span></span>

<span data-ttu-id="dd327-113">Die Installationsanweisungen für PowerShell Core unterscheiden sich für macOS und die meisten Linux-Distributionen.</span><span class="sxs-lookup"><span data-stu-id="dd327-113">The installation instructions for PowerShell Core are different for macOS and most Linux distributions.</span></span>
<span data-ttu-id="dd327-114">Eine ausführliche Anleitung finden Sie in den folgenden Artikeln:</span><span class="sxs-lookup"><span data-stu-id="dd327-114">Detailed instructions can be found in the following articles:</span></span>

* [<span data-ttu-id="dd327-115">Installieren von PowerShell Core unter macOS</span><span class="sxs-lookup"><span data-stu-id="dd327-115">Install PowerShell Core on macOS</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [<span data-ttu-id="dd327-116">Installieren von PowerShell Core unter Linux</span><span class="sxs-lookup"><span data-stu-id="dd327-116">Install PowerShell Core on Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a><span data-ttu-id="dd327-117">Installieren von Azure PowerShell für .NET Core</span><span class="sxs-lookup"><span data-stu-id="dd327-117">Install Azure PowerShell for .NET Core</span></span>

<span data-ttu-id="dd327-118">In PowerShell Core ist das PowerShellGet-Modul bereits vorinstalliert.</span><span class="sxs-lookup"><span data-stu-id="dd327-118">PowerShell Core comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="dd327-119">Für die Installation der Module in PowerShell sind erhöhte Rechte erforderlich, daher müssen Sie Ihre Sitzung als Superuser starten:</span><span class="sxs-lookup"><span data-stu-id="dd327-119">Installation of modules in PowerShell requires elevated privileges, so you'll need to start your session as superuser:</span></span>

```bash
sudo pwsh
```

<span data-ttu-id="dd327-120">Führen Sie zum Installieren von Azure PowerShell den folgenden Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="dd327-120">To install Azure PowerShell, run the following command:</span></span>

```powershell
Install-Module Az
```

> [!IMPORTANT]
> <span data-ttu-id="dd327-121">Das in einem anderen Artikel behandelte `AzureRM`-Modul ist nicht für .NET Core konzipiert und kann nicht mit PowerShell Core verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="dd327-121">The `AzureRM` module detailed in other articles is not built for .NET Core and will not work with PowerShell Core.</span></span> <span data-ttu-id="dd327-122">Die `Az`-Module enthalten Befehlsaliase für alle `AzureRM`-Cmdlets, sodass die gesamte Dokumentation für `AzureRM` gilt.</span><span class="sxs-lookup"><span data-stu-id="dd327-122">The `Az` modules contain command aliases for all `AzureRM` cmdlets, so all of the documentation for `AzureRM` applies.</span></span>

<span data-ttu-id="dd327-123">Standardmäßig ist der PowerShell-Katalog nicht als vertrauenswürdiges Repository für PowerShellGet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="dd327-123">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="dd327-124">Bei der ersten Verwendung des PowerShell-Katalogs wird die folgende Meldung angezeigt:</span><span class="sxs-lookup"><span data-stu-id="dd327-124">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="dd327-125">Antworten Sie mit `Yes` oder `Yes to All`, um die Installation fortzusetzen.</span><span class="sxs-lookup"><span data-stu-id="dd327-125">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

## <a name="sign-in"></a><span data-ttu-id="dd327-126">Anmelden</span><span class="sxs-lookup"><span data-stu-id="dd327-126">Sign in</span></span>

<span data-ttu-id="dd327-127">Damit Sie Azure PowerShell verwenden können, müssen Sie `Az` mit dem [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module)-Cmdlet in Ihre PowerShell-Sitzung laden und sich dann mit Ihren Azure-Anmeldeinformationen anmelden.</span><span class="sxs-lookup"><span data-stu-id="dd327-127">To start working with Azure PowerShell, you need to load `Az` into your PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span> <span data-ttu-id="dd327-128">Für das Importieren eines Moduls sind __keine__ erhöhten Rechte erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dd327-128">Importing a module does __not__ require elevated privileges.</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module Az
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="dd327-129">Sie müssen diese Schritte für jede neue gestartete PowerShell-Sitzung wiederholen.</span><span class="sxs-lookup"><span data-stu-id="dd327-129">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="dd327-130">Für den automatischen Import des `Az`-Moduls muss ein PowerShell-Profil eingerichtet werden. Informationen hierzu finden Sie unter [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles) (Informationen zu Profilen).</span><span class="sxs-lookup"><span data-stu-id="dd327-130">Automatically importing the `Az` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="dd327-131">Unter macOS und Linux müssen Sie zur Verwendung Ihres Profils die Umgebungsvariable `$Profile` verwenden.</span><span class="sxs-lookup"><span data-stu-id="dd327-131">On macOS and Linux, you should work with your profile through the `$Profile` environment variable.</span></span> <span data-ttu-id="dd327-132">Informationen zum sitzungsübergreifenden Speichern der Azure-Anmeldung finden Sie unter [Persisting user credentials across PowerShell sessions](context-persistence.md) (Speichern von Benutzeranmeldeinformationen zwischen PowerShell-Sitzungen).</span><span class="sxs-lookup"><span data-stu-id="dd327-132">To learn how to persist your Azure sign-in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="dd327-133">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="dd327-133">Next Steps</span></span>

<span data-ttu-id="dd327-134">Weitere Informationen zur Verwendung von Azure PowerShell finden Sie im Artikel [Erste Schritte mit Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="dd327-134">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
