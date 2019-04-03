---
ms.openlocfilehash: 2db9810e20254373a487013de50d4297d4ec50d5
ms.sourcegitcommit: 8f59e11e5c991543964154d63648aa1e6ae22512
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2019
ms.locfileid: "58475259"
---
## <a name="160---march-2019"></a><span data-ttu-id="93878-101">1.6.0: März 2019</span><span class="sxs-lookup"><span data-stu-id="93878-101">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="93878-102">Highlights seit der letzten Hauptversion</span><span class="sxs-lookup"><span data-stu-id="93878-102">Highlights since the last major release</span></span>
* <span data-ttu-id="93878-103">Allgemeine Verfügbarkeit des `Az`-Moduls</span><span class="sxs-lookup"><span data-stu-id="93878-103">General availability of `Az` module</span></span>
* <span data-ttu-id="93878-104">Weitere Informationen zum `Az`-Modul finden Sie unter folgendem Link: https://aka.ms/azps-announce.</span><span class="sxs-lookup"><span data-stu-id="93878-104">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="93878-105">Vervollständigung für Location, ResourceGroup und ResourceName hinzugefügt: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/.</span><span class="sxs-lookup"><span data-stu-id="93878-105">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="93878-106">Unterstützung für Platzhalter zu Get-Cmdlets für Az.Compute und Az.Network hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-106">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="93878-107">Interaktive und Benutzername/Kennwort-Authentifizierung ausschließlich für Windows PowerShell 5.1 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-107">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="93878-108">Unterstützung für Python 2-Runbooks in Az.Automation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-108">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="93878-109">Az.LogicApp: Neue Cmdlets für Integrationskonto-Assemblys und -Batchkonfiguration</span><span class="sxs-lookup"><span data-stu-id="93878-109">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="93878-110">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="93878-110">Az.Automation</span></span>
* <span data-ttu-id="93878-111">Änderung an der Azure Automation-Updateverwaltung, um die folgenden neuen Features zu unterstützen:</span><span class="sxs-lookup"><span data-stu-id="93878-111">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="93878-112">Dynamische Gruppierung</span><span class="sxs-lookup"><span data-stu-id="93878-112">Dynamic grouping</span></span>
    * <span data-ttu-id="93878-113">Pre-/Post-Skripts</span><span class="sxs-lookup"><span data-stu-id="93878-113">Pre-Post script</span></span>
    * <span data-ttu-id="93878-114">Neustarteinstellung</span><span class="sxs-lookup"><span data-stu-id="93878-114">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="93878-115">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="93878-115">Az.Compute</span></span>
