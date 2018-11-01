---
title: Übersicht über Azure PowerShell | Microsoft-Dokumentation
description: Eine Übersicht über Azure PowerShell mit Links zur Installation und Konfiguration.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.manager: carmonm
ms.date: 09/11/2018
ms.openlocfilehash: 32decf653a956d0b0b202b38a238f42fa831ecae
ms.sourcegitcommit: ff44dec6418a449757bded3c6ebe0a7d4c05ee6e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/01/2018
ms.locfileid: "50737814"
---
# <a name="overview-of-azure-powershell"></a><span data-ttu-id="e6ea4-103">Übersicht über Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="e6ea4-103">Overview of Azure PowerShell</span></span>

<span data-ttu-id="e6ea4-104">Azure PowerShell bietet eine Reihe von Cmdlets, die das [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview)-Modell für die Verwaltung von Azure-Ressourcen verwenden.</span><span class="sxs-lookup"><span data-stu-id="e6ea4-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span> <span data-ttu-id="e6ea4-105">Azure PowerShell kann mit [Azure Cloud Shell](/azure/cloud-shell/overview) im Browser verwendet oder auf dem lokalen Computer installiert und in einer beliebigen PowerShell-Sitzung verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="e6ea4-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can install it on your local machine and use it in any PowerShell session.</span></span>

<span data-ttu-id="e6ea4-106">Verwenden Sie [Cloud Shell](/azure/cloud-shell/overview), um Azure PowerShell in Ihrem Browser auszuführen, oder [installieren](install-azurerm-ps.md) Sie die Lösung auf Ihrem Computer.</span><span class="sxs-lookup"><span data-stu-id="e6ea4-106">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the Azure PowerShell in your browser, or [install](install-azurerm-ps.md) it on own computer.</span></span> <span data-ttu-id="e6ea4-107">Lesen Sie anschließend den Artikel mit den [ersten Schritten](get-started-azureps.md), um mit der Verwendung zu beginnen.</span><span class="sxs-lookup"><span data-stu-id="e6ea4-107">Then read the [Get Started](get-started-azureps.md) article to begin using it.</span></span> <span data-ttu-id="e6ea4-108">Informationen zur neuesten Version finden Sie in den [Versionshinweisen](release-notes-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="e6ea4-108">For information about the latest release, see the [release notes](release-notes-azureps.md).</span></span>

<span data-ttu-id="e6ea4-109">In den folgenden Beispielen werden gängige Szenarien mit Azure PowerShell veranschaulicht:</span><span class="sxs-lookup"><span data-stu-id="e6ea4-109">The following samples can help you learn how to perform common scenarios with Azure PowerShell:</span></span>

* [<span data-ttu-id="e6ea4-110">Virtuelle Linux-Computer</span><span class="sxs-lookup"><span data-stu-id="e6ea4-110">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="e6ea4-111">Virtuelle Windows-Computer</span><span class="sxs-lookup"><span data-stu-id="e6ea4-111">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="e6ea4-112">Web-Apps</span><span class="sxs-lookup"><span data-stu-id="e6ea4-112">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="e6ea4-113">SQL-Datenbanken</span><span class="sxs-lookup"><span data-stu-id="e6ea4-113">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

> [!NOTE]
> <span data-ttu-id="e6ea4-114">Bei nicht konvertierbaren Bereitstellungen mit dem klassischen Bereitstellungsmodell können Sie die Dienstverwaltungsversion von Azure PowerShell installieren.</span><span class="sxs-lookup"><span data-stu-id="e6ea4-114">If you have deployments that use the classic deployment model that cannot be converted, you can install the Service Management version of Azure PowerShell.</span></span> <span data-ttu-id="e6ea4-115">Weitere Informationen finden Sie unter [Installing the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps) (Installieren des Azure PowerShell-Dienstverwaltungsmoduls).</span><span class="sxs-lookup"><span data-stu-id="e6ea4-115">For more information, see [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span>

## <a name="learn-powershell-basics"></a><span data-ttu-id="e6ea4-116">PowerShell-Grundlagen erlernen</span><span class="sxs-lookup"><span data-stu-id="e6ea4-116">Learn PowerShell basics</span></span>

<span data-ttu-id="e6ea4-117">Falls Sie mit PowerShell noch nicht vertraut sind, kann es hilfreich sein, eine Einführung in PowerShell zu lesen.</span><span class="sxs-lookup"><span data-stu-id="e6ea4-117">If you're unfamiliar with PowerShell, an introduction to PowerShell may be helpful.</span></span>

* [<span data-ttu-id="e6ea4-118">Installieren von PowerShell</span><span class="sxs-lookup"><span data-stu-id="e6ea4-118">Installing PowerShell</span></span>](/powershell/scripting/setup/installing-windows-powershell)
* [<span data-ttu-id="e6ea4-119">Skripterstellung mit PowerShell</span><span class="sxs-lookup"><span data-stu-id="e6ea4-119">Scripting with PowerShell</span></span>](/powershell/scripting/powershell-scripting)

<span data-ttu-id="e6ea4-120">Empfehlenswert ist auch folgendes Video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1) (PowerShell-Grundlagen – Teil 1: Erste Schritte mit PowerShell).</span><span class="sxs-lookup"><span data-stu-id="e6ea4-120">You can also watch this video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span></span>

<span data-ttu-id="e6ea4-121">Oder Sie sehen sich in der Microsoft Virtual Academy die Einführung [Getting Started with PowerShell](https://mva.microsoft.com/liveevents/powershell-jumpstart) (Erste Schritte mit PowerShell) an.</span><span class="sxs-lookup"><span data-stu-id="e6ea4-121">Or attend the Microsoft Virtual Academy's [Getting Started with PowerShell Jumpstart](https://mva.microsoft.com/liveevents/powershell-jumpstart).</span></span>

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="e6ea4-122">Erweitern Ihrer Fähigkeiten mit Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="e6ea4-122">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="e6ea4-123">Automatisieren von Azure-Aufgaben mithilfe von Skripts über PowerShell</span><span class="sxs-lookup"><span data-stu-id="e6ea4-123">Automate Azure tasks using scripts with PowerShell</span></span>](/learn/modules/automate-azure-tasks-with-powershell/)
- [<span data-ttu-id="e6ea4-124">Mehr interaktives Lernen...</span><span class="sxs-lookup"><span data-stu-id="e6ea4-124">More interactive learning...</span></span>](/learn/browse/?term=powershell)

## <a name="other-azure-powershell-modules"></a><span data-ttu-id="e6ea4-125">Andere Azure PowerShell-Module</span><span class="sxs-lookup"><span data-stu-id="e6ea4-125">Other Azure PowerShell modules</span></span>

* [<span data-ttu-id="e6ea4-126">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="e6ea4-126">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
* [<span data-ttu-id="e6ea4-127">Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="e6ea4-127">Azure Information Protection</span></span>](/powershell/azure/aip/)
* [<span data-ttu-id="e6ea4-128">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e6ea4-128">Azure Service Fabric</span></span>](/powershell/azure/service-fabric/)
* [<span data-ttu-id="e6ea4-129">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="e6ea4-129">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)
