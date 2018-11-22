---
title: Migrieren von Azure PowerShell-Skripts von AzureRM zu Az
description: Hier lernen Sie die Schritte und Tools kennen, mit denen Sie Skripts vom AzureRM-Modul zum neuen Az-Modul migrieren können.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/07/2018
ms.openlocfilehash: 0c73e7ac1d47a2a97b6136fa481d0adce8de33db
ms.sourcegitcommit: 80a3da199954d0ab78765715fb49793e89a30f12
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2018
ms.locfileid: "52259637"
---
# <a name="migrate-from-azurerm-to-azure-powershell-az"></a><span data-ttu-id="b903e-103">Migrieren von AzureRM zum Az-Modul von Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="b903e-103">Migrate from AzureRM to Azure PowerShell Az</span></span>

<span data-ttu-id="b903e-104">Das Az-Modul bietet die gleichen Features wie AzureRM, verwendet aber kürzere und konsistentere Cmdlet-Namen.</span><span class="sxs-lookup"><span data-stu-id="b903e-104">The Az module has feature parity with AzureRM, but uses shorter and more consistent cmdlet names.</span></span>
<span data-ttu-id="b903e-105">Für die AzureRM-Cmdlets geschriebene Skripts funktionieren nicht automatisch auch mit dem neuen Modul.</span><span class="sxs-lookup"><span data-stu-id="b903e-105">Scripts written for the AzureRM cmdlets won't automatically work with the new module.</span></span> <span data-ttu-id="b903e-106">Zur Vereinfachung des Übergangs bietet Az Tools, die es Ihnen ermöglichen, Ihre bereits vorhandenen Skripts mit AzureRM auszuführen.</span><span class="sxs-lookup"><span data-stu-id="b903e-106">To make the transition easier, Az offers tools to allow you to run your existing scripts using AzureRM.</span></span> <span data-ttu-id="b903e-107">Eine Migration zu einem neuen Befehlssatz ist immer unangenehm. Dieser Artikel hilft Ihnen jedoch dabei, den Umstieg auf das neue Modul in die Wege zu leiten.</span><span class="sxs-lookup"><span data-stu-id="b903e-107">No migration to a new command set is ever convenient, but this article will help you get started on transitioning to the new module.</span></span>

## <a name="ensure-your-existing-scripts-work-with-the-latest-azurerm-release"></a><span data-ttu-id="b903e-108">Vergewissern, dass Ihre vorhandenen Skripts mit der neuesten AzureRM-Version funktionieren</span><span class="sxs-lookup"><span data-stu-id="b903e-108">Ensure your existing scripts work with the latest AzureRM release</span></span>

<span data-ttu-id="b903e-109">Das ist der wichtigste Schritt überhaupt.</span><span class="sxs-lookup"><span data-stu-id="b903e-109">This is the most important step!</span></span> <span data-ttu-id="b903e-110">Führen Sie Ihre vorhandenen Skripts aus, und vergewissern Sie sich, dass sie mit der _neuesten_ Version von AzureRM (__6.12.0__) funktionieren.</span><span class="sxs-lookup"><span data-stu-id="b903e-110">Run your existing scripts, and make sure that they work with the _latest_ release of AzureRM (__6.12.0__).</span></span> <span data-ttu-id="b903e-111">Sollten Ihre Skripts nicht funktionieren, lesen Sie das [AzureRM-Migrationshandbuch](migration-guide.6.0.0.md).</span><span class="sxs-lookup"><span data-stu-id="b903e-111">If your scripts don't work, make sure to read the [AzureRM migration guide](migration-guide.6.0.0.md).</span></span>

## <a name="install-the-azure-powershell-az-module"></a><span data-ttu-id="b903e-112">Installieren des Az-Moduls von Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="b903e-112">Install the Azure PowerShell Az module</span></span>

<span data-ttu-id="b903e-113">Der erste Schritt besteht darin, das Az-Modul auf Ihrer Plattform zu installieren.</span><span class="sxs-lookup"><span data-stu-id="b903e-113">The first step is to install the Az module on your platform.</span></span> <span data-ttu-id="b903e-114">Um Az installieren zu können, müssen Sie AzureRM deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="b903e-114">To install Az, you need to uninstall AzureRM.</span></span>
<span data-ttu-id="b903e-115">In den folgenden Schritten erfahren Sie, wie Sie Ihre bereits vorhandenen Skripts weiterhin ausführen und die Kompatibilität mit älteren Cmdlet-Namen sicherstellen können.</span><span class="sxs-lookup"><span data-stu-id="b903e-115">In the following steps, you'll learn how to keep running your existing scripts and enable compatibility for old cmdlet names.</span></span>

