# <a name="breaking-changes-for-microsoft-azure-powershell-500"></a><span data-ttu-id="aeb3b-101">Grundlegende Änderungen für Microsoft Azure PowerShell 5.0.0</span><span class="sxs-lookup"><span data-stu-id="aeb3b-101">Breaking changes for Microsoft Azure PowerShell 5.0.0</span></span>

<span data-ttu-id="aeb3b-102">Dieses Dokument informiert über grundlegende Änderungen und fungiert als Migrationsleitfaden für Kunden mit Microsoft Azure PowerShell-Cmdlets.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-102">This document serves as both a breaking change notification and migration guide for consumers of the Microsoft Azure PowerShell cmdlets.</span></span> <span data-ttu-id="aeb3b-103">In den einzelnen Abschnitten werden jeweils der Grund für die grundlegende Änderung und der Migrationspfad des geringsten Widerstands beschrieben.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-103">Each section describes both the impetus for the breaking change and the migration path of least resistance.</span></span> <span data-ttu-id="aeb3b-104">Ausführlichen Kontext finden Sie unter der Pull-Anforderung für die jeweilige Änderung.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-104">For in-depth context, please refer to the pull request associated with each change.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="aeb3b-105">Inhaltsverzeichnis</span><span class="sxs-lookup"><span data-stu-id="aeb3b-105">Table of Contents</span></span>