* <span data-ttu-id="93878-116">Problem mit der Pfadauflösung in „Get-AzVmBootDiagnosticsData“ behoben</span><span class="sxs-lookup"><span data-stu-id="93878-116">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="93878-117">Computeclientbibliothek auf 25.0.0. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-117">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="93878-118">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="93878-118">Az.KeyVault</span></span>
* <span data-ttu-id="93878-119">Unterstützung für Platzhalterzeichen zu KeyVault-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-119">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="93878-120">Az.Network</span><span class="sxs-lookup"><span data-stu-id="93878-120">Az.Network</span></span>
* <span data-ttu-id="93878-121">Threat Intelligence-Unterstützung für Azure Firewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-121">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="93878-122">Ressource der obersten Ebene für Application Gateway-Firewallrichtlinie und benutzerdefinierte Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-122">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="93878-123">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="93878-123">Az.RecoveryServices</span></span>
* <span data-ttu-id="93878-124">SnapshotRetentionInDays in Azure-VM-Richtlinie hinzugefügt, um sofortigen Wiederherstellungspunkt zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="93878-124">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="93878-125">Pipe-Unterstützung für das Aufheben der Registrierung eines Containers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-125">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="93878-126">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="93878-126">Az.Resources</span></span>
* <span data-ttu-id="93878-127">Unterstützung für Platzhalterzeichen für Get-AzResource und Get-AzResourceGroup aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-127">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="93878-128">Anmeldeinformationen aktualisiert, die beim Senden generischer Aufrufe an ARM verwendet werden</span><span class="sxs-lookup"><span data-stu-id="93878-128">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="93878-129">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="93878-129">Az.Sql</span></span>
* <span data-ttu-id="93878-130">Der Cmdlet-Parameter der Bedrohungserkennung (ExcludeDetectionType) wurde von „DetectionType“ in „string[]“ geändert, um ihn zukunftssicher zu machen, wenn neue DetectionTypes-Elemente hinzugefügt werden, und um AutoVervollständigen zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="93878-130">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="93878-131">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="93878-131">Az.Storage</span></span>
* <span data-ttu-id="93878-132">Unterstützung von Get-/Set-/Remove-Verwaltungsrichtlinien für Speicherkonto hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-132">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="93878-133">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="93878-133">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="93878-134">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="93878-134">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="93878-135">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="93878-135">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="93878-136">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="93878-136">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="93878-137">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="93878-137">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="93878-138">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="93878-138">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="93878-139">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="93878-139">Az.Websites</span></span>
* <span data-ttu-id="93878-140">ARM-Vorlagenfehler behoben, der zu einem Problem beim Klonen aller Slots mithilfe von „New-AzWebApp -IncludeSourceWebAppSlots“ führte</span><span class="sxs-lookup"><span data-stu-id="93878-140">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="93878-141">1.5.0: März 2019</span><span class="sxs-lookup"><span data-stu-id="93878-141">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="93878-142">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="93878-142">Az.Accounts</span></span>
* <span data-ttu-id="93878-143">Der Befehl „Register-AzModule“ wurde hinzugefügt, um von AutoRest generierte Cmdlets zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="93878-143">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="93878-144">Beispiele für „Connect-AzAccount“ wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="93878-144">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="93878-145">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="93878-145">Az.Automation</span></span>
* <span data-ttu-id="93878-146">Problem behoben, das beim Abrufen bestimmter monatlicher Zeitpläne in verschiedenen Azure Automation-Cmdlets auftrat</span><span class="sxs-lookup"><span data-stu-id="93878-146">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="93878-147">„Get-AzAutomationDscNode“ wurde korrigiert, da nur die 20 obersten Knoten zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="93878-147">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="93878-148">Jetzt werden alle Knoten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="93878-148">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="93878-149">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="93878-149">Az.Cdn</span></span>
* <span data-ttu-id="93878-150">Neue Powershell-Cmdlets zum Aktivieren/Deaktivieren von HTTPS für benutzerdefinierte Domänen hinzugefügt und alte Cmdlets außer Betrieb genommen</span><span class="sxs-lookup"><span data-stu-id="93878-150">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="93878-151">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="93878-151">Az.Compute</span></span>
* <span data-ttu-id="93878-152">Unterstützung für Platzhalterzeichen zu Get-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-152">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="93878-153">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="93878-153">Az.DataFactory</span></span>
* <span data-ttu-id="93878-154">Version des ADF .NET SDK auf 3.0.1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-154">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="93878-155">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="93878-155">Az.LogicApp</span></span>
* <span data-ttu-id="93878-156">„ListWorkflows“ wurde korrigiert, da nur die erste Seite mit Ergebnissen abgerufen wurde.</span><span class="sxs-lookup"><span data-stu-id="93878-156">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="93878-157">Az.Network</span><span class="sxs-lookup"><span data-stu-id="93878-157">Az.Network</span></span>
* <span data-ttu-id="93878-158">Unterstützung für Platzhalterzeichen zu Network-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-158">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="93878-159">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="93878-159">Az.RecoveryServices</span></span>
* <span data-ttu-id="93878-160">SQL Server jetzt in Azure-VM-Support enthalten</span><span class="sxs-lookup"><span data-stu-id="93878-160">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="93878-161">SDK-Update</span><span class="sxs-lookup"><span data-stu-id="93878-161">SDK Update</span></span>
* <span data-ttu-id="93878-162">VMappContainer-Überprüfung in „Get-ProtectableItem“ entfernt</span><span class="sxs-lookup"><span data-stu-id="93878-162">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="93878-163">„Name“ und „ServerName“ als Parameter für „Get-ProtectableItem“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-163">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="93878-164">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="93878-164">Az.Resources</span></span>
* <span data-ttu-id="93878-165">Parameter `-TemplateObject` zu Bereitstellungs-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-165">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="93878-166">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="93878-166">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="93878-167">Problem beim Piping des Ergebnisses von `Get-AzResource` an `Set-AzResource` behoben</span><span class="sxs-lookup"><span data-stu-id="93878-167">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="93878-168">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="93878-168">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="93878-169">Problem mit JSON-Datentypänderung beim Ausführen von `Set-AzResource` behoben</span><span class="sxs-lookup"><span data-stu-id="93878-169">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="93878-170">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="93878-170">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="93878-171">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="93878-171">Az.Sql</span></span>
* <span data-ttu-id="93878-172">„AuditingEndpointsCommunicator“ wird aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="93878-172">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="93878-173">Das Verhalten eines Grenzfalls beim Erstellen neuer Diagnoseeinstellungen wurde korrigiert.</span><span class="sxs-lookup"><span data-stu-id="93878-173">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="93878-174">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="93878-174">Az.Storage</span></span>
* <span data-ttu-id="93878-175">Unterstützung von „Kind BlockBlobStorage“ beim Erstellen eines Speicherkontos: New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="93878-175">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="93878-176">1.4.0 – Februar 2019</span><span class="sxs-lookup"><span data-stu-id="93878-176">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="93878-177">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="93878-177">Az.AnalysisServices</span></span>
* <span data-ttu-id="93878-178">Cmdlet „AddAzureASAccount“ als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="93878-178">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="93878-179">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="93878-179">Az.Automation</span></span>
* <span data-ttu-id="93878-180">Hilfe für „Import-AzAutomationDscNodeConfiguration“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-180">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="93878-181">Überprüfung des Konfigurationsnamens zu Cmdlet „Import-AzAutomationDscConfiguration“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-181">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="93878-182">Fehlerbehandlung für Cmdlet „Import-AzAutomationDscConfiguration“ verbessert</span><span class="sxs-lookup"><span data-stu-id="93878-182">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="93878-183">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="93878-183">Az.CognitiveServices</span></span>
* <span data-ttu-id="93878-184">„CustomSubdomainName“ als neuer optionaler Parameter für Cmdlet „New-AzCognitiveServicesAccount“ hinzugefügt, das zum Angeben der Unterdomäne für die Ressource verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="93878-184">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="93878-185">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="93878-185">Az.Compute</span></span>
* <span data-ttu-id="93878-186">Problem mit ID-Parametersätzen behoben</span><span class="sxs-lookup"><span data-stu-id="93878-186">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="93878-187">„Get-AzVMExtension“ aktualisiert, sodass alle installierten Erweiterungen aufgelistet werden, wenn der Name-Parameter nicht angegeben ist</span><span class="sxs-lookup"><span data-stu-id="93878-187">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="93878-188">Parameter „Tag“ und „ResourceId“ zum Cmdlet „Update-AzImage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-188">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="93878-189">„Get-AzVmssVM“ ohne Instanz-ID und mit „InstanceView“ können virtuelle VMSS-Computer mit Instanzansicht auflisten.</span><span class="sxs-lookup"><span data-stu-id="93878-189">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="93878-190">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="93878-190">Az.DataLakeStore</span></span>
* <span data-ttu-id="93878-191">Cmdlets zum Auflisten und Wiederherstellen gelöschter ADL-Elemente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-191">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="93878-192">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="93878-192">Az.EventHub</span></span>
* <span data-ttu-id="93878-193">Neue boolesche Eigenschaft „SkipEmptyArchives“ zum Überspringen leerer Archive in Klasse „CaptureDescription“ von EventHub hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-193">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="93878-194">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="93878-194">Az.KeyVault</span></span>
* <span data-ttu-id="93878-195">Kennzeichnung in „Set-AzKeyVaultSecret“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="93878-195">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="93878-196">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="93878-196">Az.LogicApp</span></span>
* <span data-ttu-id="93878-197">SKU „Basic“ für Integrationskonten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-197">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="93878-198">XSLT 2.0, XSLT 3.0 und Liquid-Zuordnungstypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-198">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="93878-199">Neue Cmdlets für Integrationskonto-Assemblys</span><span class="sxs-lookup"><span data-stu-id="93878-199">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="93878-200">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="93878-200">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="93878-201">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="93878-201">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="93878-202">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="93878-202">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="93878-203">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="93878-203">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="93878-204">Neue Cmdlets für Integrationskonto-Batchkonfiguration</span><span class="sxs-lookup"><span data-stu-id="93878-204">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="93878-205">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="93878-205">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="93878-206">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="93878-206">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="93878-207">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="93878-207">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="93878-208">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="93878-208">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="93878-209">Logik-App-SDK auf Version 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-209">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="93878-210">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="93878-210">Az.Monitor</span></span>
* <span data-ttu-id="93878-211">Hilfe für „Get-AzMetric“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-211">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="93878-212">Az.Network</span><span class="sxs-lookup"><span data-stu-id="93878-212">Az.Network</span></span>
* <span data-ttu-id="93878-213">Hilfebeispiel für „Add-AzApplicationGatewayCustomError“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-213">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="93878-214">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="93878-214">Az.OperationalInsights</span></span>
* <span data-ttu-id="93878-215">Zusätzliche Unterstützung für Datenquelle von „New-ApplicationInsights“ und „Get-ApplicationInsights“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="93878-215">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="93878-216">Neue Art von „ApplicationInsights“ zum Abrufen von bestimmten und von allen ApplicationInsights-Datenquellen für einen Workspace hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="93878-216">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="93878-217">Cmdlet „New-AzOperationalInsightsApplicationInsightsDataSource“ zum Erstellen einer Datenquelle anhand des angegebenen Ressourcenparameters für „Application-Insights“ hinzugefügt: „subscriptionId“, „resourceGroupName“ und „name“.</span><span class="sxs-lookup"><span data-stu-id="93878-217">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="93878-218">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="93878-218">Az.Resources</span></span>
* <span data-ttu-id="93878-219">Behebung des Problems: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="93878-219">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="93878-220">Behebung des Problems: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="93878-220">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="93878-221">Behebung des Problems: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="93878-221">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="93878-222">Fehler korrigiert, der die wiederholte Erstellung von „KeyCredentials“ verhindert</span><span class="sxs-lookup"><span data-stu-id="93878-222">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="93878-223">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="93878-223">Az.Sql</span></span>
* <span data-ttu-id="93878-224">Unterstützung für SQL DB Hyperscale-Tarif hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-224">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="93878-225">Fehler korrigiert, aufgrund dessen die Wiederherstellung wegen der Festlegung unnötiger Eigenschaften in der Wiederherstellungsanforderung fehlschlagen konnte</span><span class="sxs-lookup"><span data-stu-id="93878-225">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="93878-226">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="93878-226">Az.Websites</span></span>
* <span data-ttu-id="93878-227">Beispiel in „Get-AzWebAppSlotMetrics“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="93878-227">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="93878-228">1.3.0: Februar 2019</span><span class="sxs-lookup"><span data-stu-id="93878-228">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="93878-229">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="93878-229">Az.Accounts</span></span>
* <span data-ttu-id="93878-230">Update auf die aktuelle Version von ClientRuntime durchgeführt</span><span class="sxs-lookup"><span data-stu-id="93878-230">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="93878-231">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="93878-231">Az.AnalysisServices</span></span>
<span data-ttu-id="93878-232">Allgemeine Verfügbarkeit für Az.AnalysisServices-Modul</span><span class="sxs-lookup"><span data-stu-id="93878-232">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="93878-233">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="93878-233">Az.Compute</span></span>
* <span data-ttu-id="93878-234">AEM-Erweiterung: Unterstützung für UltraSSD und P60-, P70- und P80-Datenträger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-234">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="93878-235">Hilfebeschreibung für „Set-AzVMBootDiagnostics“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-235">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="93878-236">Hilfebeschreibung und Beispiel für „Update-AzImage“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-236">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="93878-237">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="93878-237">Az.RecoveryServices</span></span>
<span data-ttu-id="93878-238">Allgemeine Verfügbarkeit für Az.RecoveryServices-Modul.</span><span class="sxs-lookup"><span data-stu-id="93878-238">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="93878-239">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="93878-239">Az.Resources</span></span>
* <span data-ttu-id="93878-240">Kennzeichnung für Ressourcengruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="93878-240">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="93878-241">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="93878-241">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="93878-242">Problem behoben, bei dem „-ErrorAction“ von `Get-AzureRmRoleAssignment` nicht berücksichtigt wird</span><span class="sxs-lookup"><span data-stu-id="93878-242">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="93878-243">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="93878-243">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="93878-244">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="93878-244">Az.Sql</span></span>
* <span data-ttu-id="93878-245">Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-245">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="93878-246">Problem behoben, bei dem eine fehlende Anmeldung am Azure-Konto bei der Ausführung von SQL-Cmdlets zu einer nullref-Ausnahme führt</span><span class="sxs-lookup"><span data-stu-id="93878-246">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="93878-247">nullref-Ausnahme in Get-AzSqlCapability korrigiert</span><span class="sxs-lookup"><span data-stu-id="93878-247">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="93878-248">1.2.1: Januar 2019</span><span class="sxs-lookup"><span data-stu-id="93878-248">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="93878-249">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="93878-249">Az.Accounts</span></span>
* <span data-ttu-id="93878-250">Release mit richtiger Version der Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="93878-250">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="93878-251">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="93878-251">Az.AnalysisServices</span></span>
* <span data-ttu-id="93878-252">Release mit aktualisierter Authentifizierungsabhängigkeit</span><span class="sxs-lookup"><span data-stu-id="93878-252">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="93878-253">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="93878-253">Az.RecoveryServices</span></span>
* <span data-ttu-id="93878-254">Release mit aktualisierter Authentifizierungsabhängigkeit</span><span class="sxs-lookup"><span data-stu-id="93878-254">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="93878-255">1.2.0: Januar 2019</span><span class="sxs-lookup"><span data-stu-id="93878-255">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="93878-256">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="93878-256">Az.Accounts</span></span>
* <span data-ttu-id="93878-257">Interaktive und Benutzername/Kennwort-Authentifizierung ausschließlich für Windows PowerShell 5.1 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-257">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="93878-258">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-258">Update incorrect online help URLs</span></span>
* <span data-ttu-id="93878-259">Warnmeldung in PS Core für „Uninstall-AzureRm“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-259">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="93878-260">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="93878-260">Az.Aks</span></span>
* <span data-ttu-id="93878-261">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-261">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="93878-262">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="93878-262">Az.Automation</span></span>
* <span data-ttu-id="93878-263">Unterstützung für Python 2-Runbooks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-263">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="93878-264">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-264">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="93878-265">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="93878-265">Az.Cdn</span></span>
* <span data-ttu-id="93878-266">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-266">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="93878-267">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="93878-267">Az.Compute</span></span>
* <span data-ttu-id="93878-268">Cmdlet „Invoke-AzVMReimage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-268">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="93878-269">Parameter „TempDisk“ zu „Set-AzVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-269">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="93878-270">Warnmeldung von „New-AzVM“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="93878-270">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="93878-271">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="93878-271">Az.ContainerRegistry</span></span>
* <span data-ttu-id="93878-272">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-272">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="93878-273">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="93878-273">Az.DataFactory</span></span>
* <span data-ttu-id="93878-274">Version des ADF .NET SDK auf 3.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-274">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="93878-275">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="93878-275">Az.DataLakeStore</span></span>
* <span data-ttu-id="93878-276">Problem mit ADLS-Endpunkt bei Verwendung von MSI behoben</span><span class="sxs-lookup"><span data-stu-id="93878-276">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="93878-277">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="93878-277">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="93878-278">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-278">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="93878-279">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="93878-279">Az.IotHub</span></span>
* <span data-ttu-id="93878-280">Codierungsformat zu Cmdlet „Add-IotHubRoutingEndpoint“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-280">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="93878-281">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="93878-281">Az.KeyVault</span></span>
* <span data-ttu-id="93878-282">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-282">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="93878-283">Az.Network</span><span class="sxs-lookup"><span data-stu-id="93878-283">Az.Network</span></span>
* <span data-ttu-id="93878-284">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-284">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="93878-285">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="93878-285">Az.Resources</span></span>
* <span data-ttu-id="93878-286">Fehlerhafte Beispiele in Referenzdokumentation zu „New-AzADAppCredential“ und „New-AzADSpCredential“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="93878-286">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="93878-287">Problem behoben, bei dem der Pfad für den Parameter „-TemplateFile“ nicht aufgelöst wurde, bevor Cmdlets für die Bereitstellung von Ressourcengruppen ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="93878-287">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="93878-288">Az.Resources: Richtige Dokumentation für Standardwert von „New-AzureRmPolicyDefinition -Mode“ bereitgestellt</span><span class="sxs-lookup"><span data-stu-id="93878-288">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="93878-289">Az.Resources: Behebung des Problems: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="93878-289">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="93878-290">Az.Resources: Behebung des Problems: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="93878-290">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="93878-291">Formatierungsproblem für Objekt „PSResourceGroupDeployment“ behoben</span><span class="sxs-lookup"><span data-stu-id="93878-291">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="93878-292">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="93878-292">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="93878-293">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="93878-293">Az.ServiceFabric</span></span>
* <span data-ttu-id="93878-294">Rollback beim Hinzufügen eines Zertifikats zum VMSS-Modell, Auslösung einer Ausnahme. Fehlerbehebung: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="93878-294">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="93878-295">Einige Fehlermeldungen wurden korrigiert.</span><span class="sxs-lookup"><span data-stu-id="93878-295">Fix some error messages.</span></span>
* <span data-ttu-id="93878-296">Fehler bei Clustererstellung mit ARM-Standardvorlage für „New-AzServiceFabriCluster“ behoben, bei dem die Migration zu Az nicht funktioniert hat.</span><span class="sxs-lookup"><span data-stu-id="93878-296">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="93878-297">Fehler behoben beim Hinzufügen eines Cluster-/Anwendungszertifikats ausschließlich zu VM Scale Sets, die zum Cluster gehören, indem die Cluster-ID in der Erweiterung überprüft wird.</span><span class="sxs-lookup"><span data-stu-id="93878-297">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="93878-298">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="93878-298">Az.SignalR</span></span>
* <span data-ttu-id="93878-299">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-299">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="93878-300">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="93878-300">Az.Sql</span></span>
* <span data-ttu-id="93878-301">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-301">Update incorrect online help URLs</span></span>
* <span data-ttu-id="93878-302">Parameterbeschreibung für den Parameter „LicenseType“ mit möglichen Werten aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-302">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="93878-303">Fehler behoben, bei dem die Aktualisierung der Identität der verwalteten Instanz nicht funktioniert hat, wenn es sich um die einzige aktualisierte Eigenschaft gehandelt hat</span><span class="sxs-lookup"><span data-stu-id="93878-303">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="93878-304">Unterstützung für die benutzerdefinierte Sortierung auf verwalteter Instanz</span><span class="sxs-lookup"><span data-stu-id="93878-304">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="93878-305">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="93878-305">Az.Storage</span></span>
* <span data-ttu-id="93878-306">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-306">Update incorrect online help URLs</span></span>
* <span data-ttu-id="93878-307">Ausführliche Fehlermeldung beim Abrufen/Festlegen der klassischen Protokollierung bzw. Metriken für Storage Premium-Konto, da für das Storage Premium-Konto die klassische Protokollierung bzw. Metriken nicht unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="93878-307">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="93878-308">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="93878-308">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="93878-309">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="93878-309">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="93878-310">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="93878-310">Az.TrafficManager</span></span>
* <span data-ttu-id="93878-311">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-311">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="93878-312">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="93878-312">Az.Websites</span></span>
* <span data-ttu-id="93878-313">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-313">Update incorrect online help URLs</span></span>
* <span data-ttu-id="93878-314">„New-AzWebAppSSLBinding“ korrigiert, damit das Zertifikat in die richtige Ressourcengruppe bzw. an den richtigen Speicherort hochgeladen wird, wenn die App in einer ASE gehostet wird.</span><span class="sxs-lookup"><span data-stu-id="93878-314">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="93878-315">„New-AzWebAppSSLBinding“ korrigiert, damit die Tags beim Binden eines SSL-Zertifikats an eine App nicht überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="93878-315">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="93878-316">1.1.0 – Januar 2019</span><span class="sxs-lookup"><span data-stu-id="93878-316">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="93878-317">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="93878-317">Az.Accounts</span></span>
* <span data-ttu-id="93878-318">Bereich „Local“ zu „Enable-AzureRmAlias“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-318">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="93878-319">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="93878-319">Az.Compute</span></span>
* <span data-ttu-id="93878-320">Name ist jetzt optional im ID-Parametersatz für „Restart/Start/Stop/Remove/Set-AzVM“ und „Save-AzVMImage“</span><span class="sxs-lookup"><span data-stu-id="93878-320">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="93878-321">Beschreibung der ID in Hilfedateien aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-321">Updated the description of ID in help files</span></span>
* <span data-ttu-id="93878-322">Problem mit der Abwärtskompatibilität beim Az.Accounts-Modul behoben</span><span class="sxs-lookup"><span data-stu-id="93878-322">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="93878-323">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="93878-323">Az.DataLakeStore</span></span>
* <span data-ttu-id="93878-324">Aktualisierung der SDK-Version der Datenebene auf 1.1.14 für SDK-Fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="93878-324">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="93878-325">Behandlung von negativen acesstime- and modificationtime-Werten für „getfilestatus“ und „liststatus“ korrigiert, asynchrones Abbruchtoken korrigiert</span><span class="sxs-lookup"><span data-stu-id="93878-325">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="93878-326">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="93878-326">Az.EventGrid</span></span>
* <span data-ttu-id="93878-327">Zur Verwendung der API-Version 2019-01-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-327">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="93878-328">Aktualisierung der folgenden Cmdlets zur Unterstützung des neuen Szenarios in der API-Version 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="93878-328">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="93878-329">New-AzureRmEventGridSubscription: Neue optionale Parameter zum Angeben folgender Werte hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="93878-329">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="93878-330">Gültigkeitsdauer des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="93878-330">Event Time-To-Live,</span></span>
        - <span data-ttu-id="93878-331">Maximale Anzahl von Übermittlungsversuchen für die Ereignisse</span><span class="sxs-lookup"><span data-stu-id="93878-331">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="93878-332">Endpunkt für unzustellbare Nachrichten</span><span class="sxs-lookup"><span data-stu-id="93878-332">Dead letter endpoint.</span></span>
    - <span data-ttu-id="93878-333">Update-AzureRmEventGridSubscription: Neue optionale Parameter zum Angeben folgender Werte hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="93878-333">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="93878-334">Gültigkeitsdauer des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="93878-334">Event Time-To-Live,</span></span>
        - <span data-ttu-id="93878-335">Maximale Anzahl von Übermittlungsversuchen für die Ereignisse</span><span class="sxs-lookup"><span data-stu-id="93878-335">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="93878-336">Endpunkt für unzustellbare Nachrichten</span><span class="sxs-lookup"><span data-stu-id="93878-336">Dead letter endpoint.</span></span>
