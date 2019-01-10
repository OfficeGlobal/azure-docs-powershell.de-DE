## <a name="100---december-2018"></a><span data-ttu-id="d75ff-101">1.0.0 – Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="d75ff-101">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="d75ff-102">Allgemein</span><span class="sxs-lookup"><span data-stu-id="d75ff-102">General</span></span>

- <span data-ttu-id="d75ff-103">Allgemeine Verfügbarkeit des Az-Moduls</span><span class="sxs-lookup"><span data-stu-id="d75ff-103">General Availability of Az Module</span></span>
- <span data-ttu-id="d75ff-104">Onlinehilfe für jedes Modul</span><span class="sxs-lookup"><span data-stu-id="d75ff-104">Online help for each module</span></span>
- <span data-ttu-id="d75ff-105">Ausführlichere Informationen und eine Roadmap finden Sie auf der [Seite mit der Ankündigung zu Az](https://aka.ms/azps-announce).</span><span class="sxs-lookup"><span data-stu-id="d75ff-105">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="d75ff-106">Informationen zur Migration aus AzureRM finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="d75ff-106">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="d75ff-107">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d75ff-107">Az.Accounts</span></span>
- <span data-ttu-id="d75ff-108">Geändert von Az.Profile</span><span class="sxs-lookup"><span data-stu-id="d75ff-108">Changed from Az.Profile</span></span>
- <span data-ttu-id="d75ff-109">Feste Tabellenformate für Profil- und Kontexttypen</span><span class="sxs-lookup"><span data-stu-id="d75ff-109">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="d75ff-110">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d75ff-110">Az.ApiManagement</span></span>
- <span data-ttu-id="d75ff-111">Korrekturen für #7002</span><span class="sxs-lookup"><span data-stu-id="d75ff-111">Fixes for #7002</span></span>
- <span data-ttu-id="d75ff-112">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="d75ff-112">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="d75ff-113">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="d75ff-113">Az.Batch</span></span>
- <span data-ttu-id="d75ff-114">Möglichkeit zum Anzeigen der ausgeführten Version des Azure Batch-Knoten-Agents auf den VMs eines Pools mit der neuen `NodeAgentInformation`-Eigenschaft für `PSComputeNode` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d75ff-114">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="d75ff-115">Der `Caching`-Standardwert für `PSDataDisk` lautet jetzt nicht mehr `None`, sondern `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="d75ff-115">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="d75ff-116">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="d75ff-116">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="d75ff-117">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="d75ff-117">Az.Billing</span></span>
- <span data-ttu-id="d75ff-118">Kombination von Billing-, Consumption- und UsageAggregates-Cmdlets. Ausführliche Informationen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="d75ff-118">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="d75ff-119">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="d75ff-119">Az.CognitivServices</span></span>
- <span data-ttu-id="d75ff-120">Vervollständigungen für SkuName und Typem für den Vorgang New-AzureRmCognitiveServicesAccount hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-120">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="d75ff-121">GetSkusWithAccountParamSetName-Parametersatz aus Get-AzCognitiveServicesAccountSkus entfernt</span><span class="sxs-lookup"><span data-stu-id="d75ff-121">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="d75ff-122">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="d75ff-122">Az.ContainerInstance</span></span>
- <span data-ttu-id="d75ff-123">ManagedIdentity-Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-123">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="d75ff-124">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="d75ff-124">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="d75ff-125">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="d75ff-125">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="d75ff-126">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d75ff-126">Az.DataLakeStore</span></span>
- <span data-ttu-id="d75ff-127">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="d75ff-127">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="d75ff-128">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="d75ff-128">Az.Monitor</span></span>
- <span data-ttu-id="d75ff-129">Az.Insights in Az.Monitor umbenannt und weitere weniger wichtige grundlegende Änderungen durchgeführt. Informationen hierzu finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="d75ff-129">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="d75ff-130">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d75ff-130">Az.KeyVault</span></span>
- <span data-ttu-id="d75ff-131">Veraltete PurgeDisabled-Eigenschaft aus Ausgabetypen entfernt</span><span class="sxs-lookup"><span data-stu-id="d75ff-131">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="d75ff-132">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="d75ff-132">Az.MachineLearning</span></span>
- <span data-ttu-id="d75ff-133">Cmdlets des Az.MachineLearningCompute-Moduls eingebunden</span><span class="sxs-lookup"><span data-stu-id="d75ff-133">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="d75ff-134">Az.Media</span><span class="sxs-lookup"><span data-stu-id="d75ff-134">Az.Media</span></span>
- <span data-ttu-id="d75ff-135">Veralteten -Tags-Alias aus New-AzMediaService entfernt</span><span class="sxs-lookup"><span data-stu-id="d75ff-135">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="d75ff-136">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d75ff-136">Az.Network</span></span>
<span data-ttu-id="d75ff-137">Unterstützung für das Konfigurieren von RewriteRuleSets im Application Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-137">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="d75ff-138">Neu hinzugefügte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d75ff-138">New cmdlets added:</span></span>
        - <span data-ttu-id="d75ff-139">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="d75ff-139">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="d75ff-140">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="d75ff-140">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="d75ff-141">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="d75ff-141">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="d75ff-142">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="d75ff-142">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="d75ff-143">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="d75ff-143">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="d75ff-144">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="d75ff-144">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="d75ff-145">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="d75ff-145">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="d75ff-146">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="d75ff-146">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="d75ff-147">Cmdlets mit optionalem Parameter -RewriteRuleSet aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d75ff-147">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="d75ff-148">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="d75ff-148">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="d75ff-149">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="d75ff-149">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="d75ff-150">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="d75ff-150">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="d75ff-151">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="d75ff-151">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="d75ff-152">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="d75ff-152">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="d75ff-153">New-AzureRmApplicationGatewayUrlPathMapConfig: KeyVault-Unterstützung mithilfe von Identität zum Application Gateway hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d75ff-153">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="d75ff-154">Cmdlets mit optionalem Parameter aktualisiert: -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="d75ff-154">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="d75ff-155">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="d75ff-155">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="d75ff-156">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="d75ff-156">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="d75ff-157">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="d75ff-157">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="d75ff-158">Cmdlet New-AzApplicationGateway mit optionalem Parameter -UserAssignedIdentity aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d75ff-158">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="d75ff-159">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="d75ff-159">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="d75ff-160">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="d75ff-160">Az.OperationalInsights</span></span>
- <span data-ttu-id="d75ff-161">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="d75ff-161">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="d75ff-162">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="d75ff-162">Az.Profile</span></span>
- <span data-ttu-id="d75ff-163">Modulnamen in Az.Accounts geändert</span><span class="sxs-lookup"><span data-stu-id="d75ff-163">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="d75ff-164">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d75ff-164">Az.RecoveryServices</span></span>
- <span data-ttu-id="d75ff-165">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="d75ff-165">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="d75ff-166">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d75ff-166">Az.Resources</span></span>
- <span data-ttu-id="d75ff-167">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="d75ff-167">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="d75ff-168">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d75ff-168">Az.ServiceFabric</span></span>
- <span data-ttu-id="d75ff-169">Unterstützung für das Angeben des Zertifikats anhand des allgemeinen Namens und Fingerabdrucks</span><span class="sxs-lookup"><span data-stu-id="d75ff-169">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="d75ff-170">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="d75ff-170">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="d75ff-171">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="d75ff-171">Az.SIgnalR</span></span>
- <span data-ttu-id="d75ff-172">Allgemeine Verfügbarkeit für PowerShell-Cmdlets für SIgnalR</span><span class="sxs-lookup"><span data-stu-id="d75ff-172">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="d75ff-173">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d75ff-173">Az.Sql</span></span>
- <span data-ttu-id="d75ff-174">Neue Erkennungstypen Data_Exfiltration und Unsafe_Action zu Cmdlets für Bedrohungserkennung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-174">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="d75ff-175">Dokumentationsbeispiele für Cmdlets für SQL-Überwachung aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d75ff-175">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="d75ff-176">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="d75ff-176">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="d75ff-177">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d75ff-177">Az.Storage</span></span>
- <span data-ttu-id="d75ff-178">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="d75ff-178">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="d75ff-179">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d75ff-179">Az.Websites</span></span>
- <span data-ttu-id="d75ff-180">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="d75ff-180">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="d75ff-181">0.7.0 – Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="d75ff-181">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="d75ff-182">Allgemein</span><span class="sxs-lookup"><span data-stu-id="d75ff-182">General</span></span>

* <span data-ttu-id="d75ff-183">Geringe Änderungen für anstehenden Übergang von AzureRM zu Az</span><span class="sxs-lookup"><span data-stu-id="d75ff-183">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="d75ff-184">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d75ff-184">Az.Compute</span></span>

* <span data-ttu-id="d75ff-185">Unterstützung für UltraSSD und Katalogimages in einfachen Parametersätzen für `New-AzVm(ss)`-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d75ff-185">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="d75ff-186">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d75ff-186">Az.DataLakeStore</span></span>

* <span data-ttu-id="d75ff-187">Nachgestellten Schrägstrich für die Domäne des ADLS-Kontos korrigiert</span><span class="sxs-lookup"><span data-stu-id="d75ff-187">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="d75ff-188">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="d75ff-188">Az.FrontDoor</span></span>

* <span data-ttu-id="d75ff-189">Einige fehlerhafte Links behoben</span><span class="sxs-lookup"><span data-stu-id="d75ff-189">Fixed some broken links</span></span>
    - <span data-ttu-id="d75ff-190">In den Artikeln zu New-AzureRmFrontDoor und Set-AzureRmFrontDoor den Artikel-Link zum Cmdlet „New-AzureRmFrontDoorHealthProbeSettingObject“ korrigiert.</span><span class="sxs-lookup"><span data-stu-id="d75ff-190">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="d75ff-191">Im Artikel zu New-AzureRmFrontDoorManagedRuleObject den Artikel-Link zum Cmdlet „New-AzureRmFrontDoorRuleGroupOverrideObject“ korrigiert.</span><span class="sxs-lookup"><span data-stu-id="d75ff-191">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="d75ff-192">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d75ff-192">Az.RecoveryServices</span></span>

* <span data-ttu-id="d75ff-193">Clientseitige Validierungen für Wiederherstellungsvorgänge von Azure-Dateifreigaben hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d75ff-193">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="d75ff-194">storageAccountName und storageAccountResourceGroupName für AFS-Wiederherstellung optional gemacht.</span><span class="sxs-lookup"><span data-stu-id="d75ff-194">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="d75ff-195">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d75ff-195">Az.Resources</span></span>

* <span data-ttu-id="d75ff-196">Fehlerbehebung für https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="d75ff-196">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="d75ff-197">Get-AzureRmRoleAssignment für die Verwendung des Abonnementbereichs aktualisiert, wenn dieser beim Anfordern von klassischen Administratoren angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="d75ff-197">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="d75ff-198">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d75ff-198">Az.Sql</span></span>

* <span data-ttu-id="d75ff-199">Geringe Änderungen für anstehenden Übergang von AzureRM zu Az</span><span class="sxs-lookup"><span data-stu-id="d75ff-199">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="d75ff-200">Problem mit der Verwendung von Get-AzureRmSqlDatabaseVulnerabilityAssessment mit .NET Core behoben</span><span class="sxs-lookup"><span data-stu-id="d75ff-200">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="d75ff-201">Dokumentation mit Hilfemeldungen zu Cmdlets für die SQL-Überwachung geändert.</span><span class="sxs-lookup"><span data-stu-id="d75ff-201">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="d75ff-202">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d75ff-202">Az.Storage</span></span>

* <span data-ttu-id="d75ff-203">-EnableHierarchicalNamespace zu New-AzureRmStorageAccount hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-203">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="d75ff-204">Problem behoben, bei dem für das Copy File-Cmdlet am Ziel kein Quellkontext wiederverwendet werden kann, wenn -DestContext nicht eingegeben wird</span><span class="sxs-lookup"><span data-stu-id="d75ff-204">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="d75ff-205">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="d75ff-205">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="d75ff-206">Unterstützung der Konfiguration von statischen Websites</span><span class="sxs-lookup"><span data-stu-id="d75ff-206">Support Static Website configuration</span></span>
    - <span data-ttu-id="d75ff-207">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="d75ff-207">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="d75ff-208">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="d75ff-208">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="d75ff-209">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d75ff-209">Az.Websites</span></span>

* <span data-ttu-id="d75ff-210">Set-AzureRmWebApp und Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="d75ff-210">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="d75ff-211">Neuen Parameter (-AzureStoragePath) zum Angeben von Azure Storage-Pfaden hinzugefügt, die in Windows- und Linux-Container-Apps bereitgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d75ff-211">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="d75ff-212">Verwenden Sie die Ausgabe des neuen Cmdlets New-AzureRmWebAppAzureStoragePath als Parameter zum Festlegen der Azure Storage-Pfade.</span><span class="sxs-lookup"><span data-stu-id="d75ff-212">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="d75ff-213">0.6.1 – November 2018</span><span class="sxs-lookup"><span data-stu-id="d75ff-213">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="d75ff-214">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d75ff-214">Az.ApiManagement</span></span>
* <span data-ttu-id="d75ff-215">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d75ff-215">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="d75ff-216">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="d75ff-216">Az.Automation</span></span>
* <span data-ttu-id="d75ff-217">Swagger-basierte Azure Automation-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="d75ff-217">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="d75ff-218">Cmdlets zur Updateverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-218">Added Update Management cmdlets</span></span>
* <span data-ttu-id="d75ff-219">Cmdlets zur Quellcodeverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-219">Added Source Control cmdlets</span></span>
* <span data-ttu-id="d75ff-220">Cmdlet „Remove-AzureRmAutomationHybridWorkerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-220">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="d75ff-221">DSC-Befehl für die Knotenregistrierung korrigiert</span><span class="sxs-lookup"><span data-stu-id="d75ff-221">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="d75ff-222">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d75ff-222">Az.Compute</span></span>
* <span data-ttu-id="d75ff-223">Identitätsproblem für SystemAssigned-Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="d75ff-223">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="d75ff-224">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d75ff-224">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="d75ff-225">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="d75ff-225">Az.ContainerInstance</span></span>
* <span data-ttu-id="d75ff-226">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d75ff-226">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="d75ff-227">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="d75ff-227">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="d75ff-228">Beschreibung der Beispiele für Marketplace-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d75ff-228">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="d75ff-229">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d75ff-229">Az.Network</span></span>
* <span data-ttu-id="d75ff-230">Folgende Cmdlets hinzugefügt: New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="d75ff-230">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="d75ff-231">ICMP wieder unterstützten AzureFirewall-Netzwerkprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-231">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="d75ff-232">Cmdlet „Test-AzureRmNetworkWatcherConnectivity“ aktualisiert und Überprüfung für Ziel-ID, Adresse und Port hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-232">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="d75ff-233">Probleme mit Arbeitsspeicherauslastung in der VirtualNetwork-Zuordnung behoben</span><span class="sxs-lookup"><span data-stu-id="d75ff-233">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="d75ff-234">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="d75ff-234">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="d75ff-235">Problem beim Ändern der Richtlinie für eine geschützte Dateifreigabe behoben</span><span class="sxs-lookup"><span data-stu-id="d75ff-235">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="d75ff-236">Richtlinienzeitzone in Großschreibung geändert</span><span class="sxs-lookup"><span data-stu-id="d75ff-236">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="d75ff-237">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="d75ff-237">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="d75ff-238">Korrigiertes Beispiel in „New-AzureRmRecoveryServicesAsrProtectableItem“</span><span class="sxs-lookup"><span data-stu-id="d75ff-238">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="d75ff-239">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d75ff-239">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="d75ff-240">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="d75ff-240">Az.Relay</span></span>
* <span data-ttu-id="d75ff-241">Optionaler Parameter „-KeyValue“ zu Cmdlet „New-AzureRmRelayKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht</span><span class="sxs-lookup"><span data-stu-id="d75ff-241">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="d75ff-242">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d75ff-242">Az.Resources</span></span>
* <span data-ttu-id="d75ff-243">Hilfedokumentation für ressourcenidentitätsbezogene Parameter in `New-AzureRmPolicyAssignment` und `Set-AzureRmPolicyAssignment` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d75ff-243">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="d75ff-244">Beispiel für „New-AzureRmPolicyDefinition“ hinzugefügt, das „-Metadata“ nutzt</span><span class="sxs-lookup"><span data-stu-id="d75ff-244">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="d75ff-245">Korrektur, um Beibehaltung von Groß-/Kleinschreibung in Tagschlüsseln in „NetStandard“ zu ermöglichen: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="d75ff-245">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="d75ff-246">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d75ff-246">Az.ServiceFabric</span></span>
* <span data-ttu-id="d75ff-247">Benachrichtigung über veraltete Elemente für anstehende wichtige Änderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-247">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="d75ff-248">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d75ff-248">Az.Sql</span></span>
* <span data-ttu-id="d75ff-249">Neue Cmdlets für CRUD-Vorgänge in verwalteten Azure SQL-Datenbank-Instanzen und verwalteten Azure SQL-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-249">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="d75ff-250">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="d75ff-250">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="d75ff-251">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="d75ff-251">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="d75ff-252">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="d75ff-252">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="d75ff-253">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="d75ff-253">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="d75ff-254">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="d75ff-254">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="d75ff-255">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="d75ff-255">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="d75ff-256">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="d75ff-256">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="d75ff-257">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="d75ff-257">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="d75ff-258">Erweiterte Verwaltung von Überwachungsrichtlinien auf einem Server oder in einer Datenbank aktiviert</span><span class="sxs-lookup"><span data-stu-id="d75ff-258">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="d75ff-259">Neuer Parameter (PredicateExpression) hinzugefügt, um die Filterung von Überwachungsprotokollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="d75ff-259">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="d75ff-260">Cmdlets wurden angepasst, sodass sie SQL-Clients anstelle von Legacyclients verwenden.</span><span class="sxs-lookup"><span data-stu-id="d75ff-260">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="d75ff-261">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="d75ff-261">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="d75ff-262">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="d75ff-262">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="d75ff-263">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="d75ff-263">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="d75ff-264">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="d75ff-264">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="d75ff-265">Problem bei Verwendung von „Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings“ mit festgelegtem Parameter für den Speicherkontonamen behoben</span><span class="sxs-lookup"><span data-stu-id="d75ff-265">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="d75ff-266">0.5.0 – November 2018</span><span class="sxs-lookup"><span data-stu-id="d75ff-266">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="d75ff-267">Allgemein</span><span class="sxs-lookup"><span data-stu-id="d75ff-267">General</span></span>
* <span data-ttu-id="d75ff-268">Ressourcenvervollständigungen für viele Kern-Cmdlets hinzugefügt (diese ermöglichen das Durchlaufen von vorhandenen Ressourcennamen per TAB-TASTE, wenn Cmdlets interaktiv aufgerufen werden)</span><span class="sxs-lookup"><span data-stu-id="d75ff-268">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="d75ff-269">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="d75ff-269">Az.Profile</span></span>
* <span data-ttu-id="d75ff-270">Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="d75ff-270">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="d75ff-271">Parameter „TenantId“ im Cmdlet „Connect-AzAccount“ in „Tenant“ umbenannt und Alias für „TenantId“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-271">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="d75ff-272">Beschreibung von „TenantId“ für „Connect-AzAccount“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d75ff-272">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="d75ff-273">Fehlermeldung für fehlgeschlagene Anmeldung bei Angabe der Mandantendomäne korrigiert</span><span class="sxs-lookup"><span data-stu-id="d75ff-273">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="d75ff-274">Problem in Bezug auf Kontextnamenskonflikt für Konten ohne Abonnements im Mandanten behoben</span><span class="sxs-lookup"><span data-stu-id="d75ff-274">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="d75ff-275">Problem mit DataLake-Endpunkten bei Verwendung von MSI behoben</span><span class="sxs-lookup"><span data-stu-id="d75ff-275">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="d75ff-276">Problem behoben, das zur Auslösung von „Disconnect-AzAccount“ führte, wenn keine Verbindung bestand</span><span class="sxs-lookup"><span data-stu-id="d75ff-276">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="d75ff-277">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="d75ff-277">Az.CognitiveServices</span></span>
* <span data-ttu-id="d75ff-278">Vorgang „Get-AzCognitiveServicesAccountSkus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-278">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d75ff-279">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d75ff-279">Az.Compute</span></span>
* <span data-ttu-id="d75ff-280">Cmdlets Add-AzVmssVMDataDisk und Remove-AzVmssVMDataDisk hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-280">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="d75ff-281">„Get-AzVMImage“ zeigt „AutomaticOSUpgradeProperties“ an</span><span class="sxs-lookup"><span data-stu-id="d75ff-281">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="d75ff-282">Problem behoben, aufgrund dessen die Optionswerte „SetAzVMChefExtension -BootstrapOptions“ und „-JsonAttribute“ nicht im JSON-Format festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="d75ff-282">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="d75ff-283">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d75ff-283">Az.DataLakeStore</span></span>
* <span data-ttu-id="d75ff-284">Aktualisierung des DataLake-Pakets auf 1.1.10</span><span class="sxs-lookup"><span data-stu-id="d75ff-284">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="d75ff-285">Standardmäßige Parallelität zu Multithreadvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-285">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="d75ff-286">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="d75ff-286">Az.Insights</span></span>
* <span data-ttu-id="d75ff-287">Problem Nr. 7267 behoben (Bereich für automatische Skalierung)</span><span class="sxs-lookup"><span data-stu-id="d75ff-287">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="d75ff-288">Probleme beim Erstellen einer neuen Regel für die automatische Skalierung, aufgrund derer die aufgelisteten Parameter nicht richtig festgelegt wurden (Es wurde stets der Standardwert festgelegt.)</span><span class="sxs-lookup"><span data-stu-id="d75ff-288">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="d75ff-289">Problem Nr. 7513 behoben [Insights] „Set-AzDiagnosticSetting“ erfordert die explizite Angabe von Kategorien während der Erstellung der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="d75ff-289">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="d75ff-290">Nun erfordert das Cmdlet nicht die explizite Angabe der Kategorien, die während der Erstellung aktiviert werden sollen. Das bedeutet, es funktioniert wie dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d75ff-290">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d75ff-291">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d75ff-291">Az.Network</span></span>
* <span data-ttu-id="d75ff-292">„PeeringType“ wurde geändert und ist nun ein erforderlicher Parameter für die folgenden Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d75ff-292">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="d75ff-293">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="d75ff-293">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="d75ff-294">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="d75ff-294">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="d75ff-295">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="d75ff-295">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="d75ff-296">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="d75ff-296">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="d75ff-297">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="d75ff-297">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="d75ff-298">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="d75ff-298">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="d75ff-299">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="d75ff-299">Az.PolicyInsights</span></span>
* <span data-ttu-id="d75ff-300">Cmdlets für Richtlinienwartung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-300">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="d75ff-301">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d75ff-301">Az.Resources</span></span>
* <span data-ttu-id="d75ff-302">Fehlerbehebung für https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="d75ff-302">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="d75ff-303">Zulassen der Auflistung von Ressourcen mithilfe des Parameters „-ResourceId“ für „Get-AzResource“</span><span class="sxs-lookup"><span data-stu-id="d75ff-303">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="d75ff-304">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d75ff-304">Az.ServiceBus</span></span>
* <span data-ttu-id="d75ff-305">Schreibgeschützte Eigenschaft „MigrationState“ zu „PSServiceBusMigrationConfigurationAttributes“ hinzugefügt, was das Ermitteln des Migrationsstatus ermöglicht</span><span class="sxs-lookup"><span data-stu-id="d75ff-305">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="d75ff-306">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d75ff-306">Az.ServiceFabric</span></span>
* <span data-ttu-id="d75ff-307">Hinzufügen des Zertifikats zu Linux VMSS korrigiert</span><span class="sxs-lookup"><span data-stu-id="d75ff-307">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="d75ff-308">„Add-AzServiceFabricClusterCertificate“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="d75ff-308">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="d75ff-309">Verwenden des richtigen Fingerabdrucks aus dem neuen Zertifikat (Azure/service-fabric-issues#932)</span><span class="sxs-lookup"><span data-stu-id="d75ff-309">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="d75ff-310">Richtige Anzeige von Ausnahmen (Azure/service-fabric-issues#1054)</span><span class="sxs-lookup"><span data-stu-id="d75ff-310">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="d75ff-311">„Update-AzServiceFabricDurability“ korrigiert, um die Clusterkonfiguration zu aktualisieren, bevor der VMSS-Vorgang „CreateOrUpdate“ gestartet wird</span><span class="sxs-lookup"><span data-stu-id="d75ff-311">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="d75ff-312">0.4.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="d75ff-312">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="d75ff-313">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="d75ff-313">Az.Profile</span></span>
* <span data-ttu-id="d75ff-314">Problem mit „Get-AzSubscription“ in Cloud Shell behoben</span><span class="sxs-lookup"><span data-stu-id="d75ff-314">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="d75ff-315">Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="d75ff-315">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d75ff-316">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d75ff-316">Az.Compute</span></span>
* <span data-ttu-id="d75ff-317">Neue Größen zur Whitelist von VM-Größen hinzugefügt, für die bei Verwendung des einfachen Parametersatzes für „New-AzVm“ der beschleunigte Netzwerkbetrieb aktiviert wird</span><span class="sxs-lookup"><span data-stu-id="d75ff-317">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="d75ff-318">ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d75ff-318">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="d75ff-319">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d75ff-319">Az.DataLakeStore</span></span>
* <span data-ttu-id="d75ff-320">Unterstützung für Regeln für virtuelle Netzwerke hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-320">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="d75ff-321">Get-AzDataLakeStoreVirtualNetworkRule: Dient zum Abrufen oder Auflisten der Azure Data Lake Store-Regel für das virtuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="d75ff-321">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="d75ff-322">Add-AzDataLakeStoreVirtualNetworkRule: Fügt dem angegebenen Data Lake Store-Konto eine Regel für das virtuelle Netzwerk hinzu.</span><span class="sxs-lookup"><span data-stu-id="d75ff-322">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="d75ff-323">Set-AzDataLakeStoreVirtualNetworkRule: Ändert die angegebene Regel für das virtuelle Netzwerk in das angegebene Data Lake Store-Konto.</span><span class="sxs-lookup"><span data-stu-id="d75ff-323">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="d75ff-324">Remove-AzDataLakeStoreVirtualNetworkRule: Dient zum Löschen der Azure Data Lake Store-Regel für das virtuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="d75ff-324">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d75ff-325">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d75ff-325">Az.Network</span></span>
* <span data-ttu-id="d75ff-326">Cmdlet „Test-AzNetworkWatcherConnectivity“ aktualisiert, Protokollwert wird jetzt an Back-End übergeben.</span><span class="sxs-lookup"><span data-stu-id="d75ff-326">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="d75ff-327">ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d75ff-327">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="d75ff-328">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d75ff-328">Az.Resources</span></span>
* <span data-ttu-id="d75ff-329">Problem behoben, aufgrund dessen „Get-AzRoleDefinition“ eine unverständliche Ausnahme auslöst (wenn das Standardprofil kein Abonnement enthält und kein Bereich festgelegt ist), indem im Szenario eine aussagekräftige Ausnahme hinzugefügt wurde.</span><span class="sxs-lookup"><span data-stu-id="d75ff-329">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="d75ff-330">Außerdem wurde der Standardparametersatz auf „RoleDefinitionNameParameterSet“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="d75ff-330">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="d75ff-331">0.3.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="d75ff-331">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="d75ff-332">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="d75ff-332">Azure.Storage</span></span>
* <span data-ttu-id="d75ff-333">Fehler beim Kopieren von Blobs/Dateien behoben, aufgrund dessen bei einem Metadatenproblem des Ziels keine Metadaten kopiert wurden</span><span class="sxs-lookup"><span data-stu-id="d75ff-333">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="d75ff-334">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="d75ff-334">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="d75ff-335">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="d75ff-335">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="d75ff-336">Der Abruf der Speicherressourcennutzung eines bestimmten Standorts wird jetzt unterstützt, und das Hinzufügen einer Warnmeldung für den Abruf der globalen Speicherressourcennutzung ist überflüssig.</span><span class="sxs-lookup"><span data-stu-id="d75ff-336">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="d75ff-337">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="d75ff-337">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="d75ff-338">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="d75ff-338">Az.CognitiveServices</span></span>
* <span data-ttu-id="d75ff-339">„Get-AzCognitiveServicesAccountSkus“ wird ohne vorhandenes Konto unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d75ff-339">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d75ff-340">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d75ff-340">Az.Compute</span></span>
* <span data-ttu-id="d75ff-341">Korrektur von „Get-AzVM -ResourceGroupName <rg>“, sodass ggf. mehr als 50 Ergebnisse zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="d75ff-341">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="d75ff-342">Der Cmdlet-Hilfe zu „New-AzVmss“ wurde ein Beispiel für „SimpleParameterSet“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d75ff-342">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="d75ff-343">Tippfehler in der Azure Disk Encryption-Statusmeldung behoben</span><span class="sxs-lookup"><span data-stu-id="d75ff-343">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="d75ff-344">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="d75ff-344">Az.DataFactoryV2</span></span>
* <span data-ttu-id="d75ff-345">Die Version des ADF .Net-SDK wurde auf 2.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="d75ff-345">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d75ff-346">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d75ff-346">Az.Network</span></span>
* <span data-ttu-id="d75ff-347">NetworkProfile-Funktionalität wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d75ff-347">Added NetworkProfile functionality.</span></span> <span data-ttu-id="d75ff-348">Neue Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-348">new cmdlets added</span></span>
    - <span data-ttu-id="d75ff-349">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d75ff-349">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="d75ff-350">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d75ff-350">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="d75ff-351">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d75ff-351">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="d75ff-352">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d75ff-352">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="d75ff-353">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="d75ff-353">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="d75ff-354">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="d75ff-354">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="d75ff-355">Dienstzuordnungslink in Subnetzmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-355">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="d75ff-356">Cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-356">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="d75ff-357">Cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-357">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="d75ff-358">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="d75ff-358">Az.RedisCache</span></span>
* <span data-ttu-id="d75ff-359">Künftig sind beliebige Zeichenfolgen als Größenparameter zulässig.</span><span class="sxs-lookup"><span data-stu-id="d75ff-359">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="d75ff-360">P5 in Popup „PSArgumentCompleter“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-360">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="d75ff-361">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d75ff-361">Az.Resources</span></span>
* <span data-ttu-id="d75ff-362">Fehlender Parameter „-Mode“ zu „Set-AzPolicyDefinition“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d75ff-362">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="d75ff-363">Cmdlet-Fehler bei „Get-AzProviderOperation“ für Vorgänge mit Ursprung behoben, der den Benutzer enthält</span><span class="sxs-lookup"><span data-stu-id="d75ff-363">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="d75ff-364">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d75ff-364">Az.Sql</span></span>
* <span data-ttu-id="d75ff-365">Problem behoben, aufgrund dessen einige Sicherungs-Cmdlets das aktuelle Azure-Abonnements nicht erkannt haben</span><span class="sxs-lookup"><span data-stu-id="d75ff-365">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="d75ff-366">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d75ff-366">Az.Websites</span></span>
* <span data-ttu-id="d75ff-367">Neues Cmdlet „Get-AzWebAppContainerContinuousDeploymentUrl“ zum Abrufen der Webhook-URL von Continuous Deployment für Container</span><span class="sxs-lookup"><span data-stu-id="d75ff-367">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="d75ff-368">Neue Cmdlets „New-AzWebAppContainerPSSession“ und „Enter-WebAppContainerPSSession“ zum Initiieren einer PowerShell-Remotesitzung in einer Windows-Container-App</span><span class="sxs-lookup"><span data-stu-id="d75ff-368">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="d75ff-369">0.2.0 – September 2018</span><span class="sxs-lookup"><span data-stu-id="d75ff-369">0.2.0 - September 2018</span></span>
 <span data-ttu-id="d75ff-370">Erste Version</span><span class="sxs-lookup"><span data-stu-id="d75ff-370">Initial Release</span></span>