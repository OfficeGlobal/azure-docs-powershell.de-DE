---
ms.openlocfilehash: 179d22fa065944695e4769f2698e3cabc7666b04
ms.sourcegitcommit: c6fd0e490fa0e33b8b768b679682a47d8faae1cf
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/16/2019
ms.locfileid: "54342017"
---
## <a name="110---january-2019"></a><span data-ttu-id="b6e56-101">1.1.0 – Januar 2019</span><span class="sxs-lookup"><span data-stu-id="b6e56-101">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="b6e56-102">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="b6e56-102">Az.Accounts</span></span>
* <span data-ttu-id="b6e56-103">Bereich „Local“ zu „Enable-AzureRmAlias“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-103">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b6e56-104">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b6e56-104">Az.Compute</span></span>
* <span data-ttu-id="b6e56-105">Name ist jetzt optional im ID-Parametersatz für „Restart/Start/Stop/Remove/Set-AzVM“ und „Save-AzVMImage“</span><span class="sxs-lookup"><span data-stu-id="b6e56-105">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="b6e56-106">Beschreibung der ID in Hilfedateien aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-106">Updated the description of ID in help files</span></span>
* <span data-ttu-id="b6e56-107">Problem mit der Abwärtskompatibilität beim Az.Accounts-Modul behoben</span><span class="sxs-lookup"><span data-stu-id="b6e56-107">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="b6e56-108">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="b6e56-108">Az.DataLakeStore</span></span>
* <span data-ttu-id="b6e56-109">Aktualisierung der SDK-Version der Datenebene auf 1.1.14 für SDK-Fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="b6e56-109">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="b6e56-110">Behandlung von negativen acesstime- and modificationtime-Werten für „getfilestatus“ und „liststatus“ korrigiert, asynchrones Abbruchtoken korrigiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-110">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="b6e56-111">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="b6e56-111">Az.EventGrid</span></span>
* <span data-ttu-id="b6e56-112">Zur Verwendung der API-Version 2019-01-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-112">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="b6e56-113">Aktualisierung der folgenden Cmdlets zur Unterstützung des neuen Szenarios in der API-Version 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="b6e56-113">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="b6e56-114">New-AzureRmEventGridSubscription: Neue optionale Parameter zum Angeben folgender Werte hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="b6e56-114">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="b6e56-115">Gültigkeitsdauer des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="b6e56-115">Event Time-To-Live,</span></span>
        - <span data-ttu-id="b6e56-116">Maximale Anzahl von Übermittlungsversuchen für die Ereignisse</span><span class="sxs-lookup"><span data-stu-id="b6e56-116">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="b6e56-117">Endpunkt für unzustellbare Nachrichten</span><span class="sxs-lookup"><span data-stu-id="b6e56-117">Dead letter endpoint.</span></span>
    - <span data-ttu-id="b6e56-118">Update-AzureRmEventGridSubscription: Neue optionale Parameter zum Angeben folgender Werte hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="b6e56-118">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="b6e56-119">Gültigkeitsdauer des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="b6e56-119">Event Time-To-Live,</span></span>
        - <span data-ttu-id="b6e56-120">Maximale Anzahl von Übermittlungsversuchen für die Ereignisse</span><span class="sxs-lookup"><span data-stu-id="b6e56-120">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="b6e56-121">Endpunkt für unzustellbare Nachrichten</span><span class="sxs-lookup"><span data-stu-id="b6e56-121">Dead letter endpoint.</span></span>
