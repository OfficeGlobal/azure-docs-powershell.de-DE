---
title: Übersicht über Azure PowerShell
description: Enthält eine Übersicht über das Azure PowerShell Az-Modul und Informationen zur Installation und zum Einstieg.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.manager: carmonm
ms.date: 10/29/2018
ms.openlocfilehash: 7982e122d49db4d558648231d1ab8bfeed80be2d
ms.sourcegitcommit: 4acddc7026522c4fe39de2c4424917d88ee01b7e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/21/2018
ms.locfileid: "53736459"
---
# <a name="overview-of-azure-powershell"></a><span data-ttu-id="8cb12-103">Übersicht über Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="8cb12-103">Overview of Azure PowerShell</span></span>

<span data-ttu-id="8cb12-104">Azure PowerShell bietet eine Reihe von Cmdlets, die das [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview)-Modell für die Verwaltung von Azure-Ressourcen verwenden.</span><span class="sxs-lookup"><span data-stu-id="8cb12-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span> <span data-ttu-id="8cb12-105">Für Azure PowerShell wird .NET Standard verwendet, damit die Umgebung für Windows, macOS und Linux verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="8cb12-105">Azure PowerShell uses .NET Standard, making it available for Windows, macOS, and Linux.</span></span>
<span data-ttu-id="8cb12-106">Azure PowerShell steht auch über Azure Cloud Shell zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="8cb12-106">Azure PowerShell is also available from Azure Cloud Shell.</span></span>

<span data-ttu-id="8cb12-107">Verwenden Sie [Azure Cloud Shell](/azure/cloud-shell/overview), um Azure PowerShell in Ihrem Browser auszuführen, oder führen Sie die [lokale Installation](install-az-ps.md) durch.</span><span class="sxs-lookup"><span data-stu-id="8cb12-107">Use [Azure Cloud Shell](/azure/cloud-shell/overview) to run Azure PowerShell in your browser, or [install locally](install-az-ps.md).</span></span> <span data-ttu-id="8cb12-108">Lesen Sie den Artikel zu den [ersten Schritten](get-started-azureps.md), um sich über die Grundlagen von Azure PowerShell zu informieren und in die Nutzung von Azure einzusteigen.</span><span class="sxs-lookup"><span data-stu-id="8cb12-108">Check out the [Get Started](get-started-azureps.md) article to learn the Azure PowerShell basics and get started with Azure.</span></span>

