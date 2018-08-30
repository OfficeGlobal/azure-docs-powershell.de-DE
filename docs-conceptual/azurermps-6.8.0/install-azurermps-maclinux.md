---
title: Installieren von Azure PowerShell unter macOS oder Linux
description: Anleitung für die Installation von Azure PowerShell unter macOS oder Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 6e7d447ea9672c174e3f1d103bc56c11a7f37192
ms.sourcegitcommit: 9cb98f055a0525c2061f65149965d5e7c3e03ddc
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/30/2018
ms.locfileid: "43117652"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a><span data-ttu-id="c9e1d-103">Installieren von Azure PowerShell unter macOS oder Linux</span><span class="sxs-lookup"><span data-stu-id="c9e1d-103">Install Azure PowerShell on macOS or Linux</span></span>

<span data-ttu-id="c9e1d-104">Bei Windows-fremden Plattformen kann Azure PowerShell in PowerShell Core v6 ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-104">For non-Windows platforms, it's possible to run Azure PowerShell in PowerShell Core v6.</span></span> <span data-ttu-id="c9e1d-105">Diese Version von PowerShell ist für die Verwendung auf allen Plattformen konzipiert, die .NET Core unterstützen.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-105">This version of PowerShell is built for use on any platform that supports .NET Core.</span></span> <span data-ttu-id="c9e1d-106">Damit Sie diese Plattformen verwenden können, steht eine spezielle .NET Core-Version von Azure PowerShell zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-106">To work with these platforms, there's a special .NET Core version of Azure PowerShell available.</span></span>

