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
ms.openlocfilehash: 5bc3c9079cb4019bdb2255ab1f947e8ad35ae4cc
ms.sourcegitcommit: c98e3a21037ebd82936828bcb544eed902b24212
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/08/2018
ms.locfileid: "34853456"
---
# <a name="release-notes"></a><span data-ttu-id="957ef-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="957ef-103">Release notes</span></span>

<span data-ttu-id="957ef-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="957ef-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="620---june-2018"></a><span data-ttu-id="957ef-105">6.2.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="957ef-105">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="957ef-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="957ef-106">AzureRM.Profile</span></span>
* <span data-ttu-id="957ef-107">Beheben des Problems, aufgrund dessen Version 10.0.3 von Newtonsoft.Json beim Modulimport nicht geladen wurde</span><span class="sxs-lookup"><span data-stu-id="957ef-107">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="957ef-108">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="957ef-108">AzureRM.Compute</span></span>
* <span data-ttu-id="957ef-109">Feature zum Aktualisieren von virtuellen VMSS-Computern</span><span class="sxs-lookup"><span data-stu-id="957ef-109">VMSS VM Update feature</span></span>
    - <span data-ttu-id="957ef-110">Cmdlets „Update-AzureRmVmssVM“ und „New-AzureRmVMDataDisk“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="957ef-110">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="957ef-111">Fügen Sie den Parameter „VirtualMachineScaleSetVM“ zum Cmdlet „Add-AzureRmVMDataDisk“ hinzu, um das Hinzufügen eines Datenträgers zum virtuellen VMSS-Computer zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="957ef-111">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="957ef-112">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="957ef-112">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="957ef-113">Aktualisierung der ADF .Net SDK-Version auf 0.8.0-preview mit den folgenden Änderungen:</span><span class="sxs-lookup"><span data-stu-id="957ef-113">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="957ef-114">Vorgang zum Konfigurieren des Factoryrepositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="957ef-114">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="957ef-115">Der verknüpfte QuickBooks-Dienst wurde aktualisiert, um die Eigenschaften „consumerKey“ und „consumerSecret“ verfügbar zu machen.</span><span class="sxs-lookup"><span data-stu-id="957ef-115">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="957ef-116">Aktualisierung verschiedener Modelltypen von „SecretBase“ auf „Object“</span><span class="sxs-lookup"><span data-stu-id="957ef-116">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="957ef-117">Blobereignisauslöser hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="957ef-117">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="957ef-118">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="957ef-118">AzureRM.KeyVault</span></span>