<span data-ttu-id="8cb12-109">Informationen zur neuesten Azure PowerShell-Version finden Sie in den [Versionshinweisen](release-notes-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="8cb12-109">For information about the latest Azure PowerShell release, see the [release notes](release-notes-azureps.md).</span></span>

## <a name="about-the-new-az-module"></a><span data-ttu-id="8cb12-110">Informationen zum neuen Az-Modul</span><span class="sxs-lookup"><span data-stu-id="8cb12-110">About the new Az module</span></span>

<span data-ttu-id="8cb12-111">In dieser Dokumentation wird das neue Az-Modul für Azure PowerShell beschrieben.</span><span class="sxs-lookup"><span data-stu-id="8cb12-111">This documentation describes the new Az module for Azure PowerShell.</span></span> <span data-ttu-id="8cb12-112">Dieses neue Modul wurde von Grund auf in .NET Standard geschrieben.</span><span class="sxs-lookup"><span data-stu-id="8cb12-112">This new module is written from the ground up in .NET Standard.</span></span> <span data-ttu-id="8cb12-113">Bei Verwendung von .NET Standard kann Azure PowerShell unter PowerShell 5.x auf Windows oder PowerShell 6 auf einer beliebigen Plattform ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="8cb12-113">Using .NET Standard allows Azure PowerShell to run under PowerShell 5.x on Windows or PowerShell 6 on any platform.</span></span> <span data-ttu-id="8cb12-114">Das Az-Modul ist jetzt die bevorzugte Vorgehensweise für die Interaktion mit Azure über PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8cb12-114">The Az module is now the intended way to interact with Azure through PowerShell.</span></span>
<span data-ttu-id="8cb12-115">Für AzureRM werden weiterhin Fehlerbehebungen bereitgestellt, aber keine neuen Features mehr.</span><span class="sxs-lookup"><span data-stu-id="8cb12-115">AzureRM will continue to get bug fixes, but no longer receive new features.</span></span>

<span data-ttu-id="8cb12-116">Alle Details zum neuen Modul, z.B. die Umbenennung der Befehle und die Wartungspläne für AzureRM, finden Sie unter [Einführung in das Az-Modul von Azure PowerShell](new-azureps-module-az.md).</span><span class="sxs-lookup"><span data-stu-id="8cb12-116">Learn the full details about the new module, including how commands have been renamed and the maintenance plans for AzureRM, in the [Introducing the Azure PowerShell Az module](new-azureps-module-az.md).</span></span> <span data-ttu-id="8cb12-117">Wenn Sie gleich in die Nutzung des neuen Moduls einsteigen möchten, können Sie den Artikel [Migrieren von AzureRM zum Az-Modul von Azure PowerShell](migrate-from-azurerm-to-az.md) lesen.</span><span class="sxs-lookup"><span data-stu-id="8cb12-117">If you want to get started with using the new module right away, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>

<span data-ttu-id="8cb12-118">Darüber hinaus ist die [AzureRM-Dokumentation](/powershell/azure/azurerm) verfügbar.</span><span class="sxs-lookup"><span data-stu-id="8cb12-118">The [AzureRM documentation](/powershell/azure/azurerm) is also available.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="8cb12-119">Während die Azure-Dokumentation aktualisiert wird, damit die neuen Cmdlet-Namen des Moduls darin widergespiegelt werden, werden in den Artikeln unter Umständen vorerst noch die AzureRM-Befehle verwendet.</span><span class="sxs-lookup"><span data-stu-id="8cb12-119">While the Azure documentation is being updated to reflect the new module cmdlet names, articles may still use the AzureRM commands.</span></span> <span data-ttu-id="8cb12-120">Nach der Installation des Az-Moduls ist es ratsam, die Cmdlet-Aliase von AzureRM mit `Enable-AzureRmAlias` zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="8cb12-120">After installing the Az module, it's recommended that you enable the AzureRM cmdlet aliases with `Enable-AzureRmAlias`.</span></span> <span data-ttu-id="8cb12-121">Ausführlichere Informationen finden Sie im Artikel [Migrieren von AzureRM zum Az-Modul von Azure PowerShell](migrate-from-azurerm-to-az.md).</span><span class="sxs-lookup"><span data-stu-id="8cb12-121">See the [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md) article for more details.</span></span>

## <a name="common-scenarios"></a><span data-ttu-id="8cb12-122">Häufige Szenarios</span><span class="sxs-lookup"><span data-stu-id="8cb12-122">Common scenarios</span></span>

<span data-ttu-id="8cb12-123">In den folgenden Beispielen werden gängige Szenarien mit Azure PowerShell veranschaulicht:</span><span class="sxs-lookup"><span data-stu-id="8cb12-123">The following samples can help you learn how to perform common scenarios with Azure PowerShell:</span></span>

* [<span data-ttu-id="8cb12-124">Virtuelle Linux-Computer</span><span class="sxs-lookup"><span data-stu-id="8cb12-124">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="8cb12-125">Virtuelle Windows-Computer</span><span class="sxs-lookup"><span data-stu-id="8cb12-125">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="8cb12-126">Web-Apps</span><span class="sxs-lookup"><span data-stu-id="8cb12-126">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="8cb12-127">SQL-Datenbanken</span><span class="sxs-lookup"><span data-stu-id="8cb12-127">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

## <a name="learn-powershell-basics"></a><span data-ttu-id="8cb12-128">PowerShell-Grundlagen erlernen</span><span class="sxs-lookup"><span data-stu-id="8cb12-128">Learn PowerShell basics</span></span>

<span data-ttu-id="8cb12-129">Falls Sie mit PowerShell noch nicht vertraut sind, kann es hilfreich sein, eine Einführung zu lesen.</span><span class="sxs-lookup"><span data-stu-id="8cb12-129">If you're unfamiliar with PowerShell, an introduction may be helpful.</span></span>

* [<span data-ttu-id="8cb12-130">Installieren von PowerShell</span><span class="sxs-lookup"><span data-stu-id="8cb12-130">Installing PowerShell</span></span>](/powershell/scripting/setup/installing-windows-powershell)
* [<span data-ttu-id="8cb12-131">Skripterstellung mit PowerShell</span><span class="sxs-lookup"><span data-stu-id="8cb12-131">Scripting with PowerShell</span></span>](/powershell/scripting/powershell-scripting)

<span data-ttu-id="8cb12-132">Empfehlenswert ist auch folgendes Video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1) (PowerShell-Grundlagen – Teil 1: Erste Schritte mit PowerShell)</span><span class="sxs-lookup"><span data-stu-id="8cb12-132">You can also watch this video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span></span>

<span data-ttu-id="8cb12-133">Oder Sie sehen sich in der Microsoft Virtual Academy die Einführung [Getting Started with PowerShell](https://mva.microsoft.com/liveevents/powershell-jumpstart) (Erste Schritte mit PowerShell) an.</span><span class="sxs-lookup"><span data-stu-id="8cb12-133">Or attend the Microsoft Virtual Academy's [Getting Started with PowerShell Jumpstart](https://mva.microsoft.com/liveevents/powershell-jumpstart).</span></span>

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="8cb12-134">Erweitern Ihrer Fähigkeiten mit Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="8cb12-134">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="8cb12-135">Automatisieren von Azure-Aufgaben mithilfe von Skripts über PowerShell</span><span class="sxs-lookup"><span data-stu-id="8cb12-135">Automate Azure tasks using scripts with PowerShell</span></span>](/learn/modules/automate-azure-tasks-with-powershell/)
- [<span data-ttu-id="8cb12-136">Mehr interaktives Lernen...</span><span class="sxs-lookup"><span data-stu-id="8cb12-136">More interactive learning...</span></span>](/learn/browse/?term=powershell)

## <a name="other-azure-powershell-modules"></a><span data-ttu-id="8cb12-137">Andere Azure PowerShell-Module</span><span class="sxs-lookup"><span data-stu-id="8cb12-137">Other Azure PowerShell modules</span></span>

* [<span data-ttu-id="8cb12-138">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="8cb12-138">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
* [<span data-ttu-id="8cb12-139">Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="8cb12-139">Azure Information Protection</span></span>](/powershell/azure/aip/)
* [<span data-ttu-id="8cb12-140">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8cb12-140">Azure Service Fabric</span></span>](/powershell/azure/service-fabric/)
* [<span data-ttu-id="8cb12-141">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="8cb12-141">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)
