---
title: Azure PowerShell-Änderungsprotokoll | Microsoft-Dokumentation
description: Hierbei handelt es sich um einen Verlauf der Änderungen, die in der neuesten Version an Azure PowerShell vorgenommen wurden.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 5/1/2018
ms.openlocfilehash: 3811e28dda69d194d23934943fb47d562f869fc4
ms.sourcegitcommit: 5a5b6dd216d5f805204244146cf6f88ad2f34fb4
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/19/2018
ms.locfileid: "36237688"
---
# <a name="release-notes"></a><span data-ttu-id="10f3d-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="10f3d-103">Release notes</span></span>

<span data-ttu-id="10f3d-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="10f3d-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="630---june-2018"></a><span data-ttu-id="10f3d-105">6.3.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="10f3d-105">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="10f3d-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="10f3d-106">AzureRM.Profile</span></span>
* <span data-ttu-id="10f3d-107">Aktualisierte Fehlermeldungen für „Enable-AzureRmContextAutoSave“</span><span class="sxs-lookup"><span data-stu-id="10f3d-107">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="10f3d-108">Erstellen eines Kontexts für jedes Abonnement beim Ausführen von „Connect-AzureRmAccount“ ohne vorherigen Kontext</span><span class="sxs-lookup"><span data-stu-id="10f3d-108">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="10f3d-109">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="10f3d-109">Azure.Storage</span></span>
* <span data-ttu-id="10f3d-110">Zusätzliche Informationen zum Parameter „-Permissions“ in Hilfedateien</span><span class="sxs-lookup"><span data-stu-id="10f3d-110">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="10f3d-111">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="10f3d-111">AzureRM.Compute</span></span>
* <span data-ttu-id="10f3d-112">„Get-AzureRmVmDiskEncryptionStatus“ behebt ein Problem, das bei virtuellen Computern ohne Datenträger festgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="10f3d-112">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="10f3d-113">Version der Computeclientbibliothek aktualisiert, um folgende Cmdlets zu korrigieren:</span><span class="sxs-lookup"><span data-stu-id="10f3d-113">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="10f3d-114">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="10f3d-114">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="10f3d-115">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="10f3d-115">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="10f3d-116">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="10f3d-116">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="10f3d-117">Die folgenden Cmdlets wurden korrigiert, um die Vorgangs-ID und den Vorgangsstatus korrekt anzuzeigen:</span><span class="sxs-lookup"><span data-stu-id="10f3d-117">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="10f3d-118">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="10f3d-118">Start-AzureRmVM</span></span>
    - <span data-ttu-id="10f3d-119">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="10f3d-119">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="10f3d-120">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="10f3d-120">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="10f3d-121">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="10f3d-121">Set-AzureRmVM</span></span>
    - <span data-ttu-id="10f3d-122">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="10f3d-122">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="10f3d-123">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="10f3d-123">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="10f3d-124">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="10f3d-124">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="10f3d-125">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="10f3d-125">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="10f3d-126">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="10f3d-126">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="10f3d-127">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="10f3d-127">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="10f3d-128">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="10f3d-128">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="10f3d-129">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="10f3d-129">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="10f3d-130">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="10f3d-130">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="10f3d-131">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="10f3d-131">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="10f3d-132">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="10f3d-132">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="10f3d-133">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="10f3d-133">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="10f3d-134">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="10f3d-134">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="10f3d-135">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="10f3d-135">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="10f3d-136">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="10f3d-136">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="10f3d-137">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="10f3d-137">AzureRM.EventGrid</span></span>