- [<span data-ttu-id="aeb3b-106">Grundlegende Änderungen für ApiManagement-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="aeb3b-106">Breaking changes to ApiManagement cmdlets</span></span>](#breaking-changes-to-apimanagement-cmdlets)
- [<span data-ttu-id="aeb3b-107">Grundlegende Änderungen für Batch-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="aeb3b-107">Breaking changes to Batch cmdlets</span></span>](#breaking-changes-to-batch-cmdlets)
- [<span data-ttu-id="aeb3b-108">Grundlegende Änderungen für Compute-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="aeb3b-108">Breaking changes to Compute cmdlets</span></span>](#breaking-changes-to-compute-cmdlets)
- [<span data-ttu-id="aeb3b-109">Grundlegende Änderungen für EventHub-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="aeb3b-109">Breaking changes to EventHub cmdlets</span></span>](#breaking-changes-to-eventhub-cmdlets)
- [<span data-ttu-id="aeb3b-110">Grundlegende Änderungen für Insights-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="aeb3b-110">Breaking changes to Insights cmdlets</span></span>](#breaking-changes-to-insights-cmdlets)
- [<span data-ttu-id="aeb3b-111">Grundlegende Änderungen für Network-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="aeb3b-111">Breaking changes to Network cmdlets</span></span>](#breaking-changes-to-network-cmdlets)
- [<span data-ttu-id="aeb3b-112">Grundlegende Änderungen für Resources-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="aeb3b-112">Breaking changes to Resources cmdlets</span></span>](#breaking-changes-to-resources-cmdlets)
- [<span data-ttu-id="aeb3b-113">Grundlegende Änderungen für ServiceBus-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="aeb3b-113">Breaking Changes to ServiceBus Cmdlets</span></span>](#breaking-changes-to-servicebus-cmdlets)

## <a name="breaking-changes-to-apimanagement-cmdlets"></a><span data-ttu-id="aeb3b-114">Grundlegende Änderungen für ApiManagement-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="aeb3b-114">Breaking changes to ApiManagement cmdlets</span></span>

### <a name="new-azurermapimanagementbackendproxy"></a><span data-ttu-id="aeb3b-115">**New-AzureRmApiManagementBackendProxy**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-115">**New-AzureRmApiManagementBackendProxy**</span></span>
- <span data-ttu-id="aeb3b-116">Die Parameter „UserName“ und „Password“ werden durch ein PSCredential-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-116">Parameters "UserName" and "Password" are being replaced in favor of a PSCredential</span></span>

```powershell
# Old
New-AzureRmApiManagementBackendProxy [other required parameters] -UserName "plain-text string" -Password "plain-text string"

# New
New-AzureRmApiManagementBackendProxy [other required parameters] -Credential $PSCredentialVariable
```

### <a name="new-azurermapimanagementuser"></a><span data-ttu-id="aeb3b-117">**New-AzureRmApiManagementUser**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-117">**New-AzureRmApiManagementUser**</span></span>
- <span data-ttu-id="aeb3b-118">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-118">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmApiManagementUser [other required parameters] -Password "plain-text string"

# New
New-AzureRmApiManagementUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermapimanagementuser"></a><span data-ttu-id="aeb3b-119">**Set-AzureRmApiManagementUser**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-119">**Set-AzureRmApiManagementUser**</span></span>
- <span data-ttu-id="aeb3b-120">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-120">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
Set-AzureRmApiManagementUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmApiManagementUser [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-batch-cmdlets"></a><span data-ttu-id="aeb3b-121">Grundlegende Änderungen für Batch-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="aeb3b-121">Breaking changes to Batch cmdlets</span></span>

### <a name="new-azurebatchcertificate"></a><span data-ttu-id="aeb3b-122">**New-AzureBatchCertificate**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-122">**New-AzureBatchCertificate**</span></span>
- <span data-ttu-id="aeb3b-123">Der Parameter `Password` wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-123">Parameter `Password` being replaced in favor of a Secure string</span></span>

```powershell
# Old
New-AzureBatchCertificate [other required parameters] -Password "plain-text string"

# New
New-AzureBatchCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurebatchcomputenodeuser"></a><span data-ttu-id="aeb3b-124">**New-AzureBatchComputeNodeUser**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-124">**New-AzureBatchComputeNodeUser**</span></span>
- <span data-ttu-id="aeb3b-125">Der Parameter `Password` wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-125">Parameter `Password` being replaced in favor of a Secure string</span></span>

```powershell
# Old
New-AzureBatchComputeNodeUser [other required parameters] -Password "plain-text string"

# New
New-AzureBatchComputeNodeUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermbatchcomputenodeuser"></a><span data-ttu-id="aeb3b-126">**Set-AzureRmBatchComputeNodeUser**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-126">**Set-AzureRmBatchComputeNodeUser**</span></span>
- <span data-ttu-id="aeb3b-127">Der Parameter `Password` wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-127">Parameter `Password` being replaced in favor of a Secure string</span></span>

```powershell
# Old
Set-AzureRmBatchComputeNodeUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmBatchComputeNodeUser [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurebatchtask"></a><span data-ttu-id="aeb3b-128">**New-AzureBatchTask**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-128">**New-AzureBatchTask**</span></span>
 - <span data-ttu-id="aeb3b-129">Der Switch `RunElevated` wurde entfernt und durch `UserIdentity` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-129">Removed the `RunElevated` switch and replaced it with `UserIdentity`.</span></span>

```powershell
# Old
New-AzureBatchTask -Id $taskId1 -JobId $jobId -CommandLine "cmd /c echo hello" -RunElevated $TRUE

# New
$autoUser = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoUserSpecification -ArgumentList @("Task", "Admin")
$userIdentity = New-Object Microsoft.Azure.Commands.Batch.Models.PSUserIdentity $autoUser
New-AzureBatchTask -Id $taskId1 -JobId $jobId -CommandLine "cmd /c echo hello" -UserIdentity $userIdentity
```

<span data-ttu-id="aeb3b-130">Dies betrifft auch die Eigenschaft `RunElevated` für `PSCloudTask`, `PSStartTask`, `PSJobManagerTask`, `PSJobPreparationTask` und `PSJobReleaseTask`.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-130">This additionally impacts the `RunElevated` property on `PSCloudTask`, `PSStartTask`, `PSJobManagerTask`, `PSJobPreparationTask`, and `PSJobReleaseTask`.</span></span>

### <a name="psmultiinstancesettings"></a><span data-ttu-id="aeb3b-131">**PSMultiInstanceSettings**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-131">**PSMultiInstanceSettings**</span></span>

- <span data-ttu-id="aeb3b-132">Der Konstruktor `PSMultiInstanceSettings` akzeptiert anstelle eines erforderlichen `numberOfInstances`-Parameters und einen erforderlichen `coordinationCommandLine`-Parameter.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-132">`PSMultiInstanceSettings` constructor no longer takes a required `numberOfInstances` parameter, instead it takes a required `coordinationCommandLine` parameter.</span></span>

```powershell
# Old
$settings = New-Object Microsoft.Azure.Commands.Batch.Models.PSMultiInstanceSettings -ArgumentList @(2)
$settings.CoordinationCommandLine = "cmd /c echo hello"
New-AzureBatchTask [other parameters] -MultiInstanceSettings $settings

# New
$settings = New-Object Microsoft.Azure.Commands.Batch.Models.PSMultiInstanceSettings -ArgumentList @("cmd /c echo hello", 2)
New-AzureBatchTask [other parameters] -MultiInstanceSettings $settings
```

### <a name="get-azurebatchtask"></a><span data-ttu-id="aeb3b-133">**Get-AzureBatchTask**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-133">**Get-AzureBatchTask**</span></span>
 - <span data-ttu-id="aeb3b-134">Die Eigenschaft `RunElevated` für `PSCloudTask` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-134">Removed the `RunElevated` property on `PSCloudTask`.</span></span> <span data-ttu-id="aeb3b-135">Als Ersatz für `RunElevated` wurde die Eigenschaft `UserIdentity` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-135">The `UserIdentity` property has been added to replace `RunElevated`.</span></span>

```powershell
# Old
$task = Get-AzureBatchTask [parameters]
$task.RunElevated

# New
$task = Get-AzureBatchTask [parameters]
$task.UserIdentity.AutoUser.ElevationLevel
```

<span data-ttu-id="aeb3b-136">Dies betrifft auch die Eigenschaft `RunElevated` für `PSCloudTask`, `PSStartTask`, `PSJobManagerTask`, `PSJobPreparationTask` und `PSJobReleaseTask`.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-136">This additionally impacts the `RunElevated` property on `PSCloudTask`, `PSStartTask`, `PSJobManagerTask`, `PSJobPreparationTask`, and `PSJobReleaseTask`.</span></span>

### <a name="multiple-types"></a><span data-ttu-id="aeb3b-137">**Mehrere Typen**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-137">**Multiple types**</span></span>

- <span data-ttu-id="aeb3b-138">Die Eigenschaft `SchedulingError` für `PSExitConditions` wurde in `PreProcessingError` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-138">Renamed the `SchedulingError` property on `PSExitConditions` to `PreProcessingError`.</span></span>

```powershell
# Old
$task = Get-AzureBatchTask [parameters]
$task.ExitConditions.SchedulingError

# New
$task = Get-AzureBatchTask [parameters]
$task.ExitConditions.PreProcessingError
```

### <a name="multiple-types"></a><span data-ttu-id="aeb3b-139">**Mehrere Typen**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-139">**Multiple types**</span></span>

- <span data-ttu-id="aeb3b-140">Die Eigenschaft `SchedulingError` für `PSJobPreparationTaskExecutionInformation`, `PSJobReleaseTaskExecutionInformation`, `PSStartTaskInformation`, `PSSubtaskInformation` und `PSTaskExecutionInformation` wurde in `FailureInformation` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-140">Renamed the `SchedulingError` property on `PSJobPreparationTaskExecutionInformation`, `PSJobReleaseTaskExecutionInformation`, `PSStartTaskInformation`, `PSSubtaskInformation`, and `PSTaskExecutionInformation` to `FailureInformation`.</span></span>
  - <span data-ttu-id="aeb3b-141">`FailureInformation` wird im Falle eines Aufgabenfehlers zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-141">`FailureInformation` is returned any time there is a task failure.</span></span> <span data-ttu-id="aeb3b-142">Dazu zählen alle vorherigen Planungsfehler sowie Exitcodes ungleich Null und Dateiuploadfehler aus dem neuen Ausgabedateienfeature.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-142">This includes all previous scheduling error cases, as well as nonzero task exit codes, and file upload failures from the new output files feature.</span></span>
  - <span data-ttu-id="aeb3b-143">Da die Struktur unverändert bleibt, sind zur Verwendung dieses Typs keine Codeänderungen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-143">This is structured the same as before, so no code change is needed when using this type.</span></span>

```powershell
# Old
$task = Get-AzureBatchTask [parameters]
$task.ExecutionInformation.SchedulingError

# New
$task = Get-AzureBatchTask [parameters]
$task.ExecutionInformation.FailureInformation
```

<span data-ttu-id="aeb3b-144">Von dieser Änderung sind auch folgende Cmdlets betroffen: „Get-AzureBatchPool“, „Get-AzureBatchSubtask“ und „Get-AzureBatchJobPreparationAndReleaseTaskStatus“</span><span class="sxs-lookup"><span data-stu-id="aeb3b-144">This additionally impacts: Get-AzureBatchPool, Get-AzureBatchSubtask, and Get-AzureBatchJobPreparationAndReleaseTaskStatus</span></span>

### <a name="new-azurebatchpool"></a><span data-ttu-id="aeb3b-145">**New-AzureBatchPool**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-145">**New-AzureBatchPool**</span></span>
 - <span data-ttu-id="aeb3b-146">`TargetDedicated` wurde entfernt und durch `TargetDedicatedComputeNodes` und `TargetLowPriorityComputeNodes` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-146">Removed `TargetDedicated` and replaced it with `TargetDedicatedComputeNodes` and `TargetLowPriorityComputeNodes`.</span></span>
 - <span data-ttu-id="aeb3b-147">`TargetDedicatedComputeNodes` besitzt einen Alias (`TargetDedicated`).</span><span class="sxs-lookup"><span data-stu-id="aeb3b-147">`TargetDedicatedComputeNodes` has an alias `TargetDedicated`.</span></span>

```powershell
# Old
New-AzureBatchPool [other parameters] [-TargetDedicated <Int32>]

# New
New-AzureBatchPool [other parameters] [-TargetDedicatedComputeNodes <Int32>] [-TargetLowPriorityComputeNodes <Int32>]
```

<span data-ttu-id="aeb3b-148">Dies betrifft auch „Start-AzureBatchPoolResize“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-148">This also impacts: Start-AzureBatchPoolResize</span></span>

### <a name="get-azurebatchpool"></a><span data-ttu-id="aeb3b-149">**Get-AzureBatchPool**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-149">**Get-AzureBatchPool**</span></span>
 - <span data-ttu-id="aeb3b-150">Die Eigenschaften `TargetDedicated` und `CurrentDedicated` für `PSCloudPool` wurden in `TargetDedicatedComputeNodes` und `CurrentDedicatedComputeNodes` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-150">Renamed the `TargetDedicated` and `CurrentDedicated` properties on `PSCloudPool` to `TargetDedicatedComputeNodes` and `CurrentDedicatedComputeNodes`.</span></span>

```powershell
# Old
$pool = Get-AzureBatchPool [parameters]
$pool.TargetDedicated
$pool.CurrentDedicated

# New
$pool = Get-AzureBatchPool [parameters]
$pool.TargetDedicatedComputeNodes
$pool.CurrentDedicatedComputeNodes
```

### <a name="type-pscloudpool"></a><span data-ttu-id="aeb3b-151">**Typ „PSCloudPool“**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-151">**Type PSCloudPool**</span></span>

- <span data-ttu-id="aeb3b-152">`ResizeError` wurde für `PSCloudPool` in `ResizeErrors` umbenannt und ist nun eine Sammlung.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-152">Renamed `ResizeError` to `ResizeErrors` on `PSCloudPool`, and it is now a collection.</span></span>

```powershell
# Old
$pool = Get-AzureBatchPool [parameters]
$pool.ResizeError

# New
$pool = Get-AzureBatchPool [parameters]
$pool.ResizeErrors[0]
```

### <a name="new-azurebatchjob"></a><span data-ttu-id="aeb3b-153">**New-AzureBatchJob**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-153">**New-AzureBatchJob**</span></span>
- <span data-ttu-id="aeb3b-154">Die Eigenschaft `TargetDedicated` für `PSPoolSpecification` wurde in `TargetDedicatedComputeNodes` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-154">Renamed the `TargetDedicated` property on `PSPoolSpecification` to `TargetDedicatedComputeNodes`.</span></span>

```powershell
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

### <a name="get-azurebatchnodefile"></a><span data-ttu-id="aeb3b-155">**Get-AzureBatchNodeFile**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-155">**Get-AzureBatchNodeFile**</span></span>
 - <span data-ttu-id="aeb3b-156">`Name` wurde entfernt und durch `Path` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-156">Removed `Name` and replaced it with `Path`.</span></span>
 - <span data-ttu-id="aeb3b-157">`Path` besitzt einen Alias (`Name`).</span><span class="sxs-lookup"><span data-stu-id="aeb3b-157">`Path` has an alias `Name`.</span></span>

```powershell
# Old
Get-AzureBatchNodeFile [other parameters] [[-Name] <String>]

# New
Get-AzureBatchNodeFile [other parameters] [[-Path] <String>]
```

<span data-ttu-id="aeb3b-158">Dies betrifft auch „Get-AzureBatchNodeFileContent“ und „Remove-AzureBatchNodeFile“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-158">This also impacts: Get-AzureBatchNodeFileContent, Remove-AzureBatchNodeFile</span></span>

### <a name="type-psnodefile"></a><span data-ttu-id="aeb3b-159">**Typ „PSNodeFile“**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-159">Type **PSNodeFile**</span></span>

 - <span data-ttu-id="aeb3b-160">Die Eigenschaft `Name` für `PSNodeFile` wurde in `Path` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-160">Renamed the `Name` property on `PSNodeFile` to `Path`.</span></span>

```powershell
# Old
$file = Get-AzureBatchNodeFile [parameters]
$file.Name

# New
$file = Get-AzureBatchNodeFile [parameters]
$file.Path
```

### <a name="get-azurebatchsubtask"></a><span data-ttu-id="aeb3b-161">**Get-AzureBatchSubtask**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-161">**Get-AzureBatchSubtask**</span></span>
- <span data-ttu-id="aeb3b-162">Die Eigenschaften `PreviousState` und `State` von `PSSubtaskInformation` sind nicht mehr vom Typ `TaskState`, sondern vom Typ `SubtaskState`.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-162">The `PreviousState` and `State` properties of `PSSubtaskInformation` are no longer of type `TaskState`, instead they are of type `SubtaskState`.</span></span>
  - <span data-ttu-id="aeb3b-163">Im Gegensatz zu `TaskState` besitzt `SubtaskState` keinen Wert vom Typ `Active`, da sich Unteraufgaben nicht im Zustand `Active` befinden können.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-163">Unlike `TaskState`, `SubtaskState` has no `Active` value, since it is not possible for subtasks to be in an `Active` state.</span></span>

```powershell
# Old
$subtask = Get-AzureBatchSubtask [parameters]
if ($subtask.State -eq Microsoft.Azure.Batch.Common.TaskState.Running) { }

# New
$subtask = Get-AzureBatchSubtask [parameters]
if ($subtask.State -eq Microsoft.Azure.Batch.Common.SubtaskState.Running) { }
```

## <a name="breaking-changes-to-compute-cmdlets"></a><span data-ttu-id="aeb3b-164">Grundlegende Änderungen für Compute-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="aeb3b-164">Breaking changes to Compute cmdlets</span></span>

### <a name="set-azurermvmaccessextension"></a><span data-ttu-id="aeb3b-165">**Set-AzureRmVMAccessExtension**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-165">**Set-AzureRmVMAccessExtension**</span></span>
- <span data-ttu-id="aeb3b-166">Die Parameter „UserName“ und „Password“ werden durch ein PSCredential-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-166">Parameters "UserName" and "Password" are being replaced in favor of a PSCredential</span></span>

```powershell
# Old
Set-AzureRmVMAccessExtension [other required parameters] -UserName "plain-text string" -Password "plain-text string"

# New
Set-AzureRmVMAccessExtension [other required parameters] -Credential $PSCredential
```

## <a name="breaking-changes-to-eventhub-cmdlets"></a><span data-ttu-id="aeb3b-167">Grundlegende Änderungen für EventHub-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="aeb3b-167">Breaking changes to EventHub cmdlets</span></span>

### <a name="new-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="aeb3b-168">**New-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-168">**New-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="aeb3b-169">Das Cmdlet „New-AzureRmEventHubNamespaceAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-169">The 'New-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-170">Verwenden Sie das Cmdlet „New-AzureRmEventHubAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-170">Please use the 'New-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="get-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="aeb3b-171">**Get-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-171">**Get-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="aeb3b-172">Das Cmdlet „Get-AzureRmEventHubNamespaceAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-172">The 'Get-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-173">Verwenden Sie das Cmdlet „Get-AzureRmEventHubAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-173">Please use the 'Get-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="set-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="aeb3b-174">**Set-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-174">**Set-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="aeb3b-175">Das Cmdlet „Set-AzureRmEventHubNamespaceAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-175">The 'Set-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-176">Verwenden Sie das Cmdlet „Set-AzureRmEventHubAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-176">Please use the 'Set-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="remove-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="aeb3b-177">**Remove-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-177">**Remove-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="aeb3b-178">Das Cmdlet „Remove-AzureRmEventHubNamespaceAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-178">The 'Remove-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-179">Verwenden Sie das Cmdlet „Remove-AzureRmEventHubAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-179">Please use the 'Remove-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="new-azurermeventhubnamespacekey"></a><span data-ttu-id="aeb3b-180">**New-AzureRmEventHubNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-180">**New-AzureRmEventHubNamespaceKey**</span></span>
- <span data-ttu-id="aeb3b-181">Das Cmdlet „New-AzureRmEventHubNamespaceKey“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-181">The 'New-AzureRmEventHubNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-182">Verwenden Sie das Cmdlet „New-AzureRmEventHubKey“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-182">Please use the 'New-AzureRmEventHubKey' cmdlet</span></span>
    
### <a name="get-azurermeventhubnamespacekey"></a><span data-ttu-id="aeb3b-183">**Get-AzureRmEventHubNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-183">**Get-AzureRmEventHubNamespaceKey**</span></span>
- <span data-ttu-id="aeb3b-184">Das Cmdlet „Get-AzureRmEventHubNamespaceKey“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-184">The 'Get-AzureRmEventHubNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-185">Verwenden Sie das Cmdlet „Get-AzureRmEventHubKey“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-185">Please use the 'Get-AzureRmEventHubKey' cmdlet</span></span>
    
### <a name="new-azurermeventhubnamespace"></a><span data-ttu-id="aeb3b-186">**New-AzureRmEventHubNamespace**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-186">**New-AzureRmEventHubNamespace**</span></span>
- <span data-ttu-id="aeb3b-187">Die Eigenschaften „Status“ und „Enabled“ aus den Namespaceattributen werden entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-187">The property 'Status' and 'Enabled' from the NamespceAttributes will be removed.</span></span> 

```powershell
# Old
# The $namespace has Status and Enabled property  
$namespace = New-AzureRmEventHubNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Status and Enabled property    
$namespace = Get-AzureRmEventHubNamespace <parameters>
```
    
### <a name="get-azurermeventhubnamespace"></a><span data-ttu-id="aeb3b-188">**Get-AzureRmEventHubNamespace**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-188">**Get-AzureRmEventHubNamespace**</span></span>
- <span data-ttu-id="aeb3b-189">Die Eigenschaften „Status“ und „Enabled“ aus den Namespaceattributen werden entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-189">The property 'Status' and 'Enabled' from the NamespceAttributes will be removed.</span></span> 

```powershell
# Old
# The $namespace has Status and Enabled property 
$namespace = Get-AzureRmEventHubNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Status and Enabled property    
$namespace = Get-AzureRmEventHubNamespace <parameters>
```
    
### <a name="set-azurermeventhubnamespace"></a><span data-ttu-id="aeb3b-190">**Set-AzureRmEventHubNamespace**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-190">**Set-AzureRmEventHubNamespace**</span></span>
- <span data-ttu-id="aeb3b-191">Die Eigenschaften „Status“ und „Enabled“ aus den Namespaceattributen werden entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-191">The property 'Status' and 'Enabled' from the NamespceAttributes will be removed.</span></span> 

```powershell
# Old
# The $namespace has Status and Enabled property 
$namespace = Set-AzureRmEventHubNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Status and Enabled property    
$namespace = Set-AzureRmEventHubNamespace <parameters>
``` 
  
### <a name="new-azurermeventhubconsumergroup"></a><span data-ttu-id="aeb3b-192">**New-AzureRmEventHubConsumerGroup**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-192">**New-AzureRmEventHubConsumerGroup**</span></span>
- <span data-ttu-id="aeb3b-193">Die Eigenschaft „EventHubPath“ aus den ConsumerGroup-Attributen wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-193">The property 'EventHubPath' from the ConsumerGroupAttributes will be removed.</span></span>

```powershell
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = New-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = New-AzureRmEventHubConsumerGroup <parameters>
```
    
### <a name="set-azurermeventhubconsumergroup"></a><span data-ttu-id="aeb3b-194">**Set-AzureRmEventHubConsumerGroup**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-194">**Set-AzureRmEventHubConsumerGroup**</span></span>
- <span data-ttu-id="aeb3b-195">Die Eigenschaft „EventHubPath“ aus den ConsumerGroup-Attributen wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-195">The property 'EventHubPath' from the ConsumerGroupAttributes will be removed.</span></span>

```powershell
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = Set-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = Set-AzureRmEventHubConsumerGroup <parameters>
```
    
### <a name="get-azurermeventhubconsumergroup"></a><span data-ttu-id="aeb3b-196">**Get-AzureRmEventHubConsumerGroup**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-196">**Get-AzureRmEventHubConsumerGroup**</span></span>
- <span data-ttu-id="aeb3b-197">Die Eigenschaft „EventHubPath“ aus den ConsumerGroup-Attributen wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-197">The property 'EventHubPath' from the ConsumerGroupAttributes will be removed.</span></span>

```powershell
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = Get-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = Get-AzureRmEventHubConsumerGroup <parameters>
```

## <a name="breaking-changes-to-insights-cmdlets"></a><span data-ttu-id="aeb3b-198">Grundlegende Änderungen für Insights-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="aeb3b-198">Breaking changes to Insights cmdlets</span></span>

### <a name="add-azurermlogalertrule"></a><span data-ttu-id="aeb3b-199">**Add-AzureRMLogAlertRule**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-199">**Add-AzureRMLogAlertRule**</span></span>
- <span data-ttu-id="aeb3b-200">Das Cmdlet **Add-AzureRMLogAlertRule** ist veraltet.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-200">The **Add-AzureRMLogAlertRule** cmdlet has been deprecated</span></span>
- <span data-ttu-id="aeb3b-201">Nach dem 1. Oktober hat die Verwendung dieses Cmdlets keine Wirkung mehr, da die Funktion in Aktivitätsprotokollwarnungen übertragen wurde.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-201">After October 1st using this cmdlet will no longer have any effect as this functionality is being transitioned to Activity Log Alerts.</span></span> <span data-ttu-id="aeb3b-202">Weitere Informationen finden Sie unter https://aka.ms/migratemealerts.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-202">Please see https://aka.ms/migratemealerts for more information.</span></span>

### <a name="get-azurermusage"></a><span data-ttu-id="aeb3b-203">**Get-AzureRMUsage**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-203">**Get-AzureRMUsage**</span></span>
- <span data-ttu-id="aeb3b-204">Das Cmdlet **Get-AzureRMUsage** ist veraltet.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-204">The **Get-AzureRMUsage** cmdlet has been deprecated</span></span>

### <a name="get-azurermalerthistory--get-azurermautoscalehistory--get-azurermlogs"></a><span data-ttu-id="aeb3b-205">**Get-AzureRmAlertHistory**/**Get-AzureRmAutoscaleHistory**/**Get-AzureRmLogs**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-205">**Get-AzureRmAlertHistory** / **Get-AzureRmAutoscaleHistory** / **Get-AzureRmLogs**</span></span>
- <span data-ttu-id="aeb3b-206">Ausgabeänderung: Das Feld „EventChannels“ aus dem EventData-Objekt (das von diesen Cmdlets zurückgegeben wird) wird ausgemustert, da nun ein konstanter Wert (Administrator, Vorgang) zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-206">Output change: The field EventChannels from the EventData object (returned by these cmdlets) is being deprecated since it now returns a constant value (Admin,Operation.)</span></span>

### <a name="get-azurermalertrule"></a><span data-ttu-id="aeb3b-207">**Get-AzureRmAlertRule**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-207">**Get-AzureRmAlertRule**</span></span>
- <span data-ttu-id="aeb3b-208">Ausgabeänderung: Zur Verbesserung der Benutzerfreundlichkeit wird die Ausgabe dieses Cmdlets vereinfacht. (Das Eigenschaftenfeld wird entfernt.)</span><span class="sxs-lookup"><span data-stu-id="aeb3b-208">Output change: The output of this cmdlet will be flattened, i.e. elimination of the properties field, to improve the user experience.</span></span>

```powershell
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

### <a name="get-azurermautoscalesetting"></a><span data-ttu-id="aeb3b-209">**Get-AzureRmAutoscaleSetting**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-209">**Get-AzureRmAutoscaleSetting**</span></span>
- <span data-ttu-id="aeb3b-210">Ausgabeänderung: Das Feld „AutoscaleSettingResourceName“ wird ausgemustert, da es immer dem Feld „Name“ entspricht.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-210">Output change: The AutoscaleSettingResourceName field will be deprecated since it always equals the Name field.</span></span>

```powershell
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

### <a name="remove-azurermalertrule--remove-azurermlogprofile"></a><span data-ttu-id="aeb3b-211">**Remove-AzureRmAlertRule**/**Remove-AzureRmLogProfile**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-211">**Remove-AzureRmAlertRule** / **Remove-AzureRmLogProfile**</span></span>
- <span data-ttu-id="aeb3b-212">Ausgabeänderung: Die Art der Ausgabe wird geändert, um ein einzelnes Objekt mit der Anforderungs-ID und dem Statuscode zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-212">Output change: The type of the output will change to return a single object containing the request Id and the status code.</span></span>

```powershell
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

## <a name="breaking-changes-to-network-cmdlets"></a><span data-ttu-id="aeb3b-213">Grundlegende Änderungen für Network-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="aeb3b-213">Breaking changes to Network cmdlets</span></span>

### <a name="add-azurermapplicationgatewaysslcertificate"></a><span data-ttu-id="aeb3b-214">**Add-AzureRmApplicationGatewaySslCertificate**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-214">**Add-AzureRmApplicationGatewaySslCertificate**</span></span>
- <span data-ttu-id="aeb3b-215">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-215">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
Add-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
Add-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermapplicationgatewaysslcertificate"></a><span data-ttu-id="aeb3b-216">**New-AzureRmApplicationGatewaySslCertificate**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-216">**New-AzureRmApplicationGatewaySslCertificate**</span></span>
- <span data-ttu-id="aeb3b-217">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-217">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
New-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermapplicationgatewaysslcertificate"></a><span data-ttu-id="aeb3b-218">**Set-AzureRmApplicationGatewaySslCertificate**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-218">**Set-AzureRmApplicationGatewaySslCertificate**</span></span>
- <span data-ttu-id="aeb3b-219">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-219">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
Set-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
Set-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-resources-cmdlets"></a><span data-ttu-id="aeb3b-220">Grundlegende Änderungen für Resources-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="aeb3b-220">Breaking changes to Resources cmdlets</span></span>

### <a name="new-azurermadappcredential"></a><span data-ttu-id="aeb3b-221">**New-AzureRmADAppCredential**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-221">**New-AzureRmADAppCredential**</span></span>
- <span data-ttu-id="aeb3b-222">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-222">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmADAppCredential [other required parameters] -Password "plain-text string"

# New
New-AzureRmADAppCredential [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadapplication"></a><span data-ttu-id="aeb3b-223">**New-AzureRmADApplication**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-223">**New-AzureRmADApplication**</span></span>
- <span data-ttu-id="aeb3b-224">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-224">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmADApplication [other required parameters] -Password "plain-text string"

# New
New-AzureRmADApplication [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadserviceprincipal"></a><span data-ttu-id="aeb3b-225">**New-AzureRmADServicePrincipal**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-225">**New-AzureRmADServicePrincipal**</span></span>
- <span data-ttu-id="aeb3b-226">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-226">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmADServicePrincipal [other required parameters] -Password "plain-text string"

# New
New-AzureRmADServicePrincipal [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadspcredential"></a><span data-ttu-id="aeb3b-227">**New-AzureRmADSpCredential**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-227">**New-AzureRmADSpCredential**</span></span>
- <span data-ttu-id="aeb3b-228">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-228">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmADSpCredential [other required parameters] -Password "plain-text string"

# New
New-AzureRmADSpCredential [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermaduser"></a><span data-ttu-id="aeb3b-229">**New-AzureRmADUser**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-229">**New-AzureRmADUser**</span></span>
- <span data-ttu-id="aeb3b-230">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-230">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmADUser [other required parameters] -Password "plain-text string"

# New
New-AzureRmADUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermaduser"></a><span data-ttu-id="aeb3b-231">**Set-AzureRmADUser**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-231">**Set-AzureRmADUser**</span></span>
- <span data-ttu-id="aeb3b-232">Der Parameter „Password“ wird durch ein SecureString-Objekt ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-232">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
Set-AzureRmADUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmADUser [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-servicebus-cmdlets"></a><span data-ttu-id="aeb3b-233">Grundlegende Änderungen für ServiceBus-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="aeb3b-233">Breaking changes to ServiceBus cmdlets</span></span>

### <a name="get-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="aeb3b-234">**Get-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-234">**Get-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="aeb3b-235">Das Cmdlet „Get-AzureRmServiceBusTopicAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-235">The 'Get-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-236">Verwenden Sie das Cmdlet „Get-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-236">Please use the 'Get-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>    

### <a name="get-azurermservicebustopickey"></a><span data-ttu-id="aeb3b-237">**Get-AzureRmServiceBusTopicKey**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-237">**Get-AzureRmServiceBusTopicKey**</span></span>
- <span data-ttu-id="aeb3b-238">Das Cmdlet „Get-AzureRmServiceBusTopicKey“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-238">The 'Get-AzureRmServiceBusTopicKey' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-239">Verwenden Sie das Cmdlet „Get-AzureRmServiceBusKey“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-239">Please use the 'Get-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="new-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="aeb3b-240">**New-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-240">**New-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="aeb3b-241">Das Cmdlet „New-AzureRmServiceBusTopicAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-241">The 'New-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-242">Verwenden Sie das Cmdlet „New-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-242">Please use the 'New-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="new-azurermservicebustopickey"></a><span data-ttu-id="aeb3b-243">**New-AzureRmServiceBusTopicKey**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-243">**New-AzureRmServiceBusTopicKey**</span></span>
- <span data-ttu-id="aeb3b-244">Das Cmdlet „New-AzureRmServiceBusTopicKey“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-244">The 'New-AzureRmServiceBusTopicKey' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-245">Verwenden Sie das Cmdlet „New-AzureRmServiceBusKey“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-245">Please use the 'New-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="remove-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="aeb3b-246">**Remove-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-246">**Remove-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="aeb3b-247">Das Cmdlet „Remove-AzureRmServiceBusTopicAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-247">The 'Remove-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-248">Verwenden Sie das Cmdlet „Remove-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-248">Please use the 'Remove-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="set-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="aeb3b-249">**Set-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-249">**Set-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="aeb3b-250">Das Cmdlet „Set-AzureRmServiceBusTopicAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-250">The 'Set-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-251">Verwenden Sie das Cmdlet „Set-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-251">Please use the 'Set-AzureRmServiceBusAuthorizationRule'cmdlet.</span></span>

### <a name="new-azurermservicebusnamespacekey"></a><span data-ttu-id="aeb3b-252">**New-AzureRmServiceBusNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-252">**New-AzureRmServiceBusNamespaceKey**</span></span>
- <span data-ttu-id="aeb3b-253">Das Cmdlet „New-AzureRmServiceBusNamespaceKey“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-253">The 'New-AzureRmServiceBusNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-254">Verwenden Sie das Cmdlet „New-AzureRmServiceBusKey“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-254">Please use the 'New-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="get-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="aeb3b-255">**Get-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-255">**Get-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="aeb3b-256">Das Cmdlet „Get-AzureRmServiceBusQueueAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-256">The 'Get-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-257">Verwenden Sie das Cmdlet „Get-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-257">Please use the 'Get-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="get-azurermservicebusqueuekey"></a><span data-ttu-id="aeb3b-258">**Get-AzureRmServiceBusQueueKey**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-258">**Get-AzureRmServiceBusQueueKey**</span></span>
- <span data-ttu-id="aeb3b-259">Das Cmdlet „Get-AzureRmServiceBusQueueKey“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-259">The 'Get-AzureRmServiceBusQueueKey' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-260">Verwenden Sie das Cmdlet „Get-AzureRmServiceBusKey“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-260">Please use the 'Get-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="new-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="aeb3b-261">**New-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-261">**New-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="aeb3b-262">Das Cmdlet „New-AzureRmServiceBusQueueAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-262">The 'New-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-263">Verwenden Sie das Cmdlet „New-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-263">Please use the 'New-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="new-azurermservicebusqueuekey"></a><span data-ttu-id="aeb3b-264">**New-AzureRmServiceBusQueueKey**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-264">**New-AzureRmServiceBusQueueKey**</span></span>
- <span data-ttu-id="aeb3b-265">Das Cmdlet „New-AzureRmServiceBusQueueKey“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-265">The 'New-AzureRmServiceBusQueueKey' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-266">Verwenden Sie das Cmdlet „New-AzureRmServiceBusKey“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-266">Please use the 'New-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="remove-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="aeb3b-267">**Remove-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-267">**Remove-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="aeb3b-268">Das Cmdlet „Remove-AzureRmServiceBusQueueAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-268">The 'Remove-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-269">Verwenden Sie das Cmdlet „Remove-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-269">Please use the 'GRemove-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="set-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="aeb3b-270">**Set-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-270">**Set-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="aeb3b-271">Das Cmdlet „Set-AzureRmServiceBusQueueAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-271">The 'Set-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-272">Verwenden Sie das Cmdlet „Set-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-272">Please use the 'Set-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="get-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="aeb3b-273">**Get-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-273">**Get-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="aeb3b-274">Das Cmdlet „Get-AzureRmServiceBusNamespaceAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-274">The 'Get-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-275">Verwenden Sie das Cmdlet „Get-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-275">Please use the 'Get-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="get-azurermservicebusnamespacekey"></a><span data-ttu-id="aeb3b-276">**Get-AzureRmServiceBusNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-276">**Get-AzureRmServiceBusNamespaceKey**</span></span>
- <span data-ttu-id="aeb3b-277">Das Cmdlet „Get-AzureRmServiceBusNamespaceKey“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-277">The 'Get-AzureRmServiceBusNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-278">Verwenden Sie das Cmdlet „Get-AzureRmServiceBusKey“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-278">Please use the 'Get-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="new-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="aeb3b-279">**New-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-279">**New-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="aeb3b-280">Das Cmdlet „New-AzureRmServiceBusNamespaceAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-280">The 'New-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-281">Verwenden Sie das Cmdlet „New-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-281">Please use the 'New-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="remove-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="aeb3b-282">**Remove-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-282">**Remove-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="aeb3b-283">Das Cmdlet „Remove-AzureRmServiceBusNamespaceAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-283">The 'Remove-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-284">Verwenden Sie das Cmdlet „Remove-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-284">Please use the 'Remove-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="set-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="aeb3b-285">**Set-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-285">**Set-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="aeb3b-286">Das Cmdlet „Set-AzureRmServiceBusNamespaceAuthorizationRule“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-286">The 'Set-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="aeb3b-287">Verwenden Sie das Cmdlet „Set-AzureRmServiceBusAuthorizationRule“.</span><span class="sxs-lookup"><span data-stu-id="aeb3b-287">Please use the 'Set-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="type-namespaceattributes"></a><span data-ttu-id="aeb3b-288">**Typ „NamespaceAttributes“**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-288">**Type NamespaceAttributes**</span></span>
- <span data-ttu-id="aeb3b-289">Folgende Eigenschaften wurden entfernt:</span><span class="sxs-lookup"><span data-stu-id="aeb3b-289">The following properties have been removed</span></span>
    - <span data-ttu-id="aeb3b-290">Enabled</span><span class="sxs-lookup"><span data-stu-id="aeb3b-290">Enabled</span></span>
    - <span data-ttu-id="aeb3b-291">Status</span><span class="sxs-lookup"><span data-stu-id="aeb3b-291">Status</span></span>
   
```powershell
# Old
# The $namespace has Status and Enabled property 
$namespace = Get-AzureRmServiceBusNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Enabled and Status properties    
$namespace = Get-AzureRmServiceBusNamespace <parameters>
```

### <a name="type-queueattribute"></a><span data-ttu-id="aeb3b-292">**Typ „QueueAttribute“**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-292">**Type QueueAttribute**</span></span>
- <span data-ttu-id="aeb3b-293">Folgende Eigenschaften werden als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="aeb3b-293">The following properties are marked as obsolete:</span></span>
    - <span data-ttu-id="aeb3b-294">EnableBatchedOperations</span><span class="sxs-lookup"><span data-stu-id="aeb3b-294">EnableBatchedOperations</span></span>
    - <span data-ttu-id="aeb3b-295">EntityAvailabilityStatus</span><span class="sxs-lookup"><span data-stu-id="aeb3b-295">EntityAvailabilityStatus</span></span>
    - <span data-ttu-id="aeb3b-296">IsAnonymousAccessible</span><span class="sxs-lookup"><span data-stu-id="aeb3b-296">IsAnonymousAccessible</span></span>
    - <span data-ttu-id="aeb3b-297">SupportOrdering</span><span class="sxs-lookup"><span data-stu-id="aeb3b-297">SupportOrdering</span></span>

```powershell
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
   
### <a name="type-topicattribute"></a><span data-ttu-id="aeb3b-298">**Typ „TopicAttribute“**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-298">**Type TopicAttribute**</span></span>
- <span data-ttu-id="aeb3b-299">Folgende Eigenschaften werden als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="aeb3b-299">The following properties are marked as obsolete:</span></span>
    - <span data-ttu-id="aeb3b-300">Speicherort</span><span class="sxs-lookup"><span data-stu-id="aeb3b-300">Location</span></span>
    - <span data-ttu-id="aeb3b-301">IsExpress</span><span class="sxs-lookup"><span data-stu-id="aeb3b-301">IsExpress</span></span>
    - <span data-ttu-id="aeb3b-302">IsAnonymousAccessible</span><span class="sxs-lookup"><span data-stu-id="aeb3b-302">IsAnonymousAccessible</span></span>
    - <span data-ttu-id="aeb3b-303">FilteringMessagesBeforePublishing</span><span class="sxs-lookup"><span data-stu-id="aeb3b-303">FilteringMessagesBeforePublishing</span></span>
    - <span data-ttu-id="aeb3b-304">EnableSubscriptionPartitioning</span><span class="sxs-lookup"><span data-stu-id="aeb3b-304">EnableSubscriptionPartitioning</span></span>
    - <span data-ttu-id="aeb3b-305">EntityAvailabilityStatus</span><span class="sxs-lookup"><span data-stu-id="aeb3b-305">EntityAvailabilityStatus</span></span>

```powershell
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
   
### <a name="type-subscriptionattribute"></a><span data-ttu-id="aeb3b-306">**Typ „SubscriptionAttribute“**</span><span class="sxs-lookup"><span data-stu-id="aeb3b-306">**Type SubscriptionAttribute**</span></span>
- <span data-ttu-id="aeb3b-307">Folgende Eigenschaften werden als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="aeb3b-307">The following properties are marked as obsolete</span></span>
    - <span data-ttu-id="aeb3b-308">DeadLetteringOnFilterEvaluationExceptions</span><span class="sxs-lookup"><span data-stu-id="aeb3b-308">DeadLetteringOnFilterEvaluationExceptions</span></span>
    - <span data-ttu-id="aeb3b-309">EntityAvailabilityStatus</span><span class="sxs-lookup"><span data-stu-id="aeb3b-309">EntityAvailabilityStatus</span></span>
    - <span data-ttu-id="aeb3b-310">IsReadOnly</span><span class="sxs-lookup"><span data-stu-id="aeb3b-310">IsReadOnly</span></span>
    - <span data-ttu-id="aeb3b-311">Speicherort</span><span class="sxs-lookup"><span data-stu-id="aeb3b-311">Location</span></span>
   
```powershell
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