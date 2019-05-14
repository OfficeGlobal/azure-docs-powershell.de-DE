---
ms.openlocfilehash: 3848f7fb8e298d137c747405f32a0776c1a8f029
ms.sourcegitcommit: accff0c2cd6035fcda2d917f6051a5b509eb6255
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2019
ms.locfileid: "65048630"
---
## <a name="200---may-2019"></a><span data-ttu-id="79367-101">2.0.0: Mai 2019</span><span class="sxs-lookup"><span data-stu-id="79367-101">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="79367-102">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="79367-102">Az.Accounts</span></span>
* <span data-ttu-id="79367-103">Authentifizierungsbibliothek aktualisiert, um ADFS-Probleme mit der Authentifizierung per Benutzername/Kennwort zu beheben</span><span class="sxs-lookup"><span data-stu-id="79367-103">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="79367-104">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="79367-104">Az.CognitiveServices</span></span>
* <span data-ttu-id="79367-105">Ausschließliche Anzeige des Bing-Haftungsausschlusses für Bing-Suchdienste</span><span class="sxs-lookup"><span data-stu-id="79367-105">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="79367-106">Fehler behoben, der zu einem Fehler bei der Kontoerstellung führte</span><span class="sxs-lookup"><span data-stu-id="79367-106">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="79367-107">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="79367-107">Az.Compute</span></span>
* <span data-ttu-id="79367-108">Feature für die Näherungsplatzierungsgruppe</span><span class="sxs-lookup"><span data-stu-id="79367-108">Proximity placement group feature.</span></span>
    - <span data-ttu-id="79367-109">Die folgenden neuen Cmdlets wurden hinzugefügt:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="79367-109">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="79367-110">Der neue Parameter „ProximityPlacementGroupId“ wurde zu den folgenden Cmdlets hinzugefügt:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="79367-110">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="79367-111">Der Parameter „StorageAccountType“ wurde zu „New-AzGalleryImageVersion“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="79367-111">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="79367-112">„TargetRegion“ von „New-AzGalleryImageVersion“ kann „StorageAccountType“ enthalten.</span><span class="sxs-lookup"><span data-stu-id="79367-112">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="79367-113">Switch-Parameter „SkipShutdown“ wurde zu „Stop-AzVM“ und „Stop-AzVmss“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="79367-113">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="79367-114">Wichtige Änderungen</span><span class="sxs-lookup"><span data-stu-id="79367-114">Breaking changes</span></span>
    - <span data-ttu-id="79367-115">„Set-AzVMBootDiagnostics“ in „Set-AzVMBootDiagnostic“ geändert</span><span class="sxs-lookup"><span data-stu-id="79367-115">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="79367-116">„Export-AzLogAnalyticThrottledRequests“ in „Export-AzLogAnalyticThrottledRequests“ geändert</span><span class="sxs-lookup"><span data-stu-id="79367-116">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="79367-117">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="79367-117">Az.DeploymentManager</span></span>
* <span data-ttu-id="79367-118">Erste allgemein verfügbare Version der Azure-Bereitstellungs-Manager-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="79367-118">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="79367-119">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="79367-119">Az.Dns</span></span>
* <span data-ttu-id="79367-120">Automatische Delegierung des DNS-Namenservers</span><span class="sxs-lookup"><span data-stu-id="79367-120">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="79367-121">Das Cmdlet zum Erstellen einer DNS-Zone akzeptiert den übergeordneten Zonennamen als zusätzlichen optionalen Parameter.</span><span class="sxs-lookup"><span data-stu-id="79367-121">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="79367-122">NS-Einträge in der übergeordneten Zone für neu erstellte untergeordnete Zone hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-122">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="79367-123">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="79367-123">Az.FrontDoor</span></span>
* <span data-ttu-id="79367-124">Erste allgemein verfügbare Version der Azure Frontdoor-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="79367-124">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="79367-125">WAF-Cmdlets so umbenannt, dass sie „Waf“ enthalten</span><span class="sxs-lookup"><span data-stu-id="79367-125">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="79367-126">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="79367-126">Az.HDInsight</span></span>
* <span data-ttu-id="79367-127">Zwei Cmdlets entfernt:</span><span class="sxs-lookup"><span data-stu-id="79367-127">Removed two cmdlets:</span></span>
    - <span data-ttu-id="79367-128">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="79367-128">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="79367-129">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="79367-129">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="79367-130">Neues Cmdlet „Set-AzHDInsightGatewayCredential“ hinzugefügt, um „Grant-AzHDInsightHttpServicesAccess“ zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="79367-130">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="79367-131">Cmdlet „Get-AzHDInsightJobOutput“ aktualisiert, um zwischen Leserrolle und HDInsight-Bedienerrolle zu unterscheiden:</span><span class="sxs-lookup"><span data-stu-id="79367-131">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="79367-132">Benutzer mit der Rolle „Leser“ müssen den Parameter „DefaultStorageAccountKey“ explizit angeben, andernfalls treten Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="79367-132">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="79367-133">Benutzer mit der Rolle des HDInsight-Bedieners sind nicht betroffen.</span><span class="sxs-lookup"><span data-stu-id="79367-133">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="79367-134">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="79367-134">Az.Monitor</span></span>