* <span data-ttu-id="10f3d-138">ValidateNotNullOrEmpty-Überprüfungskonditionen für „SubjectBeginsWith“/„SubjectEndsWith“ im Cmdlet „Update-AzureRmEventGridSubscription“ wurden entfernt, um bei Bedarf die Änderung dieser Parameter in eine leere Zeichenfolge zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="10f3d-138">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="10f3d-139">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="10f3d-139">AzureRM.KeyVault</span></span>
* <span data-ttu-id="10f3d-140">Ein Problem wurde behoben, aufgrund dessen bei Ausführung von „Get-AzureRmKeyVault -Tag“ keine Tags zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="10f3d-140">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="10f3d-141">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="10f3d-141">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="10f3d-142">Offizielle Veröffentlichung von Policy Insights-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="10f3d-142">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="10f3d-143">Verwendung der API-Version 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="10f3d-143">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="10f3d-144">„PolicyDefinitionReferenceId“ zu den Ergebnissen von „Get-AzureRmPolicyStateSummary“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="10f3d-144">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="10f3d-145">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="10f3d-145">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="10f3d-146">Parameter „-Vault“ zu den RecoveryServices.Backup-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="10f3d-146">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="10f3d-147">Bei der Übergabe wird dadurch das Cmdlet „Set-AzureRmRecoveryServicesContext“ außer Kraft gesetzt.</span><span class="sxs-lookup"><span data-stu-id="10f3d-147">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="10f3d-148">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="10f3d-148">AzureRM.Sql</span></span>
* <span data-ttu-id="10f3d-149">Aktualisiertes Beispiel in der Hilfedatei für „Get-AzureRmSqlDatabaseExpanded“</span><span class="sxs-lookup"><span data-stu-id="10f3d-149">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="10f3d-150">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="10f3d-150">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="10f3d-151">Hilfedatei für „Add-AzureRmTrafficManagerEndpointConfig“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="10f3d-151">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="10f3d-152">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="10f3d-152">AzureRM.Websites</span></span>
* <span data-ttu-id="10f3d-153">„Set-AzureRmWebApp“ wurde aktualisiert, damit „AppSettings“ bei der Verwendung von „-AssignIdentity“ nicht außer Kraft gesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="10f3d-153">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="10f3d-154">„New-AzureRmWebAppSlot“ wurde aktualisiert, um „AppServicePlan“ als optionalen Parameter anzuerkennen</span><span class="sxs-lookup"><span data-stu-id="10f3d-154">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="10f3d-155">6.2.1: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="10f3d-155">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="10f3d-156">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="10f3d-156">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="10f3d-157">PSWorkspace-Modell aktualisiert, damit das Netzwerk „type“ als Parameter verwenden kann</span><span class="sxs-lookup"><span data-stu-id="10f3d-157">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="10f3d-158">6.2.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="10f3d-158">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="10f3d-159">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="10f3d-159">AzureRM.Profile</span></span>
* <span data-ttu-id="10f3d-160">Beheben des Problems, aufgrund dessen Version 10.0.3 von Newtonsoft.Json beim Modulimport nicht geladen wurde</span><span class="sxs-lookup"><span data-stu-id="10f3d-160">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="10f3d-161">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="10f3d-161">AzureRM.Compute</span></span>
* <span data-ttu-id="10f3d-162">Feature zum Aktualisieren von virtuellen VMSS-Computern</span><span class="sxs-lookup"><span data-stu-id="10f3d-162">VMSS VM Update feature</span></span>
    - <span data-ttu-id="10f3d-163">Cmdlets „Update-AzureRmVmssVM“ und „New-AzureRmVMDataDisk“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="10f3d-163">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="10f3d-164">Fügen Sie den Parameter „VirtualMachineScaleSetVM“ zum Cmdlet „Add-AzureRmVMDataDisk“ hinzu, um das Hinzufügen eines Datenträgers zum virtuellen VMSS-Computer zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="10f3d-164">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="10f3d-165">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="10f3d-165">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="10f3d-166">Aktualisierung der ADF .Net SDK-Version auf 0.8.0-preview mit den folgenden Änderungen:</span><span class="sxs-lookup"><span data-stu-id="10f3d-166">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="10f3d-167">Vorgang zum Konfigurieren des Factoryrepositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="10f3d-167">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="10f3d-168">Der verknüpfte QuickBooks-Dienst wurde aktualisiert, um die Eigenschaften „consumerKey“ und „consumerSecret“ verfügbar zu machen.</span><span class="sxs-lookup"><span data-stu-id="10f3d-168">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="10f3d-169">Aktualisierung verschiedener Modelltypen von „SecretBase“ auf „Object“</span><span class="sxs-lookup"><span data-stu-id="10f3d-169">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="10f3d-170">Blobereignisauslöser hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="10f3d-170">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="10f3d-171">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="10f3d-171">AzureRM.KeyVault</span></span>