* <span data-ttu-id="957ef-119">Aktualisierung der Dokumentation mit Beispielausgabe</span><span class="sxs-lookup"><span data-stu-id="957ef-119">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="957ef-120">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="957ef-120">AzureRM.Network</span></span>
* <span data-ttu-id="957ef-121">Aktivierung der Traffic Analytics-Parameter für Network Watcher-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="957ef-121">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="957ef-122">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="957ef-122">AzureRM.Resources</span></span>
* <span data-ttu-id="957ef-123">Behebung des Problems mit der Eigenschaft „Properties“ von PSResource-Objekten, die von „Get-AzureRmResource“ zurückgegeben wurden</span><span class="sxs-lookup"><span data-stu-id="957ef-123">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="957ef-124">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="957ef-124">AzureRM.Scheduler</span></span>
* <span data-ttu-id="957ef-125">Behebung des Problems, dass beim Aktualisieren von „ServiceBusQueueJob“ keine neuen Authentifizierungswerte festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="957ef-125">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="957ef-126">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="957ef-126">AzureRM.Sql</span></span>
* <span data-ttu-id="957ef-127">Aktualisierung der folgenden Cmdlets mit dem optionalen LicenseType-Parameter</span><span class="sxs-lookup"><span data-stu-id="957ef-127">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="957ef-128">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="957ef-128">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="957ef-129">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="957ef-129">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="957ef-130">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="957ef-130">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="957ef-131">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="957ef-131">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="957ef-132">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="957ef-132">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="957ef-133">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="957ef-133">AzureRM.Websites</span></span>
* <span data-ttu-id="957ef-134">„New-AzureRMWebApp“ aktualisiert, um allgemeine Algorithmen aus der Strategiebibliothek zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="957ef-134">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="957ef-135">6.1.0 – Mai 2018</span><span class="sxs-lookup"><span data-stu-id="957ef-135">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="957ef-136">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="957ef-136">AzureRM.Profile</span></span>
* <span data-ttu-id="957ef-137">Behebung eines Problems, durch das beim Ausführen von „Clear-AzureRmContext“ ein leerer Kontext mit dem Namen des vorherigen Standardkontexts beibehalten wurde und der Benutzer dadurch keinen neuen Kontext mit dem alten Namen erstellen konnte</span><span class="sxs-lookup"><span data-stu-id="957ef-137">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="957ef-138">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="957ef-138">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="957ef-139">Ermöglichung der Zuordnung von Gateways/Aufhebung der Gatewayzuordnung in AS</span><span class="sxs-lookup"><span data-stu-id="957ef-139">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="957ef-140">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="957ef-140">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="957ef-141">Unterstützung für „ApiVersions“, „ApiReleases“ und „ApiRevisions“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="957ef-141">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="957ef-142">Unterstützung für ServiceFabric-Back-End hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="957ef-142">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="957ef-143">Unterstützung für Application Insights-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="957ef-143">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="957ef-144">Unterstützung für die Erkennung von SKUs vom Typ „Basic“ als gültige SKU des API Management-Diensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="957ef-144">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="957ef-145">Unterstützung hinzugefügt, damit Zertifikate, die von der privaten Zertifizierungsstelle ausgestellt wurden, als Stamm- oder ZS-Zertifikate installiert werden können</span><span class="sxs-lookup"><span data-stu-id="957ef-145">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="957ef-146">Unterstützung für die Akzeptierung benutzerdefinierter SSL-Zertifikate über KeyVault und mehrere Proxyhostnamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="957ef-146">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="957ef-147">Unterstützung für die verwaltete Dienstidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="957ef-147">Added support for MSI identity</span></span>
* <span data-ttu-id="957ef-148">Unterstützung für die Annahme von Richtlinien über URL hinzugefügt; HINWEIS: Folgende Cmdlets werden in einem zukünftigen Release als veraltet gekennzeichnet:</span><span class="sxs-lookup"><span data-stu-id="957ef-148">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="957ef-149">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="957ef-149">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="957ef-150">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="957ef-150">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="957ef-151">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="957ef-151">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="957ef-152">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="957ef-152">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="957ef-153">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="957ef-153">AzureRM.Batch</span></span>
* <span data-ttu-id="957ef-154">Veröffentlichung des neuen Cmdlets „Get-AzureBatchPoolNodeCounts“</span><span class="sxs-lookup"><span data-stu-id="957ef-154">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="957ef-155">Veröffentlichung des neuen Cmdlets „Start-AzureBatchComputeNodeServiceLogUpload“</span><span class="sxs-lookup"><span data-stu-id="957ef-155">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="957ef-156">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="957ef-156">AzureRM.Consumption</span></span>
* <span data-ttu-id="957ef-157">Hinzufügung neuer Parameter („Expand“, „ResourceGroup“, „InstanceName“, „InstanceId“, „Tags“ und „Top“) für das Cmdlet „Get-AzureRmConsumptionUsageDetail“</span><span class="sxs-lookup"><span data-stu-id="957ef-157">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="957ef-158">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="957ef-158">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="957ef-159">Korrektur des Beispiels für „Export AzureRmDataLakeStoreChildItemProperties“</span><span class="sxs-lookup"><span data-stu-id="957ef-159">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="957ef-160">Korrektur der NULL-Parameterausnahme für rekursiven Fall in „Set-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="957ef-160">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="957ef-161">Korrektur der Hilfedateien für „Set-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ und „Remove-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="957ef-161">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="957ef-162">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="957ef-162">AzureRM.Network</span></span>
* <span data-ttu-id="957ef-163">Erhöhung der Network SDK-Version von 18.0.0-preview auf 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="957ef-163">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="957ef-164">Cmdlet zum Erstellen der Protokollkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="957ef-164">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="957ef-165">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="957ef-165">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="957ef-166">Cmdlet zum Hinzufügen einer neuen Leitungsverbindung zu einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="957ef-166">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="957ef-167">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="957ef-167">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="957ef-168">Cmdlet zum Entfernen einer Leitungsverbindung aus einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="957ef-168">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="957ef-169">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="957ef-169">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="957ef-170">Cmdlet zum Abrufen einer Leitungsverbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="957ef-170">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="957ef-171">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="957ef-171">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="957ef-172">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="957ef-172">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="957ef-173">Verwendung der Serverauthentifizierung mit generierten Zertifikaten korrigiert (Problemnr. 5998)</span><span class="sxs-lookup"><span data-stu-id="957ef-173">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="957ef-174">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="957ef-174">AzureRM.Sql</span></span>
* <span data-ttu-id="957ef-175">Überwachungscmdlets korrigiert, um das Entfernen von „AuditActions“ oder „AuditActionGroups“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="957ef-175">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="957ef-176">Problem mit „Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy“ behoben, das beim Festlegen einer neuen flexiblen Aufbewahrungsrichtlinie zu folgendem Fehler führte: „Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span><span class="sxs-lookup"><span data-stu-id="957ef-176">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="957ef-177">Please submit request with the new flexible retention policy“ (Das Konfigurieren einer langfristigen Aufbewahrungsrichtlinie mit Azure Recovery Service-Tresor und -Richtlinie wird nicht mehr unterstützt. Übermitteln Sie eine Anforderung mit der neuen flexiblen Aufbewahrungsrichtlinie.)</span><span class="sxs-lookup"><span data-stu-id="957ef-177">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="957ef-178">Aktualisierung aller Cmdlets für Azure SQL-Datenbank, für die Erstellung von Pools für elastische Datenbanken und für die Aktualisierung, sodass sie die neue Datenbank-API verwenden. Diese unterstützt die Sku-Eigenschaft für skalierungs- und tarifbezogene Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="957ef-178">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="957ef-179">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="957ef-179">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="957ef-180">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="957ef-180">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="957ef-181">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="957ef-181">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="957ef-182">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="957ef-182">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="957ef-183">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="957ef-183">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="957ef-184">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="957ef-184">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="957ef-185">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="957ef-185">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="957ef-186">Aktualisierung der Parameter für „Get-AzureRmTrafficManagerProfile“, sodass bei Verwendung des Parameters „-Name“ der Parameter „-ResourceGroupName“ erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="957ef-186">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>