* <span data-ttu-id="b6e56-122">Neue Enumerationswerte („storageQueue“ und „hybridConnection“) für die EndpointType-Option in den Cmdlets „New-AzureRmEventGridSubscription“ und „Update-AzureRmEventGridSubscription“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-122">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="b6e56-123">Anzeige einer Warnmeldung, wenn das Erstellen oder Aktualisieren des Ereignisabonnements voraussichtlich eine manuelle Aktion des Benutzers zur Folge hat</span><span class="sxs-lookup"><span data-stu-id="b6e56-123">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="b6e56-124">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="b6e56-124">Az.IotHub</span></span>
* <span data-ttu-id="b6e56-125">Auf die aktuelle Version des Iot Hub SDK aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-125">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="b6e56-126">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="b6e56-126">Az.LogicApp</span></span>
* <span data-ttu-id="b6e56-127">„Get-AzLogicApp“ listet alle Apps ohne angegebenen Namen auf</span><span class="sxs-lookup"><span data-stu-id="b6e56-127">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="b6e56-128">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b6e56-128">Az.Resources</span></span>
* <span data-ttu-id="b6e56-129">Problem mit dem Parametersatz bei Angabe der Parameter „-ODataQuery“ und „-ResourceId“ für „Get-AzResource“ behoben</span><span class="sxs-lookup"><span data-stu-id="b6e56-129">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="b6e56-130">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="b6e56-130">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="b6e56-131">Behandlung des Parameters „-Custom“ in „New/Set-AzPolicyDefinition“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-131">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="b6e56-132">Tippfehler in der Dokumentation für „New-AzDeployment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-132">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="b6e56-133">Parameter „-MailNickname“ als obligatorisch festgelegt für „New-AzADUser“</span><span class="sxs-lookup"><span data-stu-id="b6e56-133">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="b6e56-134">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="b6e56-134">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="b6e56-135">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="b6e56-135">Az.SignalR</span></span>
* <span data-ttu-id="b6e56-136">Problem mit der Abwärtskompatibilität beim Az.Accounts-Modul behoben</span><span class="sxs-lookup"><span data-stu-id="b6e56-136">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="b6e56-137">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b6e56-137">Az.Sql</span></span>
* <span data-ttu-id="b6e56-138">Abhängigkeit des Speicherverwaltungsclients zur allgemeinen SDK-Implementierung konvertiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-138">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="b6e56-139">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="b6e56-139">Az.Storage</span></span>
* <span data-ttu-id="b6e56-140">Festlegung des „StorageAccountName“ des Speicherkontexts als tatsächlichen Namen des Speicherkontos, wenn dieser mit „SAS-Token“, „OAuth“ oder „Anonym“ erstellt wird</span><span class="sxs-lookup"><span data-stu-id="b6e56-140">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="b6e56-141">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="b6e56-141">New-AzStorageContext</span></span>
* <span data-ttu-id="b6e56-142">Erstellen von SAS-Token des Blob-Momentaufnahmeobjekts mit dem Parameter „-FullUri“, Festlegung des zurückgegebenen URI als Momentaufnahme-URI</span><span class="sxs-lookup"><span data-stu-id="b6e56-142">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="b6e56-143">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="b6e56-143">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="b6e56-144">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b6e56-144">Az.Websites</span></span>
* <span data-ttu-id="b6e56-145">Fehler bei der Datumsanalyse in „Get-AzDeletedWebApp“ behoben</span><span class="sxs-lookup"><span data-stu-id="b6e56-145">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="b6e56-146">Problem mit der Abwärtskompatibilität beim Az.Accounts-Modul behoben</span><span class="sxs-lookup"><span data-stu-id="b6e56-146">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="b6e56-147">1.0.0 – Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="b6e56-147">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="b6e56-148">Allgemein</span><span class="sxs-lookup"><span data-stu-id="b6e56-148">General</span></span>

