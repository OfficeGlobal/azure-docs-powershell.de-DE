---
title: Einführung in das Az-Modul von Azure PowerShell
description: Hier finden Sie eine Einführung in das neue Az-Modul von Azure PowerShell, das das AzureRM-Modul ersetzt.
ms.date: 11/07/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: b0f31341d4344bdac5b4d657a1f66acfd9984dda
ms.sourcegitcommit: 4afdba3cd7e1d348876ce59f3503fdcd258f79ab
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/15/2018
ms.locfileid: "51574803"
---
# <a name="introducing-the-new-azure-powershell-az-module"></a><span data-ttu-id="90f32-103">Einführung in das neue Azure PowerShell Az-Modul</span><span class="sxs-lookup"><span data-stu-id="90f32-103">Introducing the new Azure PowerShell Az module</span></span>

<span data-ttu-id="90f32-104">Ab November 2018 ist das `Az`-Modul von Azure PowerShell als vollständige Public Preview verfügbar.</span><span class="sxs-lookup"><span data-stu-id="90f32-104">Starting in November 2018, the Azure PowerShell `Az` module is available for full public preview.</span></span>
<span data-ttu-id="90f32-105">Az zeichnet sich durch kürzere Befehle und eine verbesserte Stabilität aus und unterstützt Windows, macOS und Linux.</span><span class="sxs-lookup"><span data-stu-id="90f32-105">Az offers shorter commands, improved stability, and supports Windows, macOS, and Linux.</span></span> <span data-ttu-id="90f32-106">Darüber hinaus bietet Az die gleichen Features wie AzureRM sowie einen einfachen Migrationspfad.</span><span class="sxs-lookup"><span data-stu-id="90f32-106">Az also offers feature parity and an easy migration path from AzureRM.</span></span>

<span data-ttu-id="90f32-107">Az verwendet die .NET Standard-Bibliothek und kann somit unter PowerShell 5.x und PowerShell 6.x ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="90f32-107">Az uses the .NET Standard library, which means it runs on PowerShell 5.x and PowerShell 6.x.</span></span>
<span data-ttu-id="90f32-108">Da PowerShell 6.x unter Linux, macOS und Windows ausgeführt werden kann, ist Az für alle Plattformen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="90f32-108">Since PowerShell 6.x can run on Linux, macOS, and Windows, that means Az is available for all platforms.</span></span>
<span data-ttu-id="90f32-109">Die Verwendung von .NET Standard ermöglicht die Vereinheitlichung der Codebasis von Azure PowerShell mit minimalen Auswirkungen für die Benutzer.</span><span class="sxs-lookup"><span data-stu-id="90f32-109">Using .NET Standard allows us to unify the code base of Azure PowerShell with minimal impact on users.</span></span>

<span data-ttu-id="90f32-110">Da es sich bei Az um ein neues Modul handelt, wurde die Version zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="90f32-110">Az is a new module, so the version has been reset.</span></span> <span data-ttu-id="90f32-111">Die erste stabile Version hat die Nummer 1.0, das Modul bietet jedoch die gleichen Features wie AzureRM im November 2018.</span><span class="sxs-lookup"><span data-stu-id="90f32-111">The first stable release will be 1.0, but the module has feature parity with AzureRm as of November 2018.</span></span>

## <a name="upgrade-to-az"></a><span data-ttu-id="90f32-112">Upgraden auf Az</span><span class="sxs-lookup"><span data-stu-id="90f32-112">Upgrade to Az</span></span>

<span data-ttu-id="90f32-113">Benutzern wird empfohlen, ein Upgrade auf das neue `Az`-Modul durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="90f32-113">It's recommended that users upgrade to the new `Az` module.</span></span> <span data-ttu-id="90f32-114">Gehen Sie dazu wie folgt vor:</span><span class="sxs-lookup"><span data-stu-id="90f32-114">To do so:</span></span>

* [<span data-ttu-id="90f32-115">Deinstallieren Sie das AzureRM-Modul von Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="90f32-115">Uninstall the Azure PowerShell AzureRM module</span></span>](/powershell/azure/uninstall-azurerm-ps)
* [<span data-ttu-id="90f32-116">Installieren Sie das Az-Modul von Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="90f32-116">Install the Azure PowerShell Az module</span></span>](/powershell/azure/install-az-ps)
* <span data-ttu-id="90f32-117">Aktivieren Sie den Kompatibilitätsmodus für AzureRM mit `Enable-AzureRMAlias`, während Sie sich mit den neuen Befehlen vertraut machen.</span><span class="sxs-lookup"><span data-stu-id="90f32-117">Enable compatibility mode for AzureRM with `Enable-AzureRMAlias` while you become familiar with the new command set.</span></span>

