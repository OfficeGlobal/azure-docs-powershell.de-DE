---
title: Installieren von Azure PowerShell unter macOS oder Linux
description: Anleitung für die Installation von Azure PowerShell unter macOS oder Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 17912c155255b6fdfd3cfb9242163b67d405dc03
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323253"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a><span data-ttu-id="f9f23-103">Installieren von Azure PowerShell unter macOS oder Linux</span><span class="sxs-lookup"><span data-stu-id="f9f23-103">Install Azure PowerShell on macOS or Linux</span></span>

<span data-ttu-id="f9f23-104">Bei Windows-fremden Plattformen kann Azure PowerShell auf der Grundlage von PowerShell Core v6 ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="f9f23-104">For non-Windows platforms, it's possible to run Azure PowerShell on top of PowerShell Core v6.</span></span> <span data-ttu-id="f9f23-105">Im Gegensatz zur Standardversion von Azure PowerShell, die auf .NET Framework für Windows basiert, wurde dieses Produkt für .NET Core konzipiert und kann auf einer beliebigen Plattform ausgeführt werden, die die .NET Core-Laufzeit unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f9f23-105">Rather than the standard Azure PowerShell built on .NET Framework for Windows, this product is built for .NET Core and can run on any platform which supports the .Net Core runtime.</span></span>