- <span data-ttu-id="b6e56-149">Allgemeine Verfügbarkeit des Az-Moduls</span><span class="sxs-lookup"><span data-stu-id="b6e56-149">General Availability of Az Module</span></span>
- <span data-ttu-id="b6e56-150">Onlinehilfe für jedes Modul</span><span class="sxs-lookup"><span data-stu-id="b6e56-150">Online help for each module</span></span>
- <span data-ttu-id="b6e56-151">Ausführlichere Informationen und eine Roadmap finden Sie auf der [Seite mit der Ankündigung zu Az](https://aka.ms/azps-announce).</span><span class="sxs-lookup"><span data-stu-id="b6e56-151">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="b6e56-152">Informationen zur Migration aus AzureRM finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="b6e56-152">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="b6e56-153">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="b6e56-153">Az.Accounts</span></span>
- <span data-ttu-id="b6e56-154">Geändert von Az.Profile</span><span class="sxs-lookup"><span data-stu-id="b6e56-154">Changed from Az.Profile</span></span>
- <span data-ttu-id="b6e56-155">Feste Tabellenformate für Profil- und Kontexttypen</span><span class="sxs-lookup"><span data-stu-id="b6e56-155">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="b6e56-156">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="b6e56-156">Az.ApiManagement</span></span>
- <span data-ttu-id="b6e56-157">Korrekturen für #7002</span><span class="sxs-lookup"><span data-stu-id="b6e56-157">Fixes for #7002</span></span>
- <span data-ttu-id="b6e56-158">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="b6e56-158">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="b6e56-159">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="b6e56-159">Az.Batch</span></span>
- <span data-ttu-id="b6e56-160">Möglichkeit zum Anzeigen der ausgeführten Version des Azure Batch-Knoten-Agents auf den VMs eines Pools mit der neuen `NodeAgentInformation`-Eigenschaft für `PSComputeNode` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b6e56-160">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="b6e56-161">Der `Caching`-Standardwert für `PSDataDisk` lautet jetzt nicht mehr `None`, sondern `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="b6e56-161">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="b6e56-162">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="b6e56-162">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="b6e56-163">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="b6e56-163">Az.Billing</span></span>
- <span data-ttu-id="b6e56-164">Kombination von Billing-, Consumption- und UsageAggregates-Cmdlets. Ausführliche Informationen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="b6e56-164">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="b6e56-165">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="b6e56-165">Az.CognitivServices</span></span>
- <span data-ttu-id="b6e56-166">Vervollständigungen für SkuName und Typem für den Vorgang New-AzureRmCognitiveServicesAccount hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-166">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="b6e56-167">GetSkusWithAccountParamSetName-Parametersatz aus Get-AzCognitiveServicesAccountSkus entfernt</span><span class="sxs-lookup"><span data-stu-id="b6e56-167">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="b6e56-168">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="b6e56-168">Az.ContainerInstance</span></span>
- <span data-ttu-id="b6e56-169">ManagedIdentity-Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-169">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="b6e56-170">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="b6e56-170">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="b6e56-171">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="b6e56-171">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="b6e56-172">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="b6e56-172">Az.DataLakeStore</span></span>
- <span data-ttu-id="b6e56-173">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="b6e56-173">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="b6e56-174">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="b6e56-174">Az.Monitor</span></span>
- <span data-ttu-id="b6e56-175">Az.Insights in Az.Monitor umbenannt und weitere weniger wichtige grundlegende Änderungen durchgeführt. Informationen hierzu finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="b6e56-175">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="b6e56-176">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="b6e56-176">Az.KeyVault</span></span>
- <span data-ttu-id="b6e56-177">Veraltete PurgeDisabled-Eigenschaft aus Ausgabetypen entfernt</span><span class="sxs-lookup"><span data-stu-id="b6e56-177">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="b6e56-178">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="b6e56-178">Az.MachineLearning</span></span>
- <span data-ttu-id="b6e56-179">Cmdlets des Az.MachineLearningCompute-Moduls eingebunden</span><span class="sxs-lookup"><span data-stu-id="b6e56-179">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="b6e56-180">Az.Media</span><span class="sxs-lookup"><span data-stu-id="b6e56-180">Az.Media</span></span>
- <span data-ttu-id="b6e56-181">Veralteten -Tags-Alias aus New-AzMediaService entfernt</span><span class="sxs-lookup"><span data-stu-id="b6e56-181">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="b6e56-182">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b6e56-182">Az.Network</span></span>
<span data-ttu-id="b6e56-183">Unterstützung für das Konfigurieren von RewriteRuleSets im Application Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-183">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="b6e56-184">Neu hinzugefügte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="b6e56-184">New cmdlets added:</span></span>
        - <span data-ttu-id="b6e56-185">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="b6e56-185">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="b6e56-186">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="b6e56-186">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="b6e56-187">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="b6e56-187">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="b6e56-188">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="b6e56-188">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="b6e56-189">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="b6e56-189">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="b6e56-190">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="b6e56-190">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="b6e56-191">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="b6e56-191">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="b6e56-192">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="b6e56-192">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="b6e56-193">Cmdlets mit optionalem Parameter -RewriteRuleSet aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-193">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="b6e56-194">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="b6e56-194">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="b6e56-195">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="b6e56-195">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="b6e56-196">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="b6e56-196">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="b6e56-197">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="b6e56-197">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="b6e56-198">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="b6e56-198">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="b6e56-199">New-AzureRmApplicationGatewayUrlPathMapConfig: KeyVault-Unterstützung mithilfe von Identität zum Application Gateway hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b6e56-199">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="b6e56-200">Cmdlets mit optionalem Parameter aktualisiert: -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="b6e56-200">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="b6e56-201">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="b6e56-201">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="b6e56-202">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="b6e56-202">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="b6e56-203">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="b6e56-203">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="b6e56-204">Cmdlet New-AzApplicationGateway mit optionalem Parameter -UserAssignedIdentity aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-204">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="b6e56-205">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="b6e56-205">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="b6e56-206">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="b6e56-206">Az.OperationalInsights</span></span>
- <span data-ttu-id="b6e56-207">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="b6e56-207">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="b6e56-208">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="b6e56-208">Az.Profile</span></span>
- <span data-ttu-id="b6e56-209">Modulnamen in Az.Accounts geändert</span><span class="sxs-lookup"><span data-stu-id="b6e56-209">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="b6e56-210">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="b6e56-210">Az.RecoveryServices</span></span>
- <span data-ttu-id="b6e56-211">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="b6e56-211">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="b6e56-212">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b6e56-212">Az.Resources</span></span>
- <span data-ttu-id="b6e56-213">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="b6e56-213">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="b6e56-214">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="b6e56-214">Az.ServiceFabric</span></span>
- <span data-ttu-id="b6e56-215">Unterstützung für das Angeben des Zertifikats anhand des allgemeinen Namens und Fingerabdrucks</span><span class="sxs-lookup"><span data-stu-id="b6e56-215">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="b6e56-216">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="b6e56-216">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="b6e56-217">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="b6e56-217">Az.SIgnalR</span></span>
- <span data-ttu-id="b6e56-218">Allgemeine Verfügbarkeit für PowerShell-Cmdlets für SIgnalR</span><span class="sxs-lookup"><span data-stu-id="b6e56-218">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="b6e56-219">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b6e56-219">Az.Sql</span></span>
- <span data-ttu-id="b6e56-220">Neue Erkennungstypen Data_Exfiltration und Unsafe_Action zu Cmdlets für Bedrohungserkennung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-220">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="b6e56-221">Dokumentationsbeispiele für Cmdlets für SQL-Überwachung aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-221">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="b6e56-222">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="b6e56-222">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="b6e56-223">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="b6e56-223">Az.Storage</span></span>
- <span data-ttu-id="b6e56-224">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="b6e56-224">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="b6e56-225">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b6e56-225">Az.Websites</span></span>
- <span data-ttu-id="b6e56-226">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="b6e56-226">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="b6e56-227">0.7.0 – Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="b6e56-227">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="b6e56-228">Allgemein</span><span class="sxs-lookup"><span data-stu-id="b6e56-228">General</span></span>

* <span data-ttu-id="b6e56-229">Geringe Änderungen für anstehenden Übergang von AzureRM zu Az</span><span class="sxs-lookup"><span data-stu-id="b6e56-229">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="b6e56-230">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b6e56-230">Az.Compute</span></span>

* <span data-ttu-id="b6e56-231">Unterstützung für UltraSSD und Katalogimages in einfachen Parametersätzen für `New-AzVm(ss)`-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b6e56-231">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="b6e56-232">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="b6e56-232">Az.DataLakeStore</span></span>

* <span data-ttu-id="b6e56-233">Nachgestellten Schrägstrich für die Domäne des ADLS-Kontos korrigiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-233">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="b6e56-234">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="b6e56-234">Az.FrontDoor</span></span>

* <span data-ttu-id="b6e56-235">Einige fehlerhafte Links behoben</span><span class="sxs-lookup"><span data-stu-id="b6e56-235">Fixed some broken links</span></span>
    - <span data-ttu-id="b6e56-236">In den Artikeln zu New-AzureRmFrontDoor und Set-AzureRmFrontDoor den Artikel-Link zum Cmdlet „New-AzureRmFrontDoorHealthProbeSettingObject“ korrigiert.</span><span class="sxs-lookup"><span data-stu-id="b6e56-236">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="b6e56-237">Im Artikel zu New-AzureRmFrontDoorManagedRuleObject den Artikel-Link zum Cmdlet „New-AzureRmFrontDoorRuleGroupOverrideObject“ korrigiert.</span><span class="sxs-lookup"><span data-stu-id="b6e56-237">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="b6e56-238">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="b6e56-238">Az.RecoveryServices</span></span>

* <span data-ttu-id="b6e56-239">Clientseitige Validierungen für Wiederherstellungsvorgänge von Azure-Dateifreigaben hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b6e56-239">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="b6e56-240">storageAccountName und storageAccountResourceGroupName für AFS-Wiederherstellung optional gemacht.</span><span class="sxs-lookup"><span data-stu-id="b6e56-240">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="b6e56-241">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b6e56-241">Az.Resources</span></span>

* <span data-ttu-id="b6e56-242">Fehlerbehebung für https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="b6e56-242">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="b6e56-243">Get-AzureRmRoleAssignment für die Verwendung des Abonnementbereichs aktualisiert, wenn dieser beim Anfordern von klassischen Administratoren angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="b6e56-243">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="b6e56-244">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b6e56-244">Az.Sql</span></span>

* <span data-ttu-id="b6e56-245">Geringe Änderungen für anstehenden Übergang von AzureRM zu Az</span><span class="sxs-lookup"><span data-stu-id="b6e56-245">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="b6e56-246">Problem mit der Verwendung von Get-AzureRmSqlDatabaseVulnerabilityAssessment mit .NET Core behoben</span><span class="sxs-lookup"><span data-stu-id="b6e56-246">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="b6e56-247">Dokumentation mit Hilfemeldungen zu Cmdlets für die SQL-Überwachung geändert.</span><span class="sxs-lookup"><span data-stu-id="b6e56-247">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="b6e56-248">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="b6e56-248">Az.Storage</span></span>

* <span data-ttu-id="b6e56-249">-EnableHierarchicalNamespace zu New-AzureRmStorageAccount hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-249">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="b6e56-250">Problem behoben, bei dem für das Copy File-Cmdlet am Ziel kein Quellkontext wiederverwendet werden kann, wenn -DestContext nicht eingegeben wird</span><span class="sxs-lookup"><span data-stu-id="b6e56-250">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="b6e56-251">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="b6e56-251">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="b6e56-252">Unterstützung der Konfiguration von statischen Websites</span><span class="sxs-lookup"><span data-stu-id="b6e56-252">Support Static Website configuration</span></span>
    - <span data-ttu-id="b6e56-253">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="b6e56-253">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="b6e56-254">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="b6e56-254">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="b6e56-255">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b6e56-255">Az.Websites</span></span>

* <span data-ttu-id="b6e56-256">Set-AzureRmWebApp und Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="b6e56-256">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="b6e56-257">Neuen Parameter (-AzureStoragePath) zum Angeben von Azure Storage-Pfaden hinzugefügt, die in Windows- und Linux-Container-Apps bereitgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="b6e56-257">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="b6e56-258">Verwenden Sie die Ausgabe des neuen Cmdlets New-AzureRmWebAppAzureStoragePath als Parameter zum Festlegen der Azure Storage-Pfade.</span><span class="sxs-lookup"><span data-stu-id="b6e56-258">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="b6e56-259">0.6.1 – November 2018</span><span class="sxs-lookup"><span data-stu-id="b6e56-259">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="b6e56-260">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="b6e56-260">Az.ApiManagement</span></span>
* <span data-ttu-id="b6e56-261">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-261">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="b6e56-262">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="b6e56-262">Az.Automation</span></span>
* <span data-ttu-id="b6e56-263">Swagger-basierte Azure Automation-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="b6e56-263">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="b6e56-264">Cmdlets zur Updateverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-264">Added Update Management cmdlets</span></span>
* <span data-ttu-id="b6e56-265">Cmdlets zur Quellcodeverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-265">Added Source Control cmdlets</span></span>
* <span data-ttu-id="b6e56-266">Cmdlet „Remove-AzureRmAutomationHybridWorkerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-266">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="b6e56-267">DSC-Befehl für die Knotenregistrierung korrigiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-267">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="b6e56-268">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b6e56-268">Az.Compute</span></span>
* <span data-ttu-id="b6e56-269">Identitätsproblem für SystemAssigned-Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-269">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="b6e56-270">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-270">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="b6e56-271">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="b6e56-271">Az.ContainerInstance</span></span>
* <span data-ttu-id="b6e56-272">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-272">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="b6e56-273">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="b6e56-273">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="b6e56-274">Beschreibung der Beispiele für Marketplace-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-274">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="b6e56-275">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b6e56-275">Az.Network</span></span>
* <span data-ttu-id="b6e56-276">Folgende Cmdlets hinzugefügt: New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="b6e56-276">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="b6e56-277">ICMP wieder unterstützten AzureFirewall-Netzwerkprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-277">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="b6e56-278">Cmdlet „Test-AzureRmNetworkWatcherConnectivity“ aktualisiert und Überprüfung für Ziel-ID, Adresse und Port hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-278">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="b6e56-279">Probleme mit Arbeitsspeicherauslastung in der VirtualNetwork-Zuordnung behoben</span><span class="sxs-lookup"><span data-stu-id="b6e56-279">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="b6e56-280">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="b6e56-280">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="b6e56-281">Problem beim Ändern der Richtlinie für eine geschützte Dateifreigabe behoben</span><span class="sxs-lookup"><span data-stu-id="b6e56-281">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="b6e56-282">Richtlinienzeitzone in Großschreibung geändert</span><span class="sxs-lookup"><span data-stu-id="b6e56-282">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="b6e56-283">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="b6e56-283">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="b6e56-284">Korrigiertes Beispiel in „New-AzureRmRecoveryServicesAsrProtectableItem“</span><span class="sxs-lookup"><span data-stu-id="b6e56-284">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="b6e56-285">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-285">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="b6e56-286">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="b6e56-286">Az.Relay</span></span>
* <span data-ttu-id="b6e56-287">Optionaler Parameter „-KeyValue“ zu Cmdlet „New-AzureRmRelayKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht</span><span class="sxs-lookup"><span data-stu-id="b6e56-287">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="b6e56-288">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b6e56-288">Az.Resources</span></span>
* <span data-ttu-id="b6e56-289">Hilfedokumentation für ressourcenidentitätsbezogene Parameter in `New-AzureRmPolicyAssignment` und `Set-AzureRmPolicyAssignment` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-289">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="b6e56-290">Beispiel für „New-AzureRmPolicyDefinition“ hinzugefügt, das „-Metadata“ nutzt</span><span class="sxs-lookup"><span data-stu-id="b6e56-290">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="b6e56-291">Korrektur, um Beibehaltung von Groß-/Kleinschreibung in Tagschlüsseln in „NetStandard“ zu ermöglichen: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="b6e56-291">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="b6e56-292">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="b6e56-292">Az.ServiceFabric</span></span>
* <span data-ttu-id="b6e56-293">Benachrichtigung über veraltete Elemente für anstehende wichtige Änderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-293">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="b6e56-294">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b6e56-294">Az.Sql</span></span>
* <span data-ttu-id="b6e56-295">Neue Cmdlets für CRUD-Vorgänge in verwalteten Azure SQL-Datenbank-Instanzen und verwalteten Azure SQL-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-295">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="b6e56-296">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="b6e56-296">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="b6e56-297">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="b6e56-297">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="b6e56-298">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="b6e56-298">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="b6e56-299">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="b6e56-299">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="b6e56-300">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="b6e56-300">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="b6e56-301">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="b6e56-301">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="b6e56-302">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="b6e56-302">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="b6e56-303">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="b6e56-303">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="b6e56-304">Erweiterte Verwaltung von Überwachungsrichtlinien auf einem Server oder in einer Datenbank aktiviert</span><span class="sxs-lookup"><span data-stu-id="b6e56-304">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="b6e56-305">Neuer Parameter (PredicateExpression) hinzugefügt, um die Filterung von Überwachungsprotokollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b6e56-305">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="b6e56-306">Cmdlets wurden angepasst, sodass sie SQL-Clients anstelle von Legacyclients verwenden.</span><span class="sxs-lookup"><span data-stu-id="b6e56-306">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="b6e56-307">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="b6e56-307">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="b6e56-308">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="b6e56-308">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="b6e56-309">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="b6e56-309">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="b6e56-310">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="b6e56-310">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="b6e56-311">Problem bei Verwendung von „Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings“ mit festgelegtem Parameter für den Speicherkontonamen behoben</span><span class="sxs-lookup"><span data-stu-id="b6e56-311">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="b6e56-312">0.5.0 – November 2018</span><span class="sxs-lookup"><span data-stu-id="b6e56-312">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="b6e56-313">Allgemein</span><span class="sxs-lookup"><span data-stu-id="b6e56-313">General</span></span>
* <span data-ttu-id="b6e56-314">Ressourcenvervollständigungen für viele Kern-Cmdlets hinzugefügt (diese ermöglichen das Durchlaufen von vorhandenen Ressourcennamen per TAB-TASTE, wenn Cmdlets interaktiv aufgerufen werden)</span><span class="sxs-lookup"><span data-stu-id="b6e56-314">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="b6e56-315">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="b6e56-315">Az.Profile</span></span>
* <span data-ttu-id="b6e56-316">Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="b6e56-316">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="b6e56-317">Parameter „TenantId“ im Cmdlet „Connect-AzAccount“ in „Tenant“ umbenannt und Alias für „TenantId“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-317">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="b6e56-318">Beschreibung von „TenantId“ für „Connect-AzAccount“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-318">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="b6e56-319">Fehlermeldung für fehlgeschlagene Anmeldung bei Angabe der Mandantendomäne korrigiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-319">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="b6e56-320">Problem in Bezug auf Kontextnamenskonflikt für Konten ohne Abonnements im Mandanten behoben</span><span class="sxs-lookup"><span data-stu-id="b6e56-320">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="b6e56-321">Problem mit DataLake-Endpunkten bei Verwendung von MSI behoben</span><span class="sxs-lookup"><span data-stu-id="b6e56-321">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="b6e56-322">Problem behoben, das zur Auslösung von „Disconnect-AzAccount“ führte, wenn keine Verbindung bestand</span><span class="sxs-lookup"><span data-stu-id="b6e56-322">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="b6e56-323">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="b6e56-323">Az.CognitiveServices</span></span>
* <span data-ttu-id="b6e56-324">Vorgang „Get-AzCognitiveServicesAccountSkus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-324">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b6e56-325">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b6e56-325">Az.Compute</span></span>
* <span data-ttu-id="b6e56-326">Cmdlets Add-AzVmssVMDataDisk und Remove-AzVmssVMDataDisk hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-326">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="b6e56-327">„Get-AzVMImage“ zeigt „AutomaticOSUpgradeProperties“ an</span><span class="sxs-lookup"><span data-stu-id="b6e56-327">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="b6e56-328">Problem behoben, aufgrund dessen die Optionswerte „SetAzVMChefExtension -BootstrapOptions“ und „-JsonAttribute“ nicht im JSON-Format festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="b6e56-328">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="b6e56-329">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="b6e56-329">Az.DataLakeStore</span></span>
* <span data-ttu-id="b6e56-330">Aktualisierung des DataLake-Pakets auf 1.1.10</span><span class="sxs-lookup"><span data-stu-id="b6e56-330">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="b6e56-331">Standardmäßige Parallelität zu Multithreadvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-331">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="b6e56-332">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="b6e56-332">Az.Insights</span></span>
* <span data-ttu-id="b6e56-333">Problem Nr. 7267 behoben (Bereich für automatische Skalierung)</span><span class="sxs-lookup"><span data-stu-id="b6e56-333">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="b6e56-334">Probleme beim Erstellen einer neuen Regel für die automatische Skalierung, aufgrund derer die aufgelisteten Parameter nicht richtig festgelegt wurden (Es wurde stets der Standardwert festgelegt.)</span><span class="sxs-lookup"><span data-stu-id="b6e56-334">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="b6e56-335">Problem Nr. 7513 behoben [Insights] „Set-AzDiagnosticSetting“ erfordert die explizite Angabe von Kategorien während der Erstellung der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="b6e56-335">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="b6e56-336">Nun erfordert das Cmdlet nicht die explizite Angabe der Kategorien, die während der Erstellung aktiviert werden sollen. Das bedeutet, es funktioniert wie dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b6e56-336">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b6e56-337">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b6e56-337">Az.Network</span></span>
* <span data-ttu-id="b6e56-338">„PeeringType“ wurde geändert und ist nun ein erforderlicher Parameter für die folgenden Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="b6e56-338">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="b6e56-339">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="b6e56-339">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="b6e56-340">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="b6e56-340">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="b6e56-341">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="b6e56-341">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="b6e56-342">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="b6e56-342">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="b6e56-343">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="b6e56-343">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="b6e56-344">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="b6e56-344">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="b6e56-345">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="b6e56-345">Az.PolicyInsights</span></span>
* <span data-ttu-id="b6e56-346">Cmdlets für Richtlinienwartung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-346">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="b6e56-347">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b6e56-347">Az.Resources</span></span>
* <span data-ttu-id="b6e56-348">Fehlerbehebung für https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="b6e56-348">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="b6e56-349">Zulassen der Auflistung von Ressourcen mithilfe des Parameters „-ResourceId“ für „Get-AzResource“</span><span class="sxs-lookup"><span data-stu-id="b6e56-349">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="b6e56-350">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="b6e56-350">Az.ServiceBus</span></span>
* <span data-ttu-id="b6e56-351">Schreibgeschützte Eigenschaft „MigrationState“ zu „PSServiceBusMigrationConfigurationAttributes“ hinzugefügt, was das Ermitteln des Migrationsstatus ermöglicht</span><span class="sxs-lookup"><span data-stu-id="b6e56-351">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="b6e56-352">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="b6e56-352">Az.ServiceFabric</span></span>
* <span data-ttu-id="b6e56-353">Hinzufügen des Zertifikats zu Linux VMSS korrigiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-353">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="b6e56-354">„Add-AzServiceFabricClusterCertificate“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="b6e56-354">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="b6e56-355">Verwenden des richtigen Fingerabdrucks aus dem neuen Zertifikat (Azure/service-fabric-issues#932)</span><span class="sxs-lookup"><span data-stu-id="b6e56-355">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="b6e56-356">Richtige Anzeige von Ausnahmen (Azure/service-fabric-issues#1054)</span><span class="sxs-lookup"><span data-stu-id="b6e56-356">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="b6e56-357">„Update-AzServiceFabricDurability“ korrigiert, um die Clusterkonfiguration zu aktualisieren, bevor der VMSS-Vorgang „CreateOrUpdate“ gestartet wird</span><span class="sxs-lookup"><span data-stu-id="b6e56-357">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="b6e56-358">0.4.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="b6e56-358">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="b6e56-359">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="b6e56-359">Az.Profile</span></span>
* <span data-ttu-id="b6e56-360">Problem mit „Get-AzSubscription“ in Cloud Shell behoben</span><span class="sxs-lookup"><span data-stu-id="b6e56-360">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="b6e56-361">Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="b6e56-361">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b6e56-362">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b6e56-362">Az.Compute</span></span>
* <span data-ttu-id="b6e56-363">Neue Größen zur Whitelist von VM-Größen hinzugefügt, für die bei Verwendung des einfachen Parametersatzes für „New-AzVm“ der beschleunigte Netzwerkbetrieb aktiviert wird</span><span class="sxs-lookup"><span data-stu-id="b6e56-363">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="b6e56-364">ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b6e56-364">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="b6e56-365">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="b6e56-365">Az.DataLakeStore</span></span>
* <span data-ttu-id="b6e56-366">Unterstützung für Regeln für virtuelle Netzwerke hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-366">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="b6e56-367">Get-AzDataLakeStoreVirtualNetworkRule: Dient zum Abrufen oder Auflisten der Azure Data Lake Store-Regel für das virtuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="b6e56-367">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="b6e56-368">Add-AzDataLakeStoreVirtualNetworkRule: Fügt dem angegebenen Data Lake Store-Konto eine Regel für das virtuelle Netzwerk hinzu.</span><span class="sxs-lookup"><span data-stu-id="b6e56-368">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="b6e56-369">Set-AzDataLakeStoreVirtualNetworkRule: Ändert die angegebene Regel für das virtuelle Netzwerk in das angegebene Data Lake Store-Konto.</span><span class="sxs-lookup"><span data-stu-id="b6e56-369">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="b6e56-370">Remove-AzDataLakeStoreVirtualNetworkRule: Dient zum Löschen der Azure Data Lake Store-Regel für das virtuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="b6e56-370">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b6e56-371">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b6e56-371">Az.Network</span></span>
* <span data-ttu-id="b6e56-372">Cmdlet „Test-AzNetworkWatcherConnectivity“ aktualisiert, Protokollwert wird jetzt an Back-End übergeben.</span><span class="sxs-lookup"><span data-stu-id="b6e56-372">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="b6e56-373">ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b6e56-373">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="b6e56-374">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b6e56-374">Az.Resources</span></span>
* <span data-ttu-id="b6e56-375">Problem behoben, aufgrund dessen „Get-AzRoleDefinition“ eine unverständliche Ausnahme auslöst (wenn das Standardprofil kein Abonnement enthält und kein Bereich festgelegt ist), indem im Szenario eine aussagekräftige Ausnahme hinzugefügt wurde.</span><span class="sxs-lookup"><span data-stu-id="b6e56-375">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="b6e56-376">Außerdem wurde der Standardparametersatz auf „RoleDefinitionNameParameterSet“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="b6e56-376">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="b6e56-377">0.3.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="b6e56-377">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="b6e56-378">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="b6e56-378">Azure.Storage</span></span>
* <span data-ttu-id="b6e56-379">Fehler beim Kopieren von Blobs/Dateien behoben, aufgrund dessen bei einem Metadatenproblem des Ziels keine Metadaten kopiert wurden</span><span class="sxs-lookup"><span data-stu-id="b6e56-379">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="b6e56-380">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="b6e56-380">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="b6e56-381">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="b6e56-381">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="b6e56-382">Der Abruf der Speicherressourcennutzung eines bestimmten Standorts wird jetzt unterstützt, und das Hinzufügen einer Warnmeldung für den Abruf der globalen Speicherressourcennutzung ist überflüssig.</span><span class="sxs-lookup"><span data-stu-id="b6e56-382">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="b6e56-383">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="b6e56-383">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="b6e56-384">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="b6e56-384">Az.CognitiveServices</span></span>
* <span data-ttu-id="b6e56-385">„Get-AzCognitiveServicesAccountSkus“ wird ohne vorhandenes Konto unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b6e56-385">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b6e56-386">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b6e56-386">Az.Compute</span></span>
* <span data-ttu-id="b6e56-387">Korrektur von „Get-AzVM -ResourceGroupName <rg>“, sodass ggf. mehr als 50 Ergebnisse zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="b6e56-387">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="b6e56-388">Der Cmdlet-Hilfe zu „New-AzVmss“ wurde ein Beispiel für „SimpleParameterSet“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b6e56-388">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="b6e56-389">Tippfehler in der Azure Disk Encryption-Statusmeldung behoben</span><span class="sxs-lookup"><span data-stu-id="b6e56-389">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="b6e56-390">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="b6e56-390">Az.DataFactoryV2</span></span>
* <span data-ttu-id="b6e56-391">Die Version des ADF .Net-SDK wurde auf 2.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="b6e56-391">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b6e56-392">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b6e56-392">Az.Network</span></span>
* <span data-ttu-id="b6e56-393">NetworkProfile-Funktionalität wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b6e56-393">Added NetworkProfile functionality.</span></span> <span data-ttu-id="b6e56-394">Neue Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-394">new cmdlets added</span></span>
    - <span data-ttu-id="b6e56-395">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="b6e56-395">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="b6e56-396">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="b6e56-396">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="b6e56-397">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="b6e56-397">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="b6e56-398">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="b6e56-398">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="b6e56-399">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="b6e56-399">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="b6e56-400">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="b6e56-400">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="b6e56-401">Dienstzuordnungslink in Subnetzmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-401">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="b6e56-402">Cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-402">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="b6e56-403">Cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-403">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="b6e56-404">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="b6e56-404">Az.RedisCache</span></span>
* <span data-ttu-id="b6e56-405">Künftig sind beliebige Zeichenfolgen als Größenparameter zulässig.</span><span class="sxs-lookup"><span data-stu-id="b6e56-405">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="b6e56-406">P5 in Popup „PSArgumentCompleter“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-406">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="b6e56-407">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b6e56-407">Az.Resources</span></span>
* <span data-ttu-id="b6e56-408">Fehlender Parameter „-Mode“ zu „Set-AzPolicyDefinition“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b6e56-408">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="b6e56-409">Cmdlet-Fehler bei „Get-AzProviderOperation“ für Vorgänge mit Ursprung behoben, der den Benutzer enthält</span><span class="sxs-lookup"><span data-stu-id="b6e56-409">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="b6e56-410">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b6e56-410">Az.Sql</span></span>
* <span data-ttu-id="b6e56-411">Problem behoben, aufgrund dessen einige Sicherungs-Cmdlets das aktuelle Azure-Abonnements nicht erkannt haben</span><span class="sxs-lookup"><span data-stu-id="b6e56-411">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="b6e56-412">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b6e56-412">Az.Websites</span></span>
* <span data-ttu-id="b6e56-413">Neues Cmdlet „Get-AzWebAppContainerContinuousDeploymentUrl“ zum Abrufen der Webhook-URL von Continuous Deployment für Container</span><span class="sxs-lookup"><span data-stu-id="b6e56-413">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="b6e56-414">Neue Cmdlets „New-AzWebAppContainerPSSession“ und „Enter-WebAppContainerPSSession“ zum Initiieren einer PowerShell-Remotesitzung in einer Windows-Container-App</span><span class="sxs-lookup"><span data-stu-id="b6e56-414">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="b6e56-415">0.2.0 – September 2018</span><span class="sxs-lookup"><span data-stu-id="b6e56-415">0.2.0 - September 2018</span></span>
 <span data-ttu-id="b6e56-416">Erste Version</span><span class="sxs-lookup"><span data-stu-id="b6e56-416">Initial Release</span></span>