## <a name="migrate-existing-scripts-to-az"></a><span data-ttu-id="90f32-118">Migrieren bereits vorhandener Skripts zu Az</span><span class="sxs-lookup"><span data-stu-id="90f32-118">Migrate existing scripts to Az</span></span>

<span data-ttu-id="90f32-119">Größere Updates können unangenehm sein.</span><span class="sxs-lookup"><span data-stu-id="90f32-119">Major updates can be inconvenient.</span></span> <span data-ttu-id="90f32-120">Das `Az`-Modul verfügt jedoch über einen Kompatibilitätsmodus, der Ihnen die Verwendung bereits vorhandener Skripts ermöglicht, während Sie sich um die Umstellung auf die neue Syntax kümmern.</span><span class="sxs-lookup"><span data-stu-id="90f32-120">However, the `Az` module has a compatibility mode to help you use existing scripts while you work on updates to the new syntax.</span></span> <span data-ttu-id="90f32-121">Verwenden Sie das Cmdlet `Enable-AzureRmAlias`, um den `AzureRM`-Kompatibilitätsmodus zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="90f32-121">Use the `Enable-AzureRmAlias` cmdlet to enable the `AzureRM` compatibility mode.</span></span> <span data-ttu-id="90f32-122">Dieses Cmdlet definiert Cmdlet-Namen von `AzureRM` als Aliase für die neuen Cmdlet-Namen von `Az`.</span><span class="sxs-lookup"><span data-stu-id="90f32-122">This cmdlet defines `AzureRM` cmdlet names as aliases for the new `Az` cmdlet names.</span></span>

<span data-ttu-id="90f32-123">Die neuen Cmdlet-Namen sind ganz einfach zu lernen.</span><span class="sxs-lookup"><span data-stu-id="90f32-123">The new cmdlet names have been designed to be easy to learn.</span></span> <span data-ttu-id="90f32-124">Verwenden Sie in Cmdlet-Namen nicht mehr `AzureRm` oder `Azure`, sondern `Az`.</span><span class="sxs-lookup"><span data-stu-id="90f32-124">Instead of using `AzureRm` or `Azure` in cmdlet names, use `Az`.</span></span> <span data-ttu-id="90f32-125">Der alte Befehl `New-AzureRmVm` lautet nun also beispielsweise `New-AzVm`.</span><span class="sxs-lookup"><span data-stu-id="90f32-125">For example, the old command `New-AzureRmVm` has become `New-AzVm`.</span></span>

<span data-ttu-id="90f32-126">Eine umfassende Beschreibung des Migrationsprozesses finden Sie unter [Migrieren von AzureRM zum Az-Modul von Azure PowerShell](migrate-from-azurerm-to-az.md).</span><span class="sxs-lookup"><span data-stu-id="90f32-126">For a full description of the migration process, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>

## <a name="the-future-of-support-for-azurerm"></a><span data-ttu-id="90f32-127">Die Zukunft der AzureRM-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="90f32-127">The future of support for AzureRM</span></span>

<span data-ttu-id="90f32-128">Nach Veröffentlichung der Version 1.0 von `Az` im Dezember 2018 werden für das vorhandene `AzureRM`-Modul keine neuen Cmdlets oder Features mehr bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="90f32-128">The existing `AzureRM` module will no longer receive new cmdlets or features when `Az` version 1.0 is released in December 2018.</span></span> <span data-ttu-id="90f32-129">`AzureRM` wird jedoch weiterhin offiziell gepflegt, und es werden weiterhin Fehlerbehebungen bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="90f32-129">However, `AzureRM` is still officially maintained and will get bug fixes.</span></span> <span data-ttu-id="90f32-130">Es empfiehlt sich allerdings, auf das `Az`-Modul umzusteigen, um die neuesten Azure-Dienste und -Features nutzen zu können.</span><span class="sxs-lookup"><span data-stu-id="90f32-130">To keep up with the latest Azure services and features, you should switch to the `Az` module.</span></span>