* <span data-ttu-id="10f3d-172">Aktualisierung der Dokumentation mit Beispielausgabe</span><span class="sxs-lookup"><span data-stu-id="10f3d-172">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="10f3d-173">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="10f3d-173">AzureRM.Network</span></span>
* <span data-ttu-id="10f3d-174">Aktivierung der Traffic Analytics-Parameter für Network Watcher-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="10f3d-174">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="10f3d-175">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="10f3d-175">AzureRM.Resources</span></span>
* <span data-ttu-id="10f3d-176">Behebung des Problems mit der Eigenschaft „Properties“ von PSResource-Objekten, die von „Get-AzureRmResource“ zurückgegeben wurden</span><span class="sxs-lookup"><span data-stu-id="10f3d-176">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="10f3d-177">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="10f3d-177">AzureRM.Scheduler</span></span>
* <span data-ttu-id="10f3d-178">Behebung des Problems, dass beim Aktualisieren von „ServiceBusQueueJob“ keine neuen Authentifizierungswerte festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="10f3d-178">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="10f3d-179">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="10f3d-179">AzureRM.Sql</span></span>
* <span data-ttu-id="10f3d-180">Aktualisierung der folgenden Cmdlets mit dem optionalen LicenseType-Parameter</span><span class="sxs-lookup"><span data-stu-id="10f3d-180">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="10f3d-181">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="10f3d-181">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="10f3d-182">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="10f3d-182">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="10f3d-183">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="10f3d-183">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="10f3d-184">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="10f3d-184">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="10f3d-185">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="10f3d-185">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="10f3d-186">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="10f3d-186">AzureRM.Websites</span></span>
* <span data-ttu-id="10f3d-187">„New-AzureRMWebApp“ aktualisiert, um allgemeine Algorithmen aus der Strategiebibliothek zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="10f3d-187">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="10f3d-188">6.1.0 – Mai 2018</span><span class="sxs-lookup"><span data-stu-id="10f3d-188">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="10f3d-189">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="10f3d-189">AzureRM.Profile</span></span>
* <span data-ttu-id="10f3d-190">Behebung eines Problems, durch das beim Ausführen von „Clear-AzureRmContext“ ein leerer Kontext mit dem Namen des vorherigen Standardkontexts beibehalten wurde und der Benutzer dadurch keinen neuen Kontext mit dem alten Namen erstellen konnte</span><span class="sxs-lookup"><span data-stu-id="10f3d-190">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="10f3d-191">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="10f3d-191">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="10f3d-192">Ermöglichung der Zuordnung von Gateways/Aufhebung der Gatewayzuordnung in AS</span><span class="sxs-lookup"><span data-stu-id="10f3d-192">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="10f3d-193">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="10f3d-193">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="10f3d-194">Unterstützung für „ApiVersions“, „ApiReleases“ und „ApiRevisions“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="10f3d-194">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="10f3d-195">Unterstützung für ServiceFabric-Back-End hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="10f3d-195">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="10f3d-196">Unterstützung für Application Insights-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="10f3d-196">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="10f3d-197">Unterstützung für die Erkennung von SKUs vom Typ „Basic“ als gültige SKU des API Management-Diensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="10f3d-197">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="10f3d-198">Unterstützung hinzugefügt, damit Zertifikate, die von der privaten Zertifizierungsstelle ausgestellt wurden, als Stamm- oder ZS-Zertifikate installiert werden können</span><span class="sxs-lookup"><span data-stu-id="10f3d-198">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="10f3d-199">Unterstützung für die Akzeptierung benutzerdefinierter SSL-Zertifikate über KeyVault und mehrere Proxyhostnamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="10f3d-199">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="10f3d-200">Unterstützung für die verwaltete Dienstidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="10f3d-200">Added support for MSI identity</span></span>
* <span data-ttu-id="10f3d-201">Unterstützung für die Annahme von Richtlinien über URL hinzugefügt; HINWEIS: Folgende Cmdlets werden in einem zukünftigen Release als veraltet gekennzeichnet:</span><span class="sxs-lookup"><span data-stu-id="10f3d-201">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="10f3d-202">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="10f3d-202">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="10f3d-203">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="10f3d-203">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="10f3d-204">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="10f3d-204">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="10f3d-205">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="10f3d-205">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="10f3d-206">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="10f3d-206">AzureRM.Batch</span></span>
* <span data-ttu-id="10f3d-207">Veröffentlichung des neuen Cmdlets „Get-AzureBatchPoolNodeCounts“</span><span class="sxs-lookup"><span data-stu-id="10f3d-207">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="10f3d-208">Veröffentlichung des neuen Cmdlets „Start-AzureBatchComputeNodeServiceLogUpload“</span><span class="sxs-lookup"><span data-stu-id="10f3d-208">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="10f3d-209">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="10f3d-209">AzureRM.Consumption</span></span>
* <span data-ttu-id="10f3d-210">Hinzufügung neuer Parameter („Expand“, „ResourceGroup“, „InstanceName“, „InstanceId“, „Tags“ und „Top“) für das Cmdlet „Get-AzureRmConsumptionUsageDetail“</span><span class="sxs-lookup"><span data-stu-id="10f3d-210">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="10f3d-211">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="10f3d-211">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="10f3d-212">Korrektur des Beispiels für „Export AzureRmDataLakeStoreChildItemProperties“</span><span class="sxs-lookup"><span data-stu-id="10f3d-212">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="10f3d-213">Korrektur der NULL-Parameterausnahme für rekursiven Fall in „Set-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="10f3d-213">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="10f3d-214">Korrektur der Hilfedateien für „Set-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ und „Remove-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="10f3d-214">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="10f3d-215">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="10f3d-215">AzureRM.Network</span></span>
* <span data-ttu-id="10f3d-216">Erhöhung der Network SDK-Version von 18.0.0-preview auf 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="10f3d-216">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="10f3d-217">Cmdlet zum Erstellen der Protokollkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="10f3d-217">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="10f3d-218">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="10f3d-218">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="10f3d-219">Cmdlet zum Hinzufügen einer neuen Leitungsverbindung zu einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="10f3d-219">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="10f3d-220">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="10f3d-220">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="10f3d-221">Cmdlet zum Entfernen einer Leitungsverbindung aus einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="10f3d-221">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="10f3d-222">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="10f3d-222">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="10f3d-223">Cmdlet zum Abrufen einer Leitungsverbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="10f3d-223">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="10f3d-224">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="10f3d-224">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="10f3d-225">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="10f3d-225">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="10f3d-226">Verwendung der Serverauthentifizierung mit generierten Zertifikaten korrigiert (Problemnr. 5998)</span><span class="sxs-lookup"><span data-stu-id="10f3d-226">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="10f3d-227">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="10f3d-227">AzureRM.Sql</span></span>
* <span data-ttu-id="10f3d-228">Überwachungscmdlets korrigiert, um das Entfernen von „AuditActions“ oder „AuditActionGroups“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="10f3d-228">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="10f3d-229">Problem mit „Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy“ behoben, das beim Festlegen einer neuen flexiblen Aufbewahrungsrichtlinie zu folgendem Fehler führte: „Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span><span class="sxs-lookup"><span data-stu-id="10f3d-229">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="10f3d-230">Please submit request with the new flexible retention policy“ (Das Konfigurieren einer langfristigen Aufbewahrungsrichtlinie mit Azure Recovery Service-Tresor und -Richtlinie wird nicht mehr unterstützt. Übermitteln Sie eine Anforderung mit der neuen flexiblen Aufbewahrungsrichtlinie.)</span><span class="sxs-lookup"><span data-stu-id="10f3d-230">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="10f3d-231">Aktualisierung aller Cmdlets für Azure SQL-Datenbank, für die Erstellung von Pools für elastische Datenbanken und für die Aktualisierung, sodass sie die neue Datenbank-API verwenden. Diese unterstützt die Sku-Eigenschaft für skalierungs- und tarifbezogene Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="10f3d-231">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="10f3d-232">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="10f3d-232">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="10f3d-233">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="10f3d-233">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="10f3d-234">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="10f3d-234">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="10f3d-235">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="10f3d-235">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="10f3d-236">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="10f3d-236">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="10f3d-237">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="10f3d-237">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="10f3d-238">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="10f3d-238">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="10f3d-239">Aktualisierung der Parameter für „Get-AzureRmTrafficManagerProfile“, sodass bei Verwendung des Parameters „-Name“ der Parameter „-ResourceGroupName“ erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="10f3d-239">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>