> [!NOTE]
> <span data-ttu-id="c9e1d-107">PowerShell Core v6 und Azure PowerShell für .NET Core befinden sich derzeit noch in der Betaphase.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-107">At this time, both PowerShell Core v6 and Azure PowerShell for .NET Core are still in beta.</span></span>
> <span data-ttu-id="c9e1d-108">Der Support für diese Produkte ist eingeschränkt.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-108">Support for these products is limited.</span></span> <span data-ttu-id="c9e1d-109">Sollten bei Ihnen Probleme oder Fehler auftreten, melden Sie dies bitte auf GitHub.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-109">If you have problems or discover bugs, please file an issue on GitHub.</span></span>
>
> * [<span data-ttu-id="c9e1d-110">Probleme mit PowerShell Core v6</span><span class="sxs-lookup"><span data-stu-id="c9e1d-110">Issues for PowerShell Core v6</span></span>](https://github.com/PowerShell/PowerShell/issues)
> * [<span data-ttu-id="c9e1d-111">Probleme mit Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c9e1d-111">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a><span data-ttu-id="c9e1d-112">Installieren von PowerShell Core</span><span class="sxs-lookup"><span data-stu-id="c9e1d-112">Install PowerShell Core</span></span>

<span data-ttu-id="c9e1d-113">Die Installationsanweisungen für PowerShell Core unterscheiden sich für macOS und die meisten Linux-Distributionen.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-113">The installation instructions for PowerShell Core are different for macOS and most Linux distributions.</span></span>
<span data-ttu-id="c9e1d-114">Eine ausführliche Anleitung finden Sie in den folgenden Artikeln:</span><span class="sxs-lookup"><span data-stu-id="c9e1d-114">Detailed instructions can be found in the following articles:</span></span>

* [<span data-ttu-id="c9e1d-115">Installieren von PowerShell Core unter macOS</span><span class="sxs-lookup"><span data-stu-id="c9e1d-115">Install PowerShell Core on macOS</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [<span data-ttu-id="c9e1d-116">Installieren von PowerShell Core unter Linux</span><span class="sxs-lookup"><span data-stu-id="c9e1d-116">Install PowerShell Core on Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a><span data-ttu-id="c9e1d-117">Installieren von Azure PowerShell für .NET Core</span><span class="sxs-lookup"><span data-stu-id="c9e1d-117">Install Azure PowerShell for .NET Core</span></span>

<span data-ttu-id="c9e1d-118">In PowerShell Core ist das PowerShellGet-Modul bereits vorinstalliert.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-118">PowerShell Core comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="c9e1d-119">Für die Installation der Module in PowerShell sind erhöhte Rechte erforderlich, daher müssen Sie Ihre Sitzung als Superuser starten:</span><span class="sxs-lookup"><span data-stu-id="c9e1d-119">Installation of modules in PowerShell requires elevated privileges, so you'll need to start your session as superuser:</span></span>

```bash
sudo pwsh
```

<span data-ttu-id="c9e1d-120">Führen Sie zum Installieren von Azure PowerShell den folgenden Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="c9e1d-120">To install Azure PowerShell, run the following command:</span></span>

```powershell
Install-Module AzureRM.NetCore
```

> [!IMPORTANT]
> <span data-ttu-id="c9e1d-121">Das in einem anderen Artikel behandelte `AzureRM`-Modul ist nicht für .NET Core konzipiert und kann nicht mit PowerShell Core verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-121">The `AzureRM` module detailed in other articles is not built for .NET Core and will not work with PowerShell Core.</span></span> <span data-ttu-id="c9e1d-122">`AzureRM` und `AzureRM.NetCore` verwenden die gleichen Cmdlet-Namen. Der einzige Unterschied besteht also im Namen des Rollupmoduls und der .NET-Version, für die sie erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-122">Both `AzureRM` and `AzureRM.NetCore` use the same cmdlet names, so the only difference is the name of the rollup module and which .NET version they are built against.</span></span>

<span data-ttu-id="c9e1d-123">Standardmäßig ist der PowerShell-Katalog nicht als vertrauenswürdiges Repository für PowerShellGet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-123">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="c9e1d-124">Bei der ersten Verwendung des PowerShell-Katalogs wird die folgende Meldung angezeigt:</span><span class="sxs-lookup"><span data-stu-id="c9e1d-124">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="c9e1d-125">Antworten Sie mit `Yes` oder `Yes to All`, um die Installation fortzusetzen.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-125">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

## <a name="sign-in"></a><span data-ttu-id="c9e1d-126">Anmelden</span><span class="sxs-lookup"><span data-stu-id="c9e1d-126">Sign in</span></span>

<span data-ttu-id="c9e1d-127">Damit Sie Azure PowerShell verwenden können, müssen Sie `AzureRM.Netcore` mit dem [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module)-Cmdlet in Ihre PowerShell-Sitzung laden und sich dann mit Ihren Azure-Anmeldeinformationen anmelden.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-127">To start working with Azure PowerShell, you need to load `AzureRM.Netcore` into your PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span> <span data-ttu-id="c9e1d-128">Für das Importieren eines Moduls sind __keine__ erhöhten Rechte erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-128">Importing a module does __not__ require elevated privileges.</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module AzureRM.Netcore
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="c9e1d-129">Sie müssen diese Schritte für jede neue gestartete PowerShell-Sitzung wiederholen.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-129">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="c9e1d-130">Für den automatischen Import des `AzureRM`-Moduls muss ein PowerShell-Profil eingerichtet werden. Informationen hierzu finden Sie unter [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles) (Informationen zu Profilen).</span><span class="sxs-lookup"><span data-stu-id="c9e1d-130">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="c9e1d-131">Unter macOS und Linux müssen Sie zur Verwendung Ihres Profils die Umgebungsvariable `$Profile` verwenden.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-131">On macOS and Linux, you should work with your profile through the `$Profile` environment variable.</span></span> <span data-ttu-id="c9e1d-132">Informationen zum sitzungsübergreifenden Speichern der Azure-Anmeldung finden Sie unter [Persisting user credentials across PowerShell sessions](context-persistence.md) (Speichern von Benutzeranmeldeinformationen zwischen PowerShell-Sitzungen).</span><span class="sxs-lookup"><span data-stu-id="c9e1d-132">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="available-cmdlets"></a><span data-ttu-id="c9e1d-133">Verfügbare Cmdlets</span><span class="sxs-lookup"><span data-stu-id="c9e1d-133">Available cmdlets</span></span>

<span data-ttu-id="c9e1d-134">Die Azure PowerShell-Module für .NET Core befinden sich noch in der Entwicklungsphase.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-134">The Azure PowerShell modules for .NET Core are still in development.</span></span> <span data-ttu-id="c9e1d-135">Diese Module bieten nicht den vollständigen Satz der Cmdlets, die für die Windows-Version der Module verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-135">These modules do not provide the full set of cmdlets that are available for the Windows version of the modules.</span></span> <span data-ttu-id="c9e1d-136">Die folgenden Funktionen werden in AzureRM.Netcore-Module implementiert:</span><span class="sxs-lookup"><span data-stu-id="c9e1d-136">The following functions are implemented in AzureRM.Netcore modules:</span></span>

* <span data-ttu-id="c9e1d-137">Kontenverwaltung</span><span class="sxs-lookup"><span data-stu-id="c9e1d-137">Account management</span></span>
  * <span data-ttu-id="c9e1d-138">Anmelden mit einem Microsoft-Konto, Unternehmenskonto oder Dienstprinzipal über Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c9e1d-138">Sign in with Microsoft account, Organizational account, or Service Principal through Microsoft Azure Active Directory</span></span>
  * <span data-ttu-id="c9e1d-139">Speichern Sie die Anmeldeinformationen mit Save-AzureRmContext auf einem Datenträger, und laden Sie gespeicherte Anmeldeinformationen mit Import-AzureRmContext.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-139">Save Credentials to disk with Save-AzureRmContext and load saved credentials using Import-AzureRmContext</span></span>
* <span data-ttu-id="c9e1d-140">Environment</span><span class="sxs-lookup"><span data-stu-id="c9e1d-140">Environment</span></span>
  * <span data-ttu-id="c9e1d-141">Abrufen der verschiedenen vorkonfigurierten Microsoft Azure-Umgebungen</span><span class="sxs-lookup"><span data-stu-id="c9e1d-141">Get the different out-of-box Microsoft Azure environments</span></span>
  * <span data-ttu-id="c9e1d-142">Hinzufügen/Einrichten/Entfernen angepasster Umgebungen (z.B. Ihrer Azure Stack- oder Windows Azure Pack-Umgebungen)</span><span class="sxs-lookup"><span data-stu-id="c9e1d-142">Add/Set/Remove customized environments (like your Azure Stack or Windows Azure Pack environments)</span></span>
* <span data-ttu-id="c9e1d-143">Cmdlets auf Verwaltungsebene für Azure-Dienste, die Resource Manager- und Service Management-Schnittstellen nutzen.</span><span class="sxs-lookup"><span data-stu-id="c9e1d-143">Management plane cmdlets for Azure services using Resource Manager and Service Management interfaces.</span></span>
  * <span data-ttu-id="c9e1d-144">Virtual Machine</span><span class="sxs-lookup"><span data-stu-id="c9e1d-144">Virtual Machine</span></span>
  * <span data-ttu-id="c9e1d-145">App Service (Websites)</span><span class="sxs-lookup"><span data-stu-id="c9e1d-145">App Service (Websites)</span></span>
  * <span data-ttu-id="c9e1d-146">SQL-Datenbank</span><span class="sxs-lookup"><span data-stu-id="c9e1d-146">SQL Database</span></span>
  * <span data-ttu-id="c9e1d-147">Speicher</span><span class="sxs-lookup"><span data-stu-id="c9e1d-147">Storage</span></span>
  * <span data-ttu-id="c9e1d-148">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="c9e1d-148">Network</span></span>

## <a name="next-steps"></a><span data-ttu-id="c9e1d-149">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="c9e1d-149">Next Steps</span></span>

<span data-ttu-id="c9e1d-150">Weitere Informationen zur Verwendung von Azure PowerShell finden Sie im Artikel [Erste Schritte mit Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="c9e1d-150">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
