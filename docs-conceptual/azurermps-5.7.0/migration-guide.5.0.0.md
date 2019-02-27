---
title: Grundlegende Änderungen für Microsoft Azure PowerShell 5.0.0
description: Dieser Migrationsleitfaden enthält eine Liste mit grundlegenden Änderungen, die in Version 5 an Azure PowerShell vorgenommen wurden.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/01/2018
ms.openlocfilehash: b4cbeb1b523664fb49c4640eaafd56e3b843ebaa
ms.sourcegitcommit: 2054a8f74cd9bf5a50ea7fdfddccaa632c842934
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "56144273"
---
# <a name="breaking-changes-for-microsoft-azure-powershell-500"></a><span data-ttu-id="12878-103">Grundlegende Änderungen für Microsoft Azure PowerShell 5.0.0</span><span class="sxs-lookup"><span data-stu-id="12878-103">Breaking changes for Microsoft Azure PowerShell 5.0.0</span></span>

<span data-ttu-id="12878-104">Dieses Dokument informiert über grundlegende Änderungen und fungiert als Migrationsleitfaden für Kunden mit Microsoft Azure PowerShell-Cmdlets.</span><span class="sxs-lookup"><span data-stu-id="12878-104">This document serves as both a breaking change notification and migration guide for consumers of the Microsoft Azure PowerShell cmdlets.</span></span> <span data-ttu-id="12878-105">In den einzelnen Abschnitten werden jeweils der Grund für die grundlegende Änderung und der Migrationspfad des geringsten Widerstands beschrieben.</span><span class="sxs-lookup"><span data-stu-id="12878-105">Each section describes both the impetus for the breaking change and the migration path of least resistance.</span></span> <span data-ttu-id="12878-106">Ausführlichen Kontext finden Sie unter der Pull-Anforderung für die jeweilige Änderung.</span><span class="sxs-lookup"><span data-stu-id="12878-106">For in-depth context, please refer to the pull request associated with each change.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="12878-107">Inhaltsverzeichnis</span><span class="sxs-lookup"><span data-stu-id="12878-107">Table of Contents</span></span>