> [!NOTE]
> <span data-ttu-id="f9f23-106">PowerShell Core v6 und Azure PowerShell für .NET Core befinden sich derzeit noch in der Betaphase.</span><span class="sxs-lookup"><span data-stu-id="f9f23-106">At this time, both PowerShell Core v6 and Azure PowerShell for .NET Core are still in beta.</span></span>
> <span data-ttu-id="f9f23-107">Der Support für diese Produkte ist eingeschränkt.</span><span class="sxs-lookup"><span data-stu-id="f9f23-107">Support for these products is limited.</span></span> <span data-ttu-id="f9f23-108">Sollten bei Ihnen Probleme oder Fehler auftreten, melden Sie dies bitte auf GitHub.</span><span class="sxs-lookup"><span data-stu-id="f9f23-108">If you have problems or discover bugs, please file an issue on GitHub.</span></span>
>
> * [<span data-ttu-id="f9f23-109">Probleme mit PowerShell Core v6</span><span class="sxs-lookup"><span data-stu-id="f9f23-109">Issues for PowerShell Core v6</span></span>](https://github.com/PowerShell/PowerShell/issues)
> * [<span data-ttu-id="f9f23-110">Probleme mit Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="f9f23-110">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core-v6"></a><span data-ttu-id="f9f23-111">Installieren von PowerShell Core v6</span><span class="sxs-lookup"><span data-stu-id="f9f23-111">Install PowerShell Core v6</span></span>

<span data-ttu-id="f9f23-112">Die Installation von PowerShell Core v6 unter Linux oder macOS variiert je nach Linux-Distribution und Betriebssystemversion.</span><span class="sxs-lookup"><span data-stu-id="f9f23-112">Installing PowerShell Core v6 on Linux or macOS varies depending on the Linux distribution and OS version.</span></span>
<span data-ttu-id="f9f23-113">Eine ausführliche Anleitung finden Sie in den folgenden Artikeln:</span><span class="sxs-lookup"><span data-stu-id="f9f23-113">Detailed instructions can be found in the following articles:</span></span>

- [<span data-ttu-id="f9f23-114">Installieren von PowerShell Core unter macOS</span><span class="sxs-lookup"><span data-stu-id="f9f23-114">Install PowerShell Core on macOS</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos)
- [<span data-ttu-id="f9f23-115">Installieren von PowerShell Core unter Linux</span><span class="sxs-lookup"><span data-stu-id="f9f23-115">Install PowerShell Core on Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a><span data-ttu-id="f9f23-116">Installieren von Azure PowerShell für .NET Core</span><span class="sxs-lookup"><span data-stu-id="f9f23-116">Install Azure PowerShell for .NET Core</span></span>

<span data-ttu-id="f9f23-117">In PowerShell Core v6 ist das PowerShellGet-Modul bereits vorinstalliert.</span><span class="sxs-lookup"><span data-stu-id="f9f23-117">PowerShell Core v6 comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="f9f23-118">Dies vereinfacht die Installation eines beliebigen, im PowerShell-Katalog veröffentlichten Moduls.</span><span class="sxs-lookup"><span data-stu-id="f9f23-118">This makes it easy to install any module that is published to the PowerShell Gallery.</span></span> <span data-ttu-id="f9f23-119">Um Azure PowerShell zu installieren, öffnen Sie eine neue PowerShell-Sitzung, und führen Sie den folgenden Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="f9f23-119">To install Azure PowerShell, open a new PowerShell session and run the following command:</span></span>

```powershell
Install-Module AzureRM.NetCore
```

## <a name="load-the-azurermnetcore-module"></a><span data-ttu-id="f9f23-120">Laden des AzureRM.Netcore-Moduls</span><span class="sxs-lookup"><span data-stu-id="f9f23-120">Load the AzureRM.Netcore module</span></span>

<span data-ttu-id="f9f23-121">Nach der Installation des Moduls müssen Sie das Modul in der PowerShell-Sitzung laden.</span><span class="sxs-lookup"><span data-stu-id="f9f23-121">Once the module is installed, you need to load the module into your PowerShell session.</span></span> <span data-ttu-id="f9f23-122">Module werden wie folgt mit dem Cmdlet `Import-Module` geladen:</span><span class="sxs-lookup"><span data-stu-id="f9f23-122">Modules are loaded using the `Import-Module` cmdlet, as follows:</span></span>

```powershell
Import-Module AzureRM.Netcore
Import-Module AzureRM.Profile.Netcore
```

<span data-ttu-id="f9f23-123">Nach Abschluss des Imports können Sie das neu installierte Modul testen, indem Sie versuchen, sich mithilfe des folgenden Befehls bei Azure anzumelden:</span><span class="sxs-lookup"><span data-stu-id="f9f23-123">After the import completes, you can test your newly installed and module by attempting to sign into Azure using the following command:</span></span>

```powershell
Connect-AzureRmAccount
```

<span data-ttu-id="f9f23-124">Der obige Befehl sollte Sie auffordern, zu `https://aka.ms/devicelogin` zu wechseln und den bereitgestellten Code einzugeben.</span><span class="sxs-lookup"><span data-stu-id="f9f23-124">The above command should prompt you to go to `https://aka.ms/devicelogin` and enter the provided code.</span></span>

## <a name="available-cmdlets"></a><span data-ttu-id="f9f23-125">Verfügbare Cmdlets</span><span class="sxs-lookup"><span data-stu-id="f9f23-125">Available cmdlets</span></span>

<span data-ttu-id="f9f23-126">Die Azure PowerShell-Module für .NET Standard sind immer noch in der Entwicklungsphase.</span><span class="sxs-lookup"><span data-stu-id="f9f23-126">The Azure PowerShell modules for .NET Standard are still in development.</span></span> <span data-ttu-id="f9f23-127">Diese Module bieten nicht den vollständigen Satz der Cmdlets, die für die Windows-Version der Module verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="f9f23-127">These modules do not provide the full set of cmdlets that are available for the Windows version of the modules.</span></span> <span data-ttu-id="f9f23-128">Die folgenden Funktionen werden in AzureRM.Netcore-Module implementiert:</span><span class="sxs-lookup"><span data-stu-id="f9f23-128">The following functions are implemented in AzureRM.Netcore modules:</span></span>

* <span data-ttu-id="f9f23-129">Kontenverwaltung</span><span class="sxs-lookup"><span data-stu-id="f9f23-129">Account management</span></span>
  - <span data-ttu-id="f9f23-130">Melden Sie sich mit dem Microsoft-Konto, Unternehmenskonto oder einem Dienstprinzipal über Microsoft Azure Active Directory an.</span><span class="sxs-lookup"><span data-stu-id="f9f23-130">Login with Microsoft account, Organizational account, or Service Principal through Microsoft Azure Active Directory</span></span>
  - <span data-ttu-id="f9f23-131">Speichern Sie die Anmeldeinformationen mit Save-AzureRmContext auf einem Datenträger, und laden Sie gespeicherte Anmeldeinformationen mit Import-AzureRmContext.</span><span class="sxs-lookup"><span data-stu-id="f9f23-131">Save Credentials to disk with Save-AzureRmContext and load saved credentials using Import-AzureRmContext</span></span>
* <span data-ttu-id="f9f23-132">Environment</span><span class="sxs-lookup"><span data-stu-id="f9f23-132">Environment</span></span>
  - <span data-ttu-id="f9f23-133">Abrufen der verschiedenen vorkonfigurierten Microsoft Azure-Umgebungen</span><span class="sxs-lookup"><span data-stu-id="f9f23-133">Get the different out-of-box Microsoft Azure environments</span></span>
  - <span data-ttu-id="f9f23-134">Hinzufügen/Einrichten/Entfernen angepasster Umgebungen (z.B. Ihrer Azure Stack- oder Windows Azure Pack-Umgebungen)</span><span class="sxs-lookup"><span data-stu-id="f9f23-134">Add/Set/Remove customized environments (like your Azure Stack or Windows Azure Pack environments)</span></span>
* <span data-ttu-id="f9f23-135">Cmdlets auf Verwaltungsebene für Azure-Dienste, die Resource Manager- und Service Management-Schnittstellen nutzen.</span><span class="sxs-lookup"><span data-stu-id="f9f23-135">Management plane cmdlets for Azure services using Resource Manager and Service Management interfaces.</span></span>
  - <span data-ttu-id="f9f23-136">Virtual Machine</span><span class="sxs-lookup"><span data-stu-id="f9f23-136">Virtual Machine</span></span>
  - <span data-ttu-id="f9f23-137">App Service (Websites)</span><span class="sxs-lookup"><span data-stu-id="f9f23-137">App Service (Websites)</span></span>
  - <span data-ttu-id="f9f23-138">SQL-Datenbank</span><span class="sxs-lookup"><span data-stu-id="f9f23-138">SQL Database</span></span>
  - <span data-ttu-id="f9f23-139">Speicher</span><span class="sxs-lookup"><span data-stu-id="f9f23-139">Storage</span></span>
  - <span data-ttu-id="f9f23-140">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f9f23-140">Network</span></span>

## <a name="next-steps"></a><span data-ttu-id="f9f23-141">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="f9f23-141">Next Steps</span></span>

<span data-ttu-id="f9f23-142">Weitere Informationen zur Verwendung von Azure PowerShell finden Sie im Artikel [Erste Schritte mit Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="f9f23-142">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