<span data-ttu-id="b903e-116">Gehen Sie zum Installieren des Az-Moduls von Azure PowerShell wie folgt vor:</span><span class="sxs-lookup"><span data-stu-id="b903e-116">To install the Azure PowerShell Az module, follow these steps:</span></span>

* <span data-ttu-id="b903e-117">[Deinstallieren Sie das AzureRM-Modul.](uninstall-azurerm-ps.md)</span><span class="sxs-lookup"><span data-stu-id="b903e-117">[Uninstall the AzureRM module](uninstall-azurerm-ps.md).</span></span> <span data-ttu-id="b903e-118">Achten Sie darauf, _alle_ installierten Versionen von AzureRM zu entfernen, nicht nur die neueste Version.</span><span class="sxs-lookup"><span data-stu-id="b903e-118">Make sure that you remove _all_ installed versions of AzureRM, not just the most recent version.</span></span>
* [<span data-ttu-id="b903e-119">Installieren Sie das Az-Modul.</span><span class="sxs-lookup"><span data-stu-id="b903e-119">Install the Az module</span></span>](install-az-ps.md)

## <a name="a-namealiasesenable-azurerm-alias-mode"></a><span data-ttu-id="b903e-120"><a name="aliases"/>Aktivieren des AzureRM-Aliasmodus</span><span class="sxs-lookup"><span data-stu-id="b903e-120"><a name="aliases"/>Enable AzureRM alias mode</span></span>

<span data-ttu-id="b903e-121">Wenn Sie AzureRM deinstalliert haben und Ihre Skripts mit der neuesten Version von AzureRM funktionieren, können Sie den Kompatibilitätsmodus für das Az-Modul aktivieren.</span><span class="sxs-lookup"><span data-stu-id="b903e-121">With AzureRM uninstalled and your scripts working with the latest AzureRM version, now is the time to enable the compatibility mode for the Az module.</span></span> <span data-ttu-id="b903e-122">Die Kompatibilität wird mithilfe des folgenden Befehls aktiviert:</span><span class="sxs-lookup"><span data-stu-id="b903e-122">Compatibility is enabled with the command:</span></span>

```powershell-interactive
Enable-AzureRmAlias -Scope CurrentUser
```

<span data-ttu-id="b903e-123">Aliase ermöglichen die Verwendung alter Cmdlet-Namen bei installiertem `Az`-Modul.</span><span class="sxs-lookup"><span data-stu-id="b903e-123">Aliases enable the ability to use old cmdlet names with the `Az` module installed.</span></span> <span data-ttu-id="b903e-124">Diese Aliase werden in das Benutzerprofil für den ausgewählten Bereich geschrieben.</span><span class="sxs-lookup"><span data-stu-id="b903e-124">These aliases are written to the user profile for the selected scope.</span></span> <span data-ttu-id="b903e-125">Sollte kein Benutzerprofil vorhanden sein, wird eines erstellt.</span><span class="sxs-lookup"><span data-stu-id="b903e-125">If no user profile exists, one is created.</span></span>

> [!WARNING]
>
> <span data-ttu-id="b903e-126">Sie können für diesen Befehl zwar einen anderen Bereich (`-Scope`) verwenden, dies wird jedoch nicht empfohlen.</span><span class="sxs-lookup"><span data-stu-id="b903e-126">You can use a different `-Scope` for this command, but it's not recommended!</span></span> <span data-ttu-id="b903e-127">Da Aliase in das Benutzerprofil für den ausgewählten Bereich geschrieben werden, empfiehlt es sich, sie auf einen möglichst kleinen Bereich zu beschränken.</span><span class="sxs-lookup"><span data-stu-id="b903e-127">Aliases are written to the user profile for the selected scope, so keep enabling them to as limited a scope as possible.</span></span> <span data-ttu-id="b903e-128">Eine systemweite Aktivierung von Aliasen kann auch zu Problemen für andere Benutzer führen, die `AzureRM` in ihrem lokalen Bereich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="b903e-128">Enabling aliases system-wide could also cause issues for other users which have `AzureRM` installed in their local scope.</span></span>