- [<span data-ttu-id="12878-108">Grundlegende Änderungen für ApiManagement-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="12878-108">Breaking changes to ApiManagement cmdlets</span></span>](#breaking-changes-to-apimanagement-cmdlets)
- [<span data-ttu-id="12878-109">Grundlegende Änderungen für Batch-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="12878-109">Breaking changes to Batch cmdlets</span></span>](#breaking-changes-to-batch-cmdlets)
- [<span data-ttu-id="12878-110">Grundlegende Änderungen für Compute-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="12878-110">Breaking changes to Compute cmdlets</span></span>](#breaking-changes-to-compute-cmdlets)
- [<span data-ttu-id="12878-111">Grundlegende Änderungen für EventHub-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="12878-111">Breaking changes to EventHub cmdlets</span></span>](#breaking-changes-to-eventhub-cmdlets)
- [<span data-ttu-id="12878-112">Grundlegende Änderungen für Insights-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="12878-112">Breaking changes to Insights cmdlets</span></span>](#breaking-changes-to-insights-cmdlets)
- [<span data-ttu-id="12878-113">Grundlegende Änderungen für Network-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="12878-113">Breaking changes to Network cmdlets</span></span>](#breaking-changes-to-network-cmdlets)
- [<span data-ttu-id="12878-114">Grundlegende Änderungen für Resources-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="12878-114">Breaking changes to Resources cmdlets</span></span>](#breaking-changes-to-resources-cmdlets)
- [<span data-ttu-id="12878-115">Grundlegende Änderungen für ServiceBus-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="12878-115">Breaking Changes to ServiceBus Cmdlets</span></span>](#breaking-changes-to-servicebus-cmdlets)

## <a name="breaking-changes-to-apimanagement-cmdlets"></a><span data-ttu-id="12878-116">Grundlegende Änderungen für ApiManagement-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="12878-116">Breaking changes to ApiManagement cmdlets</span></span>

### <a name="new-azurermapimanagementbackendproxy"></a><span data-ttu-id="12878-117">**New-AzureRmApiManagementBackendProxy**</span><span class="sxs-lookup"><span data-stu-id="12878-117">**New-AzureRmApiManagementBackendProxy**</span></span>
- <span data-ttu-id="12878-118">Die Parameter „UserName“ und „Password“ werden durch ein PSCredential-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-118">Parameters "UserName" and "Password" are being replaced in favor of a PSCredential</span></span>

```powershell-interactive
# Old
New-AzureRmApiManagementBackendProxy [other required parameters] -UserName "plain-text string" -Password "plain-text string"

# New
New-AzureRmApiManagementBackendProxy [other required parameters] -Credential $PSCredentialVariable
```

### <a name="new-azurermapimanagementuser"></a><span data-ttu-id="12878-119">**New-AzureRmApiManagementUser**</span><span class="sxs-lookup"><span data-stu-id="12878-119">**New-AzureRmApiManagementUser**</span></span>
- <span data-ttu-id="12878-120">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-120">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
New-AzureRmApiManagementUser [other required parameters] -Password "plain-text string"

# New
New-AzureRmApiManagementUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermapimanagementuser"></a><span data-ttu-id="12878-121">**Set-AzureRmApiManagementUser**</span><span class="sxs-lookup"><span data-stu-id="12878-121">**Set-AzureRmApiManagementUser**</span></span>
- <span data-ttu-id="12878-122">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-122">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
Set-AzureRmApiManagementUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmApiManagementUser [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-batch-cmdlets"></a><span data-ttu-id="12878-123">Grundlegende Änderungen für Batch-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="12878-123">Breaking changes to Batch cmdlets</span></span>

### <a name="new-azurebatchcertificate"></a><span data-ttu-id="12878-124">**New-AzureBatchCertificate**</span><span class="sxs-lookup"><span data-stu-id="12878-124">**New-AzureBatchCertificate**</span></span>
- <span data-ttu-id="12878-125">Der Parameter `Password` wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-125">Parameter `Password` being replaced in favor of a Secure string</span></span>

```powershell-interactive
# Old
New-AzureBatchCertificate [other required parameters] -Password "plain-text string"

# New
New-AzureBatchCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurebatchcomputenodeuser"></a><span data-ttu-id="12878-126">**New-AzureBatchComputeNodeUser**</span><span class="sxs-lookup"><span data-stu-id="12878-126">**New-AzureBatchComputeNodeUser**</span></span>
- <span data-ttu-id="12878-127">Der Parameter `Password` wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-127">Parameter `Password` being replaced in favor of a Secure string</span></span>

```powershell-interactive
# Old
New-AzureBatchComputeNodeUser [other required parameters] -Password "plain-text string"

# New
New-AzureBatchComputeNodeUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermbatchcomputenodeuser"></a><span data-ttu-id="12878-128">**Set-AzureRmBatchComputeNodeUser**</span><span class="sxs-lookup"><span data-stu-id="12878-128">**Set-AzureRmBatchComputeNodeUser**</span></span>
- <span data-ttu-id="12878-129">Der Parameter `Password` wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-129">Parameter `Password` being replaced in favor of a Secure string</span></span>

```powershell-interactive
# Old
Set-AzureRmBatchComputeNodeUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmBatchComputeNodeUser [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurebatchtask"></a><span data-ttu-id="12878-130">**New-AzureBatchTask**</span><span class="sxs-lookup"><span data-stu-id="12878-130">**New-AzureBatchTask**</span></span>
 - <span data-ttu-id="12878-131">Der Switch `RunElevated` wurde entfernt und durch `UserIdentity` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-131">Removed the `RunElevated` switch and replaced it with `UserIdentity`.</span></span>

```powershell-interactive
# Old
New-AzureBatchTask -Id $taskId1 -JobId $jobId -CommandLine "cmd /c echo hello" -RunElevated $TRUE

# New
$autoUser = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoUserSpecification -ArgumentList @("Task", "Admin")
$userIdentity = New-Object Microsoft.Azure.Commands.Batch.Models.PSUserIdentity $autoUser
New-AzureBatchTask -Id $taskId1 -JobId $jobId -CommandLine "cmd /c echo hello" -UserIdentity $userIdentity
```

<span data-ttu-id="12878-132">Dies betrifft auch die Eigenschaft `RunElevated` für `PSCloudTask`, `PSStartTask`, `PSJobManagerTask`, `PSJobPreparationTask` und `PSJobReleaseTask`.</span><span class="sxs-lookup"><span data-stu-id="12878-132">This additionally impacts the `RunElevated` property on `PSCloudTask`, `PSStartTask`, `PSJobManagerTask`, `PSJobPreparationTask`, and `PSJobReleaseTask`.</span></span>

### <a name="psmultiinstancesettings"></a><span data-ttu-id="12878-133">**PSMultiInstanceSettings**</span><span class="sxs-lookup"><span data-stu-id="12878-133">**PSMultiInstanceSettings**</span></span>

- <span data-ttu-id="12878-134">Der Konstruktor `PSMultiInstanceSettings` akzeptiert anstelle eines erforderlichen `numberOfInstances`-Parameters und einen erforderlichen `coordinationCommandLine`-Parameter.</span><span class="sxs-lookup"><span data-stu-id="12878-134">`PSMultiInstanceSettings` constructor no longer takes a required `numberOfInstances` parameter, instead it takes a required `coordinationCommandLine` parameter.</span></span>

```powershell-interactive
# Old
$settings = New-Object Microsoft.Azure.Commands.Batch.Models.PSMultiInstanceSettings -ArgumentList @(2)
$settings.CoordinationCommandLine = "cmd /c echo hello"
New-AzureBatchTask [other parameters] -MultiInstanceSettings $settings

# New
$settings = New-Object Microsoft.Azure.Commands.Batch.Models.PSMultiInstanceSettings -ArgumentList @("cmd /c echo hello", 2)
New-AzureBatchTask [other parameters] -MultiInstanceSettings $settings
```

### <a name="get-azurebatchtask"></a><span data-ttu-id="12878-135">**Get-AzureBatchTask**</span><span class="sxs-lookup"><span data-stu-id="12878-135">**Get-AzureBatchTask**</span></span>
 - <span data-ttu-id="12878-136">Die Eigenschaft `RunElevated` für `PSCloudTask` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-136">Removed the `RunElevated` property on `PSCloudTask`.</span></span> <span data-ttu-id="12878-137">Als Ersatz für `RunElevated` wurde die Eigenschaft `UserIdentity` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="12878-137">The `UserIdentity` property has been added to replace `RunElevated`.</span></span>

```powershell-interactive
# Old
$task = Get-AzureBatchTask [parameters]
$task.RunElevated

# New
$task = Get-AzureBatchTask [parameters]
$task.UserIdentity.AutoUser.ElevationLevel
```

<span data-ttu-id="12878-138">Dies betrifft auch die Eigenschaft `RunElevated` für `PSCloudTask`, `PSStartTask`, `PSJobManagerTask`, `PSJobPreparationTask` und `PSJobReleaseTask`.</span><span class="sxs-lookup"><span data-stu-id="12878-138">This additionally impacts the `RunElevated` property on `PSCloudTask`, `PSStartTask`, `PSJobManagerTask`, `PSJobPreparationTask`, and `PSJobReleaseTask`.</span></span>

### <a name="multiple-types"></a><span data-ttu-id="12878-139">**Mehrere Typen**</span><span class="sxs-lookup"><span data-stu-id="12878-139">**Multiple types**</span></span>

- <span data-ttu-id="12878-140">Die Eigenschaft `SchedulingError` für `PSExitConditions` wurde in `PreProcessingError` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="12878-140">Renamed the `SchedulingError` property on `PSExitConditions` to `PreProcessingError`.</span></span>

```powershell-interactive
# Old
$task = Get-AzureBatchTask [parameters]
$task.ExitConditions.SchedulingError

# New
$task = Get-AzureBatchTask [parameters]
$task.ExitConditions.PreProcessingError
```

### <a name="multiple-types"></a><span data-ttu-id="12878-141">**Mehrere Typen**</span><span class="sxs-lookup"><span data-stu-id="12878-141">**Multiple types**</span></span>

- <span data-ttu-id="12878-142">Die Eigenschaft `SchedulingError` für `PSJobPreparationTaskExecutionInformation`, `PSJobReleaseTaskExecutionInformation`, `PSStartTaskInformation`, `PSSubtaskInformation` und `PSTaskExecutionInformation` wurde in `FailureInformation` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="12878-142">Renamed the `SchedulingError` property on `PSJobPreparationTaskExecutionInformation`, `PSJobReleaseTaskExecutionInformation`, `PSStartTaskInformation`, `PSSubtaskInformation`, and `PSTaskExecutionInformation` to `FailureInformation`.</span></span>
  - <span data-ttu-id="12878-143">`FailureInformation` wird im Falle eines Aufgabenfehlers zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12878-143">`FailureInformation` is returned any time there is a task failure.</span></span> <span data-ttu-id="12878-144">Dazu zählen alle vorherigen Planungsfehler sowie Exitcodes ungleich Null und Dateiuploadfehler aus dem neuen Ausgabedateienfeature.</span><span class="sxs-lookup"><span data-stu-id="12878-144">This includes all previous scheduling error cases, as well as nonzero task exit codes, and file upload failures from the new output files feature.</span></span>
  - <span data-ttu-id="12878-145">Da die Struktur unverändert bleibt, sind zur Verwendung dieses Typs keine Codeänderungen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="12878-145">This is structured the same as before, so no code change is needed when using this type.</span></span>

```powershell-interactive
# Old
$task = Get-AzureBatchTask [parameters]
$task.ExecutionInformation.SchedulingError

# New
$task = Get-AzureBatchTask [parameters]
$task.ExecutionInformation.FailureInformation
```

<span data-ttu-id="12878-146">Dies wirkt sich auch auf Folgendes aus: Get-AzureBatchPool, Get-AzureBatchSubtask und Get-AzureBatchJobPreparationAndReleaseTaskStatus</span><span class="sxs-lookup"><span data-stu-id="12878-146">This additionally impacts: Get-AzureBatchPool, Get-AzureBatchSubtask, and Get-AzureBatchJobPreparationAndReleaseTaskStatus</span></span>

### <a name="new-azurebatchpool"></a><span data-ttu-id="12878-147">**New-AzureBatchPool**</span><span class="sxs-lookup"><span data-stu-id="12878-147">**New-AzureBatchPool**</span></span>
 - <span data-ttu-id="12878-148">`TargetDedicated` wurde entfernt und durch `TargetDedicatedComputeNodes` und `TargetLowPriorityComputeNodes` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-148">Removed `TargetDedicated` and replaced it with `TargetDedicatedComputeNodes` and `TargetLowPriorityComputeNodes`.</span></span>
 - <span data-ttu-id="12878-149">`TargetDedicatedComputeNodes` besitzt einen Alias (`TargetDedicated`).</span><span class="sxs-lookup"><span data-stu-id="12878-149">`TargetDedicatedComputeNodes` has an alias `TargetDedicated`.</span></span>

```powershell-interactive
# Old
New-AzureBatchPool [other parameters] [-TargetDedicated <Int32>]

# New
New-AzureBatchPool [other parameters] [-TargetDedicatedComputeNodes <Int32>] [-TargetLowPriorityComputeNodes <Int32>]
```

<span data-ttu-id="12878-150">Dies wirkt sich auch auf Folgendes aus: Start-AzureBatchPoolResize</span><span class="sxs-lookup"><span data-stu-id="12878-150">This also impacts: Start-AzureBatchPoolResize</span></span>

### <a name="get-azurebatchpool"></a><span data-ttu-id="12878-151">**Get-AzureBatchPool**</span><span class="sxs-lookup"><span data-stu-id="12878-151">**Get-AzureBatchPool**</span></span>
 - <span data-ttu-id="12878-152">Die Eigenschaften `TargetDedicated` und `CurrentDedicated` für `PSCloudPool` wurden in `TargetDedicatedComputeNodes` und `CurrentDedicatedComputeNodes` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="12878-152">Renamed the `TargetDedicated` and `CurrentDedicated` properties on `PSCloudPool` to `TargetDedicatedComputeNodes` and `CurrentDedicatedComputeNodes`.</span></span>

```powershell-interactive
# Old
$pool = Get-AzureBatchPool [parameters]
$pool.TargetDedicated
$pool.CurrentDedicated

# New
$pool = Get-AzureBatchPool [parameters]
$pool.TargetDedicatedComputeNodes
$pool.CurrentDedicatedComputeNodes
```

### <a name="type-pscloudpool"></a><span data-ttu-id="12878-153">**Typ „PSCloudPool“**</span><span class="sxs-lookup"><span data-stu-id="12878-153">**Type PSCloudPool**</span></span>

- <span data-ttu-id="12878-154">`ResizeError` wurde für `PSCloudPool` in `ResizeErrors` umbenannt und ist nun eine Sammlung.</span><span class="sxs-lookup"><span data-stu-id="12878-154">Renamed `ResizeError` to `ResizeErrors` on `PSCloudPool`, and it is now a collection.</span></span>

```powershell-interactive
# Old
$pool = Get-AzureBatchPool [parameters]
$pool.ResizeError

# New
$pool = Get-AzureBatchPool [parameters]
$pool.ResizeErrors[0]
```

### <a name="new-azurebatchjob"></a><span data-ttu-id="12878-155">**New-AzureBatchJob**</span><span class="sxs-lookup"><span data-stu-id="12878-155">**New-AzureBatchJob**</span></span>
- <span data-ttu-id="12878-156">Die Eigenschaft `TargetDedicated` für `PSPoolSpecification` wurde in `TargetDedicatedComputeNodes` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="12878-156">Renamed the `TargetDedicated` property on `PSPoolSpecification` to `TargetDedicatedComputeNodes`.</span></span>

```powershell-interactive
# Old
$poolInfo = New-Object Microsoft.Azure.Commands.Batch.Models.PSPoolInformation
$poolInfo.AutoPoolSpecification = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoPoolSpecification
$poolInfo.AutoPoolSpecification.PoolSpecification = New-Object Microsoft.Azure.Commands.Batch.Models.PSPoolSpecification
$poolInfo.AutoPoolSpecification.PoolSpecification.TargetDedicated = 5
New-AzureBatchJob [other parameters] -PoolInformation $poolInfo

# New
$poolInfo = New-Object Microsoft.Azure.Commands.Batch.Models.PSPoolInformation
$poolInfo.AutoPoolSpecification = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoPoolSpecification
$poolInfo.AutoPoolSpecification.PoolSpecification = New-Object Microsoft.Azure.Commands.Batch.Models.PSPoolSpecification
$poolInfo.AutoPoolSpecification.PoolSpecification.TargetDedicatedComputeNodes = 5
New-AzureBatchJob [other parameters] -PoolInformation $poolInfo
```

### <a name="get-azurebatchnodefile"></a><span data-ttu-id="12878-157">**Get-AzureBatchNodeFile**</span><span class="sxs-lookup"><span data-stu-id="12878-157">**Get-AzureBatchNodeFile**</span></span>
 - <span data-ttu-id="12878-158">`Name` wurde entfernt und durch `Path` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-158">Removed `Name` and replaced it with `Path`.</span></span>
 - <span data-ttu-id="12878-159">`Path` besitzt einen Alias (`Name`).</span><span class="sxs-lookup"><span data-stu-id="12878-159">`Path` has an alias `Name`.</span></span>

```powershell-interactive
# Old
Get-AzureBatchNodeFile [other parameters] [[-Name] <String>]

# New
Get-AzureBatchNodeFile [other parameters] [[-Path] <String>]
```

<span data-ttu-id="12878-160">Dies wirkt sich auch auf Folgendes aus: Get-AzureBatchNodeFileContent, Remove-AzureBatchNodeFile</span><span class="sxs-lookup"><span data-stu-id="12878-160">This also impacts: Get-AzureBatchNodeFileContent, Remove-AzureBatchNodeFile</span></span>

### <a name="type-psnodefile"></a><span data-ttu-id="12878-161">**Typ „PSNodeFile“**</span><span class="sxs-lookup"><span data-stu-id="12878-161">Type **PSNodeFile**</span></span>

 - <span data-ttu-id="12878-162">Die Eigenschaft `Name` für `PSNodeFile` wurde in `Path` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="12878-162">Renamed the `Name` property on `PSNodeFile` to `Path`.</span></span>

```powershell-interactive
# Old
$file = Get-AzureBatchNodeFile [parameters]
$file.Name

# New
$file = Get-AzureBatchNodeFile [parameters]
$file.Path
```

### <a name="get-azurebatchsubtask"></a><span data-ttu-id="12878-163">**Get-AzureBatchSubtask**</span><span class="sxs-lookup"><span data-stu-id="12878-163">**Get-AzureBatchSubtask**</span></span>
- <span data-ttu-id="12878-164">Die Eigenschaften `PreviousState` und `State` von `PSSubtaskInformation` sind nicht mehr vom Typ `TaskState`, sondern vom Typ `SubtaskState`.</span><span class="sxs-lookup"><span data-stu-id="12878-164">The `PreviousState` and `State` properties of `PSSubtaskInformation` are no longer of type `TaskState`, instead they are of type `SubtaskState`.</span></span>
  - <span data-ttu-id="12878-165">Im Gegensatz zu `TaskState` besitzt `SubtaskState` keinen Wert vom Typ `Active`, da sich Unteraufgaben nicht im Zustand `Active` befinden können.</span><span class="sxs-lookup"><span data-stu-id="12878-165">Unlike `TaskState`, `SubtaskState` has no `Active` value, since it is not possible for subtasks to be in an `Active` state.</span></span>

```powershell-interactive
# Old
$subtask = Get-AzureBatchSubtask [parameters]
if ($subtask.State -eq Microsoft.Azure.Batch.Common.TaskState.Running) { }

# New
$subtask = Get-AzureBatchSubtask [parameters]
if ($subtask.State -eq Microsoft.Azure.Batch.Common.SubtaskState.Running) { }
```

## <a name="breaking-changes-to-compute-cmdlets"></a><span data-ttu-id="12878-166">Grundlegende Änderungen für Compute-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="12878-166">Breaking changes to Compute cmdlets</span></span>

### <a name="set-azurermvmaccessextension"></a><span data-ttu-id="12878-167">**Set-AzureRmVMAccessExtension**</span><span class="sxs-lookup"><span data-stu-id="12878-167">**Set-AzureRmVMAccessExtension**</span></span>
- <span data-ttu-id="12878-168">Die Parameter „UserName“ und „Password“ werden durch ein PSCredential-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-168">Parameters "UserName" and "Password" are being replaced in favor of a PSCredential</span></span>

```powershell-interactive
# Old
Set-AzureRmVMAccessExtension [other required parameters] -UserName "plain-text string" -Password "plain-text string"

# New
Set-AzureRmVMAccessExtension [other required parameters] -Credential $PSCredential
```

## <a name="breaking-changes-to-eventhub-cmdlets"></a><span data-ttu-id="12878-169">Grundlegende Änderungen für EventHub-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="12878-169">Breaking changes to EventHub cmdlets</span></span>

### <a name="new-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="12878-170">**New-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="12878-170">**New-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="12878-171">Das Cmdlet „New-AzureRmEventHubNamespaceAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-171">The 'New-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="12878-172">Verwenden Sie das Cmdlet „New-AzureRmEventHubAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="12878-172">Please use the 'New-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="get-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="12878-173">**Get-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="12878-173">**Get-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="12878-174">Das Cmdlet „Get-AzureRmEventHubNamespaceAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-174">The 'Get-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="12878-175">Verwenden Sie das Cmdlet „Get-AzureRmEventHubAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="12878-175">Please use the 'Get-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="set-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="12878-176">**Set-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="12878-176">**Set-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="12878-177">Das Cmdlet „Set-AzureRmEventHubNamespaceAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-177">The 'Set-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="12878-178">Verwenden Sie das Cmdlet „Set-AzureRmEventHubAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="12878-178">Please use the 'Set-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="remove-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="12878-179">**Remove-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="12878-179">**Remove-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="12878-180">Das Cmdlet „Remove-AzureRmEventHubNamespaceAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-180">The 'Remove-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="12878-181">Verwenden Sie das Cmdlet „Remove-AzureRmEventHubAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="12878-181">Please use the 'Remove-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="new-azurermeventhubnamespacekey"></a><span data-ttu-id="12878-182">**New-AzureRmEventHubNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="12878-182">**New-AzureRmEventHubNamespaceKey**</span></span>
- <span data-ttu-id="12878-183">Das Cmdlet „New-AzureRmEventHubNamespaceKey“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-183">The 'New-AzureRmEventHubNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="12878-184">Verwenden Sie das Cmdlet „New-AzureRmEventHubKey“.</span><span class="sxs-lookup"><span data-stu-id="12878-184">Please use the 'New-AzureRmEventHubKey' cmdlet</span></span>
    
### <a name="get-azurermeventhubnamespacekey"></a><span data-ttu-id="12878-185">**Get-AzureRmEventHubNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="12878-185">**Get-AzureRmEventHubNamespaceKey**</span></span>
- <span data-ttu-id="12878-186">Das Cmdlet „Get-AzureRmEventHubNamespaceKey“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-186">The 'Get-AzureRmEventHubNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="12878-187">Verwenden Sie das Cmdlet „Get-AzureRmEventHubKey“.</span><span class="sxs-lookup"><span data-stu-id="12878-187">Please use the 'Get-AzureRmEventHubKey' cmdlet</span></span>
    
### <a name="new-azurermeventhubnamespace"></a><span data-ttu-id="12878-188">**New-AzureRmEventHubNamespace**</span><span class="sxs-lookup"><span data-stu-id="12878-188">**New-AzureRmEventHubNamespace**</span></span>
- <span data-ttu-id="12878-189">Die Eigenschaften „Status“ und „Enabled“ aus den Namespaceattributen werden entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-189">The property 'Status' and 'Enabled' from the NamespceAttributes will be removed.</span></span> 

```powershell-interactive
# Old
# The $namespace has Status and Enabled property  
$namespace = New-AzureRmEventHubNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Status and Enabled property    
$namespace = Get-AzureRmEventHubNamespace <parameters>
```
    
### <a name="get-azurermeventhubnamespace"></a><span data-ttu-id="12878-190">**Get-AzureRmEventHubNamespace**</span><span class="sxs-lookup"><span data-stu-id="12878-190">**Get-AzureRmEventHubNamespace**</span></span>
- <span data-ttu-id="12878-191">Die Eigenschaften „Status“ und „Enabled“ aus den Namespaceattributen werden entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-191">The property 'Status' and 'Enabled' from the NamespceAttributes will be removed.</span></span> 

```powershell-interactive
# Old
# The $namespace has Status and Enabled property 
$namespace = Get-AzureRmEventHubNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Status and Enabled property    
$namespace = Get-AzureRmEventHubNamespace <parameters>
```
    
### <a name="set-azurermeventhubnamespace"></a><span data-ttu-id="12878-192">**Set-AzureRmEventHubNamespace**</span><span class="sxs-lookup"><span data-stu-id="12878-192">**Set-AzureRmEventHubNamespace**</span></span>
- <span data-ttu-id="12878-193">Die Eigenschaften „Status“ und „Enabled“ aus den Namespaceattributen werden entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-193">The property 'Status' and 'Enabled' from the NamespceAttributes will be removed.</span></span> 

```powershell-interactive
# Old
# The $namespace has Status and Enabled property 
$namespace = Set-AzureRmEventHubNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Status and Enabled property    
$namespace = Set-AzureRmEventHubNamespace <parameters>
``` 
  
### <a name="new-azurermeventhubconsumergroup"></a><span data-ttu-id="12878-194">**New-AzureRmEventHubConsumerGroup**</span><span class="sxs-lookup"><span data-stu-id="12878-194">**New-AzureRmEventHubConsumerGroup**</span></span>
- <span data-ttu-id="12878-195">Die Eigenschaft „EventHubPath“ aus den ConsumerGroup-Attributen wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-195">The property 'EventHubPath' from the ConsumerGroupAttributes will be removed.</span></span>

```powershell-interactive
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = New-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = New-AzureRmEventHubConsumerGroup <parameters>
```
    
### <a name="set-azurermeventhubconsumergroup"></a><span data-ttu-id="12878-196">**Set-AzureRmEventHubConsumerGroup**</span><span class="sxs-lookup"><span data-stu-id="12878-196">**Set-AzureRmEventHubConsumerGroup**</span></span>
- <span data-ttu-id="12878-197">Die Eigenschaft „EventHubPath“ aus den ConsumerGroup-Attributen wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-197">The property 'EventHubPath' from the ConsumerGroupAttributes will be removed.</span></span>

```powershell-interactive
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = Set-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = Set-AzureRmEventHubConsumerGroup <parameters>
```
    
### <a name="get-azurermeventhubconsumergroup"></a><span data-ttu-id="12878-198">**Get-AzureRmEventHubConsumerGroup**</span><span class="sxs-lookup"><span data-stu-id="12878-198">**Get-AzureRmEventHubConsumerGroup**</span></span>
- <span data-ttu-id="12878-199">Die Eigenschaft „EventHubPath“ aus den ConsumerGroup-Attributen wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-199">The property 'EventHubPath' from the ConsumerGroupAttributes will be removed.</span></span>

```powershell-interactive
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = Get-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = Get-AzureRmEventHubConsumerGroup <parameters>
```

## <a name="breaking-changes-to-insights-cmdlets"></a><span data-ttu-id="12878-200">Grundlegende Änderungen für Insights-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="12878-200">Breaking changes to Insights cmdlets</span></span>

### <a name="add-azurermlogalertrule"></a><span data-ttu-id="12878-201">**Add-AzureRMLogAlertRule**</span><span class="sxs-lookup"><span data-stu-id="12878-201">**Add-AzureRMLogAlertRule**</span></span>
- <span data-ttu-id="12878-202">Das Cmdlet **Add-AzureRMLogAlertRule** ist veraltet.</span><span class="sxs-lookup"><span data-stu-id="12878-202">The **Add-AzureRMLogAlertRule** cmdlet has been deprecated</span></span>
- <span data-ttu-id="12878-203">Nach dem 1. Oktober hat die Verwendung dieses Cmdlets keine Wirkung mehr, da die Funktion in Aktivitätsprotokollwarnungen übertragen wurde.</span><span class="sxs-lookup"><span data-stu-id="12878-203">After October 1st using this cmdlet will no longer have any effect as this functionality is being transitioned to Activity Log Alerts.</span></span> <span data-ttu-id="12878-204">Unter https://aka.ms/migratemealerts finden Sie weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="12878-204">Please see https://aka.ms/migratemealerts for more information.</span></span>

### <a name="get-azurermusage"></a><span data-ttu-id="12878-205">**Get-AzureRMUsage**</span><span class="sxs-lookup"><span data-stu-id="12878-205">**Get-AzureRMUsage**</span></span>
- <span data-ttu-id="12878-206">Das Cmdlet **Get-AzureRMUsage** ist veraltet.</span><span class="sxs-lookup"><span data-stu-id="12878-206">The **Get-AzureRMUsage** cmdlet has been deprecated</span></span>

### <a name="get-azurermalerthistory--get-azurermautoscalehistory--get-azurermlogs"></a><span data-ttu-id="12878-207">**Get-AzureRmAlertHistory**/**Get-AzureRmAutoscaleHistory**/**Get-AzureRmLogs**</span><span class="sxs-lookup"><span data-stu-id="12878-207">**Get-AzureRmAlertHistory** / **Get-AzureRmAutoscaleHistory** / **Get-AzureRmLogs**</span></span>
- <span data-ttu-id="12878-208">Ausgabeänderung: Das Feld „EventChannels“ aus dem EventData-Objekt (das von diesen Cmdlets zurückgegeben wird) wird ausgemustert, da nun ein konstanter Wert (Administrator, Vorgang) zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="12878-208">Output change: The field EventChannels from the EventData object (returned by these cmdlets) is being deprecated since it now returns a constant value (Admin,Operation.)</span></span>

### <a name="get-azurermalertrule"></a><span data-ttu-id="12878-209">**Get-AzureRmAlertRule**</span><span class="sxs-lookup"><span data-stu-id="12878-209">**Get-AzureRmAlertRule**</span></span>
- <span data-ttu-id="12878-210">Ausgabeänderung: Zur Verbesserung der Benutzerfreundlichkeit wird die Ausgabe dieses Cmdlets vereinfacht. (Das Eigenschaftenfeld wird entfernt.)</span><span class="sxs-lookup"><span data-stu-id="12878-210">Output change: The output of this cmdlet will be flattened, i.e. elimination of the properties field, to improve the user experience.</span></span>

```powershell-interactive
# Old
$rules = Get-AzureRmAlertRule -ResourceGroup $resourceGroup
if ($rules -and $rules.count -ge 1)
{
    Write-Host -Foreground Red "Error updating alert rule"
    Write-Host $rules[0].Id
    Write-Host $rules[0].Properties.IsEnabled
    Write-Host $rules[0].Properties.Condition
}

# New
$rules = Get-AzureRmAlertRule -ResourceGroup $resourceGroup
if ($rules -and $rules.count -ge 1)
{
    Write-Host -Foreground red "Error updating alert rule"
    Write-Host $rules[0].Id

    # Properties will remain for a while
    Write-Host $rules[0].Properties.IsEnabled
      
    # But the properties will be at the top level too. Later Properties will be removed
    Write-Host $rules[0].IsEnabled
    Write-Host $rules[0].Condition
}
```

### <a name="get-azurermautoscalesetting"></a><span data-ttu-id="12878-211">**Get-AzureRmAutoscaleSetting**</span><span class="sxs-lookup"><span data-stu-id="12878-211">**Get-AzureRmAutoscaleSetting**</span></span>
- <span data-ttu-id="12878-212">Ausgabeänderung: Das Feld „AutoscaleSettingResourceName“ wird ausgemustert, da es immer dem Feld „Name“ entspricht.</span><span class="sxs-lookup"><span data-stu-id="12878-212">Output change: The AutoscaleSettingResourceName field will be deprecated since it always equals the Name field.</span></span>

```powershell-interactive
# Old
$s1 = Get-AzureRmAutoscaleSetting -ResourceGroup $resourceGroup -Name MySetting
if ($s1.AutoscaleSettingResourceName -ne $s1.Name)
{
    Write-Host "There is something wrong with the name"
}

# New
$s1 = Get-AzureRmAutoscaleSetting -ResourceGroup $resourceGroup -Name MySetting
    
# there won't be a AutoscaleSettingResourceName
Write-Host $s1.Name    
```

### <a name="remove-azurermalertrule--remove-azurermlogprofile"></a><span data-ttu-id="12878-213">**Remove-AzureRmAlertRule**/**Remove-AzureRmLogProfile**</span><span class="sxs-lookup"><span data-stu-id="12878-213">**Remove-AzureRmAlertRule** / **Remove-AzureRmLogProfile**</span></span>
- <span data-ttu-id="12878-214">Ausgabeänderung: Die Art der Ausgabe wird geändert, um ein einzelnes Objekt mit der Anforderungs-ID und dem Statuscode zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="12878-214">Output change: The type of the output will change to return a single object containing the request Id and the status code.</span></span>

```powershell-interactive
# Old
$s1 = Remove-AzureRmAlertRule -ResourceGroup $resourceGroup -name $ruleName
if ($s1 -ne $null)
{
    $r = $s1[0].RequestId
    $s = $s1[0].StatusCode
}

# New
$s1 = Remove-AzureRmAlertRule -ResourceGroup $resourceGroup -name $ruleName
$r = $s1.RequestId
$s = $s1.StatusCode
```

## <a name="breaking-changes-to-network-cmdlets"></a><span data-ttu-id="12878-215">Grundlegende Änderungen für Network-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="12878-215">Breaking changes to Network cmdlets</span></span>

### <a name="add-azurermapplicationgatewaysslcertificate"></a><span data-ttu-id="12878-216">**Add-AzureRmApplicationGatewaySslCertificate**</span><span class="sxs-lookup"><span data-stu-id="12878-216">**Add-AzureRmApplicationGatewaySslCertificate**</span></span>
- <span data-ttu-id="12878-217">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-217">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
Add-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
Add-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermapplicationgatewaysslcertificate"></a><span data-ttu-id="12878-218">**New-AzureRmApplicationGatewaySslCertificate**</span><span class="sxs-lookup"><span data-stu-id="12878-218">**New-AzureRmApplicationGatewaySslCertificate**</span></span>
- <span data-ttu-id="12878-219">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-219">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
New-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
New-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermapplicationgatewaysslcertificate"></a><span data-ttu-id="12878-220">**Set-AzureRmApplicationGatewaySslCertificate**</span><span class="sxs-lookup"><span data-stu-id="12878-220">**Set-AzureRmApplicationGatewaySslCertificate**</span></span>
- <span data-ttu-id="12878-221">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-221">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
Set-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
Set-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-resources-cmdlets"></a><span data-ttu-id="12878-222">Grundlegende Änderungen für Resources-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="12878-222">Breaking changes to Resources cmdlets</span></span>

### <a name="new-azurermadappcredential"></a><span data-ttu-id="12878-223">**New-AzureRmADAppCredential**</span><span class="sxs-lookup"><span data-stu-id="12878-223">**New-AzureRmADAppCredential**</span></span>
- <span data-ttu-id="12878-224">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-224">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
New-AzureRmADAppCredential [other required parameters] -Password "plain-text string"

# New
New-AzureRmADAppCredential [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadapplication"></a><span data-ttu-id="12878-225">**New-AzureRmADApplication**</span><span class="sxs-lookup"><span data-stu-id="12878-225">**New-AzureRmADApplication**</span></span>
- <span data-ttu-id="12878-226">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-226">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
New-AzureRmADApplication [other required parameters] -Password "plain-text string"

# New
New-AzureRmADApplication [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadserviceprincipal"></a><span data-ttu-id="12878-227">**New-AzureRmADServicePrincipal**</span><span class="sxs-lookup"><span data-stu-id="12878-227">**New-AzureRmADServicePrincipal**</span></span>
- <span data-ttu-id="12878-228">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-228">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
New-AzureRmADServicePrincipal [other required parameters] -Password "plain-text string"

# New
New-AzureRmADServicePrincipal [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadspcredential"></a><span data-ttu-id="12878-229">**New-AzureRmADSpCredential**</span><span class="sxs-lookup"><span data-stu-id="12878-229">**New-AzureRmADSpCredential**</span></span>
- <span data-ttu-id="12878-230">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-230">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
New-AzureRmADSpCredential [other required parameters] -Password "plain-text string"

# New
New-AzureRmADSpCredential [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermaduser"></a><span data-ttu-id="12878-231">**New-AzureRmADUser**</span><span class="sxs-lookup"><span data-stu-id="12878-231">**New-AzureRmADUser**</span></span>
- <span data-ttu-id="12878-232">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-232">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
New-AzureRmADUser [other required parameters] -Password "plain-text string"

# New
New-AzureRmADUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermaduser"></a><span data-ttu-id="12878-233">**Set-AzureRmADUser**</span><span class="sxs-lookup"><span data-stu-id="12878-233">**Set-AzureRmADUser**</span></span>
- <span data-ttu-id="12878-234">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="12878-234">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
Set-AzureRmADUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmADUser [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-servicebus-cmdlets"></a><span data-ttu-id="12878-235">Grundlegende Änderungen für ServiceBus-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="12878-235">Breaking changes to ServiceBus cmdlets</span></span>

### <a name="get-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="12878-236">**Get-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="12878-236">**Get-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="12878-237">Das Cmdlet „Get-AzureRmServiceBusTopicAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-237">The 'Get-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="12878-238">Verwenden Sie das Cmdlet „Get-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="12878-238">Please use the 'Get-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>    

### <a name="get-azurermservicebustopickey"></a><span data-ttu-id="12878-239">**Get-AzureRmServiceBusTopicKey**</span><span class="sxs-lookup"><span data-stu-id="12878-239">**Get-AzureRmServiceBusTopicKey**</span></span>
- <span data-ttu-id="12878-240">Das Cmdlet „Get-AzureRmServiceBusTopicKey“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-240">The 'Get-AzureRmServiceBusTopicKey' cmdlet has been removed.</span></span> <span data-ttu-id="12878-241">Verwenden Sie das Cmdlet „Get-AzureRmServiceBusKey“.</span><span class="sxs-lookup"><span data-stu-id="12878-241">Please use the 'Get-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="new-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="12878-242">**New-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="12878-242">**New-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="12878-243">Das Cmdlet „New-AzureRmServiceBusTopicAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-243">The 'New-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="12878-244">Verwenden Sie das Cmdlet „New-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="12878-244">Please use the 'New-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="new-azurermservicebustopickey"></a><span data-ttu-id="12878-245">**New-AzureRmServiceBusTopicKey**</span><span class="sxs-lookup"><span data-stu-id="12878-245">**New-AzureRmServiceBusTopicKey**</span></span>
- <span data-ttu-id="12878-246">Das Cmdlet „New-AzureRmServiceBusTopicKey“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-246">The 'New-AzureRmServiceBusTopicKey' cmdlet has been removed.</span></span> <span data-ttu-id="12878-247">Verwenden Sie das Cmdlet „New-AzureRmServiceBusKey“.</span><span class="sxs-lookup"><span data-stu-id="12878-247">Please use the 'New-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="remove-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="12878-248">**Remove-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="12878-248">**Remove-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="12878-249">Das Cmdlet „Remove-AzureRmServiceBusTopicAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-249">The 'Remove-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="12878-250">Verwenden Sie das Cmdlet „Remove-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="12878-250">Please use the 'Remove-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="set-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="12878-251">**Set-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="12878-251">**Set-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="12878-252">Das Cmdlet „Set-AzureRmServiceBusTopicAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-252">The 'Set-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="12878-253">Verwenden Sie das Cmdlet „Set-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="12878-253">Please use the 'Set-AzureRmServiceBusAuthorizationRule'cmdlet.</span></span>

### <a name="new-azurermservicebusnamespacekey"></a><span data-ttu-id="12878-254">**New-AzureRmServiceBusNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="12878-254">**New-AzureRmServiceBusNamespaceKey**</span></span>
- <span data-ttu-id="12878-255">Das Cmdlet „New-AzureRmServiceBusNamespaceKey“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-255">The 'New-AzureRmServiceBusNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="12878-256">Verwenden Sie das Cmdlet „New-AzureRmServiceBusKey“.</span><span class="sxs-lookup"><span data-stu-id="12878-256">Please use the 'New-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="get-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="12878-257">**Get-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="12878-257">**Get-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="12878-258">Das Cmdlet „Get-AzureRmServiceBusQueueAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-258">The 'Get-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="12878-259">Verwenden Sie das Cmdlet „Get-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="12878-259">Please use the 'Get-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="get-azurermservicebusqueuekey"></a><span data-ttu-id="12878-260">**Get-AzureRmServiceBusQueueKey**</span><span class="sxs-lookup"><span data-stu-id="12878-260">**Get-AzureRmServiceBusQueueKey**</span></span>
- <span data-ttu-id="12878-261">Das Cmdlet „Get-AzureRmServiceBusQueueKey“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-261">The 'Get-AzureRmServiceBusQueueKey' cmdlet has been removed.</span></span> <span data-ttu-id="12878-262">Verwenden Sie das Cmdlet „Get-AzureRmServiceBusKey“.</span><span class="sxs-lookup"><span data-stu-id="12878-262">Please use the 'Get-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="new-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="12878-263">**New-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="12878-263">**New-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="12878-264">Das Cmdlet „New-AzureRmServiceBusQueueAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-264">The 'New-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="12878-265">Verwenden Sie das Cmdlet „New-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="12878-265">Please use the 'New-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="new-azurermservicebusqueuekey"></a><span data-ttu-id="12878-266">**New-AzureRmServiceBusQueueKey**</span><span class="sxs-lookup"><span data-stu-id="12878-266">**New-AzureRmServiceBusQueueKey**</span></span>
- <span data-ttu-id="12878-267">Das Cmdlet „New-AzureRmServiceBusQueueKey“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-267">The 'New-AzureRmServiceBusQueueKey' cmdlet has been removed.</span></span> <span data-ttu-id="12878-268">Verwenden Sie das Cmdlet „New-AzureRmServiceBusKey“.</span><span class="sxs-lookup"><span data-stu-id="12878-268">Please use the 'New-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="remove-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="12878-269">**Remove-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="12878-269">**Remove-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="12878-270">Das Cmdlet „Remove-AzureRmServiceBusQueueAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-270">The 'Remove-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="12878-271">Verwenden Sie das Cmdlet „Remove-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="12878-271">Please use the 'GRemove-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="set-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="12878-272">**Set-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="12878-272">**Set-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="12878-273">Das Cmdlet „Set-AzureRmServiceBusQueueAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-273">The 'Set-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="12878-274">Verwenden Sie das Cmdlet „Set-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="12878-274">Please use the 'Set-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="get-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="12878-275">**Get-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="12878-275">**Get-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="12878-276">Das Cmdlet „Get-AzureRmServiceBusNamespaceAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-276">The 'Get-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="12878-277">Verwenden Sie das Cmdlet „Get-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="12878-277">Please use the 'Get-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="get-azurermservicebusnamespacekey"></a><span data-ttu-id="12878-278">**Get-AzureRmServiceBusNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="12878-278">**Get-AzureRmServiceBusNamespaceKey**</span></span>
- <span data-ttu-id="12878-279">Das Cmdlet „Get-AzureRmServiceBusNamespaceKey“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-279">The 'Get-AzureRmServiceBusNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="12878-280">Verwenden Sie das Cmdlet „Get-AzureRmServiceBusKey“.</span><span class="sxs-lookup"><span data-stu-id="12878-280">Please use the 'Get-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="new-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="12878-281">**New-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="12878-281">**New-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="12878-282">Das Cmdlet „New-AzureRmServiceBusNamespaceAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-282">The 'New-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="12878-283">Verwenden Sie das Cmdlet „New-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="12878-283">Please use the 'New-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="remove-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="12878-284">**Remove-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="12878-284">**Remove-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="12878-285">Das Cmdlet „Remove-AzureRmServiceBusNamespaceAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-285">The 'Remove-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="12878-286">Verwenden Sie das Cmdlet „Remove-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="12878-286">Please use the 'Remove-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="set-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="12878-287">**Set-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="12878-287">**Set-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="12878-288">Das Cmdlet „Set-AzureRmServiceBusNamespaceAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="12878-288">The 'Set-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="12878-289">Verwenden Sie das Cmdlet „Set-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="12878-289">Please use the 'Set-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="type-namespaceattributes"></a><span data-ttu-id="12878-290">**Typ „NamespaceAttributes“**</span><span class="sxs-lookup"><span data-stu-id="12878-290">**Type NamespaceAttributes**</span></span>
- <span data-ttu-id="12878-291">Folgende Eigenschaften wurden entfernt:</span><span class="sxs-lookup"><span data-stu-id="12878-291">The following properties have been removed</span></span>
    - <span data-ttu-id="12878-292">Aktiviert</span><span class="sxs-lookup"><span data-stu-id="12878-292">Enabled</span></span>
    - <span data-ttu-id="12878-293">Status</span><span class="sxs-lookup"><span data-stu-id="12878-293">Status</span></span>
   
```powershell-interactive
# Old
# The $namespace has Status and Enabled property 
$namespace = Get-AzureRmServiceBusNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Enabled and Status properties    
$namespace = Get-AzureRmServiceBusNamespace <parameters>
```

### <a name="type-queueattribute"></a><span data-ttu-id="12878-294">**Typ „QueueAttribute“**</span><span class="sxs-lookup"><span data-stu-id="12878-294">**Type QueueAttribute**</span></span>
- <span data-ttu-id="12878-295">Folgende Eigenschaften werden als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="12878-295">The following properties are marked as obsolete:</span></span>
    - <span data-ttu-id="12878-296">EnableBatchedOperations</span><span class="sxs-lookup"><span data-stu-id="12878-296">EnableBatchedOperations</span></span>
    - <span data-ttu-id="12878-297">EntityAvailabilityStatus</span><span class="sxs-lookup"><span data-stu-id="12878-297">EntityAvailabilityStatus</span></span>
    - <span data-ttu-id="12878-298">IsAnonymousAccessible</span><span class="sxs-lookup"><span data-stu-id="12878-298">IsAnonymousAccessible</span></span>
    - <span data-ttu-id="12878-299">SupportOrdering</span><span class="sxs-lookup"><span data-stu-id="12878-299">SupportOrdering</span></span>

```powershell-interactive
# Old
# The $queue has EntityAvailabilityStatus, EnableBatchedOperations, IsAnonymousAccessible and SupportOrdering properties
$queue = Get-AzureRmServiceBusQueue <parameters>
$queue.EntityAvailabilityStatus
$queue.EnableBatchedOperations
$queue.IsAnonymousAccessible
$queue.SupportOrdering  

# New
# The call remains the same, but the returned values Queue object will not have the EntityAvailabilityStatus, EnableBatchedOperations, IsAnonymousAccessible and SupportOrdering properties    
$queue = Get-AzureRmServiceBusQueue <parameters>
```
   
### <a name="type-topicattribute"></a><span data-ttu-id="12878-300">**Typ „TopicAttribute“**</span><span class="sxs-lookup"><span data-stu-id="12878-300">**Type TopicAttribute**</span></span>
- <span data-ttu-id="12878-301">Folgende Eigenschaften werden als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="12878-301">The following properties are marked as obsolete:</span></span>
    - <span data-ttu-id="12878-302">Standort</span><span class="sxs-lookup"><span data-stu-id="12878-302">Location</span></span>
    - <span data-ttu-id="12878-303">IsExpress</span><span class="sxs-lookup"><span data-stu-id="12878-303">IsExpress</span></span>
    - <span data-ttu-id="12878-304">IsAnonymousAccessible</span><span class="sxs-lookup"><span data-stu-id="12878-304">IsAnonymousAccessible</span></span>
    - <span data-ttu-id="12878-305">FilteringMessagesBeforePublishing</span><span class="sxs-lookup"><span data-stu-id="12878-305">FilteringMessagesBeforePublishing</span></span>
    - <span data-ttu-id="12878-306">EnableSubscriptionPartitioning</span><span class="sxs-lookup"><span data-stu-id="12878-306">EnableSubscriptionPartitioning</span></span>
    - <span data-ttu-id="12878-307">EntityAvailabilityStatus</span><span class="sxs-lookup"><span data-stu-id="12878-307">EntityAvailabilityStatus</span></span>

```powershell-interactive
# Old
# The $topic has EntityAvailabilityStatus, EnableSubscriptionPartitioning, IsAnonymousAccessible, IsExpress, Location and FilteringMessagesBeforePublishing properties
$topic = Get-AzureRmServiceBusTopic <parameters>
$topic.EntityAvailabilityStatus
$topic.EnableSubscriptionPartitioning
$topic.IsAnonymousAccessible
$topic.IsExpress
$topic.FilteringMessagesBeforePublishing
$topic.Location

# New
# The call remains the same, but the returned values Topic object will not have the EntityAvailabilityStatus, EnableBatchedOperations, IsAnonymousAccessible and SupportOrdering properties    
$topic = Get-AzureRmServiceBusTopic <parameters>
```
   
### <a name="type-subscriptionattribute"></a><span data-ttu-id="12878-308">**Typ „SubscriptionAttribute“**</span><span class="sxs-lookup"><span data-stu-id="12878-308">**Type SubscriptionAttribute**</span></span>
- <span data-ttu-id="12878-309">Folgende Eigenschaften werden als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="12878-309">The following properties are marked as obsolete</span></span>
    - <span data-ttu-id="12878-310">DeadLetteringOnFilterEvaluationExceptions</span><span class="sxs-lookup"><span data-stu-id="12878-310">DeadLetteringOnFilterEvaluationExceptions</span></span>
    - <span data-ttu-id="12878-311">EntityAvailabilityStatus</span><span class="sxs-lookup"><span data-stu-id="12878-311">EntityAvailabilityStatus</span></span>
    - <span data-ttu-id="12878-312">IsReadOnly</span><span class="sxs-lookup"><span data-stu-id="12878-312">IsReadOnly</span></span>
    - <span data-ttu-id="12878-313">Standort</span><span class="sxs-lookup"><span data-stu-id="12878-313">Location</span></span>
   
```powershell-interactive
# Old
# The $subscription has EntityAvailabilityStatus, EnableSubscriptionPartitioning, IsAnonymousAccessible, IsExpress, Location and FilteringMessagesBeforePublishing properties
$subscription = Get-AzureRmServiceBussubscription <parameters>
$subscription.EntityAvailabilityStatus
$subscription.EnableSubscriptionPartitioning
$subscription.IsAnonymousAccessible
$subscription.IsExpress
$subscription.FilteringMessagesBeforePublishing
$subscription.Location

# New
# The call remains the same, but the returned values Topic object will not have the EntityAvailabilityStatus, EnableBatchedOperations, IsAnonymousAccessible and SupportOrdering properties    
$subscription = Get-AzureRmServiceBussubscription <parameters>
```