* <span data-ttu-id="93878-337">Neue Enumerationswerte („storageQueue“ und „hybridConnection“) für die EndpointType-Option in den Cmdlets „New-AzureRmEventGridSubscription“ und „Update-AzureRmEventGridSubscription“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-337">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="93878-338">Anzeige einer Warnmeldung, wenn das Erstellen oder Aktualisieren des Ereignisabonnements voraussichtlich eine manuelle Aktion des Benutzers zur Folge hat</span><span class="sxs-lookup"><span data-stu-id="93878-338">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="93878-339">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="93878-339">Az.IotHub</span></span>
* <span data-ttu-id="93878-340">Auf die aktuelle Version des Iot Hub SDK aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-340">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="93878-341">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="93878-341">Az.LogicApp</span></span>
* <span data-ttu-id="93878-342">„Get-AzLogicApp“ listet alle Apps ohne angegebenen Namen auf</span><span class="sxs-lookup"><span data-stu-id="93878-342">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="93878-343">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="93878-343">Az.Resources</span></span>
* <span data-ttu-id="93878-344">Problem mit dem Parametersatz bei Angabe der Parameter „-ODataQuery“ und „-ResourceId“ für „Get-AzResource“ behoben</span><span class="sxs-lookup"><span data-stu-id="93878-344">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="93878-345">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="93878-345">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="93878-346">Behandlung des Parameters „-Custom“ in „New/Set-AzPolicyDefinition“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="93878-346">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="93878-347">Tippfehler in der Dokumentation für „New-AzDeployment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="93878-347">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="93878-348">Parameter „-MailNickname“ als obligatorisch festgelegt für „New-AzADUser“</span><span class="sxs-lookup"><span data-stu-id="93878-348">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="93878-349">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="93878-349">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="93878-350">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="93878-350">Az.SignalR</span></span>
* <span data-ttu-id="93878-351">Problem mit der Abwärtskompatibilität beim Az.Accounts-Modul behoben</span><span class="sxs-lookup"><span data-stu-id="93878-351">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="93878-352">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="93878-352">Az.Sql</span></span>
* <span data-ttu-id="93878-353">Abhängigkeit des Speicherverwaltungsclients zur allgemeinen SDK-Implementierung konvertiert</span><span class="sxs-lookup"><span data-stu-id="93878-353">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="93878-354">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="93878-354">Az.Storage</span></span>
* <span data-ttu-id="93878-355">Festlegung des „StorageAccountName“ des Speicherkontexts als tatsächlichen Namen des Speicherkontos, wenn dieser mit „SAS-Token“, „OAuth“ oder „Anonym“ erstellt wird</span><span class="sxs-lookup"><span data-stu-id="93878-355">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="93878-356">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="93878-356">New-AzStorageContext</span></span>
* <span data-ttu-id="93878-357">Erstellen von SAS-Token des Blob-Momentaufnahmeobjekts mit dem Parameter „-FullUri“, Festlegung des zurückgegebenen URI als Momentaufnahme-URI</span><span class="sxs-lookup"><span data-stu-id="93878-357">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="93878-358">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="93878-358">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="93878-359">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="93878-359">Az.Websites</span></span>
* <span data-ttu-id="93878-360">Fehler bei der Datumsanalyse in „Get-AzDeletedWebApp“ behoben</span><span class="sxs-lookup"><span data-stu-id="93878-360">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="93878-361">Problem mit der Abwärtskompatibilität beim Az.Accounts-Modul behoben</span><span class="sxs-lookup"><span data-stu-id="93878-361">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="93878-362">1.0.0 – Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="93878-362">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="93878-363">Allgemein</span><span class="sxs-lookup"><span data-stu-id="93878-363">General</span></span>

