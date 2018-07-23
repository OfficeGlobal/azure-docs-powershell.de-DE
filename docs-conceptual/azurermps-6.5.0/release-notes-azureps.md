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
ms.openlocfilehash: e9fa2d75c1c4e6ffaa2f7dd8e400f5b13dd4527d
ms.sourcegitcommit: 8b882d1c27d9e323447ff85f56d11bbf5e244d7f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/18/2018
ms.locfileid: "39110482"
---
# <a name="release-notes"></a><span data-ttu-id="4c18f-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="4c18f-103">Release notes</span></span>

<span data-ttu-id="4c18f-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="4c18f-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="650---july-2018"></a><span data-ttu-id="4c18f-105">6.5.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="4c18f-105">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="4c18f-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="4c18f-106">AzureRM.Profile</span></span>
* <span data-ttu-id="4c18f-107">Hilfe für „Get-AzureRmContextAutosaveSetting“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4c18f-107">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="4c18f-108">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="4c18f-108">Azure.Storage</span></span>
* <span data-ttu-id="4c18f-109">Unterstützung des Blob- oder Dateiuploads mit lesegeschütztem SAS-Token</span><span class="sxs-lookup"><span data-stu-id="4c18f-109">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="4c18f-110">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="4c18f-110">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="4c18f-111">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="4c18f-111">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="4c18f-112">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="4c18f-112">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="4c18f-113">Erforderliche Eigenschaft „ResourceGroupName“ zu AS hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4c18f-113">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="4c18f-114">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="4c18f-114">AzureRM.Automation</span></span>
* <span data-ttu-id="4c18f-115">Hilfe aktualisiert und Beispiel für „New-AzureRMAutomationSchedule“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-115">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="4c18f-116">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="4c18f-116">AzureRM.Compute</span></span>
* <span data-ttu-id="4c18f-117">Parameter „-Tag“ zu „Update/New-AzureRmAvailabilitySet“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-117">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="4c18f-118">Beispiel für „Add-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-118">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="4c18f-119">Beispiele für „Remove-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-119">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="4c18f-120">Hilfe für „Set-AzureRmVMAccessExtension“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4c18f-120">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="4c18f-121">„SimpleParameterSet“ für „New-AzureRmVmss“ so aktualisiert, dass „SinglePlacementGroup“ standardmäßig auf „false“ festgelegt ist, und Switch-Parameter „SinglePlacementGroup“ hinzugefügt, der dem Benutzer das Erstellen der VMSS in einer einzelnen Platzierungsgruppe ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="4c18f-121">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="4c18f-122">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="4c18f-122">AzureRM.EventHub</span></span>
* <span data-ttu-id="4c18f-123">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSEventHubDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="4c18f-123">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="4c18f-124">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="4c18f-124">AzureRM.KeyVault</span></span>
* <span data-ttu-id="4c18f-125">Fehlermeldung für „Set-AzureRmKeyVaultAccessPolicy“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4c18f-125">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="4c18f-126">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="4c18f-126">AzureRM.LogicApp</span></span>
* <span data-ttu-id="4c18f-127">Fehler „Parametersatz konnte nicht aufgelöst werden“ in „New-AzureRmLogicApp“behoben</span><span class="sxs-lookup"><span data-stu-id="4c18f-127">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="4c18f-128">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="4c18f-128">AzureRM.Network</span></span>
* <span data-ttu-id="4c18f-129">Peering über mehrere virtuelle Netzwerke in mehreren Mandanten für „Set/Add-AzureRmVirtualNetworkPeering“ aktiviert</span><span class="sxs-lookup"><span data-stu-id="4c18f-129">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="4c18f-130">Folgende Cmdlets für Application Gateway aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4c18f-130">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="4c18f-131">New-AzureRmApplicationGateway: EnableFIPS-Flag und Zonenunterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-131">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="4c18f-132">New-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-132">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="4c18f-133">Set-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-133">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="4c18f-134">RouteTable-Cmdlets mit aktueller Generatorversion erneut generiert</span><span class="sxs-lookup"><span data-stu-id="4c18f-134">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="4c18f-135">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="4c18f-135">AzureRM.Relay</span></span>
* <span data-ttu-id="4c18f-136">Markdowndateien aktualisiert, Problem mit Parametername in Beispiel behoben</span><span class="sxs-lookup"><span data-stu-id="4c18f-136">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="4c18f-137">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="4c18f-137">AzureRM.Resources</span></span>
* <span data-ttu-id="4c18f-138">Roleassignment- und roledefinition-Cmdlets aktualisiert:</span><span class="sxs-lookup"><span data-stu-id="4c18f-138">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="4c18f-139">Zusätzliche roledefinition-Aufrufe entfernt, die als Teil des Pagings durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="4c18f-139">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="4c18f-140">Get-AzureRmRoleAssignment-Cmdlet korrigiert</span><span class="sxs-lookup"><span data-stu-id="4c18f-140">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="4c18f-141">Befehlsparameterfunktion von „-ExpandPrincipalGroups“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="4c18f-141">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="4c18f-142">Problem mit „Get-AzureRmResource“ behoben, aufgrund dessen die Groß-/Kleinschreibung des Parameters „-ResourceType“ beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="4c18f-142">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="4c18f-143">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="4c18f-143">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="4c18f-144">top- und skip-Parameter zu Listen-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-144">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="4c18f-145">Cmdlets für die Migration von Standard- zu Premium-Namespace hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="4c18f-145">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="4c18f-146">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="4c18f-146">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="4c18f-147">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="4c18f-147">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="4c18f-148">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="4c18f-148">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="4c18f-149">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="4c18f-149">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="4c18f-150">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="4c18f-150">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="4c18f-151">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSServiceBusDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="4c18f-151">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="4c18f-152">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="4c18f-152">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="4c18f-153">Beispiel für „New-AzureRmServiceFabricCluster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-153">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="4c18f-154">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="4c18f-154">AzureRM.Sql</span></span>
* <span data-ttu-id="4c18f-155">Neue Cmdlets für „Management.Sql“ hinzugefügt, um Kunden das Hinzufügen des TDE-Zertifikats zu einer SQL Server-Instanz oder einer verwalteten Instanz zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4c18f-155">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="4c18f-156">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="4c18f-156">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="4c18f-157">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="4c18f-157">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="4c18f-158">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="4c18f-158">AzureRM.Websites</span></span>
* <span data-ttu-id="4c18f-159">Wenn `Set-AzureRmWebApp -AssignIdentity` und `Set-AzureRmWebAppSlot -AssignIdentity` auf „false“ festgelegt sind, wird jetzt die Identity-Eigenschaft aus dem Websiteobjekt entfernt. Auch das Vorschau-Tag wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="4c18f-159">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="4c18f-160">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics`-Beispiel aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4c18f-160">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="4c18f-161">Unterstützung von `Set-AzureRmWebApp -PhpVersion` als gültige PHP-Version eingestellt</span><span class="sxs-lookup"><span data-stu-id="4c18f-161">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="4c18f-162">6.4.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="4c18f-162">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="4c18f-163">Allgemein</span><span class="sxs-lookup"><span data-stu-id="4c18f-163">General</span></span>
* <span data-ttu-id="4c18f-164">Formatierung von OutputType in Hilfedateien für die meisten Module korrigiert</span><span class="sxs-lookup"><span data-stu-id="4c18f-164">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="4c18f-165">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="4c18f-165">AzureRM.Profile</span></span>
* <span data-ttu-id="4c18f-166">Attribut „Ps1Xml“ wurde den Standardausgabetypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-166">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="4c18f-167">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="4c18f-167">AzureRM.Compute</span></span>
* <span data-ttu-id="4c18f-168">IP-Tag-Funktion für VMSS</span><span class="sxs-lookup"><span data-stu-id="4c18f-168">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="4c18f-169">Cmdlet „New-AzureRmVmssIpTagConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-169">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="4c18f-170">IpTag-Parameter zu „New-AzureRmVmssIpConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-170">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="4c18f-171">Funktion für automatisches Betriebssystemrollback für VMSS</span><span class="sxs-lookup"><span data-stu-id="4c18f-171">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="4c18f-172">DisableAutoRollback-Parameter zu „New-AzureRmVmssConfig“ und „Update-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-172">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="4c18f-173">Funktion für Upgradeverlauf des Betriebssystems für VMSS</span><span class="sxs-lookup"><span data-stu-id="4c18f-173">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="4c18f-174">Switch-Parameter „OSUpgradeHistory“ zu „Get-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-174">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="4c18f-175">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="4c18f-175">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="4c18f-176">Unterstützung für Katalog-ACLs über die folgenden Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="4c18f-176">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="4c18f-177">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="4c18f-177">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="4c18f-178">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="4c18f-178">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="4c18f-179">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="4c18f-179">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="4c18f-180">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="4c18f-180">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="4c18f-181">Abbruchunterstützung und Nachverfolgung des Fortschritts für „Set-AzureRmDataLakeStoreItemAclEntry“, „Remove-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-181">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="4c18f-182">Abbruchunterstützung „Export-AzureRmDataLakeStoreChildItemProperties“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-182">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="4c18f-183">Leerung von Debugmeldungen für Cmdlets korrigiert, die rekursive Vorgänge durchführt</span><span class="sxs-lookup"><span data-stu-id="4c18f-183">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="4c18f-184">Speicherort des Test von DataLake-Cmdlets korrigiert</span><span class="sxs-lookup"><span data-stu-id="4c18f-184">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="4c18f-185">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="4c18f-185">AzureRM.EventHub</span></span>
* <span data-ttu-id="4c18f-186">Optionaler Parameter „MaxCount“ zu Listenvorgangs-Cmdlets „Get-AzureRmEventHub“ und „Get-AzureRmEventHubConsumerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-186">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="4c18f-187">Problem in Cmdlet „New-AzureRmEventHub“ behoben, aufgrund dessen beim Erstellen einer neuen EventHub-Instanz mindestens ein Parameter benötigt wurde.</span><span class="sxs-lookup"><span data-stu-id="4c18f-187">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="4c18f-188">Standardparametersatz wurde bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="4c18f-188">Provided Default Parameter set.</span></span>
* <span data-ttu-id="4c18f-189">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmEventHubKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="4c18f-189">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="4c18f-190">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="4c18f-190">AzureRM.KeyVault</span></span>
* <span data-ttu-id="4c18f-191">Problem behoben, aufgrund dessen von „Get-AzureRmKeyVault -Tag“ alle Ressourcen zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="4c18f-191">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="4c18f-192">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="4c18f-192">AzureRM.Network</span></span>
* <span data-ttu-id="4c18f-193">Neue SKUs für zonenredundante VirtualNetworkGateways-Instanzen verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="4c18f-193">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="4c18f-194">Neue Befehle für Funktion hinzugefügt: ExpressRoute-Partner-APIs über ARM</span><span class="sxs-lookup"><span data-stu-id="4c18f-194">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="4c18f-195">Get-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-195">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="4c18f-196">Set-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-196">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="4c18f-197">Add-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-197">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="4c18f-198">Get-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-198">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="4c18f-199">Remove-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-199">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="4c18f-200">Get-AzureRMExpressRouteCrossConnectionArpTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-200">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="4c18f-201">Get-AzureRMExpressRouteCrossConnectionRouteTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-201">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="4c18f-202">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-202">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="4c18f-203">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="4c18f-203">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="4c18f-204">Cmdlet „Get-AzureRmRecoveryServicesBackupStatus“ wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4c18f-204">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="4c18f-205">Dieses Cmdlet überprüft anhand der ID eines virtuellen Computers, ob dieser durch einen Tresor im Abonnement geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="4c18f-205">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="4c18f-206">Wenn ein solcher Tresor vorhanden ist, gibt das Cmdlet die Tresordetails aus.</span><span class="sxs-lookup"><span data-stu-id="4c18f-206">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="4c18f-207">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="4c18f-207">AzureRM.Resources</span></span>
* <span data-ttu-id="4c18f-208">Cmdlets vom Typ „Get-AzureRmPolicyAssignment“ aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="4c18f-208">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="4c18f-209">Unterstützung für das Auflisten von „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-209">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="4c18f-210">Unterstützung für das Abrufen einzelner Arbeitsaufträge mit „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-210">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="4c18f-211">Switches „-Effective“ und „-All“ zu Steuerparameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-211">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="4c18f-212">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicyDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4c18f-212">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="4c18f-213">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="4c18f-213">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="4c18f-214">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="4c18f-214">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="4c18f-215">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicySetDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4c18f-215">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="4c18f-216">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="4c18f-216">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="4c18f-217">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="4c18f-217">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="4c18f-218">Unterstützung für KeyVault-Geheimnisverweis in Parametern hinzugefügt, wenn „TemplateParameterObject“ in „New-AzureRmResourceGroupDeployment“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="4c18f-218">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="4c18f-219">Problem behoben, aufgrund dessen, der Parameter „-EndDate“ für „New-AzureRmADAppCredential“ ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="4c18f-219">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="4c18f-220">Problem behoben, aufgrund dessen „Add-AzureRmADGroupMember“ eine falsche URL für Anforderungen verwendete</span><span class="sxs-lookup"><span data-stu-id="4c18f-220">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="4c18f-221">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="4c18f-221">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="4c18f-222">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmServiceBusKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="4c18f-222">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="4c18f-223">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="4c18f-223">AzureRM.Sql</span></span>
* <span data-ttu-id="4c18f-224">Benutzerdefinierte Wiederherstellungspunkte für SQLDW in Hilfe zu „New-AzureRmSqlDatabaseRestorePoint“ erläutert</span><span class="sxs-lookup"><span data-stu-id="4c18f-224">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="4c18f-225">Dokumentation von Parameter „-ComputeGeneration“ in mehreren Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4c18f-225">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="4c18f-226">6.3.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="4c18f-226">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="4c18f-227">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="4c18f-227">AzureRM.Profile</span></span>
* <span data-ttu-id="4c18f-228">Aktualisierte Fehlermeldungen für „Enable-AzureRmContextAutoSave“</span><span class="sxs-lookup"><span data-stu-id="4c18f-228">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="4c18f-229">Erstellen eines Kontexts für jedes Abonnement beim Ausführen von „Connect-AzureRmAccount“ ohne vorherigen Kontext</span><span class="sxs-lookup"><span data-stu-id="4c18f-229">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="4c18f-230">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="4c18f-230">Azure.Storage</span></span>
* <span data-ttu-id="4c18f-231">Zusätzliche Informationen zum Parameter „-Permissions“ in Hilfedateien</span><span class="sxs-lookup"><span data-stu-id="4c18f-231">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="4c18f-232">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="4c18f-232">AzureRM.Compute</span></span>
* <span data-ttu-id="4c18f-233">„Get-AzureRmVmDiskEncryptionStatus“ behebt ein Problem, das bei virtuellen Computern ohne Datenträger festgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="4c18f-233">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="4c18f-234">Version der Computeclientbibliothek aktualisiert, um folgende Cmdlets zu korrigieren:</span><span class="sxs-lookup"><span data-stu-id="4c18f-234">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="4c18f-235">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="4c18f-235">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="4c18f-236">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="4c18f-236">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="4c18f-237">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="4c18f-237">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="4c18f-238">Die folgenden Cmdlets wurden korrigiert, um die Vorgangs-ID und den Vorgangsstatus korrekt anzuzeigen:</span><span class="sxs-lookup"><span data-stu-id="4c18f-238">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="4c18f-239">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="4c18f-239">Start-AzureRmVM</span></span>
    - <span data-ttu-id="4c18f-240">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="4c18f-240">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="4c18f-241">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="4c18f-241">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="4c18f-242">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="4c18f-242">Set-AzureRmVM</span></span>
    - <span data-ttu-id="4c18f-243">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="4c18f-243">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="4c18f-244">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="4c18f-244">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="4c18f-245">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="4c18f-245">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="4c18f-246">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="4c18f-246">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="4c18f-247">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="4c18f-247">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="4c18f-248">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="4c18f-248">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="4c18f-249">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="4c18f-249">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="4c18f-250">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="4c18f-250">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="4c18f-251">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="4c18f-251">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="4c18f-252">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="4c18f-252">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="4c18f-253">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="4c18f-253">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="4c18f-254">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="4c18f-254">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="4c18f-255">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="4c18f-255">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="4c18f-256">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="4c18f-256">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="4c18f-257">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="4c18f-257">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="4c18f-258">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="4c18f-258">AzureRM.EventGrid</span></span>
* <span data-ttu-id="4c18f-259">ValidateNotNullOrEmpty-Überprüfungskonditionen für „SubjectBeginsWith“/„SubjectEndsWith“ im Cmdlet „Update-AzureRmEventGridSubscription“ wurden entfernt, um bei Bedarf die Änderung dieser Parameter in eine leere Zeichenfolge zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="4c18f-259">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="4c18f-260">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="4c18f-260">AzureRM.KeyVault</span></span>
* <span data-ttu-id="4c18f-261">Ein Problem wurde behoben, aufgrund dessen bei Ausführung von „Get-AzureRmKeyVault -Tag“ keine Tags zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="4c18f-261">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="4c18f-262">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="4c18f-262">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="4c18f-263">Offizielle Veröffentlichung von Policy Insights-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="4c18f-263">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="4c18f-264">Verwendung der API-Version 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="4c18f-264">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="4c18f-265">„PolicyDefinitionReferenceId“ zu den Ergebnissen von „Get-AzureRmPolicyStateSummary“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-265">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="4c18f-266">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="4c18f-266">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="4c18f-267">Parameter „-Vault“ zu den RecoveryServices.Backup-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4c18f-267">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="4c18f-268">Bei der Übergabe wird dadurch das Cmdlet „Set-AzureRmRecoveryServicesContext“ außer Kraft gesetzt.</span><span class="sxs-lookup"><span data-stu-id="4c18f-268">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="4c18f-269">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="4c18f-269">AzureRM.Sql</span></span>
* <span data-ttu-id="4c18f-270">Aktualisiertes Beispiel in der Hilfedatei für „Get-AzureRmSqlDatabaseExpanded“</span><span class="sxs-lookup"><span data-stu-id="4c18f-270">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="4c18f-271">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="4c18f-271">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="4c18f-272">Hilfedatei für „Add-AzureRmTrafficManagerEndpointConfig“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4c18f-272">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="4c18f-273">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="4c18f-273">AzureRM.Websites</span></span>
* <span data-ttu-id="4c18f-274">„Set-AzureRmWebApp“ wurde aktualisiert, damit „AppSettings“ bei der Verwendung von „-AssignIdentity“ nicht außer Kraft gesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="4c18f-274">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="4c18f-275">„New-AzureRmWebAppSlot“ wurde aktualisiert, um „AppServicePlan“ als optionalen Parameter anzuerkennen</span><span class="sxs-lookup"><span data-stu-id="4c18f-275">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="4c18f-276">6.2.1: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="4c18f-276">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="4c18f-277">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="4c18f-277">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="4c18f-278">PSWorkspace-Modell aktualisiert, damit das Netzwerk „type“ als Parameter verwenden kann</span><span class="sxs-lookup"><span data-stu-id="4c18f-278">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="4c18f-279">6.2.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="4c18f-279">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="4c18f-280">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="4c18f-280">AzureRM.Profile</span></span>
* <span data-ttu-id="4c18f-281">Beheben des Problems, aufgrund dessen Version 10.0.3 von Newtonsoft.Json beim Modulimport nicht geladen wurde</span><span class="sxs-lookup"><span data-stu-id="4c18f-281">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="4c18f-282">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="4c18f-282">AzureRM.Compute</span></span>
* <span data-ttu-id="4c18f-283">Feature zum Aktualisieren von virtuellen VMSS-Computern</span><span class="sxs-lookup"><span data-stu-id="4c18f-283">VMSS VM Update feature</span></span>
    - <span data-ttu-id="4c18f-284">Cmdlets „Update-AzureRmVmssVM“ und „New-AzureRmVMDataDisk“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-284">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="4c18f-285">Fügen Sie den Parameter „VirtualMachineScaleSetVM“ zum Cmdlet „Add-AzureRmVMDataDisk“ hinzu, um das Hinzufügen eines Datenträgers zum virtuellen VMSS-Computer zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="4c18f-285">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="4c18f-286">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="4c18f-286">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="4c18f-287">Aktualisierung der ADF .Net SDK-Version auf 0.8.0-preview mit den folgenden Änderungen:</span><span class="sxs-lookup"><span data-stu-id="4c18f-287">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="4c18f-288">Vorgang zum Konfigurieren des Factoryrepositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-288">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="4c18f-289">Der verknüpfte QuickBooks-Dienst wurde aktualisiert, um die Eigenschaften „consumerKey“ und „consumerSecret“ verfügbar zu machen.</span><span class="sxs-lookup"><span data-stu-id="4c18f-289">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="4c18f-290">Aktualisierung verschiedener Modelltypen von „SecretBase“ auf „Object“</span><span class="sxs-lookup"><span data-stu-id="4c18f-290">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="4c18f-291">Blobereignisauslöser hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-291">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="4c18f-292">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="4c18f-292">AzureRM.KeyVault</span></span>
* <span data-ttu-id="4c18f-293">Aktualisierung der Dokumentation mit Beispielausgabe</span><span class="sxs-lookup"><span data-stu-id="4c18f-293">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="4c18f-294">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="4c18f-294">AzureRM.Network</span></span>
* <span data-ttu-id="4c18f-295">Aktivierung der Traffic Analytics-Parameter für Network Watcher-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="4c18f-295">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="4c18f-296">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="4c18f-296">AzureRM.Resources</span></span>
* <span data-ttu-id="4c18f-297">Behebung des Problems mit der Eigenschaft „Properties“ von PSResource-Objekten, die von „Get-AzureRmResource“ zurückgegeben wurden</span><span class="sxs-lookup"><span data-stu-id="4c18f-297">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="4c18f-298">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="4c18f-298">AzureRM.Scheduler</span></span>
* <span data-ttu-id="4c18f-299">Behebung des Problems, dass beim Aktualisieren von „ServiceBusQueueJob“ keine neuen Authentifizierungswerte festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="4c18f-299">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="4c18f-300">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="4c18f-300">AzureRM.Sql</span></span>
* <span data-ttu-id="4c18f-301">Aktualisierung der folgenden Cmdlets mit dem optionalen LicenseType-Parameter</span><span class="sxs-lookup"><span data-stu-id="4c18f-301">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="4c18f-302">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="4c18f-302">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="4c18f-303">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="4c18f-303">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="4c18f-304">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="4c18f-304">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="4c18f-305">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="4c18f-305">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="4c18f-306">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="4c18f-306">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="4c18f-307">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="4c18f-307">AzureRM.Websites</span></span>
* <span data-ttu-id="4c18f-308">„New-AzureRMWebApp“ aktualisiert, um allgemeine Algorithmen aus der Strategiebibliothek zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="4c18f-308">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="4c18f-309">6.1.0 – Mai 2018</span><span class="sxs-lookup"><span data-stu-id="4c18f-309">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="4c18f-310">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="4c18f-310">AzureRM.Profile</span></span>
* <span data-ttu-id="4c18f-311">Behebung eines Problems, durch das beim Ausführen von „Clear-AzureRmContext“ ein leerer Kontext mit dem Namen des vorherigen Standardkontexts beibehalten wurde und der Benutzer dadurch keinen neuen Kontext mit dem alten Namen erstellen konnte</span><span class="sxs-lookup"><span data-stu-id="4c18f-311">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="4c18f-312">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="4c18f-312">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="4c18f-313">Ermöglichung der Zuordnung von Gateways/Aufhebung der Gatewayzuordnung in AS</span><span class="sxs-lookup"><span data-stu-id="4c18f-313">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="4c18f-314">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="4c18f-314">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="4c18f-315">Unterstützung für „ApiVersions“, „ApiReleases“ und „ApiRevisions“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-315">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="4c18f-316">Unterstützung für ServiceFabric-Back-End hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-316">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="4c18f-317">Unterstützung für Application Insights-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-317">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="4c18f-318">Unterstützung für die Erkennung von SKUs vom Typ „Basic“ als gültige SKU des API Management-Diensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-318">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="4c18f-319">Unterstützung hinzugefügt, damit Zertifikate, die von der privaten Zertifizierungsstelle ausgestellt wurden, als Stamm- oder ZS-Zertifikate installiert werden können</span><span class="sxs-lookup"><span data-stu-id="4c18f-319">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="4c18f-320">Unterstützung für die Akzeptierung benutzerdefinierter SSL-Zertifikate über KeyVault und mehrere Proxyhostnamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-320">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="4c18f-321">Unterstützung für die verwaltete Dienstidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-321">Added support for MSI identity</span></span>
* <span data-ttu-id="4c18f-322">Unterstützung für die Annahme von Richtlinien über URL hinzugefügt; HINWEIS: Folgende Cmdlets werden in einem zukünftigen Release als veraltet gekennzeichnet:</span><span class="sxs-lookup"><span data-stu-id="4c18f-322">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="4c18f-323">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="4c18f-323">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="4c18f-324">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="4c18f-324">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="4c18f-325">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="4c18f-325">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="4c18f-326">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="4c18f-326">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="4c18f-327">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="4c18f-327">AzureRM.Batch</span></span>
* <span data-ttu-id="4c18f-328">Veröffentlichung des neuen Cmdlets „Get-AzureBatchPoolNodeCounts“</span><span class="sxs-lookup"><span data-stu-id="4c18f-328">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="4c18f-329">Veröffentlichung des neuen Cmdlets „Start-AzureBatchComputeNodeServiceLogUpload“</span><span class="sxs-lookup"><span data-stu-id="4c18f-329">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="4c18f-330">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="4c18f-330">AzureRM.Consumption</span></span>
* <span data-ttu-id="4c18f-331">Hinzufügung neuer Parameter („Expand“, „ResourceGroup“, „InstanceName“, „InstanceId“, „Tags“ und „Top“) für das Cmdlet „Get-AzureRmConsumptionUsageDetail“</span><span class="sxs-lookup"><span data-stu-id="4c18f-331">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="4c18f-332">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="4c18f-332">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="4c18f-333">Korrektur des Beispiels für „Export AzureRmDataLakeStoreChildItemProperties“</span><span class="sxs-lookup"><span data-stu-id="4c18f-333">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="4c18f-334">Korrektur der NULL-Parameterausnahme für rekursiven Fall in „Set-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="4c18f-334">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="4c18f-335">Korrektur der Hilfedateien für „Set-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ und „Remove-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="4c18f-335">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="4c18f-336">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="4c18f-336">AzureRM.Network</span></span>
* <span data-ttu-id="4c18f-337">Erhöhung der Network SDK-Version von 18.0.0-preview auf 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="4c18f-337">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="4c18f-338">Cmdlet zum Erstellen der Protokollkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-338">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="4c18f-339">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="4c18f-339">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="4c18f-340">Cmdlet zum Hinzufügen einer neuen Leitungsverbindung zu einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-340">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="4c18f-341">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="4c18f-341">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="4c18f-342">Cmdlet zum Entfernen einer Leitungsverbindung aus einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-342">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="4c18f-343">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="4c18f-343">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="4c18f-344">Cmdlet zum Abrufen einer Leitungsverbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4c18f-344">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="4c18f-345">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="4c18f-345">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="4c18f-346">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="4c18f-346">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="4c18f-347">Verwendung der Serverauthentifizierung mit generierten Zertifikaten korrigiert (Problemnr. 5998)</span><span class="sxs-lookup"><span data-stu-id="4c18f-347">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="4c18f-348">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="4c18f-348">AzureRM.Sql</span></span>
* <span data-ttu-id="4c18f-349">Überwachungscmdlets korrigiert, um das Entfernen von „AuditActions“ oder „AuditActionGroups“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4c18f-349">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="4c18f-350">Problem mit „Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy“ behoben, das beim Festlegen einer neuen flexiblen Aufbewahrungsrichtlinie zu folgendem Fehler führte: „Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span><span class="sxs-lookup"><span data-stu-id="4c18f-350">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="4c18f-351">Please submit request with the new flexible retention policy“ (Das Konfigurieren einer langfristigen Aufbewahrungsrichtlinie mit Azure Recovery Service-Tresor und -Richtlinie wird nicht mehr unterstützt. Übermitteln Sie eine Anforderung mit der neuen flexiblen Aufbewahrungsrichtlinie.)</span><span class="sxs-lookup"><span data-stu-id="4c18f-351">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="4c18f-352">Aktualisierung aller Cmdlets für Azure SQL-Datenbank, für die Erstellung von Pools für elastische Datenbanken und für die Aktualisierung, sodass sie die neue Datenbank-API verwenden. Diese unterstützt die Sku-Eigenschaft für skalierungs- und tarifbezogene Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="4c18f-352">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="4c18f-353">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="4c18f-353">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="4c18f-354">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="4c18f-354">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="4c18f-355">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="4c18f-355">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="4c18f-356">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="4c18f-356">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="4c18f-357">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="4c18f-357">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="4c18f-358">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="4c18f-358">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="4c18f-359">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="4c18f-359">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="4c18f-360">Aktualisierung der Parameter für „Get-AzureRmTrafficManagerProfile“, sodass bei Verwendung des Parameters „-Name“ der Parameter „-ResourceGroupName“ erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="4c18f-360">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>