<span data-ttu-id="b903e-129">Führen Sie Ihre Skripts nach der Aktivierung des Aliasmodus erneut aus, um sich zu vergewissern, dass sie weiterhin wie erwartet funktionieren.</span><span class="sxs-lookup"><span data-stu-id="b903e-129">Once the alias mode is enabled, run your scripts again to confirm that they still function as expected.</span></span> 

## <a name="change-module-imports-and-cmdlet-names"></a><span data-ttu-id="b903e-130">Ändern der Modulimporte und Cmdlet-Namen</span><span class="sxs-lookup"><span data-stu-id="b903e-130">Change module imports and cmdlet names</span></span>

<span data-ttu-id="b903e-131">Ganz allgemein haben sich die Modulnamen geändert, sodass `AzureRM` und `Azure` zu `Az` werden. Gleiches gilt für die Cmdlets.</span><span class="sxs-lookup"><span data-stu-id="b903e-131">In general, the module names have been changed so that `AzureRM` and `Azure` become `Az`, and the same for cmdlets.</span></span>
<span data-ttu-id="b903e-132">So wurde beispielsweise das Modul `AzureRM.Compute` in `Az.Compute` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="b903e-132">For example, the `AzureRM.Compute` module has been renamed to `Az.Compute`.</span></span> <span data-ttu-id="b903e-133">`New-AzureRmVM` wurde zu `New-AzVM`, und `Get-AzureStorageBlob` ist jetzt `Get-AzStorageBlob`.</span><span class="sxs-lookup"><span data-stu-id="b903e-133">`New-AzureRmVM` has become `New-AzVM`, and `Get-AzureStorageBlob` is now `Get-AzStorageBlob`.</span></span>

<span data-ttu-id="b903e-134">Es gibt allerdings Ausnahmen für diese Namensänderung, die Sie kennen sollten, bevor Sie etwas umbenennen:</span><span class="sxs-lookup"><span data-stu-id="b903e-134">There are exceptions to this naming change that you should be aware of before doing any renaming:</span></span>

| <span data-ttu-id="b903e-135">AzureRM-Modul</span><span class="sxs-lookup"><span data-stu-id="b903e-135">AzureRM module</span></span> | <span data-ttu-id="b903e-136">Az-Modul</span><span class="sxs-lookup"><span data-stu-id="b903e-136">Az module</span></span> |
|----------------|-----------|
| <span data-ttu-id="b903e-137">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="b903e-137">AzureRM.DataFactories</span></span> | <span data-ttu-id="b903e-138">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="b903e-138">Az.DataFactory</span></span> |
| <span data-ttu-id="b903e-139">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="b903e-139">AzureRM.DataFactoryV2</span></span> | <span data-ttu-id="b903e-140">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="b903e-140">Az.DataFactory</span></span> |
| <span data-ttu-id="b903e-141">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="b903e-141">AzureRM.RecoveryServices.Backup</span></span> | <span data-ttu-id="b903e-142">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="b903e-142">Az.RecoveryServices</span></span> |
| <span data-ttu-id="b903e-143">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="b903e-143">AzureRM.RecoveryServices.SiteRecovery</span></span> | <span data-ttu-id="b903e-144">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="b903e-144">Az.RecoveryServices</span></span> |

## <a name="summary"></a><span data-ttu-id="b903e-145">Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="b903e-145">Summary</span></span>

<span data-ttu-id="b903e-146">Mithilfe dieser Schritte können Sie alle Ihre bereits vorhandenen Skripts für die Verwendung des neuen Moduls aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="b903e-146">By following these steps, you can update all of your existing scripts to use the new module.</span></span> <span data-ttu-id="b903e-147">Falls Sie Fragen haben oder bei Ihrer Migration Probleme aufgetreten sind, kommentieren Sie diesen Artikel, damit wir die Anweisungen verbessern können.</span><span class="sxs-lookup"><span data-stu-id="b903e-147">If you have any questions or problems with these steps that made your migration difficult, please comment on this article so that we can improve the instructions.</span></span>