* <span data-ttu-id="79367-135">Neue Cmdlets für SQR-API (Scheduled Query Rule, geplante Abfrageregel)</span><span class="sxs-lookup"><span data-stu-id="79367-135">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="79367-136">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="79367-136">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="79367-137">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="79367-137">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="79367-138">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="79367-138">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="79367-139">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="79367-139">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="79367-140">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="79367-140">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="79367-141">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="79367-141">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="79367-142">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="79367-142">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="79367-143">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="79367-143">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="79367-144">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="79367-144">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="79367-145">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="79367-145">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="79367-146">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="79367-146">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="79367-147">[Weitere Informationen](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules) zur SQR-API</span><span class="sxs-lookup"><span data-stu-id="79367-147">[More](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="79367-148">„Az.Monitor.md“ aktualisiert, um Cmdlets für metrikbasierte GenV2-Warnungsregel (nicht klassisch) einzuschließen</span><span class="sxs-lookup"><span data-stu-id="79367-148">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="79367-149">Az.Network</span><span class="sxs-lookup"><span data-stu-id="79367-149">Az.Network</span></span>
* <span data-ttu-id="79367-150">Unterstützung für NAT-Gatewayressource hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-150">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="79367-151">Neue Cmdlets</span><span class="sxs-lookup"><span data-stu-id="79367-151">New cmdlets</span></span>
        - <span data-ttu-id="79367-152">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="79367-152">New-AzNatGateway</span></span>
        - <span data-ttu-id="79367-153">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="79367-153">Get-AzNatGateway</span></span>
        - <span data-ttu-id="79367-154">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="79367-154">Set-AzNatGateway</span></span>
        - <span data-ttu-id="79367-155">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="79367-155">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="79367-156">Aktualisierte Cmdlets</span><span class="sxs-lookup"><span data-stu-id="79367-156">Updated cmdlets</span></span>
        - <span data-ttu-id="79367-157">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="79367-157">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="79367-158">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="79367-158">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="79367-159">Folgende Befehle für das Feature aktualisiert: Benutzerdefinierte Routen für Brooklyn-Gateway festgelegt/entfernt</span><span class="sxs-lookup"><span data-stu-id="79367-159">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="79367-160">„New-AzVirtualNetworkGateway“ aktualisiert: Zusätzlicher optionaler Parameter „-CustomRoute“ hinzugefügt, um die Adresspräfixe als benutzerdefinierte Routen für das Gateway festlegen zu können.</span><span class="sxs-lookup"><span data-stu-id="79367-160">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="79367-161">„Set-AzVirtualNetworkGateway“ aktualisiert: Zusätzlicher optionaler Parameter „-CustomRoute“ hinzugefügt, um die Adresspräfixe als benutzerdefinierte Routen für das Gateway festlegen zu können.</span><span class="sxs-lookup"><span data-stu-id="79367-161">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="79367-162">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="79367-162">Az.PolicyInsights</span></span>
* <span data-ttu-id="79367-163">Unterstützung für die Abfrage von Richtlinienauswertungsdetails</span><span class="sxs-lookup"><span data-stu-id="79367-163">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="79367-164">Parameter „-Expand“ zu „Get-AzPolicyState“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-164">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="79367-165">Unterstützung für „-Expand PolicyEvaluationDetails“</span><span class="sxs-lookup"><span data-stu-id="79367-165">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="79367-166">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="79367-166">Az.RecoveryServices</span></span>
* <span data-ttu-id="79367-167">Unterstützung für abonnementübergreifende Azure-zu-Azure-Sitewiederherstellung</span><span class="sxs-lookup"><span data-stu-id="79367-167">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="79367-168">Markierung anstehender wichtiger Änderungen für Azure Site Recovery</span><span class="sxs-lookup"><span data-stu-id="79367-168">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="79367-169">Fehlerbehebung für Azure Site Recovery-Wiederherstellungsplan und -Aktionsplan</span><span class="sxs-lookup"><span data-stu-id="79367-169">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="79367-170">Fehlerbehebung für die Aktualisierung der Azure Site Recovery-Netzwerkzuordnung für Azure zu Azure</span><span class="sxs-lookup"><span data-stu-id="79367-170">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="79367-171">Fehlerbehebung für die Aktualisierung der Azure Site Recovery-Schutzrichtung für Azure zu Azure für verwaltete Datenträger</span><span class="sxs-lookup"><span data-stu-id="79367-171">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="79367-172">Weitere kleinere Korrekturen</span><span class="sxs-lookup"><span data-stu-id="79367-172">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="79367-173">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="79367-173">Az.Relay</span></span>
* <span data-ttu-id="79367-174">Korrektur von Tippfehlern in Kundennachrichten</span><span class="sxs-lookup"><span data-stu-id="79367-174">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="79367-175">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="79367-175">Az.ServiceBus</span></span>
* <span data-ttu-id="79367-176">Neue Cmdlets für „NetworkRuleSet“ des Namespace hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-176">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="79367-177">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="79367-177">Az.Storage</span></span>
* <span data-ttu-id="79367-178">Upgrade auf Speicherclientbibliothek 10.0.1 (Namespace aller Objekte von diesem SDK von „Microsoft.WindowsAzure.Storage.*“ in „Microsoft.Azure.Storage.*“ geändert)</span><span class="sxs-lookup"><span data-stu-id="79367-178">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="79367-179">Upgrade auf Microsoft.Azure.Management.Storage 11.0.0, um die neue API-Version 2019-04-01 zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="79367-179">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="79367-180">Art des Standardspeicherkontos bei der Speicherkontoerstellung von „Storage“ in „StorageV2“ geändert</span><span class="sxs-lookup"><span data-stu-id="79367-180">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="79367-181">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="79367-181">New-AzStorageAccount</span></span>
* <span data-ttu-id="79367-182">Vom Speicherkonto-Cmdlet ausgegebener SKU-Name (Sku.Name) durch Hinzufügen eines Unterstrichs an SKU-Eingabename angepasst (Beispiel: „StandardLRS“ > „Standard_LRS“).</span><span class="sxs-lookup"><span data-stu-id="79367-182">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="79367-183">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="79367-183">New-AzStorageAccount</span></span>
    - <span data-ttu-id="79367-184">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="79367-184">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="79367-185">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="79367-185">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="79367-186">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="79367-186">Az.Websites</span></span>
* <span data-ttu-id="79367-187">Die Eigenschaft „Kind“ wird nun für PSSite-Objekte festgelegt, die von „Get-AzWebApp“ zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="79367-187">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="79367-188">„Get-AzWebApp\*Metrics“ und „Get-AzAppServicePlanMetrics“ als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="79367-188">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="79367-189">1.8.0: April 2019</span><span class="sxs-lookup"><span data-stu-id="79367-189">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="79367-190">Highlights seit der letzten Hauptversion</span><span class="sxs-lookup"><span data-stu-id="79367-190">Highlights since the last major release</span></span>
* <span data-ttu-id="79367-191">Allgemeine Verfügbarkeit des `Az`-Moduls</span><span class="sxs-lookup"><span data-stu-id="79367-191">General availability of `Az` module</span></span>
* <span data-ttu-id="79367-192">Weitere Informationen zum `Az`-Modul finden Sie unter folgendem Link: https://aka.ms/azps-announce.</span><span class="sxs-lookup"><span data-stu-id="79367-192">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="79367-193">Vervollständigung für Location, ResourceGroup und ResourceName hinzugefügt: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/.</span><span class="sxs-lookup"><span data-stu-id="79367-193">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="79367-194">Unterstützung für Platzhalter zu Get-Cmdlets für Az.Compute und Az.Network hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-194">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="79367-195">Interaktive und Benutzername/Kennwort-Authentifizierung ausschließlich für Windows PowerShell 5.1 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-195">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="79367-196">Unterstützung für Python 2-Runbooks in Az.Automation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-196">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="79367-197">Az.LogicApp: Neue Cmdlets für Integrationskonto-Assemblys und -Batchkonfiguration</span><span class="sxs-lookup"><span data-stu-id="79367-197">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="79367-198">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="79367-198">Az.Accounts</span></span>
* <span data-ttu-id="79367-199">„Uninstall-AzureRm“ aktualisiert, um Module unter Mac ordnungsgemäß zu löschen</span><span class="sxs-lookup"><span data-stu-id="79367-199">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="79367-200">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="79367-200">Az.Batch</span></span>
* <span data-ttu-id="79367-201">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="79367-201">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="79367-202">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="79367-202">Az.Cdn</span></span>
* <span data-ttu-id="79367-203">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="79367-203">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="79367-204">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="79367-204">Az.CognitiveServices</span></span>
* <span data-ttu-id="79367-205">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="79367-205">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="79367-206">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="79367-206">Az.Compute</span></span>
* <span data-ttu-id="79367-207">Problem mit der AEM-Installation behoben, wenn die Ressourcen-IDs von Datenträgern Ressourcengruppen in Kleinbuchstaben enthielten</span><span class="sxs-lookup"><span data-stu-id="79367-207">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="79367-208">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="79367-208">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="79367-209">Dokumentation für Platzhalter korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-209">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="79367-210">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="79367-210">Az.DataFactory</span></span>
* <span data-ttu-id="79367-211">„SsisProperties“ hinzugefügt, falls „NodeCount“ für verwaltete Integration Runtime nicht NULL ist</span><span class="sxs-lookup"><span data-stu-id="79367-211">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="79367-212">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="79367-212">Az.DataLakeStore</span></span>
* <span data-ttu-id="79367-213">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="79367-213">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="79367-214">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="79367-214">Az.EventGrid</span></span>
* <span data-ttu-id="79367-215">Hilfetext für Endpunkt aktualisiert, um anzugeben, dass Ressourcen erstellt werden müssen, bevor die Cmdlets zum Erstellen/Aktualisieren von Ereignisabonnements verwendet werden</span><span class="sxs-lookup"><span data-stu-id="79367-215">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="79367-216">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="79367-216">Az.EventHub</span></span>
* <span data-ttu-id="79367-217">Neue Cmdlets für „NetworkRuleSet“ des Namespace hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-217">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="79367-218">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="79367-218">Az.HDInsight</span></span>
* <span data-ttu-id="79367-219">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="79367-219">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="79367-220">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="79367-220">Az.IotHub</span></span>
* <span data-ttu-id="79367-221">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="79367-221">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="79367-222">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="79367-222">Az.KeyVault</span></span>
* <span data-ttu-id="79367-223">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="79367-223">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="79367-224">Dokumentation für Platzhalter korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-224">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="79367-225">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="79367-225">Az.MachineLearning</span></span>
* <span data-ttu-id="79367-226">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="79367-226">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="79367-227">Az.Media</span><span class="sxs-lookup"><span data-stu-id="79367-227">Az.Media</span></span>
* <span data-ttu-id="79367-228">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="79367-228">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="79367-229">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="79367-229">Az.Monitor</span></span>
  * <span data-ttu-id="79367-230">Neue Cmdlets für metrikbasierte GenV2-Warnungsregel (nicht klassisch)</span><span class="sxs-lookup"><span data-stu-id="79367-230">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="79367-231">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="79367-231">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="79367-232">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="79367-232">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="79367-233">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="79367-233">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="79367-234">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="79367-234">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="79367-235">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="79367-235">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="79367-236">Monitor SDK auf Version 0.22.0-preview aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-236">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="79367-237">Az.Network</span><span class="sxs-lookup"><span data-stu-id="79367-237">Az.Network</span></span>
* <span data-ttu-id="79367-238">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="79367-238">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="79367-239">Dokumentation für Platzhalter korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-239">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="79367-240">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="79367-240">Az.NotificationHubs</span></span>
* <span data-ttu-id="79367-241">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="79367-241">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="79367-242">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="79367-242">Az.OperationalInsights</span></span>
* <span data-ttu-id="79367-243">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="79367-243">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="79367-244">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="79367-244">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="79367-245">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="79367-245">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="79367-246">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="79367-246">Az.RecoveryServices</span></span>
* <span data-ttu-id="79367-247">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="79367-247">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="79367-248">Tabellenformat für SQL auf Azure-VM aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-248">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="79367-249">Alternative Methode zum Abrufen des Speicherorts in „AzureFileShare“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-249">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="79367-250">„ScheduleRunDays“ in SchedulePolicy-Objekt gemäß Zeitzone aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-250">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="79367-251">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="79367-251">Az.RedisCache</span></span>
* <span data-ttu-id="79367-252">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="79367-252">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="79367-253">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="79367-253">Az.Resources</span></span>
* <span data-ttu-id="79367-254">Dokumentation für Platzhalter korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-254">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="79367-255">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="79367-255">Az.Sql</span></span>
* <span data-ttu-id="79367-256">Abhängigkeit vom Monitor SDK durch allgemeinen Code ersetzt</span><span class="sxs-lookup"><span data-stu-id="79367-256">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="79367-257">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="79367-257">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="79367-258">Verbesserter Prozess für Klassifizierung mehrerer Spalten</span><span class="sxs-lookup"><span data-stu-id="79367-258">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="79367-259">SKU-Eigenschaften (SKU-Name, Familie, Kapazität) in Antwort von „Get-AzSqlServerServiceObjective“ aufgenommen und standardmäßig als Tabelle formatiert</span><span class="sxs-lookup"><span data-stu-id="79367-259">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="79367-260">Möglichkeit zum Ausführen von „Get-AzSqlServerServiceObjective“ nach Standort, ohne dass bereits ein Server in der Region vorhanden sein muss</span><span class="sxs-lookup"><span data-stu-id="79367-260">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="79367-261">Unterstützung für Zeitzonenparameter bei der Erstellung einer verwalteten Instanz</span><span class="sxs-lookup"><span data-stu-id="79367-261">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="79367-262">Dokumentation für Platzhalter korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-262">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="79367-263">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="79367-263">Az.Websites</span></span>
* <span data-ttu-id="79367-264">„Set-AzWebApp“ und „Set-AzWebAppSlot“ korrigiert, sodass die Tags bei der Ausführung nicht entfernt werden</span><span class="sxs-lookup"><span data-stu-id="79367-264">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="79367-265">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="79367-265">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="79367-266">WebSites SDK aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-266">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="79367-267">AdminSiteName-Eigenschaft aus „PSAppServicePlan“ entfernt</span><span class="sxs-lookup"><span data-stu-id="79367-267">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="79367-268">1.7.0: April 2019</span><span class="sxs-lookup"><span data-stu-id="79367-268">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="79367-269">Highlights seit der letzten Hauptversion</span><span class="sxs-lookup"><span data-stu-id="79367-269">Highlights since the last major release</span></span>
* <span data-ttu-id="79367-270">Allgemeine Verfügbarkeit des `Az`-Moduls</span><span class="sxs-lookup"><span data-stu-id="79367-270">General availability of `Az` module</span></span>
* <span data-ttu-id="79367-271">Weitere Informationen zum `Az`-Modul finden Sie unter folgendem Link: https://aka.ms/azps-announce.</span><span class="sxs-lookup"><span data-stu-id="79367-271">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="79367-272">Vervollständigung für Location, ResourceGroup und ResourceName hinzugefügt: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/.</span><span class="sxs-lookup"><span data-stu-id="79367-272">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="79367-273">Unterstützung für Platzhalter zu Get-Cmdlets für Az.Compute und Az.Network hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-273">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="79367-274">Interaktive und Benutzername/Kennwort-Authentifizierung ausschließlich für Windows PowerShell 5.1 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-274">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="79367-275">Unterstützung für Python 2-Runbooks in Az.Automation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-275">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="79367-276">Az.LogicApp: Neue Cmdlets für Integrationskonto-Assemblys und -Batchkonfiguration</span><span class="sxs-lookup"><span data-stu-id="79367-276">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="79367-277">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="79367-277">Az.Accounts</span></span>
* <span data-ttu-id="79367-278">„Add-AzEnvironment“ und „Set-AzEnvironment“ aktualisiert, um den Parameter „AzureAnalysisServicesEndpointResourceId“ zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="79367-278">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="79367-279">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="79367-279">Az.AnalysisServices</span></span>
* <span data-ttu-id="79367-280">ServiceClient wird in Cmdlets für die Datenebene verwendet, und die ursprüngliche Authentifizierungslogik wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="79367-280">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="79367-281">„Add-AzureASAccount“ wird als Wrapper von „Connect-AzAccount“ festgelegt, um einen Breaking Change zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="79367-281">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="79367-282">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="79367-282">Az.Automation</span></span>
* <span data-ttu-id="79367-283">Fehler des Cmdlets „Fixed New-AzAutomationSoftwareUpdateConfiguration“ für Einschlüsse behoben.</span><span class="sxs-lookup"><span data-stu-id="79367-283">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="79367-284">Die Parameter „IncludedKbNumber“ und „IncludedPackageNameMask“ sollten nun funktionieren.</span><span class="sxs-lookup"><span data-stu-id="79367-284">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="79367-285">Fehlerbehebung für eine dynamische Gruppe der Azure Automation-Updateverwaltung</span><span class="sxs-lookup"><span data-stu-id="79367-285">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="79367-286">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="79367-286">Az.Compute</span></span>
* <span data-ttu-id="79367-287">Parameter „HyperVGeneration“ zu „New-AzDiskConfig“ und „New-AzSnapshotConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-287">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="79367-288">Zulassen der VM-Erstellung mit einem Katalogimage aus anderen Mandanten</span><span class="sxs-lookup"><span data-stu-id="79367-288">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="79367-289">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="79367-289">Az.ContainerInstance</span></span>
* <span data-ttu-id="79367-290">Problem im Parameter „-Command“ von „New-AzContainerGroup“ behoben, das dazu führte, dass ein nachgestelltes leeres Argument hinzugefügt wurde</span><span class="sxs-lookup"><span data-stu-id="79367-290">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="79367-291">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="79367-291">Az.DataFactory</span></span>
* <span data-ttu-id="79367-292">Version des ADF .NET SDK auf 3.0.2 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-292">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="79367-293">Cmdlet „Set-AzDataFactoryV2“ mit zusätzlichen Parametern für RepoConfiguration-Einstellungen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-293">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="79367-294">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="79367-294">Az.Resources</span></span>
* <span data-ttu-id="79367-295">Verarbeitung von Anbietern für „Get-AzResource“ bei der Angabe der Parameter „-ResourceId“ oder „-ResourceGroupName“, „-Name“ und „-ResourceType“ verbessert</span><span class="sxs-lookup"><span data-stu-id="79367-295">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="79367-296">Fehlerbehandlung für „Test-AzDeployment“ und „Test-AzResourceGroupDeployment“ verbessert</span><span class="sxs-lookup"><span data-stu-id="79367-296">Improve error handling for for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="79367-297">Behandlung von außerhalb der Bereitstellungsüberprüfung aufgetretenen Fehlern und stattdessen Aufnahme in die Ausgabe des Befehls</span><span class="sxs-lookup"><span data-stu-id="79367-297">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="79367-298">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="79367-298">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="79367-299">Switch-Parameter „-IgnoreDynamicParameters“ zu Bereitstellungs-Cmdlets hinzugefügt, um Aufforderung in Skript- und Auftragsszenarien zu überspringen</span><span class="sxs-lookup"><span data-stu-id="79367-299">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="79367-300">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="79367-300">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="79367-301">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="79367-301">Az.Sql</span></span>
* <span data-ttu-id="79367-302">Unterstützung für Klassifizierung von Datenbankdaten</span><span class="sxs-lookup"><span data-stu-id="79367-302">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="79367-303">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="79367-303">Az.Storage</span></span>
* <span data-ttu-id="79367-304">Melden eines ausführlichen Fehlers beim Erstellen des Storage-Kontexts mit dem Parameter „-UseConnectedAccount“, aber ohne Azure-Anmeldekonto</span><span class="sxs-lookup"><span data-stu-id="79367-304">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="79367-305">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="79367-305">New-AzStorageContext</span></span>
* <span data-ttu-id="79367-306">Unterstützung für das Verwalten von Blobdiensteigenschaften eines bestimmten Storage-Kontos mit einer API der Verwaltungsebene</span><span class="sxs-lookup"><span data-stu-id="79367-306">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="79367-307">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="79367-307">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="79367-308">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="79367-308">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="79367-309">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="79367-309">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="79367-310">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="79367-310">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="79367-311">Unterstützung von „-AsJob“ für Cmdlets für den Upload und Download von Blobs und Dateien</span><span class="sxs-lookup"><span data-stu-id="79367-311">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="79367-312">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="79367-312">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="79367-313">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="79367-313">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="79367-314">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="79367-314">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="79367-315">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="79367-315">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="79367-316">1.6.0: März 2019</span><span class="sxs-lookup"><span data-stu-id="79367-316">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="79367-317">Highlights seit der letzten Hauptversion</span><span class="sxs-lookup"><span data-stu-id="79367-317">Highlights since the last major release</span></span>
* <span data-ttu-id="79367-318">Allgemeine Verfügbarkeit des `Az`-Moduls</span><span class="sxs-lookup"><span data-stu-id="79367-318">General availability of `Az` module</span></span>
* <span data-ttu-id="79367-319">Weitere Informationen zum `Az`-Modul finden Sie unter folgendem Link: https://aka.ms/azps-announce.</span><span class="sxs-lookup"><span data-stu-id="79367-319">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="79367-320">Vervollständigung für Location, ResourceGroup und ResourceName hinzugefügt: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/.</span><span class="sxs-lookup"><span data-stu-id="79367-320">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="79367-321">Unterstützung für Platzhalter zu Get-Cmdlets für Az.Compute und Az.Network hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-321">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="79367-322">Interaktive und Benutzername/Kennwort-Authentifizierung ausschließlich für Windows PowerShell 5.1 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-322">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="79367-323">Unterstützung für Python 2-Runbooks in Az.Automation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-323">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="79367-324">Az.LogicApp: Neue Cmdlets für Integrationskonto-Assemblys und -Batchkonfiguration</span><span class="sxs-lookup"><span data-stu-id="79367-324">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="79367-325">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="79367-325">Az.Automation</span></span>
* <span data-ttu-id="79367-326">Änderung an der Azure Automation-Updateverwaltung, um die folgenden neuen Features zu unterstützen:</span><span class="sxs-lookup"><span data-stu-id="79367-326">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="79367-327">Dynamische Gruppierung</span><span class="sxs-lookup"><span data-stu-id="79367-327">Dynamic grouping</span></span>
    * <span data-ttu-id="79367-328">Pre-/Post-Skripts</span><span class="sxs-lookup"><span data-stu-id="79367-328">Pre-Post script</span></span>
    * <span data-ttu-id="79367-329">Neustarteinstellung</span><span class="sxs-lookup"><span data-stu-id="79367-329">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="79367-330">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="79367-330">Az.Compute</span></span>
* <span data-ttu-id="79367-331">Problem mit der Pfadauflösung in „Get-AzVmBootDiagnosticsData“ behoben</span><span class="sxs-lookup"><span data-stu-id="79367-331">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="79367-332">Computeclientbibliothek auf 25.0.0. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-332">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="79367-333">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="79367-333">Az.KeyVault</span></span>
* <span data-ttu-id="79367-334">Unterstützung für Platzhalterzeichen zu KeyVault-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-334">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="79367-335">Az.Network</span><span class="sxs-lookup"><span data-stu-id="79367-335">Az.Network</span></span>
* <span data-ttu-id="79367-336">Threat Intelligence-Unterstützung für Azure Firewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-336">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="79367-337">Ressource der obersten Ebene für Application Gateway-Firewallrichtlinie und benutzerdefinierte Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-337">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="79367-338">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="79367-338">Az.RecoveryServices</span></span>
* <span data-ttu-id="79367-339">SnapshotRetentionInDays in Azure-VM-Richtlinie hinzugefügt, um sofortigen Wiederherstellungspunkt zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="79367-339">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="79367-340">Pipe-Unterstützung für das Aufheben der Registrierung eines Containers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-340">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="79367-341">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="79367-341">Az.Resources</span></span>
* <span data-ttu-id="79367-342">Unterstützung für Platzhalterzeichen für Get-AzResource und Get-AzResourceGroup aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-342">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="79367-343">Anmeldeinformationen aktualisiert, die beim Senden generischer Aufrufe an ARM verwendet werden</span><span class="sxs-lookup"><span data-stu-id="79367-343">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="79367-344">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="79367-344">Az.Sql</span></span>
* <span data-ttu-id="79367-345">Der Cmdlet-Parameter der Bedrohungserkennung (ExcludeDetectionType) wurde von „DetectionType“ in „string[]“ geändert, um ihn zukunftssicher zu machen, wenn neue DetectionTypes-Elemente hinzugefügt werden, und um AutoVervollständigen zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="79367-345">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="79367-346">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="79367-346">Az.Storage</span></span>
* <span data-ttu-id="79367-347">Unterstützung von Get-/Set-/Remove-Verwaltungsrichtlinien für Speicherkonto hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-347">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="79367-348">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="79367-348">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="79367-349">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="79367-349">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="79367-350">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="79367-350">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="79367-351">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="79367-351">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="79367-352">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="79367-352">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="79367-353">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="79367-353">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="79367-354">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="79367-354">Az.Websites</span></span>
* <span data-ttu-id="79367-355">ARM-Vorlagenfehler behoben, der zu einem Problem beim Klonen aller Slots mithilfe von „New-AzWebApp -IncludeSourceWebAppSlots“ führte</span><span class="sxs-lookup"><span data-stu-id="79367-355">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="79367-356">1.5.0: März 2019</span><span class="sxs-lookup"><span data-stu-id="79367-356">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="79367-357">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="79367-357">Az.Accounts</span></span>
* <span data-ttu-id="79367-358">Der Befehl „Register-AzModule“ wurde hinzugefügt, um von AutoRest generierte Cmdlets zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="79367-358">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="79367-359">Beispiele für „Connect-AzAccount“ wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="79367-359">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="79367-360">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="79367-360">Az.Automation</span></span>
* <span data-ttu-id="79367-361">Problem behoben, das beim Abrufen bestimmter monatlicher Zeitpläne in verschiedenen Azure Automation-Cmdlets auftrat</span><span class="sxs-lookup"><span data-stu-id="79367-361">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="79367-362">„Get-AzAutomationDscNode“ wurde korrigiert, da nur die 20 obersten Knoten zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="79367-362">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="79367-363">Jetzt werden alle Knoten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79367-363">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="79367-364">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="79367-364">Az.Cdn</span></span>
* <span data-ttu-id="79367-365">Neue Powershell-Cmdlets zum Aktivieren/Deaktivieren von HTTPS für benutzerdefinierte Domänen hinzugefügt und alte Cmdlets außer Betrieb genommen</span><span class="sxs-lookup"><span data-stu-id="79367-365">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="79367-366">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="79367-366">Az.Compute</span></span>
* <span data-ttu-id="79367-367">Unterstützung für Platzhalterzeichen zu Get-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-367">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="79367-368">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="79367-368">Az.DataFactory</span></span>
* <span data-ttu-id="79367-369">Version des ADF .NET SDK auf 3.0.1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-369">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="79367-370">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="79367-370">Az.LogicApp</span></span>
* <span data-ttu-id="79367-371">„ListWorkflows“ wurde korrigiert, da nur die erste Seite mit Ergebnissen abgerufen wurde.</span><span class="sxs-lookup"><span data-stu-id="79367-371">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="79367-372">Az.Network</span><span class="sxs-lookup"><span data-stu-id="79367-372">Az.Network</span></span>
* <span data-ttu-id="79367-373">Unterstützung für Platzhalterzeichen zu Network-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-373">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="79367-374">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="79367-374">Az.RecoveryServices</span></span>
* <span data-ttu-id="79367-375">SQL Server jetzt in Azure-VM-Support enthalten</span><span class="sxs-lookup"><span data-stu-id="79367-375">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="79367-376">SDK-Update</span><span class="sxs-lookup"><span data-stu-id="79367-376">SDK Update</span></span>
* <span data-ttu-id="79367-377">VMappContainer-Überprüfung in „Get-ProtectableItem“ entfernt</span><span class="sxs-lookup"><span data-stu-id="79367-377">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="79367-378">„Name“ und „ServerName“ als Parameter für „Get-ProtectableItem“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-378">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="79367-379">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="79367-379">Az.Resources</span></span>
* <span data-ttu-id="79367-380">Parameter `-TemplateObject` zu Bereitstellungs-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-380">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="79367-381">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="79367-381">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="79367-382">Problem beim Piping des Ergebnisses von `Get-AzResource` an `Set-AzResource` behoben</span><span class="sxs-lookup"><span data-stu-id="79367-382">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="79367-383">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="79367-383">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="79367-384">Problem mit JSON-Datentypänderung beim Ausführen von `Set-AzResource` behoben</span><span class="sxs-lookup"><span data-stu-id="79367-384">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="79367-385">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="79367-385">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="79367-386">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="79367-386">Az.Sql</span></span>
* <span data-ttu-id="79367-387">„AuditingEndpointsCommunicator“ wird aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="79367-387">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="79367-388">Das Verhalten eines Grenzfalls beim Erstellen neuer Diagnoseeinstellungen wurde korrigiert.</span><span class="sxs-lookup"><span data-stu-id="79367-388">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="79367-389">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="79367-389">Az.Storage</span></span>
* <span data-ttu-id="79367-390">Unterstützung von „Kind BlockBlobStorage“ beim Erstellen eines Speicherkontos: New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="79367-390">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="79367-391">1.4.0 – Februar 2019</span><span class="sxs-lookup"><span data-stu-id="79367-391">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="79367-392">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="79367-392">Az.AnalysisServices</span></span>
* <span data-ttu-id="79367-393">Cmdlet „AddAzureASAccount“ als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="79367-393">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="79367-394">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="79367-394">Az.Automation</span></span>
* <span data-ttu-id="79367-395">Hilfe für „Import-AzAutomationDscNodeConfiguration“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-395">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="79367-396">Überprüfung des Konfigurationsnamens zu Cmdlet „Import-AzAutomationDscConfiguration“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-396">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="79367-397">Fehlerbehandlung für Cmdlet „Import-AzAutomationDscConfiguration“ verbessert</span><span class="sxs-lookup"><span data-stu-id="79367-397">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="79367-398">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="79367-398">Az.CognitiveServices</span></span>
* <span data-ttu-id="79367-399">„CustomSubdomainName“ als neuer optionaler Parameter für Cmdlet „New-AzCognitiveServicesAccount“ hinzugefügt, das zum Angeben der Unterdomäne für die Ressource verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="79367-399">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="79367-400">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="79367-400">Az.Compute</span></span>
* <span data-ttu-id="79367-401">Problem mit ID-Parametersätzen behoben</span><span class="sxs-lookup"><span data-stu-id="79367-401">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="79367-402">„Get-AzVMExtension“ aktualisiert, sodass alle installierten Erweiterungen aufgelistet werden, wenn der Name-Parameter nicht angegeben ist</span><span class="sxs-lookup"><span data-stu-id="79367-402">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="79367-403">Parameter „Tag“ und „ResourceId“ zum Cmdlet „Update-AzImage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-403">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="79367-404">„Get-AzVmssVM“ ohne Instanz-ID und mit „InstanceView“ können virtuelle VMSS-Computer mit Instanzansicht auflisten.</span><span class="sxs-lookup"><span data-stu-id="79367-404">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="79367-405">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="79367-405">Az.DataLakeStore</span></span>
* <span data-ttu-id="79367-406">Cmdlets zum Auflisten und Wiederherstellen gelöschter ADL-Elemente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-406">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="79367-407">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="79367-407">Az.EventHub</span></span>
* <span data-ttu-id="79367-408">Neue boolesche Eigenschaft „SkipEmptyArchives“ zum Überspringen leerer Archive in Klasse „CaptureDescription“ von EventHub hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-408">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="79367-409">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="79367-409">Az.KeyVault</span></span>
* <span data-ttu-id="79367-410">Kennzeichnung in „Set-AzKeyVaultSecret“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-410">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="79367-411">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="79367-411">Az.LogicApp</span></span>
* <span data-ttu-id="79367-412">SKU „Basic“ für Integrationskonten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-412">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="79367-413">XSLT 2.0, XSLT 3.0 und Liquid-Zuordnungstypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-413">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="79367-414">Neue Cmdlets für Integrationskonto-Assemblys</span><span class="sxs-lookup"><span data-stu-id="79367-414">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="79367-415">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="79367-415">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="79367-416">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="79367-416">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="79367-417">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="79367-417">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="79367-418">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="79367-418">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="79367-419">Neue Cmdlets für Integrationskonto-Batchkonfiguration</span><span class="sxs-lookup"><span data-stu-id="79367-419">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="79367-420">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="79367-420">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="79367-421">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="79367-421">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="79367-422">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="79367-422">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="79367-423">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="79367-423">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="79367-424">Logik-App-SDK auf Version 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-424">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="79367-425">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="79367-425">Az.Monitor</span></span>
* <span data-ttu-id="79367-426">Hilfe für „Get-AzMetric“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-426">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="79367-427">Az.Network</span><span class="sxs-lookup"><span data-stu-id="79367-427">Az.Network</span></span>
* <span data-ttu-id="79367-428">Hilfebeispiel für „Add-AzApplicationGatewayCustomError“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-428">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="79367-429">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="79367-429">Az.OperationalInsights</span></span>
* <span data-ttu-id="79367-430">Zusätzliche Unterstützung für Datenquelle von „New-ApplicationInsights“ und „Get-ApplicationInsights“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="79367-430">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="79367-431">Neue Art von „ApplicationInsights“ zum Abrufen von bestimmten und von allen ApplicationInsights-Datenquellen für einen Workspace hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="79367-431">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="79367-432">Cmdlet „New-AzOperationalInsightsApplicationInsightsDataSource“ zum Erstellen einer Datenquelle anhand des angegebenen Ressourcenparameters für „Application-Insights“ hinzugefügt: „subscriptionId“, „resourceGroupName“ und „name“.</span><span class="sxs-lookup"><span data-stu-id="79367-432">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="79367-433">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="79367-433">Az.Resources</span></span>
* <span data-ttu-id="79367-434">Behebung des Problems: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="79367-434">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="79367-435">Behebung des Problems: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="79367-435">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="79367-436">Behebung des Problems: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="79367-436">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="79367-437">Fehler korrigiert, der die wiederholte Erstellung von „KeyCredentials“ verhindert</span><span class="sxs-lookup"><span data-stu-id="79367-437">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="79367-438">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="79367-438">Az.Sql</span></span>
* <span data-ttu-id="79367-439">Unterstützung für SQL DB Hyperscale-Tarif hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-439">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="79367-440">Fehler korrigiert, aufgrund dessen die Wiederherstellung wegen der Festlegung unnötiger Eigenschaften in der Wiederherstellungsanforderung fehlschlagen konnte</span><span class="sxs-lookup"><span data-stu-id="79367-440">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="79367-441">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="79367-441">Az.Websites</span></span>
* <span data-ttu-id="79367-442">Beispiel in „Get-AzWebAppSlotMetrics“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-442">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="79367-443">1.3.0: Februar 2019</span><span class="sxs-lookup"><span data-stu-id="79367-443">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="79367-444">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="79367-444">Az.Accounts</span></span>
* <span data-ttu-id="79367-445">Update auf die aktuelle Version von ClientRuntime durchgeführt</span><span class="sxs-lookup"><span data-stu-id="79367-445">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="79367-446">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="79367-446">Az.AnalysisServices</span></span>
<span data-ttu-id="79367-447">Allgemeine Verfügbarkeit für Az.AnalysisServices-Modul</span><span class="sxs-lookup"><span data-stu-id="79367-447">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="79367-448">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="79367-448">Az.Compute</span></span>
* <span data-ttu-id="79367-449">AEM-Erweiterung: Unterstützung für UltraSSD und P60-, P70- und P80-Datenträger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-449">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="79367-450">Hilfebeschreibung für „Set-AzVMBootDiagnostics“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-450">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="79367-451">Hilfebeschreibung und Beispiel für „Update-AzImage“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-451">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="79367-452">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="79367-452">Az.RecoveryServices</span></span>
<span data-ttu-id="79367-453">Allgemeine Verfügbarkeit für Az.RecoveryServices-Modul.</span><span class="sxs-lookup"><span data-stu-id="79367-453">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="79367-454">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="79367-454">Az.Resources</span></span>
* <span data-ttu-id="79367-455">Kennzeichnung für Ressourcengruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-455">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="79367-456">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="79367-456">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="79367-457">Problem behoben, bei dem „-ErrorAction“ von `Get-AzureRmRoleAssignment` nicht berücksichtigt wird</span><span class="sxs-lookup"><span data-stu-id="79367-457">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="79367-458">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="79367-458">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="79367-459">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="79367-459">Az.Sql</span></span>
* <span data-ttu-id="79367-460">Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-460">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="79367-461">Problem behoben, bei dem eine fehlende Anmeldung am Azure-Konto bei der Ausführung von SQL-Cmdlets zu einer nullref-Ausnahme führt</span><span class="sxs-lookup"><span data-stu-id="79367-461">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="79367-462">nullref-Ausnahme in Get-AzSqlCapability korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-462">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="79367-463">1.2.1: Januar 2019</span><span class="sxs-lookup"><span data-stu-id="79367-463">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="79367-464">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="79367-464">Az.Accounts</span></span>
* <span data-ttu-id="79367-465">Release mit richtiger Version der Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="79367-465">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="79367-466">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="79367-466">Az.AnalysisServices</span></span>
* <span data-ttu-id="79367-467">Release mit aktualisierter Authentifizierungsabhängigkeit</span><span class="sxs-lookup"><span data-stu-id="79367-467">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="79367-468">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="79367-468">Az.RecoveryServices</span></span>
* <span data-ttu-id="79367-469">Release mit aktualisierter Authentifizierungsabhängigkeit</span><span class="sxs-lookup"><span data-stu-id="79367-469">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="79367-470">1.2.0: Januar 2019</span><span class="sxs-lookup"><span data-stu-id="79367-470">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="79367-471">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="79367-471">Az.Accounts</span></span>
* <span data-ttu-id="79367-472">Interaktive und Benutzername/Kennwort-Authentifizierung ausschließlich für Windows PowerShell 5.1 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-472">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="79367-473">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-473">Update incorrect online help URLs</span></span>
* <span data-ttu-id="79367-474">Warnmeldung in PS Core für „Uninstall-AzureRm“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-474">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="79367-475">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="79367-475">Az.Aks</span></span>
* <span data-ttu-id="79367-476">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-476">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="79367-477">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="79367-477">Az.Automation</span></span>
* <span data-ttu-id="79367-478">Unterstützung für Python 2-Runbooks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-478">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="79367-479">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-479">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="79367-480">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="79367-480">Az.Cdn</span></span>
* <span data-ttu-id="79367-481">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-481">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="79367-482">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="79367-482">Az.Compute</span></span>
* <span data-ttu-id="79367-483">Cmdlet „Invoke-AzVMReimage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-483">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="79367-484">Parameter „TempDisk“ zu „Set-AzVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-484">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="79367-485">Warnmeldung von „New-AzVM“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-485">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="79367-486">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="79367-486">Az.ContainerRegistry</span></span>
* <span data-ttu-id="79367-487">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-487">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="79367-488">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="79367-488">Az.DataFactory</span></span>
* <span data-ttu-id="79367-489">Version des ADF .NET SDK auf 3.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-489">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="79367-490">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="79367-490">Az.DataLakeStore</span></span>
* <span data-ttu-id="79367-491">Problem mit ADLS-Endpunkt bei Verwendung von MSI behoben</span><span class="sxs-lookup"><span data-stu-id="79367-491">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="79367-492">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="79367-492">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="79367-493">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-493">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="79367-494">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="79367-494">Az.IotHub</span></span>
* <span data-ttu-id="79367-495">Codierungsformat zu Cmdlet „Add-IotHubRoutingEndpoint“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-495">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="79367-496">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="79367-496">Az.KeyVault</span></span>
* <span data-ttu-id="79367-497">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-497">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="79367-498">Az.Network</span><span class="sxs-lookup"><span data-stu-id="79367-498">Az.Network</span></span>
* <span data-ttu-id="79367-499">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-499">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="79367-500">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="79367-500">Az.Resources</span></span>
* <span data-ttu-id="79367-501">Fehlerhafte Beispiele in Referenzdokumentation zu „New-AzADAppCredential“ und „New-AzADSpCredential“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-501">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="79367-502">Problem behoben, bei dem der Pfad für den Parameter „-TemplateFile“ nicht aufgelöst wurde, bevor Cmdlets für die Bereitstellung von Ressourcengruppen ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="79367-502">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="79367-503">Az.Resources: Richtige Dokumentation für Standardwert von „New-AzureRmPolicyDefinition -Mode“ bereitgestellt</span><span class="sxs-lookup"><span data-stu-id="79367-503">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="79367-504">Az.Resources: Behebung des Problems: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="79367-504">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="79367-505">Az.Resources: Behebung des Problems: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="79367-505">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="79367-506">Formatierungsproblem für Objekt „PSResourceGroupDeployment“ behoben</span><span class="sxs-lookup"><span data-stu-id="79367-506">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="79367-507">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="79367-507">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="79367-508">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="79367-508">Az.ServiceFabric</span></span>
* <span data-ttu-id="79367-509">Rollback beim Hinzufügen eines Zertifikats zum VMSS-Modell, Auslösung einer Ausnahme. Fehlerbehebung: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="79367-509">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="79367-510">Einige Fehlermeldungen wurden korrigiert.</span><span class="sxs-lookup"><span data-stu-id="79367-510">Fix some error messages.</span></span>
* <span data-ttu-id="79367-511">Fehler bei Clustererstellung mit ARM-Standardvorlage für „New-AzServiceFabriCluster“ behoben, bei dem die Migration zu Az nicht funktioniert hat.</span><span class="sxs-lookup"><span data-stu-id="79367-511">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="79367-512">Fehler behoben beim Hinzufügen eines Cluster-/Anwendungszertifikats ausschließlich zu VM Scale Sets, die zum Cluster gehören, indem die Cluster-ID in der Erweiterung überprüft wird.</span><span class="sxs-lookup"><span data-stu-id="79367-512">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="79367-513">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="79367-513">Az.SignalR</span></span>
* <span data-ttu-id="79367-514">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-514">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="79367-515">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="79367-515">Az.Sql</span></span>
* <span data-ttu-id="79367-516">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-516">Update incorrect online help URLs</span></span>
* <span data-ttu-id="79367-517">Parameterbeschreibung für den Parameter „LicenseType“ mit möglichen Werten aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-517">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="79367-518">Fehler behoben, bei dem die Aktualisierung der Identität der verwalteten Instanz nicht funktioniert hat, wenn es sich um die einzige aktualisierte Eigenschaft gehandelt hat</span><span class="sxs-lookup"><span data-stu-id="79367-518">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="79367-519">Unterstützung für die benutzerdefinierte Sortierung auf verwalteter Instanz</span><span class="sxs-lookup"><span data-stu-id="79367-519">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="79367-520">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="79367-520">Az.Storage</span></span>
* <span data-ttu-id="79367-521">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-521">Update incorrect online help URLs</span></span>
* <span data-ttu-id="79367-522">Ausführliche Fehlermeldung beim Abrufen/Festlegen der klassischen Protokollierung bzw. Metriken für Storage Premium-Konto, da für das Storage Premium-Konto die klassische Protokollierung bzw. Metriken nicht unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="79367-522">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="79367-523">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="79367-523">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="79367-524">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="79367-524">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="79367-525">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="79367-525">Az.TrafficManager</span></span>
* <span data-ttu-id="79367-526">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-526">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="79367-527">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="79367-527">Az.Websites</span></span>
* <span data-ttu-id="79367-528">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-528">Update incorrect online help URLs</span></span>
* <span data-ttu-id="79367-529">„New-AzWebAppSSLBinding“ korrigiert, damit das Zertifikat in die richtige Ressourcengruppe bzw. an den richtigen Speicherort hochgeladen wird, wenn die App in einer ASE gehostet wird.</span><span class="sxs-lookup"><span data-stu-id="79367-529">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="79367-530">„New-AzWebAppSSLBinding“ korrigiert, damit die Tags beim Binden eines SSL-Zertifikats an eine App nicht überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="79367-530">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="79367-531">1.1.0 – Januar 2019</span><span class="sxs-lookup"><span data-stu-id="79367-531">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="79367-532">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="79367-532">Az.Accounts</span></span>
* <span data-ttu-id="79367-533">Bereich „Local“ zu „Enable-AzureRmAlias“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-533">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="79367-534">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="79367-534">Az.Compute</span></span>
* <span data-ttu-id="79367-535">Name ist jetzt optional im ID-Parametersatz für „Restart/Start/Stop/Remove/Set-AzVM“ und „Save-AzVMImage“</span><span class="sxs-lookup"><span data-stu-id="79367-535">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="79367-536">Beschreibung der ID in Hilfedateien aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-536">Updated the description of ID in help files</span></span>
* <span data-ttu-id="79367-537">Problem mit der Abwärtskompatibilität beim Az.Accounts-Modul behoben</span><span class="sxs-lookup"><span data-stu-id="79367-537">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="79367-538">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="79367-538">Az.DataLakeStore</span></span>
* <span data-ttu-id="79367-539">Aktualisierung der SDK-Version der Datenebene auf 1.1.14 für SDK-Fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="79367-539">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="79367-540">Behandlung von negativen acesstime- and modificationtime-Werten für „getfilestatus“ und „liststatus“ korrigiert, asynchrones Abbruchtoken korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-540">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="79367-541">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="79367-541">Az.EventGrid</span></span>
* <span data-ttu-id="79367-542">Zur Verwendung der API-Version 2019-01-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-542">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="79367-543">Aktualisierung der folgenden Cmdlets zur Unterstützung des neuen Szenarios in der API-Version 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="79367-543">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="79367-544">New-AzureRmEventGridSubscription: Neue optionale Parameter zum Angeben folgender Werte hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="79367-544">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="79367-545">Gültigkeitsdauer des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="79367-545">Event Time-To-Live,</span></span>
        - <span data-ttu-id="79367-546">Maximale Anzahl von Übermittlungsversuchen für die Ereignisse</span><span class="sxs-lookup"><span data-stu-id="79367-546">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="79367-547">Endpunkt für unzustellbare Nachrichten</span><span class="sxs-lookup"><span data-stu-id="79367-547">Dead letter endpoint.</span></span>
    - <span data-ttu-id="79367-548">Update-AzureRmEventGridSubscription: Neue optionale Parameter zum Angeben folgender Werte hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="79367-548">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="79367-549">Gültigkeitsdauer des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="79367-549">Event Time-To-Live,</span></span>
        - <span data-ttu-id="79367-550">Maximale Anzahl von Übermittlungsversuchen für die Ereignisse</span><span class="sxs-lookup"><span data-stu-id="79367-550">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="79367-551">Endpunkt für unzustellbare Nachrichten</span><span class="sxs-lookup"><span data-stu-id="79367-551">Dead letter endpoint.</span></span>
* <span data-ttu-id="79367-552">Neue Enumerationswerte („storageQueue“ und „hybridConnection“) für die EndpointType-Option in den Cmdlets „New-AzureRmEventGridSubscription“ und „Update-AzureRmEventGridSubscription“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-552">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="79367-553">Anzeige einer Warnmeldung, wenn das Erstellen oder Aktualisieren des Ereignisabonnements voraussichtlich eine manuelle Aktion des Benutzers zur Folge hat</span><span class="sxs-lookup"><span data-stu-id="79367-553">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="79367-554">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="79367-554">Az.IotHub</span></span>
* <span data-ttu-id="79367-555">Auf die aktuelle Version des Iot Hub SDK aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-555">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="79367-556">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="79367-556">Az.LogicApp</span></span>
* <span data-ttu-id="79367-557">„Get-AzLogicApp“ listet alle Apps ohne angegebenen Namen auf</span><span class="sxs-lookup"><span data-stu-id="79367-557">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="79367-558">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="79367-558">Az.Resources</span></span>
* <span data-ttu-id="79367-559">Problem mit dem Parametersatz bei Angabe der Parameter „-ODataQuery“ und „-ResourceId“ für „Get-AzResource“ behoben</span><span class="sxs-lookup"><span data-stu-id="79367-559">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="79367-560">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="79367-560">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="79367-561">Behandlung des Parameters „-Custom“ in „New/Set-AzPolicyDefinition“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-561">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="79367-562">Tippfehler in der Dokumentation für „New-AzDeployment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-562">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="79367-563">Parameter „-MailNickname“ als obligatorisch festgelegt für „New-AzADUser“</span><span class="sxs-lookup"><span data-stu-id="79367-563">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="79367-564">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="79367-564">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="79367-565">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="79367-565">Az.SignalR</span></span>
* <span data-ttu-id="79367-566">Problem mit der Abwärtskompatibilität beim Az.Accounts-Modul behoben</span><span class="sxs-lookup"><span data-stu-id="79367-566">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="79367-567">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="79367-567">Az.Sql</span></span>
* <span data-ttu-id="79367-568">Abhängigkeit des Speicherverwaltungsclients zur allgemeinen SDK-Implementierung konvertiert</span><span class="sxs-lookup"><span data-stu-id="79367-568">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="79367-569">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="79367-569">Az.Storage</span></span>
* <span data-ttu-id="79367-570">Festlegung des „StorageAccountName“ des Speicherkontexts als tatsächlichen Namen des Speicherkontos, wenn dieser mit „SAS-Token“, „OAuth“ oder „Anonym“ erstellt wird</span><span class="sxs-lookup"><span data-stu-id="79367-570">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="79367-571">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="79367-571">New-AzStorageContext</span></span>
* <span data-ttu-id="79367-572">Erstellen von SAS-Token des Blob-Momentaufnahmeobjekts mit dem Parameter „-FullUri“, Festlegung des zurückgegebenen URI als Momentaufnahme-URI</span><span class="sxs-lookup"><span data-stu-id="79367-572">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="79367-573">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="79367-573">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="79367-574">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="79367-574">Az.Websites</span></span>
* <span data-ttu-id="79367-575">Fehler bei der Datumsanalyse in „Get-AzDeletedWebApp“ behoben</span><span class="sxs-lookup"><span data-stu-id="79367-575">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="79367-576">Problem mit der Abwärtskompatibilität beim Az.Accounts-Modul behoben</span><span class="sxs-lookup"><span data-stu-id="79367-576">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="79367-577">1.0.0 – Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="79367-577">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="79367-578">Allgemein</span><span class="sxs-lookup"><span data-stu-id="79367-578">General</span></span>

- <span data-ttu-id="79367-579">Allgemeine Verfügbarkeit des Az-Moduls</span><span class="sxs-lookup"><span data-stu-id="79367-579">General Availability of Az Module</span></span>
- <span data-ttu-id="79367-580">Onlinehilfe für jedes Modul</span><span class="sxs-lookup"><span data-stu-id="79367-580">Online help for each module</span></span>
- <span data-ttu-id="79367-581">Ausführlichere Informationen und eine Roadmap finden Sie auf der [Seite mit der Ankündigung zu Az](https://aka.ms/azps-announce).</span><span class="sxs-lookup"><span data-stu-id="79367-581">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="79367-582">Informationen zur Migration aus AzureRM finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="79367-582">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="79367-583">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="79367-583">Az.Accounts</span></span>
- <span data-ttu-id="79367-584">Geändert von Az.Profile</span><span class="sxs-lookup"><span data-stu-id="79367-584">Changed from Az.Profile</span></span>
- <span data-ttu-id="79367-585">Feste Tabellenformate für Profil- und Kontexttypen</span><span class="sxs-lookup"><span data-stu-id="79367-585">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="79367-586">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="79367-586">Az.ApiManagement</span></span>
- <span data-ttu-id="79367-587">Korrekturen für #7002</span><span class="sxs-lookup"><span data-stu-id="79367-587">Fixes for #7002</span></span>
- <span data-ttu-id="79367-588">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="79367-588">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="79367-589">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="79367-589">Az.Batch</span></span>
- <span data-ttu-id="79367-590">Möglichkeit zum Anzeigen der ausgeführten Version des Azure Batch-Knoten-Agents auf den VMs eines Pools mit der neuen `NodeAgentInformation`-Eigenschaft für `PSComputeNode` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="79367-590">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="79367-591">Der `Caching`-Standardwert für `PSDataDisk` lautet jetzt nicht mehr `None`, sondern `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="79367-591">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="79367-592">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="79367-592">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="79367-593">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="79367-593">Az.Billing</span></span>
- <span data-ttu-id="79367-594">Kombination von Billing-, Consumption- und UsageAggregates-Cmdlets. Ausführliche Informationen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="79367-594">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="79367-595">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="79367-595">Az.CognitivServices</span></span>
- <span data-ttu-id="79367-596">Vervollständigungen für SkuName und Typem für den Vorgang New-AzureRmCognitiveServicesAccount hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-596">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="79367-597">GetSkusWithAccountParamSetName-Parametersatz aus Get-AzCognitiveServicesAccountSkus entfernt</span><span class="sxs-lookup"><span data-stu-id="79367-597">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="79367-598">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="79367-598">Az.ContainerInstance</span></span>
- <span data-ttu-id="79367-599">ManagedIdentity-Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-599">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="79367-600">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="79367-600">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="79367-601">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="79367-601">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="79367-602">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="79367-602">Az.DataLakeStore</span></span>
- <span data-ttu-id="79367-603">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="79367-603">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="79367-604">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="79367-604">Az.Monitor</span></span>
- <span data-ttu-id="79367-605">Az.Insights in Az.Monitor umbenannt und weitere weniger wichtige grundlegende Änderungen durchgeführt. Informationen hierzu finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="79367-605">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="79367-606">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="79367-606">Az.KeyVault</span></span>
- <span data-ttu-id="79367-607">Veraltete PurgeDisabled-Eigenschaft aus Ausgabetypen entfernt</span><span class="sxs-lookup"><span data-stu-id="79367-607">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="79367-608">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="79367-608">Az.MachineLearning</span></span>
- <span data-ttu-id="79367-609">Cmdlets des Az.MachineLearningCompute-Moduls eingebunden</span><span class="sxs-lookup"><span data-stu-id="79367-609">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="79367-610">Az.Media</span><span class="sxs-lookup"><span data-stu-id="79367-610">Az.Media</span></span>
- <span data-ttu-id="79367-611">Veralteten -Tags-Alias aus New-AzMediaService entfernt</span><span class="sxs-lookup"><span data-stu-id="79367-611">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="79367-612">Az.Network</span><span class="sxs-lookup"><span data-stu-id="79367-612">Az.Network</span></span>
<span data-ttu-id="79367-613">Unterstützung für das Konfigurieren von RewriteRuleSets im Application Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-613">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="79367-614">Neu hinzugefügte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="79367-614">New cmdlets added:</span></span>
        - <span data-ttu-id="79367-615">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="79367-615">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="79367-616">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="79367-616">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="79367-617">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="79367-617">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="79367-618">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="79367-618">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="79367-619">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="79367-619">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="79367-620">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="79367-620">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="79367-621">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="79367-621">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="79367-622">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="79367-622">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="79367-623">Cmdlets mit optionalem Parameter -RewriteRuleSet aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-623">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="79367-624">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="79367-624">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="79367-625">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="79367-625">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="79367-626">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="79367-626">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="79367-627">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="79367-627">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="79367-628">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="79367-628">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="79367-629">New-AzureRmApplicationGatewayUrlPathMapConfig: KeyVault-Unterstützung mithilfe von Identität zum Application Gateway hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="79367-629">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="79367-630">Cmdlets mit optionalem Parameter aktualisiert: -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="79367-630">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="79367-631">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="79367-631">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="79367-632">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="79367-632">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="79367-633">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="79367-633">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="79367-634">Cmdlet New-AzApplicationGateway mit optionalem Parameter -UserAssignedIdentity aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-634">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="79367-635">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="79367-635">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="79367-636">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="79367-636">Az.OperationalInsights</span></span>
- <span data-ttu-id="79367-637">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="79367-637">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="79367-638">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="79367-638">Az.Profile</span></span>
- <span data-ttu-id="79367-639">Modulnamen in Az.Accounts geändert</span><span class="sxs-lookup"><span data-stu-id="79367-639">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="79367-640">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="79367-640">Az.RecoveryServices</span></span>
- <span data-ttu-id="79367-641">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="79367-641">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="79367-642">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="79367-642">Az.Resources</span></span>
- <span data-ttu-id="79367-643">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="79367-643">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="79367-644">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="79367-644">Az.ServiceFabric</span></span>
- <span data-ttu-id="79367-645">Unterstützung für das Angeben des Zertifikats anhand des allgemeinen Namens und Fingerabdrucks</span><span class="sxs-lookup"><span data-stu-id="79367-645">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="79367-646">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="79367-646">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="79367-647">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="79367-647">Az.SIgnalR</span></span>
- <span data-ttu-id="79367-648">Allgemeine Verfügbarkeit für PowerShell-Cmdlets für SIgnalR</span><span class="sxs-lookup"><span data-stu-id="79367-648">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="79367-649">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="79367-649">Az.Sql</span></span>
- <span data-ttu-id="79367-650">Neue Erkennungstypen Data_Exfiltration und Unsafe_Action zu Cmdlets für Bedrohungserkennung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-650">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="79367-651">Dokumentationsbeispiele für Cmdlets für SQL-Überwachung aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-651">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="79367-652">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="79367-652">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="79367-653">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="79367-653">Az.Storage</span></span>
- <span data-ttu-id="79367-654">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="79367-654">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="79367-655">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="79367-655">Az.Websites</span></span>
- <span data-ttu-id="79367-656">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="79367-656">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="79367-657">0.7.0 – Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="79367-657">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="79367-658">Allgemein</span><span class="sxs-lookup"><span data-stu-id="79367-658">General</span></span>

* <span data-ttu-id="79367-659">Geringe Änderungen für anstehenden Übergang von AzureRM zu Az</span><span class="sxs-lookup"><span data-stu-id="79367-659">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="79367-660">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="79367-660">Az.Compute</span></span>

* <span data-ttu-id="79367-661">Unterstützung für UltraSSD und Katalogimages in einfachen Parametersätzen für `New-AzVm(ss)`-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="79367-661">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="79367-662">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="79367-662">Az.DataLakeStore</span></span>

* <span data-ttu-id="79367-663">Nachgestellten Schrägstrich für die Domäne des ADLS-Kontos korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-663">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="79367-664">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="79367-664">Az.FrontDoor</span></span>

* <span data-ttu-id="79367-665">Einige fehlerhafte Links behoben</span><span class="sxs-lookup"><span data-stu-id="79367-665">Fixed some broken links</span></span>
    - <span data-ttu-id="79367-666">In den Artikeln zu New-AzureRmFrontDoor und Set-AzureRmFrontDoor den Artikel-Link zum Cmdlet „New-AzureRmFrontDoorHealthProbeSettingObject“ korrigiert.</span><span class="sxs-lookup"><span data-stu-id="79367-666">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="79367-667">Im Artikel zu New-AzureRmFrontDoorManagedRuleObject den Artikel-Link zum Cmdlet „New-AzureRmFrontDoorRuleGroupOverrideObject“ korrigiert.</span><span class="sxs-lookup"><span data-stu-id="79367-667">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="79367-668">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="79367-668">Az.RecoveryServices</span></span>

* <span data-ttu-id="79367-669">Clientseitige Validierungen für Wiederherstellungsvorgänge von Azure-Dateifreigaben hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="79367-669">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="79367-670">storageAccountName und storageAccountResourceGroupName für AFS-Wiederherstellung optional gemacht.</span><span class="sxs-lookup"><span data-stu-id="79367-670">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="79367-671">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="79367-671">Az.Resources</span></span>

* <span data-ttu-id="79367-672">Fehlerbehebung für https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="79367-672">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="79367-673">Get-AzureRmRoleAssignment für die Verwendung des Abonnementbereichs aktualisiert, wenn dieser beim Anfordern von klassischen Administratoren angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="79367-673">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="79367-674">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="79367-674">Az.Sql</span></span>

* <span data-ttu-id="79367-675">Geringe Änderungen für anstehenden Übergang von AzureRM zu Az</span><span class="sxs-lookup"><span data-stu-id="79367-675">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="79367-676">Problem mit der Verwendung von Get-AzureRmSqlDatabaseVulnerabilityAssessment mit .NET Core behoben</span><span class="sxs-lookup"><span data-stu-id="79367-676">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="79367-677">Dokumentation mit Hilfemeldungen zu Cmdlets für die SQL-Überwachung geändert.</span><span class="sxs-lookup"><span data-stu-id="79367-677">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="79367-678">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="79367-678">Az.Storage</span></span>

* <span data-ttu-id="79367-679">-EnableHierarchicalNamespace zu New-AzureRmStorageAccount hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-679">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="79367-680">Problem behoben, bei dem für das Copy File-Cmdlet am Ziel kein Quellkontext wiederverwendet werden kann, wenn -DestContext nicht eingegeben wird</span><span class="sxs-lookup"><span data-stu-id="79367-680">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="79367-681">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="79367-681">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="79367-682">Unterstützung der Konfiguration von statischen Websites</span><span class="sxs-lookup"><span data-stu-id="79367-682">Support Static Website configuration</span></span>
    - <span data-ttu-id="79367-683">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="79367-683">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="79367-684">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="79367-684">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="79367-685">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="79367-685">Az.Websites</span></span>

* <span data-ttu-id="79367-686">Set-AzureRmWebApp und Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="79367-686">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="79367-687">Neuen Parameter (-AzureStoragePath) zum Angeben von Azure Storage-Pfaden hinzugefügt, die in Windows- und Linux-Container-Apps bereitgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="79367-687">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="79367-688">Verwenden Sie die Ausgabe des neuen Cmdlets New-AzureRmWebAppAzureStoragePath als Parameter zum Festlegen der Azure Storage-Pfade.</span><span class="sxs-lookup"><span data-stu-id="79367-688">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="79367-689">0.6.1 – November 2018</span><span class="sxs-lookup"><span data-stu-id="79367-689">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="79367-690">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="79367-690">Az.ApiManagement</span></span>
* <span data-ttu-id="79367-691">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-691">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="79367-692">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="79367-692">Az.Automation</span></span>
* <span data-ttu-id="79367-693">Swagger-basierte Azure Automation-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="79367-693">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="79367-694">Cmdlets zur Updateverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-694">Added Update Management cmdlets</span></span>
* <span data-ttu-id="79367-695">Cmdlets zur Quellcodeverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-695">Added Source Control cmdlets</span></span>
* <span data-ttu-id="79367-696">Cmdlet „Remove-AzureRmAutomationHybridWorkerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-696">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="79367-697">DSC-Befehl für die Knotenregistrierung korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-697">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="79367-698">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="79367-698">Az.Compute</span></span>
* <span data-ttu-id="79367-699">Identitätsproblem für SystemAssigned-Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-699">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="79367-700">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-700">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="79367-701">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="79367-701">Az.ContainerInstance</span></span>
* <span data-ttu-id="79367-702">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-702">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="79367-703">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="79367-703">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="79367-704">Beschreibung der Beispiele für Marketplace-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-704">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="79367-705">Az.Network</span><span class="sxs-lookup"><span data-stu-id="79367-705">Az.Network</span></span>
* <span data-ttu-id="79367-706">Folgende Cmdlets hinzugefügt: New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="79367-706">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="79367-707">ICMP wieder unterstützten AzureFirewall-Netzwerkprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-707">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="79367-708">Cmdlet „Test-AzureRmNetworkWatcherConnectivity“ aktualisiert und Überprüfung für Ziel-ID, Adresse und Port hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-708">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="79367-709">Probleme mit Arbeitsspeicherauslastung in der VirtualNetwork-Zuordnung behoben</span><span class="sxs-lookup"><span data-stu-id="79367-709">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="79367-710">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="79367-710">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="79367-711">Problem beim Ändern der Richtlinie für eine geschützte Dateifreigabe behoben</span><span class="sxs-lookup"><span data-stu-id="79367-711">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="79367-712">Richtlinienzeitzone in Großschreibung geändert</span><span class="sxs-lookup"><span data-stu-id="79367-712">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="79367-713">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="79367-713">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="79367-714">Korrigiertes Beispiel in „New-AzureRmRecoveryServicesAsrProtectableItem“</span><span class="sxs-lookup"><span data-stu-id="79367-714">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="79367-715">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-715">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="79367-716">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="79367-716">Az.Relay</span></span>
* <span data-ttu-id="79367-717">Optionaler Parameter „-KeyValue“ zu Cmdlet „New-AzureRmRelayKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht</span><span class="sxs-lookup"><span data-stu-id="79367-717">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="79367-718">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="79367-718">Az.Resources</span></span>
* <span data-ttu-id="79367-719">Hilfedokumentation für ressourcenidentitätsbezogene Parameter in `New-AzureRmPolicyAssignment` und `Set-AzureRmPolicyAssignment` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-719">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="79367-720">Beispiel für „New-AzureRmPolicyDefinition“ hinzugefügt, das „-Metadata“ nutzt</span><span class="sxs-lookup"><span data-stu-id="79367-720">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="79367-721">Korrektur, um Beibehaltung von Groß-/Kleinschreibung in Tagschlüsseln in „NetStandard“ zu ermöglichen: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="79367-721">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="79367-722">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="79367-722">Az.ServiceFabric</span></span>
* <span data-ttu-id="79367-723">Benachrichtigung über veraltete Elemente für anstehende wichtige Änderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-723">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="79367-724">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="79367-724">Az.Sql</span></span>
* <span data-ttu-id="79367-725">Neue Cmdlets für CRUD-Vorgänge in verwalteten Azure SQL-Datenbank-Instanzen und verwalteten Azure SQL-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-725">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="79367-726">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="79367-726">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="79367-727">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="79367-727">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="79367-728">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="79367-728">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="79367-729">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="79367-729">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="79367-730">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="79367-730">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="79367-731">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="79367-731">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="79367-732">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="79367-732">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="79367-733">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="79367-733">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="79367-734">Erweiterte Verwaltung von Überwachungsrichtlinien auf einem Server oder in einer Datenbank aktiviert</span><span class="sxs-lookup"><span data-stu-id="79367-734">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="79367-735">Neuer Parameter (PredicateExpression) hinzugefügt, um die Filterung von Überwachungsprotokollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="79367-735">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="79367-736">Cmdlets wurden angepasst, sodass sie SQL-Clients anstelle von Legacyclients verwenden.</span><span class="sxs-lookup"><span data-stu-id="79367-736">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="79367-737">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="79367-737">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="79367-738">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="79367-738">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="79367-739">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="79367-739">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="79367-740">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="79367-740">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="79367-741">Problem bei Verwendung von „Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings“ mit festgelegtem Parameter für den Speicherkontonamen behoben</span><span class="sxs-lookup"><span data-stu-id="79367-741">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="79367-742">0.5.0 – November 2018</span><span class="sxs-lookup"><span data-stu-id="79367-742">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="79367-743">Allgemein</span><span class="sxs-lookup"><span data-stu-id="79367-743">General</span></span>
* <span data-ttu-id="79367-744">Ressourcenvervollständigungen für viele Kern-Cmdlets hinzugefügt (diese ermöglichen das Durchlaufen von vorhandenen Ressourcennamen per TAB-TASTE, wenn Cmdlets interaktiv aufgerufen werden)</span><span class="sxs-lookup"><span data-stu-id="79367-744">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="79367-745">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="79367-745">Az.Profile</span></span>
* <span data-ttu-id="79367-746">Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="79367-746">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="79367-747">Parameter „TenantId“ im Cmdlet „Connect-AzAccount“ in „Tenant“ umbenannt und Alias für „TenantId“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-747">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="79367-748">Beschreibung von „TenantId“ für „Connect-AzAccount“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="79367-748">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="79367-749">Fehlermeldung für fehlgeschlagene Anmeldung bei Angabe der Mandantendomäne korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-749">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="79367-750">Problem in Bezug auf Kontextnamenskonflikt für Konten ohne Abonnements im Mandanten behoben</span><span class="sxs-lookup"><span data-stu-id="79367-750">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="79367-751">Problem mit DataLake-Endpunkten bei Verwendung von MSI behoben</span><span class="sxs-lookup"><span data-stu-id="79367-751">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="79367-752">Problem behoben, das zur Auslösung von „Disconnect-AzAccount“ führte, wenn keine Verbindung bestand</span><span class="sxs-lookup"><span data-stu-id="79367-752">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="79367-753">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="79367-753">Az.CognitiveServices</span></span>
* <span data-ttu-id="79367-754">Vorgang „Get-AzCognitiveServicesAccountSkus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-754">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="79367-755">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="79367-755">Az.Compute</span></span>
* <span data-ttu-id="79367-756">Cmdlets Add-AzVmssVMDataDisk und Remove-AzVmssVMDataDisk hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-756">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="79367-757">„Get-AzVMImage“ zeigt „AutomaticOSUpgradeProperties“ an</span><span class="sxs-lookup"><span data-stu-id="79367-757">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="79367-758">Problem behoben, aufgrund dessen die Optionswerte „SetAzVMChefExtension -BootstrapOptions“ und „-JsonAttribute“ nicht im JSON-Format festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="79367-758">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="79367-759">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="79367-759">Az.DataLakeStore</span></span>
* <span data-ttu-id="79367-760">Aktualisierung des DataLake-Pakets auf 1.1.10</span><span class="sxs-lookup"><span data-stu-id="79367-760">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="79367-761">Standardmäßige Parallelität zu Multithreadvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-761">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="79367-762">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="79367-762">Az.Insights</span></span>
* <span data-ttu-id="79367-763">Problem Nr. 7267 behoben (Bereich für automatische Skalierung)</span><span class="sxs-lookup"><span data-stu-id="79367-763">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="79367-764">Probleme beim Erstellen einer neuen Regel für die automatische Skalierung, aufgrund derer die aufgelisteten Parameter nicht richtig festgelegt wurden (Es wurde stets der Standardwert festgelegt.)</span><span class="sxs-lookup"><span data-stu-id="79367-764">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="79367-765">Problem Nr. 7513 behoben [Insights] „Set-AzDiagnosticSetting“ erfordert die explizite Angabe von Kategorien während der Erstellung der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="79367-765">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="79367-766">Nun erfordert das Cmdlet nicht die explizite Angabe der Kategorien, die während der Erstellung aktiviert werden sollen. Das bedeutet, es funktioniert wie dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="79367-766">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="79367-767">Az.Network</span><span class="sxs-lookup"><span data-stu-id="79367-767">Az.Network</span></span>
* <span data-ttu-id="79367-768">„PeeringType“ wurde geändert und ist nun ein erforderlicher Parameter für die folgenden Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="79367-768">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="79367-769">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="79367-769">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="79367-770">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="79367-770">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="79367-771">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="79367-771">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="79367-772">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="79367-772">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="79367-773">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="79367-773">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="79367-774">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="79367-774">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="79367-775">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="79367-775">Az.PolicyInsights</span></span>
* <span data-ttu-id="79367-776">Cmdlets für Richtlinienwartung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-776">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="79367-777">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="79367-777">Az.Resources</span></span>
* <span data-ttu-id="79367-778">Fehlerbehebung für https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="79367-778">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="79367-779">Zulassen der Auflistung von Ressourcen mithilfe des Parameters „-ResourceId“ für „Get-AzResource“</span><span class="sxs-lookup"><span data-stu-id="79367-779">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="79367-780">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="79367-780">Az.ServiceBus</span></span>
* <span data-ttu-id="79367-781">Schreibgeschützte Eigenschaft „MigrationState“ zu „PSServiceBusMigrationConfigurationAttributes“ hinzugefügt, was das Ermitteln des Migrationsstatus ermöglicht</span><span class="sxs-lookup"><span data-stu-id="79367-781">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="79367-782">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="79367-782">Az.ServiceFabric</span></span>
* <span data-ttu-id="79367-783">Hinzufügen des Zertifikats zu Linux VMSS korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-783">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="79367-784">„Add-AzServiceFabricClusterCertificate“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="79367-784">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="79367-785">Verwenden des richtigen Fingerabdrucks aus dem neuen Zertifikat (Azure/service-fabric-issues#932)</span><span class="sxs-lookup"><span data-stu-id="79367-785">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="79367-786">Richtige Anzeige von Ausnahmen (Azure/service-fabric-issues#1054)</span><span class="sxs-lookup"><span data-stu-id="79367-786">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="79367-787">„Update-AzServiceFabricDurability“ korrigiert, um die Clusterkonfiguration zu aktualisieren, bevor der VMSS-Vorgang „CreateOrUpdate“ gestartet wird</span><span class="sxs-lookup"><span data-stu-id="79367-787">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="79367-788">0.4.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="79367-788">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="79367-789">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="79367-789">Az.Profile</span></span>
* <span data-ttu-id="79367-790">Problem mit „Get-AzSubscription“ in Cloud Shell behoben</span><span class="sxs-lookup"><span data-stu-id="79367-790">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="79367-791">Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="79367-791">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="79367-792">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="79367-792">Az.Compute</span></span>
* <span data-ttu-id="79367-793">Neue Größen zur Whitelist von VM-Größen hinzugefügt, für die bei Verwendung des einfachen Parametersatzes für „New-AzVm“ der beschleunigte Netzwerkbetrieb aktiviert wird</span><span class="sxs-lookup"><span data-stu-id="79367-793">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="79367-794">ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="79367-794">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="79367-795">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="79367-795">Az.DataLakeStore</span></span>
* <span data-ttu-id="79367-796">Unterstützung für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-796">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="79367-797">Get-AzDataLakeStoreVirtualNetworkRule: Dient zum Abrufen oder Auflisten der Azure Data Lake Store-Regel für das virtuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="79367-797">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="79367-798">Add-AzDataLakeStoreVirtualNetworkRule: Fügt dem angegebenen Data Lake Store-Konto eine Regel für das virtuelle Netzwerk hinzu.</span><span class="sxs-lookup"><span data-stu-id="79367-798">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="79367-799">Set-AzDataLakeStoreVirtualNetworkRule: Ändert die angegebene Regel für das virtuelle Netzwerk in das angegebene Data Lake Store-Konto.</span><span class="sxs-lookup"><span data-stu-id="79367-799">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="79367-800">Remove-AzDataLakeStoreVirtualNetworkRule: Dient zum Löschen der Azure Data Lake Store-Regel für das virtuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="79367-800">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="79367-801">Az.Network</span><span class="sxs-lookup"><span data-stu-id="79367-801">Az.Network</span></span>
* <span data-ttu-id="79367-802">Cmdlet „Test-AzNetworkWatcherConnectivity“ aktualisiert, Protokollwert wird jetzt an Back-End übergeben.</span><span class="sxs-lookup"><span data-stu-id="79367-802">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="79367-803">ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="79367-803">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="79367-804">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="79367-804">Az.Resources</span></span>
* <span data-ttu-id="79367-805">Problem behoben, aufgrund dessen „Get-AzRoleDefinition“ eine unverständliche Ausnahme auslöst (wenn das Standardprofil kein Abonnement enthält und kein Bereich festgelegt ist), indem im Szenario eine aussagekräftige Ausnahme hinzugefügt wurde.</span><span class="sxs-lookup"><span data-stu-id="79367-805">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="79367-806">Außerdem wurde der Standardparametersatz auf „RoleDefinitionNameParameterSet“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="79367-806">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="79367-807">0.3.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="79367-807">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="79367-808">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="79367-808">Azure.Storage</span></span>
* <span data-ttu-id="79367-809">Fehler beim Kopieren von Blobs/Dateien behoben, aufgrund dessen bei einem Metadatenproblem des Ziels keine Metadaten kopiert wurden</span><span class="sxs-lookup"><span data-stu-id="79367-809">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="79367-810">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="79367-810">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="79367-811">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="79367-811">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="79367-812">Der Abruf der Speicherressourcennutzung eines bestimmten Standorts wird jetzt unterstützt, und das Hinzufügen einer Warnmeldung für den Abruf der globalen Speicherressourcennutzung ist überflüssig.</span><span class="sxs-lookup"><span data-stu-id="79367-812">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="79367-813">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="79367-813">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="79367-814">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="79367-814">Az.CognitiveServices</span></span>
* <span data-ttu-id="79367-815">„Get-AzCognitiveServicesAccountSkus“ wird ohne vorhandenes Konto unterstützt.</span><span class="sxs-lookup"><span data-stu-id="79367-815">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="79367-816">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="79367-816">Az.Compute</span></span>
* <span data-ttu-id="79367-817">Korrektur von „Get-AzVM -ResourceGroupName <rg>“, sodass ggf. mehr als 50 Ergebnisse zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="79367-817">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="79367-818">Der Cmdlet-Hilfe zu „New-AzVmss“ wurde ein Beispiel für „SimpleParameterSet“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="79367-818">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="79367-819">Tippfehler in der Azure Disk Encryption-Statusmeldung behoben</span><span class="sxs-lookup"><span data-stu-id="79367-819">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="79367-820">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="79367-820">Az.DataFactoryV2</span></span>
* <span data-ttu-id="79367-821">Die Version des ADF .Net-SDK wurde auf 2.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="79367-821">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="79367-822">Az.Network</span><span class="sxs-lookup"><span data-stu-id="79367-822">Az.Network</span></span>
* <span data-ttu-id="79367-823">NetworkProfile-Funktionalität wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="79367-823">Added NetworkProfile functionality.</span></span> <span data-ttu-id="79367-824">Neue Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-824">new cmdlets added</span></span>
    - <span data-ttu-id="79367-825">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="79367-825">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="79367-826">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="79367-826">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="79367-827">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="79367-827">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="79367-828">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="79367-828">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="79367-829">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="79367-829">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="79367-830">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="79367-830">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="79367-831">Dienstzuordnungslink in Subnetzmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-831">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="79367-832">Cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-832">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="79367-833">Cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-833">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="79367-834">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="79367-834">Az.RedisCache</span></span>
* <span data-ttu-id="79367-835">Künftig sind beliebige Zeichenfolgen als Größenparameter zulässig.</span><span class="sxs-lookup"><span data-stu-id="79367-835">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="79367-836">P5 in Popup „PSArgumentCompleter“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-836">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="79367-837">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="79367-837">Az.Resources</span></span>
* <span data-ttu-id="79367-838">Fehlender Parameter „-Mode“ zu „Set-AzPolicyDefinition“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="79367-838">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="79367-839">Cmdlet-Fehler bei „Get-AzProviderOperation“ für Vorgänge mit Ursprung behoben, der den Benutzer enthält</span><span class="sxs-lookup"><span data-stu-id="79367-839">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="79367-840">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="79367-840">Az.Sql</span></span>
* <span data-ttu-id="79367-841">Problem behoben, aufgrund dessen einige Sicherungs-Cmdlets das aktuelle Azure-Abonnements nicht erkannt haben</span><span class="sxs-lookup"><span data-stu-id="79367-841">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="79367-842">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="79367-842">Az.Websites</span></span>
* <span data-ttu-id="79367-843">Neues Cmdlet „Get-AzWebAppContainerContinuousDeploymentUrl“ zum Abrufen der Webhook-URL von Continuous Deployment für Container</span><span class="sxs-lookup"><span data-stu-id="79367-843">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="79367-844">Neue Cmdlets „New-AzWebAppContainerPSSession“ und „Enter-WebAppContainerPSSession“ zum Initiieren einer PowerShell-Remotesitzung in einer Windows-Container-App</span><span class="sxs-lookup"><span data-stu-id="79367-844">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="79367-845">0.2.0 – September 2018</span><span class="sxs-lookup"><span data-stu-id="79367-845">0.2.0 - September 2018</span></span>
 <span data-ttu-id="79367-846">Erste Version</span><span class="sxs-lookup"><span data-stu-id="79367-846">Initial Release</span></span>