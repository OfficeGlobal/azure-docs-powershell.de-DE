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
ms.openlocfilehash: bdd8e69a2ea9df8b4fff100e1f3cc4c82d2d9d9d
ms.sourcegitcommit: 80a3da199954d0ab78765715fb49793e89a30f12
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2018
ms.locfileid: "52259709"
---
# <a name="overview-of-azure-powershell"></a><span data-ttu-id="450f8-103">Übersicht über Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="450f8-103">Overview of Azure PowerShell</span></span>

<span data-ttu-id="450f8-104">Azure PowerShell bietet eine Reihe von Cmdlets, die das [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview)-Modell für die Verwaltung von Azure-Ressourcen verwenden.</span><span class="sxs-lookup"><span data-stu-id="450f8-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span> <span data-ttu-id="450f8-105">Azure PowerShell kann mit [Azure Cloud Shell](/azure/cloud-shell/overview) im Browser verwendet oder auf dem lokalen Computer installiert und in einer beliebigen PowerShell-Sitzung verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="450f8-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can install it on your local machine and use it in any PowerShell session.</span></span>

<span data-ttu-id="450f8-106">Verwenden Sie [Cloud Shell](/azure/cloud-shell/overview), um Azure PowerShell in Ihrem Browser auszuführen, oder [installieren](install-azurerm-ps.md) Sie die Lösung auf Ihrem Computer.</span><span class="sxs-lookup"><span data-stu-id="450f8-106">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the Azure PowerShell in your browser, or [install](install-azurerm-ps.md) it on own computer.</span></span> <span data-ttu-id="450f8-107">Lesen Sie anschließend den Artikel mit den [ersten Schritten](get-started-azureps.md), um mit der Verwendung zu beginnen.</span><span class="sxs-lookup"><span data-stu-id="450f8-107">Then read the [Get Started](get-started-azureps.md) article to begin using it.</span></span> <span data-ttu-id="450f8-108">Informationen zur neuesten Version finden Sie in den [Versionshinweisen](release-notes-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="450f8-108">For information about the latest release, see the [release notes](release-notes-azureps.md).</span></span>

<span data-ttu-id="450f8-109">In den folgenden Beispielen werden gängige Szenarien mit Azure PowerShell veranschaulicht:</span><span class="sxs-lookup"><span data-stu-id="450f8-109">The following samples can help you learn how to perform common scenarios with Azure PowerShell:</span></span>

* [<span data-ttu-id="450f8-110">Virtuelle Linux-Computer</span><span class="sxs-lookup"><span data-stu-id="450f8-110">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="450f8-111">Virtuelle Windows-Computer</span><span class="sxs-lookup"><span data-stu-id="450f8-111">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="450f8-112">Web-Apps</span><span class="sxs-lookup"><span data-stu-id="450f8-112">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="450f8-113">SQL-Datenbanken</span><span class="sxs-lookup"><span data-stu-id="450f8-113">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

[!INCLUDE[az-replacing-azurerm](../includes/az-replacing-azurerm.md)]

## <a name="learn-powershell-basics"></a><span data-ttu-id="450f8-114">PowerShell-Grundlagen erlernen</span><span class="sxs-lookup"><span data-stu-id="450f8-114">Learn PowerShell basics</span></span>

<span data-ttu-id="450f8-115">Falls Sie mit PowerShell noch nicht vertraut sind, kann es hilfreich sein, eine Einführung in PowerShell zu lesen.</span><span class="sxs-lookup"><span data-stu-id="450f8-115">If you're unfamiliar with PowerShell, an introduction to PowerShell may be helpful.</span></span>

* [<span data-ttu-id="450f8-116">Installieren von PowerShell</span><span class="sxs-lookup"><span data-stu-id="450f8-116">Installing PowerShell</span></span>](/powershell/scripting/setup/installing-windows-powershell)
* [<span data-ttu-id="450f8-117">Skripterstellung mit PowerShell</span><span class="sxs-lookup"><span data-stu-id="450f8-117">Scripting with PowerShell</span></span>](/powershell/scripting/powershell-scripting)

<span data-ttu-id="450f8-118">Empfehlenswert ist auch folgendes Video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1) (PowerShell-Grundlagen – Teil 1: Erste Schritte mit PowerShell).</span><span class="sxs-lookup"><span data-stu-id="450f8-118">You can also watch this video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span></span>

<span data-ttu-id="450f8-119">Oder Sie sehen sich in der Microsoft Virtual Academy die Einführung [Getting Started with PowerShell](https://mva.microsoft.com/liveevents/powershell-jumpstart) (Erste Schritte mit PowerShell) an.</span><span class="sxs-lookup"><span data-stu-id="450f8-119">Or attend the Microsoft Virtual Academy's [Getting Started with PowerShell Jumpstart](https://mva.microsoft.com/liveevents/powershell-jumpstart).</span></span>

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="450f8-120">Erweitern Ihrer Fähigkeiten mit Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="450f8-120">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="450f8-121">Automatisieren von Azure-Aufgaben mithilfe von Skripts über PowerShell</span><span class="sxs-lookup"><span data-stu-id="450f8-121">Automate Azure tasks using scripts with PowerShell</span></span>](/learn/modules/automate-azure-tasks-with-powershell/)
- [<span data-ttu-id="450f8-122">Mehr interaktives Lernen...</span><span class="sxs-lookup"><span data-stu-id="450f8-122">More interactive learning...</span></span>](/learn/browse/?term=powershell)

## <a name="other-azure-powershell-modules"></a><span data-ttu-id="450f8-123">Andere Azure PowerShell-Module</span><span class="sxs-lookup"><span data-stu-id="450f8-123">Other Azure PowerShell modules</span></span>

* [<span data-ttu-id="450f8-124">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="450f8-124">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
* [<span data-ttu-id="450f8-125">Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="450f8-125">Azure Information Protection</span></span>](/powershell/azure/aip/)
* [<span data-ttu-id="450f8-126">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="450f8-126">Azure Service Fabric</span></span>](/powershell/azure/service-fabric/)
* [<span data-ttu-id="450f8-127">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="450f8-127">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)