- <span data-ttu-id="93878-364">Allgemeine Verfügbarkeit des Az-Moduls</span><span class="sxs-lookup"><span data-stu-id="93878-364">General Availability of Az Module</span></span>
- <span data-ttu-id="93878-365">Onlinehilfe für jedes Modul</span><span class="sxs-lookup"><span data-stu-id="93878-365">Online help for each module</span></span>
- <span data-ttu-id="93878-366">Ausführlichere Informationen und eine Roadmap finden Sie auf der [Seite mit der Ankündigung zu Az](https://aka.ms/azps-announce).</span><span class="sxs-lookup"><span data-stu-id="93878-366">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="93878-367">Informationen zur Migration aus AzureRM finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="93878-367">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="93878-368">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="93878-368">Az.Accounts</span></span>
- <span data-ttu-id="93878-369">Geändert von Az.Profile</span><span class="sxs-lookup"><span data-stu-id="93878-369">Changed from Az.Profile</span></span>
- <span data-ttu-id="93878-370">Feste Tabellenformate für Profil- und Kontexttypen</span><span class="sxs-lookup"><span data-stu-id="93878-370">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="93878-371">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="93878-371">Az.ApiManagement</span></span>
- <span data-ttu-id="93878-372">Korrekturen für #7002</span><span class="sxs-lookup"><span data-stu-id="93878-372">Fixes for #7002</span></span>
- <span data-ttu-id="93878-373">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="93878-373">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="93878-374">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="93878-374">Az.Batch</span></span>
- <span data-ttu-id="93878-375">Möglichkeit zum Anzeigen der ausgeführten Version des Azure Batch-Knoten-Agents auf den VMs eines Pools mit der neuen `NodeAgentInformation`-Eigenschaft für `PSComputeNode` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="93878-375">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="93878-376">Der `Caching`-Standardwert für `PSDataDisk` lautet jetzt nicht mehr `None`, sondern `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="93878-376">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="93878-377">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="93878-377">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="93878-378">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="93878-378">Az.Billing</span></span>
- <span data-ttu-id="93878-379">Kombination von Billing-, Consumption- und UsageAggregates-Cmdlets. Ausführliche Informationen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="93878-379">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="93878-380">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="93878-380">Az.CognitivServices</span></span>
- <span data-ttu-id="93878-381">Vervollständigungen für SkuName und Typem für den Vorgang New-AzureRmCognitiveServicesAccount hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-381">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="93878-382">GetSkusWithAccountParamSetName-Parametersatz aus Get-AzCognitiveServicesAccountSkus entfernt</span><span class="sxs-lookup"><span data-stu-id="93878-382">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="93878-383">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="93878-383">Az.ContainerInstance</span></span>
- <span data-ttu-id="93878-384">ManagedIdentity-Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-384">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="93878-385">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="93878-385">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="93878-386">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="93878-386">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="93878-387">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="93878-387">Az.DataLakeStore</span></span>
- <span data-ttu-id="93878-388">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="93878-388">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="93878-389">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="93878-389">Az.Monitor</span></span>
- <span data-ttu-id="93878-390">Az.Insights in Az.Monitor umbenannt und weitere weniger wichtige grundlegende Änderungen durchgeführt. Informationen hierzu finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="93878-390">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="93878-391">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="93878-391">Az.KeyVault</span></span>
- <span data-ttu-id="93878-392">Veraltete PurgeDisabled-Eigenschaft aus Ausgabetypen entfernt</span><span class="sxs-lookup"><span data-stu-id="93878-392">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="93878-393">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="93878-393">Az.MachineLearning</span></span>
- <span data-ttu-id="93878-394">Cmdlets des Az.MachineLearningCompute-Moduls eingebunden</span><span class="sxs-lookup"><span data-stu-id="93878-394">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="93878-395">Az.Media</span><span class="sxs-lookup"><span data-stu-id="93878-395">Az.Media</span></span>
- <span data-ttu-id="93878-396">Veralteten -Tags-Alias aus New-AzMediaService entfernt</span><span class="sxs-lookup"><span data-stu-id="93878-396">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="93878-397">Az.Network</span><span class="sxs-lookup"><span data-stu-id="93878-397">Az.Network</span></span>
<span data-ttu-id="93878-398">Unterstützung für das Konfigurieren von RewriteRuleSets im Application Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-398">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="93878-399">Neu hinzugefügte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="93878-399">New cmdlets added:</span></span>
        - <span data-ttu-id="93878-400">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="93878-400">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="93878-401">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="93878-401">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="93878-402">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="93878-402">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="93878-403">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="93878-403">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="93878-404">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="93878-404">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="93878-405">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="93878-405">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="93878-406">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="93878-406">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="93878-407">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="93878-407">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="93878-408">Cmdlets mit optionalem Parameter -RewriteRuleSet aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-408">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="93878-409">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="93878-409">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="93878-410">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="93878-410">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="93878-411">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="93878-411">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="93878-412">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="93878-412">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="93878-413">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="93878-413">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="93878-414">New-AzureRmApplicationGatewayUrlPathMapConfig: KeyVault-Unterstützung mithilfe von Identität zum Application Gateway hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="93878-414">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="93878-415">Cmdlets mit optionalem Parameter aktualisiert: -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="93878-415">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="93878-416">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="93878-416">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="93878-417">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="93878-417">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="93878-418">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="93878-418">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="93878-419">Cmdlet New-AzApplicationGateway mit optionalem Parameter -UserAssignedIdentity aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-419">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="93878-420">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="93878-420">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="93878-421">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="93878-421">Az.OperationalInsights</span></span>
- <span data-ttu-id="93878-422">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="93878-422">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="93878-423">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="93878-423">Az.Profile</span></span>
- <span data-ttu-id="93878-424">Modulnamen in Az.Accounts geändert</span><span class="sxs-lookup"><span data-stu-id="93878-424">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="93878-425">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="93878-425">Az.RecoveryServices</span></span>
- <span data-ttu-id="93878-426">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="93878-426">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="93878-427">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="93878-427">Az.Resources</span></span>
- <span data-ttu-id="93878-428">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="93878-428">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="93878-429">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="93878-429">Az.ServiceFabric</span></span>
- <span data-ttu-id="93878-430">Unterstützung für das Angeben des Zertifikats anhand des allgemeinen Namens und Fingerabdrucks</span><span class="sxs-lookup"><span data-stu-id="93878-430">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="93878-431">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="93878-431">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="93878-432">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="93878-432">Az.SIgnalR</span></span>
- <span data-ttu-id="93878-433">Allgemeine Verfügbarkeit für PowerShell-Cmdlets für SIgnalR</span><span class="sxs-lookup"><span data-stu-id="93878-433">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="93878-434">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="93878-434">Az.Sql</span></span>
- <span data-ttu-id="93878-435">Neue Erkennungstypen Data_Exfiltration und Unsafe_Action zu Cmdlets für Bedrohungserkennung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-435">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="93878-436">Dokumentationsbeispiele für Cmdlets für SQL-Überwachung aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-436">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="93878-437">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="93878-437">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="93878-438">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="93878-438">Az.Storage</span></span>
- <span data-ttu-id="93878-439">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="93878-439">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="93878-440">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="93878-440">Az.Websites</span></span>
- <span data-ttu-id="93878-441">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="93878-441">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="93878-442">0.7.0 – Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="93878-442">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="93878-443">Allgemein</span><span class="sxs-lookup"><span data-stu-id="93878-443">General</span></span>

* <span data-ttu-id="93878-444">Geringe Änderungen für anstehenden Übergang von AzureRM zu Az</span><span class="sxs-lookup"><span data-stu-id="93878-444">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="93878-445">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="93878-445">Az.Compute</span></span>

* <span data-ttu-id="93878-446">Unterstützung für UltraSSD und Katalogimages in einfachen Parametersätzen für `New-AzVm(ss)`-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="93878-446">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="93878-447">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="93878-447">Az.DataLakeStore</span></span>

* <span data-ttu-id="93878-448">Nachgestellten Schrägstrich für die Domäne des ADLS-Kontos korrigiert</span><span class="sxs-lookup"><span data-stu-id="93878-448">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="93878-449">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="93878-449">Az.FrontDoor</span></span>

* <span data-ttu-id="93878-450">Einige fehlerhafte Links behoben</span><span class="sxs-lookup"><span data-stu-id="93878-450">Fixed some broken links</span></span>
    - <span data-ttu-id="93878-451">In den Artikeln zu New-AzureRmFrontDoor und Set-AzureRmFrontDoor den Artikel-Link zum Cmdlet „New-AzureRmFrontDoorHealthProbeSettingObject“ korrigiert.</span><span class="sxs-lookup"><span data-stu-id="93878-451">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="93878-452">Im Artikel zu New-AzureRmFrontDoorManagedRuleObject den Artikel-Link zum Cmdlet „New-AzureRmFrontDoorRuleGroupOverrideObject“ korrigiert.</span><span class="sxs-lookup"><span data-stu-id="93878-452">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="93878-453">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="93878-453">Az.RecoveryServices</span></span>

* <span data-ttu-id="93878-454">Clientseitige Validierungen für Wiederherstellungsvorgänge von Azure-Dateifreigaben hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="93878-454">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="93878-455">storageAccountName und storageAccountResourceGroupName für AFS-Wiederherstellung optional gemacht.</span><span class="sxs-lookup"><span data-stu-id="93878-455">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="93878-456">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="93878-456">Az.Resources</span></span>

* <span data-ttu-id="93878-457">Fehlerbehebung für https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="93878-457">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="93878-458">Get-AzureRmRoleAssignment für die Verwendung des Abonnementbereichs aktualisiert, wenn dieser beim Anfordern von klassischen Administratoren angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="93878-458">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="93878-459">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="93878-459">Az.Sql</span></span>

* <span data-ttu-id="93878-460">Geringe Änderungen für anstehenden Übergang von AzureRM zu Az</span><span class="sxs-lookup"><span data-stu-id="93878-460">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="93878-461">Problem mit der Verwendung von Get-AzureRmSqlDatabaseVulnerabilityAssessment mit .NET Core behoben</span><span class="sxs-lookup"><span data-stu-id="93878-461">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="93878-462">Dokumentation mit Hilfemeldungen zu Cmdlets für die SQL-Überwachung geändert.</span><span class="sxs-lookup"><span data-stu-id="93878-462">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="93878-463">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="93878-463">Az.Storage</span></span>

* <span data-ttu-id="93878-464">-EnableHierarchicalNamespace zu New-AzureRmStorageAccount hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-464">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="93878-465">Problem behoben, bei dem für das Copy File-Cmdlet am Ziel kein Quellkontext wiederverwendet werden kann, wenn -DestContext nicht eingegeben wird</span><span class="sxs-lookup"><span data-stu-id="93878-465">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="93878-466">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="93878-466">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="93878-467">Unterstützung der Konfiguration von statischen Websites</span><span class="sxs-lookup"><span data-stu-id="93878-467">Support Static Website configuration</span></span>
    - <span data-ttu-id="93878-468">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="93878-468">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="93878-469">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="93878-469">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="93878-470">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="93878-470">Az.Websites</span></span>

* <span data-ttu-id="93878-471">Set-AzureRmWebApp und Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="93878-471">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="93878-472">Neuen Parameter (-AzureStoragePath) zum Angeben von Azure Storage-Pfaden hinzugefügt, die in Windows- und Linux-Container-Apps bereitgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="93878-472">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="93878-473">Verwenden Sie die Ausgabe des neuen Cmdlets New-AzureRmWebAppAzureStoragePath als Parameter zum Festlegen der Azure Storage-Pfade.</span><span class="sxs-lookup"><span data-stu-id="93878-473">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="93878-474">0.6.1 – November 2018</span><span class="sxs-lookup"><span data-stu-id="93878-474">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="93878-475">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="93878-475">Az.ApiManagement</span></span>
* <span data-ttu-id="93878-476">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-476">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="93878-477">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="93878-477">Az.Automation</span></span>
* <span data-ttu-id="93878-478">Swagger-basierte Azure Automation-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="93878-478">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="93878-479">Cmdlets zur Updateverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-479">Added Update Management cmdlets</span></span>
* <span data-ttu-id="93878-480">Cmdlets zur Quellcodeverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-480">Added Source Control cmdlets</span></span>
* <span data-ttu-id="93878-481">Cmdlet „Remove-AzureRmAutomationHybridWorkerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-481">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="93878-482">DSC-Befehl für die Knotenregistrierung korrigiert</span><span class="sxs-lookup"><span data-stu-id="93878-482">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="93878-483">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="93878-483">Az.Compute</span></span>
* <span data-ttu-id="93878-484">Identitätsproblem für SystemAssigned-Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="93878-484">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="93878-485">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-485">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="93878-486">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="93878-486">Az.ContainerInstance</span></span>
* <span data-ttu-id="93878-487">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-487">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="93878-488">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="93878-488">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="93878-489">Beschreibung der Beispiele für Marketplace-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-489">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="93878-490">Az.Network</span><span class="sxs-lookup"><span data-stu-id="93878-490">Az.Network</span></span>
* <span data-ttu-id="93878-491">Folgende Cmdlets hinzugefügt: New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="93878-491">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="93878-492">ICMP wieder unterstützten AzureFirewall-Netzwerkprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-492">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="93878-493">Cmdlet „Test-AzureRmNetworkWatcherConnectivity“ aktualisiert und Überprüfung für Ziel-ID, Adresse und Port hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-493">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="93878-494">Probleme mit Arbeitsspeicherauslastung in der VirtualNetwork-Zuordnung behoben</span><span class="sxs-lookup"><span data-stu-id="93878-494">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="93878-495">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="93878-495">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="93878-496">Problem beim Ändern der Richtlinie für eine geschützte Dateifreigabe behoben</span><span class="sxs-lookup"><span data-stu-id="93878-496">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="93878-497">Richtlinienzeitzone in Großschreibung geändert</span><span class="sxs-lookup"><span data-stu-id="93878-497">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="93878-498">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="93878-498">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="93878-499">Korrigiertes Beispiel in „New-AzureRmRecoveryServicesAsrProtectableItem“</span><span class="sxs-lookup"><span data-stu-id="93878-499">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="93878-500">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-500">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="93878-501">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="93878-501">Az.Relay</span></span>
* <span data-ttu-id="93878-502">Optionaler Parameter „-KeyValue“ zu Cmdlet „New-AzureRmRelayKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht</span><span class="sxs-lookup"><span data-stu-id="93878-502">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="93878-503">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="93878-503">Az.Resources</span></span>
* <span data-ttu-id="93878-504">Hilfedokumentation für ressourcenidentitätsbezogene Parameter in `New-AzureRmPolicyAssignment` und `Set-AzureRmPolicyAssignment` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-504">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="93878-505">Beispiel für „New-AzureRmPolicyDefinition“ hinzugefügt, das „-Metadata“ nutzt</span><span class="sxs-lookup"><span data-stu-id="93878-505">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="93878-506">Korrektur, um Beibehaltung von Groß-/Kleinschreibung in Tagschlüsseln in „NetStandard“ zu ermöglichen: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="93878-506">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="93878-507">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="93878-507">Az.ServiceFabric</span></span>
* <span data-ttu-id="93878-508">Benachrichtigung über veraltete Elemente für anstehende wichtige Änderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-508">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="93878-509">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="93878-509">Az.Sql</span></span>
* <span data-ttu-id="93878-510">Neue Cmdlets für CRUD-Vorgänge in verwalteten Azure SQL-Datenbank-Instanzen und verwalteten Azure SQL-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-510">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="93878-511">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="93878-511">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="93878-512">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="93878-512">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="93878-513">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="93878-513">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="93878-514">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="93878-514">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="93878-515">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="93878-515">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="93878-516">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="93878-516">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="93878-517">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="93878-517">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="93878-518">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="93878-518">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="93878-519">Erweiterte Verwaltung von Überwachungsrichtlinien auf einem Server oder in einer Datenbank aktiviert</span><span class="sxs-lookup"><span data-stu-id="93878-519">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="93878-520">Neuer Parameter (PredicateExpression) hinzugefügt, um die Filterung von Überwachungsprotokollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="93878-520">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="93878-521">Cmdlets wurden angepasst, sodass sie SQL-Clients anstelle von Legacyclients verwenden.</span><span class="sxs-lookup"><span data-stu-id="93878-521">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="93878-522">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="93878-522">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="93878-523">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="93878-523">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="93878-524">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="93878-524">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="93878-525">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="93878-525">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="93878-526">Problem bei Verwendung von „Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings“ mit festgelegtem Parameter für den Speicherkontonamen behoben</span><span class="sxs-lookup"><span data-stu-id="93878-526">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="93878-527">0.5.0 – November 2018</span><span class="sxs-lookup"><span data-stu-id="93878-527">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="93878-528">Allgemein</span><span class="sxs-lookup"><span data-stu-id="93878-528">General</span></span>
* <span data-ttu-id="93878-529">Ressourcenvervollständigungen für viele Kern-Cmdlets hinzugefügt (diese ermöglichen das Durchlaufen von vorhandenen Ressourcennamen per TAB-TASTE, wenn Cmdlets interaktiv aufgerufen werden)</span><span class="sxs-lookup"><span data-stu-id="93878-529">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="93878-530">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="93878-530">Az.Profile</span></span>
* <span data-ttu-id="93878-531">Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="93878-531">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="93878-532">Parameter „TenantId“ im Cmdlet „Connect-AzAccount“ in „Tenant“ umbenannt und Alias für „TenantId“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-532">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="93878-533">Beschreibung von „TenantId“ für „Connect-AzAccount“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="93878-533">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="93878-534">Fehlermeldung für fehlgeschlagene Anmeldung bei Angabe der Mandantendomäne korrigiert</span><span class="sxs-lookup"><span data-stu-id="93878-534">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="93878-535">Problem in Bezug auf Kontextnamenskonflikt für Konten ohne Abonnements im Mandanten behoben</span><span class="sxs-lookup"><span data-stu-id="93878-535">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="93878-536">Problem mit DataLake-Endpunkten bei Verwendung von MSI behoben</span><span class="sxs-lookup"><span data-stu-id="93878-536">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="93878-537">Problem behoben, das zur Auslösung von „Disconnect-AzAccount“ führte, wenn keine Verbindung bestand</span><span class="sxs-lookup"><span data-stu-id="93878-537">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="93878-538">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="93878-538">Az.CognitiveServices</span></span>
* <span data-ttu-id="93878-539">Vorgang „Get-AzCognitiveServicesAccountSkus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-539">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="93878-540">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="93878-540">Az.Compute</span></span>
* <span data-ttu-id="93878-541">Cmdlets Add-AzVmssVMDataDisk und Remove-AzVmssVMDataDisk hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-541">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="93878-542">„Get-AzVMImage“ zeigt „AutomaticOSUpgradeProperties“ an</span><span class="sxs-lookup"><span data-stu-id="93878-542">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="93878-543">Problem behoben, aufgrund dessen die Optionswerte „SetAzVMChefExtension -BootstrapOptions“ und „-JsonAttribute“ nicht im JSON-Format festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="93878-543">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="93878-544">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="93878-544">Az.DataLakeStore</span></span>
* <span data-ttu-id="93878-545">Aktualisierung des DataLake-Pakets auf 1.1.10</span><span class="sxs-lookup"><span data-stu-id="93878-545">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="93878-546">Standardmäßige Parallelität zu Multithreadvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-546">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="93878-547">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="93878-547">Az.Insights</span></span>
* <span data-ttu-id="93878-548">Problem Nr. 7267 behoben (Bereich für automatische Skalierung)</span><span class="sxs-lookup"><span data-stu-id="93878-548">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="93878-549">Probleme beim Erstellen einer neuen Regel für die automatische Skalierung, aufgrund derer die aufgelisteten Parameter nicht richtig festgelegt wurden (Es wurde stets der Standardwert festgelegt.)</span><span class="sxs-lookup"><span data-stu-id="93878-549">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="93878-550">Problem Nr. 7513 behoben [Insights] „Set-AzDiagnosticSetting“ erfordert die explizite Angabe von Kategorien während der Erstellung der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="93878-550">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="93878-551">Nun erfordert das Cmdlet nicht die explizite Angabe der Kategorien, die während der Erstellung aktiviert werden sollen. Das bedeutet, es funktioniert wie dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="93878-551">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="93878-552">Az.Network</span><span class="sxs-lookup"><span data-stu-id="93878-552">Az.Network</span></span>
* <span data-ttu-id="93878-553">„PeeringType“ wurde geändert und ist nun ein erforderlicher Parameter für die folgenden Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="93878-553">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="93878-554">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="93878-554">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="93878-555">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="93878-555">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="93878-556">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="93878-556">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="93878-557">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="93878-557">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="93878-558">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="93878-558">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="93878-559">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="93878-559">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="93878-560">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="93878-560">Az.PolicyInsights</span></span>
* <span data-ttu-id="93878-561">Cmdlets für Richtlinienwartung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-561">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="93878-562">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="93878-562">Az.Resources</span></span>
* <span data-ttu-id="93878-563">Fehlerbehebung für https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="93878-563">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="93878-564">Zulassen der Auflistung von Ressourcen mithilfe des Parameters „-ResourceId“ für „Get-AzResource“</span><span class="sxs-lookup"><span data-stu-id="93878-564">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="93878-565">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="93878-565">Az.ServiceBus</span></span>
* <span data-ttu-id="93878-566">Schreibgeschützte Eigenschaft „MigrationState“ zu „PSServiceBusMigrationConfigurationAttributes“ hinzugefügt, was das Ermitteln des Migrationsstatus ermöglicht</span><span class="sxs-lookup"><span data-stu-id="93878-566">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="93878-567">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="93878-567">Az.ServiceFabric</span></span>
* <span data-ttu-id="93878-568">Hinzufügen des Zertifikats zu Linux VMSS korrigiert</span><span class="sxs-lookup"><span data-stu-id="93878-568">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="93878-569">„Add-AzServiceFabricClusterCertificate“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="93878-569">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="93878-570">Verwenden des richtigen Fingerabdrucks aus dem neuen Zertifikat (Azure/service-fabric-issues#932)</span><span class="sxs-lookup"><span data-stu-id="93878-570">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="93878-571">Richtige Anzeige von Ausnahmen (Azure/service-fabric-issues#1054)</span><span class="sxs-lookup"><span data-stu-id="93878-571">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="93878-572">„Update-AzServiceFabricDurability“ korrigiert, um die Clusterkonfiguration zu aktualisieren, bevor der VMSS-Vorgang „CreateOrUpdate“ gestartet wird</span><span class="sxs-lookup"><span data-stu-id="93878-572">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="93878-573">0.4.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="93878-573">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="93878-574">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="93878-574">Az.Profile</span></span>
* <span data-ttu-id="93878-575">Problem mit „Get-AzSubscription“ in Cloud Shell behoben</span><span class="sxs-lookup"><span data-stu-id="93878-575">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="93878-576">Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="93878-576">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="93878-577">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="93878-577">Az.Compute</span></span>
* <span data-ttu-id="93878-578">Neue Größen zur Whitelist von VM-Größen hinzugefügt, für die bei Verwendung des einfachen Parametersatzes für „New-AzVm“ der beschleunigte Netzwerkbetrieb aktiviert wird</span><span class="sxs-lookup"><span data-stu-id="93878-578">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="93878-579">ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="93878-579">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="93878-580">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="93878-580">Az.DataLakeStore</span></span>
* <span data-ttu-id="93878-581">Unterstützung für Regeln für virtuelle Netzwerke hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-581">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="93878-582">Get-AzDataLakeStoreVirtualNetworkRule: Dient zum Abrufen oder Auflisten der Azure Data Lake Store-Regel für das virtuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="93878-582">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="93878-583">Add-AzDataLakeStoreVirtualNetworkRule: Fügt dem angegebenen Data Lake Store-Konto eine Regel für das virtuelle Netzwerk hinzu.</span><span class="sxs-lookup"><span data-stu-id="93878-583">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="93878-584">Set-AzDataLakeStoreVirtualNetworkRule: Ändert die angegebene Regel für das virtuelle Netzwerk in das angegebene Data Lake Store-Konto.</span><span class="sxs-lookup"><span data-stu-id="93878-584">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="93878-585">Remove-AzDataLakeStoreVirtualNetworkRule: Dient zum Löschen der Azure Data Lake Store-Regel für das virtuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="93878-585">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="93878-586">Az.Network</span><span class="sxs-lookup"><span data-stu-id="93878-586">Az.Network</span></span>
* <span data-ttu-id="93878-587">Cmdlet „Test-AzNetworkWatcherConnectivity“ aktualisiert, Protokollwert wird jetzt an Back-End übergeben.</span><span class="sxs-lookup"><span data-stu-id="93878-587">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="93878-588">ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="93878-588">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="93878-589">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="93878-589">Az.Resources</span></span>
* <span data-ttu-id="93878-590">Problem behoben, aufgrund dessen „Get-AzRoleDefinition“ eine unverständliche Ausnahme auslöst (wenn das Standardprofil kein Abonnement enthält und kein Bereich festgelegt ist), indem im Szenario eine aussagekräftige Ausnahme hinzugefügt wurde.</span><span class="sxs-lookup"><span data-stu-id="93878-590">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="93878-591">Außerdem wurde der Standardparametersatz auf „RoleDefinitionNameParameterSet“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="93878-591">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="93878-592">0.3.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="93878-592">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="93878-593">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="93878-593">Azure.Storage</span></span>
* <span data-ttu-id="93878-594">Fehler beim Kopieren von Blobs/Dateien behoben, aufgrund dessen bei einem Metadatenproblem des Ziels keine Metadaten kopiert wurden</span><span class="sxs-lookup"><span data-stu-id="93878-594">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="93878-595">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="93878-595">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="93878-596">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="93878-596">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="93878-597">Der Abruf der Speicherressourcennutzung eines bestimmten Standorts wird jetzt unterstützt, und das Hinzufügen einer Warnmeldung für den Abruf der globalen Speicherressourcennutzung ist überflüssig.</span><span class="sxs-lookup"><span data-stu-id="93878-597">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="93878-598">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="93878-598">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="93878-599">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="93878-599">Az.CognitiveServices</span></span>
* <span data-ttu-id="93878-600">„Get-AzCognitiveServicesAccountSkus“ wird ohne vorhandenes Konto unterstützt.</span><span class="sxs-lookup"><span data-stu-id="93878-600">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="93878-601">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="93878-601">Az.Compute</span></span>
* <span data-ttu-id="93878-602">Korrektur von „Get-AzVM -ResourceGroupName <rg>“, sodass ggf. mehr als 50 Ergebnisse zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="93878-602">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="93878-603">Der Cmdlet-Hilfe zu „New-AzVmss“ wurde ein Beispiel für „SimpleParameterSet“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="93878-603">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="93878-604">Tippfehler in der Azure Disk Encryption-Statusmeldung behoben</span><span class="sxs-lookup"><span data-stu-id="93878-604">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="93878-605">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="93878-605">Az.DataFactoryV2</span></span>
* <span data-ttu-id="93878-606">Die Version des ADF .Net-SDK wurde auf 2.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="93878-606">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="93878-607">Az.Network</span><span class="sxs-lookup"><span data-stu-id="93878-607">Az.Network</span></span>
* <span data-ttu-id="93878-608">NetworkProfile-Funktionalität wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="93878-608">Added NetworkProfile functionality.</span></span> <span data-ttu-id="93878-609">Neue Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-609">new cmdlets added</span></span>
    - <span data-ttu-id="93878-610">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="93878-610">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="93878-611">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="93878-611">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="93878-612">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="93878-612">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="93878-613">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="93878-613">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="93878-614">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="93878-614">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="93878-615">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="93878-615">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="93878-616">Dienstzuordnungslink in Subnetzmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-616">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="93878-617">Cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-617">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="93878-618">Cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-618">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="93878-619">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="93878-619">Az.RedisCache</span></span>
* <span data-ttu-id="93878-620">Künftig sind beliebige Zeichenfolgen als Größenparameter zulässig.</span><span class="sxs-lookup"><span data-stu-id="93878-620">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="93878-621">P5 in Popup „PSArgumentCompleter“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-621">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="93878-622">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="93878-622">Az.Resources</span></span>
* <span data-ttu-id="93878-623">Fehlender Parameter „-Mode“ zu „Set-AzPolicyDefinition“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="93878-623">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="93878-624">Cmdlet-Fehler bei „Get-AzProviderOperation“ für Vorgänge mit Ursprung behoben, der den Benutzer enthält</span><span class="sxs-lookup"><span data-stu-id="93878-624">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="93878-625">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="93878-625">Az.Sql</span></span>
* <span data-ttu-id="93878-626">Problem behoben, aufgrund dessen einige Sicherungs-Cmdlets das aktuelle Azure-Abonnements nicht erkannt haben</span><span class="sxs-lookup"><span data-stu-id="93878-626">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="93878-627">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="93878-627">Az.Websites</span></span>
* <span data-ttu-id="93878-628">Neues Cmdlet „Get-AzWebAppContainerContinuousDeploymentUrl“ zum Abrufen der Webhook-URL von Continuous Deployment für Container</span><span class="sxs-lookup"><span data-stu-id="93878-628">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="93878-629">Neue Cmdlets „New-AzWebAppContainerPSSession“ und „Enter-WebAppContainerPSSession“ zum Initiieren einer PowerShell-Remotesitzung in einer Windows-Container-App</span><span class="sxs-lookup"><span data-stu-id="93878-629">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="93878-630">0.2.0 – September 2018</span><span class="sxs-lookup"><span data-stu-id="93878-630">0.2.0 - September 2018</span></span>
 <span data-ttu-id="93878-631">Erste Version</span><span class="sxs-lookup"><span data-stu-id="93878-631">Initial Release</span></span>