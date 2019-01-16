---
title: Einführung in das Az-Modul von Azure PowerShell
description: Hier finden Sie eine Einführung in das neue Az-Modul von Azure PowerShell, das das AzureRM-Modul ersetzt.
ms.date: 12/13/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: d08bca962b6ff65d25135150824b7c24fbd20103
ms.sourcegitcommit: 007a733342f37894d4aaec7a859dc1ca93c00c92
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/04/2019
ms.locfileid: "54012345"
---
# <a name="introducing-the-new-azure-powershell-az-module"></a><span data-ttu-id="4d81a-103">Einführung in das neue Azure PowerShell Az-Modul</span><span class="sxs-lookup"><span data-stu-id="4d81a-103">Introducing the new Azure PowerShell Az module</span></span>

<span data-ttu-id="4d81a-104">Ab Dezember 2018 ist das Az-Modul von Azure PowerShell allgemein verfügbar und jetzt das beabsichtigte PowerShell-Modul für die Interaktion mit Azure.</span><span class="sxs-lookup"><span data-stu-id="4d81a-104">Starting in December 2018, the Azure PowerShell Az module is in general release and now the intended PowerShell module for interacting with Azure.</span></span> <span data-ttu-id="4d81a-105">Az verfügt über kürzere Befehle, verbesserte Stabilität und plattformübergreifende Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="4d81a-105">Az offers shorter commands, improved stability, and cross-platform support.</span></span> <span data-ttu-id="4d81a-106">Darüber hinaus bietet Az die gleichen Features wie AzureRM sowie einen einfachen Migrationspfad.</span><span class="sxs-lookup"><span data-stu-id="4d81a-106">Az also offers feature parity and an easy migration path from AzureRM.</span></span>

<span data-ttu-id="4d81a-107">Az verwendet die .NET Standard-Bibliothek und kann somit unter PowerShell 5.x und PowerShell 6.x ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="4d81a-107">Az uses the .NET Standard library, which means it runs on PowerShell 5.x and PowerShell 6.x.</span></span>
<span data-ttu-id="4d81a-108">Da PowerShell 6.x unter Linux, macOS und Windows ausgeführt werden kann, ist Azure PowerShell jetzt für alle Plattformen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="4d81a-108">Since PowerShell 6.x can run on Linux, macOS, and Windows, Azure PowerShell is now available for all platforms.</span></span>
<span data-ttu-id="4d81a-109">Die Verwendung von .NET Standard ermöglicht die Vereinheitlichung der Codebasis von Azure PowerShell mit minimalen Auswirkungen für die Benutzer.</span><span class="sxs-lookup"><span data-stu-id="4d81a-109">Using .NET Standard allows us to unify the code base of Azure PowerShell with minimal impact on users.</span></span>

<span data-ttu-id="4d81a-110">Da es sich bei Az um ein neues Modul handelt, wurde die Version auf 1.0.0 zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="4d81a-110">Az is a new module, so the version has been reset to 1.0.0.</span></span>

## <a name="upgrade-to-az"></a><span data-ttu-id="4d81a-111">Upgraden auf Az</span><span class="sxs-lookup"><span data-stu-id="4d81a-111">Upgrade to Az</span></span>

<span data-ttu-id="4d81a-112">Allen Benutzern wird empfohlen, ein Upgrade auf das neue Az-Modul durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="4d81a-112">It's recommended that all users upgrade to the new Az module.</span></span> <span data-ttu-id="4d81a-113">Gehen Sie dazu wie folgt vor:</span><span class="sxs-lookup"><span data-stu-id="4d81a-113">To do so:</span></span>

* <span data-ttu-id="4d81a-114">__EMPFOHLEN__: [Deinstallieren Sie das AzureRM-Modul von Azure PowerShell.](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)</span><span class="sxs-lookup"><span data-stu-id="4d81a-114">__RECOMMENDED__: [Uninstall the Azure PowerShell AzureRM module](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)</span></span>
* [<span data-ttu-id="4d81a-115">Installieren Sie das Az-Modul von Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4d81a-115">Install the Azure PowerShell Az module</span></span>](/powershell/azure/install-az-ps)
* <span data-ttu-id="4d81a-116">Aktivieren Sie den Kompatibilitätsmodus, um Aliase für AzureRM-Cmdlets mit `Enable-AzureRMAlias` hinzuzufügen, während Sie sich mit den neuen Befehlen vertraut machen.</span><span class="sxs-lookup"><span data-stu-id="4d81a-116">Enable compatibility mode to add aliases for AzureRM cmdlets with `Enable-AzureRMAlias` while you become familiar with the new command set.</span></span> <span data-ttu-id="4d81a-117">Aktivieren Sie die Aliase __nur__, wenn Sie AzureRM nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="4d81a-117">__Only__ enable aliases if you do not have AzureRM installed.</span></span>

## <a name="migrate-existing-scripts-to-az"></a><span data-ttu-id="4d81a-118">Migrieren bereits vorhandener Skripts zu Az</span><span class="sxs-lookup"><span data-stu-id="4d81a-118">Migrate existing scripts to Az</span></span>

<span data-ttu-id="4d81a-119">Größere Updates können unangenehm sein.</span><span class="sxs-lookup"><span data-stu-id="4d81a-119">Major updates can be inconvenient.</span></span> <span data-ttu-id="4d81a-120">Das Az-Modul verfügt aber über einen Kompatibilitätsmodus, der Ihnen die Verwendung bereits vorhandener Skripts ermöglicht, während Sie sich um die Umstellung auf die neue Syntax kümmern.</span><span class="sxs-lookup"><span data-stu-id="4d81a-120">However, the Az module has a compatibility mode to help you use existing scripts while you work on updates to the new syntax.</span></span> <span data-ttu-id="4d81a-121">Verwenden Sie das Cmdlet `Enable-AzureRmAlias`, um den AzureRM-Kompatibilitätsmodus zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="4d81a-121">Use the `Enable-AzureRmAlias` cmdlet to enable the AzureRM compatibility mode.</span></span> <span data-ttu-id="4d81a-122">Dieses Cmdlet definiert Namen von AzureRM-Cmdlets als Aliase für die neuen Namen von Az-Cmdlets.</span><span class="sxs-lookup"><span data-stu-id="4d81a-122">This cmdlet defines AzureRM cmdlet names as aliases for the new Az cmdlet names.</span></span>

<span data-ttu-id="4d81a-123">Die neuen Cmdlet-Namen sind ganz einfach zu lernen.</span><span class="sxs-lookup"><span data-stu-id="4d81a-123">The new cmdlet names have been designed to be easy to learn.</span></span> <span data-ttu-id="4d81a-124">Verwenden Sie in Cmdlet-Namen nicht mehr `AzureRm` oder `Azure`, sondern `Az`.</span><span class="sxs-lookup"><span data-stu-id="4d81a-124">Instead of using `AzureRm` or `Azure` in cmdlet names, use `Az`.</span></span> <span data-ttu-id="4d81a-125">Der alte Befehl `New-AzureRMVm` lautet nun also beispielsweise `New-AzVm`.</span><span class="sxs-lookup"><span data-stu-id="4d81a-125">For example, the old command `New-AzureRMVm` has become `New-AzVm`.</span></span>

<span data-ttu-id="4d81a-126">Eine umfassende Beschreibung des Migrationsprozesses finden Sie unter [Migrieren von AzureRM zum Az-Modul von Azure PowerShell](migrate-from-azurerm-to-az.md).</span><span class="sxs-lookup"><span data-stu-id="4d81a-126">For a full description of the migration process, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>

## <a name="the-future-of-support-for-azurerm"></a><span data-ttu-id="4d81a-127">Die Zukunft der AzureRM-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="4d81a-127">The future of support for AzureRM</span></span>

<span data-ttu-id="4d81a-128">Für das vorhandene AzureRM-Modul werden keine neuen Cmdlets oder Features mehr bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="4d81a-128">The existing AzureRM module will no longer receive new cmdlets or features.</span></span> <span data-ttu-id="4d81a-129">AzureRM wird bis Dezember 2020 aber weiterhin offiziell gepflegt und mit Fehlerbehebungen versehen.</span><span class="sxs-lookup"><span data-stu-id="4d81a-129">However, AzureRM is still officially maintained and will get bug fixes up through December 2020.</span></span> <span data-ttu-id="4d81a-130">Es ist ratsam, auf das Az-Modul umzusteigen, damit Sie die neuesten Azure-Dienste und -Features nutzen können.</span><span class="sxs-lookup"><span data-stu-id="4d81a-130">To keep up with the latest Azure services and features, switch to the Az module.</span></span>
