---
ms.openlocfilehash: 9915ff37e59a73c1d226a216213fd9016b55d3d4
ms.sourcegitcommit: 447276d46ffeeb37f0c07a570536665e36c5ddb8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "57882299"
---
## <a name="150---march-2019"></a><span data-ttu-id="cde94-101">1.5.0: März 2019</span><span class="sxs-lookup"><span data-stu-id="cde94-101">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cde94-102">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cde94-102">Az.Accounts</span></span>
* <span data-ttu-id="cde94-103">Der Befehl „Register-AzModule“ wurde hinzugefügt, um von AutoRest generierte Cmdlets zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="cde94-103">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="cde94-104">Beispiele für „Connect-AzAccount“ wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="cde94-104">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cde94-105">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cde94-105">Az.Automation</span></span>
* <span data-ttu-id="cde94-106">Problem behoben, das beim Abrufen bestimmter monatlicher Zeitpläne in verschiedenen Azure Automation-Cmdlets auftrat</span><span class="sxs-lookup"><span data-stu-id="cde94-106">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="cde94-107">„Get-AzAutomationDscNode“ wurde korrigiert, da nur die 20 obersten Knoten zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="cde94-107">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="cde94-108">Jetzt werden alle Knoten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cde94-108">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="cde94-109">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="cde94-109">Az.Cdn</span></span>
* <span data-ttu-id="cde94-110">Neue Powershell-Cmdlets zum Aktivieren/Deaktivieren von HTTPS für benutzerdefinierte Domänen hinzugefügt und alte Cmdlets außer Betrieb genommen</span><span class="sxs-lookup"><span data-stu-id="cde94-110">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cde94-111">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cde94-111">Az.Compute</span></span>
* <span data-ttu-id="cde94-112">Unterstützung für Platzhalterzeichen zu Get-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-112">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cde94-113">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cde94-113">Az.DataFactory</span></span>
* <span data-ttu-id="cde94-114">Version des ADF .NET SDK auf 3.0.1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-114">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="cde94-115">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="cde94-115">Az.LogicApp</span></span>
* <span data-ttu-id="cde94-116">„ListWorkflows“ wurde korrigiert, da nur die erste Seite mit Ergebnissen abgerufen wurde.</span><span class="sxs-lookup"><span data-stu-id="cde94-116">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cde94-117">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cde94-117">Az.Network</span></span>
* <span data-ttu-id="cde94-118">Unterstützung für Platzhalterzeichen zu Network-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-118">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cde94-119">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cde94-119">Az.RecoveryServices</span></span>
* <span data-ttu-id="cde94-120">SQL Server jetzt in Azure-VM-Support enthalten</span><span class="sxs-lookup"><span data-stu-id="cde94-120">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="cde94-121">SDK-Update</span><span class="sxs-lookup"><span data-stu-id="cde94-121">SDK Update</span></span>
* <span data-ttu-id="cde94-122">VMappContainer-Überprüfung in „Get-ProtectableItem“ entfernt</span><span class="sxs-lookup"><span data-stu-id="cde94-122">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="cde94-123">„Name“ und „ServerName“ als Parameter für „Get-ProtectableItem“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-123">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="cde94-124">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cde94-124">Az.Resources</span></span>
* <span data-ttu-id="cde94-125">Parameter `-TemplateObject` zu Bereitstellungs-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-125">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="cde94-126">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="cde94-126">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="cde94-127">Problem beim Piping des Ergebnisses von `Get-AzResource` an `Set-AzResource` behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-127">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="cde94-128">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="cde94-128">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="cde94-129">Problem mit JSON-Datentypänderung beim Ausführen von `Set-AzResource` behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-129">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="cde94-130">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="cde94-130">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="cde94-131">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cde94-131">Az.Sql</span></span>
* <span data-ttu-id="cde94-132">„AuditingEndpointsCommunicator“ wird aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="cde94-132">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="cde94-133">Das Verhalten eines Grenzfalls beim Erstellen neuer Diagnoseeinstellungen wurde korrigiert.</span><span class="sxs-lookup"><span data-stu-id="cde94-133">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cde94-134">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cde94-134">Az.Storage</span></span>
* <span data-ttu-id="cde94-135">Unterstützung von „Kind BlockBlobStorage“ beim Erstellen eines Speicherkontos: New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="cde94-135">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="cde94-136">1.4.0 – Februar 2019</span><span class="sxs-lookup"><span data-stu-id="cde94-136">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="cde94-137">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="cde94-137">Az.AnalysisServices</span></span>
* <span data-ttu-id="cde94-138">Cmdlet „AddAzureASAccount“ als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="cde94-138">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cde94-139">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cde94-139">Az.Automation</span></span>
* <span data-ttu-id="cde94-140">Hilfe für „Import-AzAutomationDscNodeConfiguration“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-140">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="cde94-141">Überprüfung des Konfigurationsnamens zu Cmdlet „Import-AzAutomationDscConfiguration“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-141">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="cde94-142">Fehlerbehandlung für Cmdlet „Import-AzAutomationDscConfiguration“ verbessert</span><span class="sxs-lookup"><span data-stu-id="cde94-142">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="cde94-143">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="cde94-143">Az.CognitiveServices</span></span>
* <span data-ttu-id="cde94-144">„CustomSubdomainName“ als neuer optionaler Parameter für Cmdlet „New-AzCognitiveServicesAccount“ hinzugefügt, das zum Angeben der Unterdomäne für die Ressource verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="cde94-144">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cde94-145">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cde94-145">Az.Compute</span></span>
* <span data-ttu-id="cde94-146">Problem mit ID-Parametersätzen behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-146">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="cde94-147">„Get-AzVMExtension“ aktualisiert, sodass alle installierten Erweiterungen aufgelistet werden, wenn der Name-Parameter nicht angegeben ist</span><span class="sxs-lookup"><span data-stu-id="cde94-147">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="cde94-148">Parameter „Tag“ und „ResourceId“ zum Cmdlet „Update-AzImage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-148">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="cde94-149">„Get-AzVmssVM“ ohne Instanz-ID und mit „InstanceView“ können virtuelle VMSS-Computer mit Instanzansicht auflisten.</span><span class="sxs-lookup"><span data-stu-id="cde94-149">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cde94-150">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cde94-150">Az.DataLakeStore</span></span>
* <span data-ttu-id="cde94-151">Cmdlets zum Auflisten und Wiederherstellen gelöschter ADL-Elemente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-151">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="cde94-152">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="cde94-152">Az.EventHub</span></span>
* <span data-ttu-id="cde94-153">Neue boolesche Eigenschaft „SkipEmptyArchives“ zum Überspringen leerer Archive in Klasse „CaptureDescription“ von EventHub hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-153">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="cde94-154">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cde94-154">Az.KeyVault</span></span>
* <span data-ttu-id="cde94-155">Kennzeichnung in „Set-AzKeyVaultSecret“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="cde94-155">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="cde94-156">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="cde94-156">Az.LogicApp</span></span>
* <span data-ttu-id="cde94-157">SKU „Basic“ für Integrationskonten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-157">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="cde94-158">XSLT 2.0, XSLT 3.0 und Liquid-Zuordnungstypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-158">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="cde94-159">Neue Cmdlets für Integrationskonto-Assemblys</span><span class="sxs-lookup"><span data-stu-id="cde94-159">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="cde94-160">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="cde94-160">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="cde94-161">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="cde94-161">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="cde94-162">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="cde94-162">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="cde94-163">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="cde94-163">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="cde94-164">Neue Cmdlets für Integrationskonto-Batchkonfiguration</span><span class="sxs-lookup"><span data-stu-id="cde94-164">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="cde94-165">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="cde94-165">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="cde94-166">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="cde94-166">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="cde94-167">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="cde94-167">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="cde94-168">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="cde94-168">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="cde94-169">Logik-App-SDK auf Version 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-169">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="cde94-170">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="cde94-170">Az.Monitor</span></span>
* <span data-ttu-id="cde94-171">Hilfe für „Get-AzMetric“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-171">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cde94-172">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cde94-172">Az.Network</span></span>
* <span data-ttu-id="cde94-173">Hilfebeispiel für „Add-AzApplicationGatewayCustomError“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-173">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="cde94-174">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="cde94-174">Az.OperationalInsights</span></span>
* <span data-ttu-id="cde94-175">Zusätzliche Unterstützung für Datenquelle von „New-ApplicationInsights“ und „Get-ApplicationInsights“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="cde94-175">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="cde94-176">Neue Art von „ApplicationInsights“ zum Abrufen von bestimmten und von allen ApplicationInsights-Datenquellen für einen Workspace hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="cde94-176">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="cde94-177">Cmdlet „New-AzOperationalInsightsApplicationInsightsDataSource“ zum Erstellen einer Datenquelle anhand des angegebenen Ressourcenparameters für „Application-Insights“ hinzugefügt: „subscriptionId“, „resourceGroupName“ und „name“.</span><span class="sxs-lookup"><span data-stu-id="cde94-177">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="cde94-178">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cde94-178">Az.Resources</span></span>
* <span data-ttu-id="cde94-179">Behebung des Problems: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="cde94-179">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="cde94-180">Behebung des Problems: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="cde94-180">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="cde94-181">Behebung des Problems: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="cde94-181">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="cde94-182">Fehler korrigiert, der die wiederholte Erstellung von „KeyCredentials“ verhindert</span><span class="sxs-lookup"><span data-stu-id="cde94-182">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="cde94-183">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cde94-183">Az.Sql</span></span>
* <span data-ttu-id="cde94-184">Unterstützung für SQL DB Hyperscale-Tarif hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-184">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="cde94-185">Fehler korrigiert, aufgrund dessen die Wiederherstellung wegen der Festlegung unnötiger Eigenschaften in der Wiederherstellungsanforderung fehlschlagen konnte</span><span class="sxs-lookup"><span data-stu-id="cde94-185">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cde94-186">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cde94-186">Az.Websites</span></span>
* <span data-ttu-id="cde94-187">Beispiel in „Get-AzWebAppSlotMetrics“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="cde94-187">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="cde94-188">1.3.0: Februar 2019</span><span class="sxs-lookup"><span data-stu-id="cde94-188">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cde94-189">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cde94-189">Az.Accounts</span></span>
* <span data-ttu-id="cde94-190">Update auf die aktuelle Version von ClientRuntime durchgeführt</span><span class="sxs-lookup"><span data-stu-id="cde94-190">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="cde94-191">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="cde94-191">Az.AnalysisServices</span></span>
<span data-ttu-id="cde94-192">Allgemeine Verfügbarkeit für Az.AnalysisServices-Modul</span><span class="sxs-lookup"><span data-stu-id="cde94-192">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cde94-193">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cde94-193">Az.Compute</span></span>
* <span data-ttu-id="cde94-194">AEM-Erweiterung: Unterstützung für UltraSSD und P60-, P70- und P80-Datenträger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-194">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="cde94-195">Hilfebeschreibung für „Set-AzVMBootDiagnostics“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-195">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="cde94-196">Hilfebeschreibung und Beispiel für „Update-AzImage“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-196">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cde94-197">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cde94-197">Az.RecoveryServices</span></span>
<span data-ttu-id="cde94-198">Allgemeine Verfügbarkeit für Az.RecoveryServices-Modul.</span><span class="sxs-lookup"><span data-stu-id="cde94-198">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="cde94-199">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cde94-199">Az.Resources</span></span>
* <span data-ttu-id="cde94-200">Kennzeichnung für Ressourcengruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="cde94-200">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="cde94-201">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="cde94-201">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="cde94-202">Problem behoben, bei dem „-ErrorAction“ von `Get-AzureRmRoleAssignment` nicht berücksichtigt wird</span><span class="sxs-lookup"><span data-stu-id="cde94-202">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="cde94-203">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="cde94-203">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="cde94-204">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cde94-204">Az.Sql</span></span>
* <span data-ttu-id="cde94-205">Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-205">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="cde94-206">Problem behoben, bei dem eine fehlende Anmeldung am Azure-Konto bei der Ausführung von SQL-Cmdlets zu einer nullref-Ausnahme führt</span><span class="sxs-lookup"><span data-stu-id="cde94-206">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="cde94-207">nullref-Ausnahme in Get-AzSqlCapability korrigiert</span><span class="sxs-lookup"><span data-stu-id="cde94-207">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="cde94-208">1.2.1: Januar 2019</span><span class="sxs-lookup"><span data-stu-id="cde94-208">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cde94-209">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cde94-209">Az.Accounts</span></span>
* <span data-ttu-id="cde94-210">Release mit richtiger Version der Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="cde94-210">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="cde94-211">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="cde94-211">Az.AnalysisServices</span></span>
* <span data-ttu-id="cde94-212">Release mit aktualisierter Authentifizierungsabhängigkeit</span><span class="sxs-lookup"><span data-stu-id="cde94-212">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cde94-213">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cde94-213">Az.RecoveryServices</span></span>
* <span data-ttu-id="cde94-214">Release mit aktualisierter Authentifizierungsabhängigkeit</span><span class="sxs-lookup"><span data-stu-id="cde94-214">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="cde94-215">1.2.0: Januar 2019</span><span class="sxs-lookup"><span data-stu-id="cde94-215">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cde94-216">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cde94-216">Az.Accounts</span></span>
* <span data-ttu-id="cde94-217">Interaktive und Benutzername/Kennwort-Authentifizierung ausschließlich für Windows PowerShell 5.1 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-217">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="cde94-218">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-218">Update incorrect online help URLs</span></span>
* <span data-ttu-id="cde94-219">Warnmeldung in PS Core für „Uninstall-AzureRm“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-219">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="cde94-220">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="cde94-220">Az.Aks</span></span>
* <span data-ttu-id="cde94-221">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-221">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cde94-222">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cde94-222">Az.Automation</span></span>
* <span data-ttu-id="cde94-223">Unterstützung für Python 2-Runbooks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-223">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="cde94-224">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-224">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="cde94-225">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="cde94-225">Az.Cdn</span></span>
* <span data-ttu-id="cde94-226">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-226">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cde94-227">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cde94-227">Az.Compute</span></span>
* <span data-ttu-id="cde94-228">Cmdlet „Invoke-AzVMReimage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-228">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="cde94-229">Parameter „TempDisk“ zu „Set-AzVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-229">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="cde94-230">Warnmeldung von „New-AzVM“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="cde94-230">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="cde94-231">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="cde94-231">Az.ContainerRegistry</span></span>
* <span data-ttu-id="cde94-232">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-232">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cde94-233">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cde94-233">Az.DataFactory</span></span>
* <span data-ttu-id="cde94-234">Version des ADF .NET SDK auf 3.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-234">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cde94-235">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cde94-235">Az.DataLakeStore</span></span>
* <span data-ttu-id="cde94-236">Problem mit ADLS-Endpunkt bei Verwendung von MSI behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-236">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="cde94-237">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="cde94-237">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="cde94-238">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-238">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="cde94-239">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="cde94-239">Az.IotHub</span></span>
* <span data-ttu-id="cde94-240">Codierungsformat zu Cmdlet „Add-IotHubRoutingEndpoint“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-240">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="cde94-241">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cde94-241">Az.KeyVault</span></span>
* <span data-ttu-id="cde94-242">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-242">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cde94-243">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cde94-243">Az.Network</span></span>
* <span data-ttu-id="cde94-244">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-244">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="cde94-245">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cde94-245">Az.Resources</span></span>
* <span data-ttu-id="cde94-246">Fehlerhafte Beispiele in Referenzdokumentation zu „New-AzADAppCredential“ und „New-AzADSpCredential“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="cde94-246">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="cde94-247">Problem behoben, bei dem der Pfad für den Parameter „-TemplateFile“ nicht aufgelöst wurde, bevor Cmdlets für die Bereitstellung von Ressourcengruppen ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="cde94-247">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="cde94-248">Az.Resources: Richtige Dokumentation für Standardwert von „New-AzureRmPolicyDefinition -Mode“ bereitgestellt</span><span class="sxs-lookup"><span data-stu-id="cde94-248">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="cde94-249">Az.Resources: Behebung des Problems: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="cde94-249">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="cde94-250">Az.Resources: Behebung des Problems: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="cde94-250">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="cde94-251">Formatierungsproblem für Objekt „PSResourceGroupDeployment“ behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-251">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="cde94-252">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="cde94-252">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="cde94-253">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cde94-253">Az.ServiceFabric</span></span>
* <span data-ttu-id="cde94-254">Rollback beim Hinzufügen eines Zertifikats zum VMSS-Modell, Auslösung einer Ausnahme. Fehlerbehebung: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="cde94-254">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="cde94-255">Einige Fehlermeldungen wurden korrigiert.</span><span class="sxs-lookup"><span data-stu-id="cde94-255">Fix some error messages.</span></span>
* <span data-ttu-id="cde94-256">Fehler bei Clustererstellung mit ARM-Standardvorlage für „New-AzServiceFabriCluster“ behoben, bei dem die Migration zu Az nicht funktioniert hat.</span><span class="sxs-lookup"><span data-stu-id="cde94-256">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="cde94-257">Fehler behoben beim Hinzufügen eines Cluster-/Anwendungszertifikats ausschließlich zu VM Scale Sets, die zum Cluster gehören, indem die Cluster-ID in der Erweiterung überprüft wird.</span><span class="sxs-lookup"><span data-stu-id="cde94-257">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="cde94-258">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="cde94-258">Az.SignalR</span></span>
* <span data-ttu-id="cde94-259">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-259">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="cde94-260">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cde94-260">Az.Sql</span></span>
* <span data-ttu-id="cde94-261">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-261">Update incorrect online help URLs</span></span>
* <span data-ttu-id="cde94-262">Parameterbeschreibung für den Parameter „LicenseType“ mit möglichen Werten aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-262">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="cde94-263">Fehler behoben, bei dem die Aktualisierung der Identität der verwalteten Instanz nicht funktioniert hat, wenn es sich um die einzige aktualisierte Eigenschaft gehandelt hat</span><span class="sxs-lookup"><span data-stu-id="cde94-263">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="cde94-264">Unterstützung für die benutzerdefinierte Sortierung auf verwalteter Instanz</span><span class="sxs-lookup"><span data-stu-id="cde94-264">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cde94-265">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cde94-265">Az.Storage</span></span>
* <span data-ttu-id="cde94-266">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-266">Update incorrect online help URLs</span></span>
* <span data-ttu-id="cde94-267">Ausführliche Fehlermeldung beim Abrufen/Festlegen der klassischen Protokollierung bzw. Metriken für Storage Premium-Konto, da für das Storage Premium-Konto die klassische Protokollierung bzw. Metriken nicht unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="cde94-267">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="cde94-268">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="cde94-268">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="cde94-269">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="cde94-269">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="cde94-270">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="cde94-270">Az.TrafficManager</span></span>
* <span data-ttu-id="cde94-271">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-271">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cde94-272">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cde94-272">Az.Websites</span></span>
* <span data-ttu-id="cde94-273">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-273">Update incorrect online help URLs</span></span>
* <span data-ttu-id="cde94-274">„New-AzWebAppSSLBinding“ korrigiert, damit das Zertifikat in die richtige Ressourcengruppe bzw. an den richtigen Speicherort hochgeladen wird, wenn die App in einer ASE gehostet wird.</span><span class="sxs-lookup"><span data-stu-id="cde94-274">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="cde94-275">„New-AzWebAppSSLBinding“ korrigiert, damit die Tags beim Binden eines SSL-Zertifikats an eine App nicht überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="cde94-275">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="cde94-276">1.1.0 – Januar 2019</span><span class="sxs-lookup"><span data-stu-id="cde94-276">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cde94-277">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cde94-277">Az.Accounts</span></span>
* <span data-ttu-id="cde94-278">Bereich „Local“ zu „Enable-AzureRmAlias“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-278">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cde94-279">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cde94-279">Az.Compute</span></span>
* <span data-ttu-id="cde94-280">Name ist jetzt optional im ID-Parametersatz für „Restart/Start/Stop/Remove/Set-AzVM“ und „Save-AzVMImage“</span><span class="sxs-lookup"><span data-stu-id="cde94-280">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="cde94-281">Beschreibung der ID in Hilfedateien aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-281">Updated the description of ID in help files</span></span>
* <span data-ttu-id="cde94-282">Problem mit der Abwärtskompatibilität beim Az.Accounts-Modul behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-282">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cde94-283">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cde94-283">Az.DataLakeStore</span></span>
* <span data-ttu-id="cde94-284">Aktualisierung der SDK-Version der Datenebene auf 1.1.14 für SDK-Fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="cde94-284">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="cde94-285">Behandlung von negativen acesstime- and modificationtime-Werten für „getfilestatus“ und „liststatus“ korrigiert, asynchrones Abbruchtoken korrigiert</span><span class="sxs-lookup"><span data-stu-id="cde94-285">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="cde94-286">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="cde94-286">Az.EventGrid</span></span>
* <span data-ttu-id="cde94-287">Zur Verwendung der API-Version 2019-01-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-287">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="cde94-288">Aktualisierung der folgenden Cmdlets zur Unterstützung des neuen Szenarios in der API-Version 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="cde94-288">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="cde94-289">New-AzureRmEventGridSubscription: Neue optionale Parameter zum Angeben folgender Werte hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="cde94-289">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="cde94-290">Gültigkeitsdauer des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="cde94-290">Event Time-To-Live,</span></span>
        - <span data-ttu-id="cde94-291">Maximale Anzahl von Übermittlungsversuchen für die Ereignisse</span><span class="sxs-lookup"><span data-stu-id="cde94-291">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="cde94-292">Endpunkt für unzustellbare Nachrichten</span><span class="sxs-lookup"><span data-stu-id="cde94-292">Dead letter endpoint.</span></span>
    - <span data-ttu-id="cde94-293">Update-AzureRmEventGridSubscription: Neue optionale Parameter zum Angeben folgender Werte hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="cde94-293">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="cde94-294">Gültigkeitsdauer des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="cde94-294">Event Time-To-Live,</span></span>
        - <span data-ttu-id="cde94-295">Maximale Anzahl von Übermittlungsversuchen für die Ereignisse</span><span class="sxs-lookup"><span data-stu-id="cde94-295">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="cde94-296">Endpunkt für unzustellbare Nachrichten</span><span class="sxs-lookup"><span data-stu-id="cde94-296">Dead letter endpoint.</span></span>
* <span data-ttu-id="cde94-297">Neue Enumerationswerte („storageQueue“ und „hybridConnection“) für die EndpointType-Option in den Cmdlets „New-AzureRmEventGridSubscription“ und „Update-AzureRmEventGridSubscription“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-297">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="cde94-298">Anzeige einer Warnmeldung, wenn das Erstellen oder Aktualisieren des Ereignisabonnements voraussichtlich eine manuelle Aktion des Benutzers zur Folge hat</span><span class="sxs-lookup"><span data-stu-id="cde94-298">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="cde94-299">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="cde94-299">Az.IotHub</span></span>
* <span data-ttu-id="cde94-300">Auf die aktuelle Version des Iot Hub SDK aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-300">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="cde94-301">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="cde94-301">Az.LogicApp</span></span>
* <span data-ttu-id="cde94-302">„Get-AzLogicApp“ listet alle Apps ohne angegebenen Namen auf</span><span class="sxs-lookup"><span data-stu-id="cde94-302">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="cde94-303">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cde94-303">Az.Resources</span></span>
* <span data-ttu-id="cde94-304">Problem mit dem Parametersatz bei Angabe der Parameter „-ODataQuery“ und „-ResourceId“ für „Get-AzResource“ behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-304">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="cde94-305">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="cde94-305">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="cde94-306">Behandlung des Parameters „-Custom“ in „New/Set-AzPolicyDefinition“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="cde94-306">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="cde94-307">Tippfehler in der Dokumentation für „New-AzDeployment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="cde94-307">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="cde94-308">Parameter „-MailNickname“ als obligatorisch festgelegt für „New-AzADUser“</span><span class="sxs-lookup"><span data-stu-id="cde94-308">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="cde94-309">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="cde94-309">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="cde94-310">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="cde94-310">Az.SignalR</span></span>
* <span data-ttu-id="cde94-311">Problem mit der Abwärtskompatibilität beim Az.Accounts-Modul behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-311">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="cde94-312">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cde94-312">Az.Sql</span></span>
* <span data-ttu-id="cde94-313">Abhängigkeit des Speicherverwaltungsclients zur allgemeinen SDK-Implementierung konvertiert</span><span class="sxs-lookup"><span data-stu-id="cde94-313">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cde94-314">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cde94-314">Az.Storage</span></span>
* <span data-ttu-id="cde94-315">Festlegung des „StorageAccountName“ des Speicherkontexts als tatsächlichen Namen des Speicherkontos, wenn dieser mit „SAS-Token“, „OAuth“ oder „Anonym“ erstellt wird</span><span class="sxs-lookup"><span data-stu-id="cde94-315">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="cde94-316">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="cde94-316">New-AzStorageContext</span></span>
* <span data-ttu-id="cde94-317">Erstellen von SAS-Token des Blob-Momentaufnahmeobjekts mit dem Parameter „-FullUri“, Festlegung des zurückgegebenen URI als Momentaufnahme-URI</span><span class="sxs-lookup"><span data-stu-id="cde94-317">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="cde94-318">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="cde94-318">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cde94-319">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cde94-319">Az.Websites</span></span>
* <span data-ttu-id="cde94-320">Fehler bei der Datumsanalyse in „Get-AzDeletedWebApp“ behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-320">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="cde94-321">Problem mit der Abwärtskompatibilität beim Az.Accounts-Modul behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-321">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="cde94-322">1.0.0 – Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="cde94-322">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="cde94-323">Allgemein</span><span class="sxs-lookup"><span data-stu-id="cde94-323">General</span></span>

- <span data-ttu-id="cde94-324">Allgemeine Verfügbarkeit des Az-Moduls</span><span class="sxs-lookup"><span data-stu-id="cde94-324">General Availability of Az Module</span></span>
- <span data-ttu-id="cde94-325">Onlinehilfe für jedes Modul</span><span class="sxs-lookup"><span data-stu-id="cde94-325">Online help for each module</span></span>
- <span data-ttu-id="cde94-326">Ausführlichere Informationen und eine Roadmap finden Sie auf der [Seite mit der Ankündigung zu Az](https://aka.ms/azps-announce).</span><span class="sxs-lookup"><span data-stu-id="cde94-326">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="cde94-327">Informationen zur Migration aus AzureRM finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="cde94-327">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="cde94-328">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cde94-328">Az.Accounts</span></span>
- <span data-ttu-id="cde94-329">Geändert von Az.Profile</span><span class="sxs-lookup"><span data-stu-id="cde94-329">Changed from Az.Profile</span></span>
- <span data-ttu-id="cde94-330">Feste Tabellenformate für Profil- und Kontexttypen</span><span class="sxs-lookup"><span data-stu-id="cde94-330">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="cde94-331">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="cde94-331">Az.ApiManagement</span></span>
- <span data-ttu-id="cde94-332">Korrekturen für #7002</span><span class="sxs-lookup"><span data-stu-id="cde94-332">Fixes for #7002</span></span>
- <span data-ttu-id="cde94-333">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="cde94-333">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="cde94-334">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="cde94-334">Az.Batch</span></span>
- <span data-ttu-id="cde94-335">Möglichkeit zum Anzeigen der ausgeführten Version des Azure Batch-Knoten-Agents auf den VMs eines Pools mit der neuen `NodeAgentInformation`-Eigenschaft für `PSComputeNode` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="cde94-335">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="cde94-336">Der `Caching`-Standardwert für `PSDataDisk` lautet jetzt nicht mehr `None`, sondern `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="cde94-336">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="cde94-337">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="cde94-337">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="cde94-338">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="cde94-338">Az.Billing</span></span>
- <span data-ttu-id="cde94-339">Kombination von Billing-, Consumption- und UsageAggregates-Cmdlets. Ausführliche Informationen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="cde94-339">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="cde94-340">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="cde94-340">Az.CognitivServices</span></span>
- <span data-ttu-id="cde94-341">Vervollständigungen für SkuName und Typem für den Vorgang New-AzureRmCognitiveServicesAccount hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-341">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="cde94-342">GetSkusWithAccountParamSetName-Parametersatz aus Get-AzCognitiveServicesAccountSkus entfernt</span><span class="sxs-lookup"><span data-stu-id="cde94-342">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="cde94-343">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="cde94-343">Az.ContainerInstance</span></span>
- <span data-ttu-id="cde94-344">ManagedIdentity-Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-344">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="cde94-345">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="cde94-345">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="cde94-346">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="cde94-346">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="cde94-347">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cde94-347">Az.DataLakeStore</span></span>
- <span data-ttu-id="cde94-348">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="cde94-348">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="cde94-349">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="cde94-349">Az.Monitor</span></span>
- <span data-ttu-id="cde94-350">Az.Insights in Az.Monitor umbenannt und weitere weniger wichtige grundlegende Änderungen durchgeführt. Informationen hierzu finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="cde94-350">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="cde94-351">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cde94-351">Az.KeyVault</span></span>
- <span data-ttu-id="cde94-352">Veraltete PurgeDisabled-Eigenschaft aus Ausgabetypen entfernt</span><span class="sxs-lookup"><span data-stu-id="cde94-352">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="cde94-353">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="cde94-353">Az.MachineLearning</span></span>
- <span data-ttu-id="cde94-354">Cmdlets des Az.MachineLearningCompute-Moduls eingebunden</span><span class="sxs-lookup"><span data-stu-id="cde94-354">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="cde94-355">Az.Media</span><span class="sxs-lookup"><span data-stu-id="cde94-355">Az.Media</span></span>
- <span data-ttu-id="cde94-356">Veralteten -Tags-Alias aus New-AzMediaService entfernt</span><span class="sxs-lookup"><span data-stu-id="cde94-356">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="cde94-357">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cde94-357">Az.Network</span></span>
<span data-ttu-id="cde94-358">Unterstützung für das Konfigurieren von RewriteRuleSets im Application Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-358">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="cde94-359">Neu hinzugefügte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="cde94-359">New cmdlets added:</span></span>
        - <span data-ttu-id="cde94-360">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cde94-360">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cde94-361">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cde94-361">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cde94-362">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cde94-362">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cde94-363">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cde94-363">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cde94-364">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cde94-364">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cde94-365">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="cde94-365">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="cde94-366">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="cde94-366">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="cde94-367">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="cde94-367">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="cde94-368">Cmdlets mit optionalem Parameter -RewriteRuleSet aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-368">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="cde94-369">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="cde94-369">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="cde94-370">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="cde94-370">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="cde94-371">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="cde94-371">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="cde94-372">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="cde94-372">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="cde94-373">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="cde94-373">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="cde94-374">New-AzureRmApplicationGatewayUrlPathMapConfig: KeyVault-Unterstützung mithilfe von Identität zum Application Gateway hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="cde94-374">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="cde94-375">Cmdlets mit optionalem Parameter aktualisiert: -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="cde94-375">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="cde94-376">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="cde94-376">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="cde94-377">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="cde94-377">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="cde94-378">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="cde94-378">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="cde94-379">Cmdlet New-AzApplicationGateway mit optionalem Parameter -UserAssignedIdentity aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-379">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="cde94-380">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="cde94-380">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="cde94-381">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="cde94-381">Az.OperationalInsights</span></span>
- <span data-ttu-id="cde94-382">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="cde94-382">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="cde94-383">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="cde94-383">Az.Profile</span></span>
- <span data-ttu-id="cde94-384">Modulnamen in Az.Accounts geändert</span><span class="sxs-lookup"><span data-stu-id="cde94-384">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="cde94-385">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cde94-385">Az.RecoveryServices</span></span>
- <span data-ttu-id="cde94-386">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="cde94-386">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="cde94-387">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cde94-387">Az.Resources</span></span>
- <span data-ttu-id="cde94-388">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="cde94-388">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="cde94-389">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cde94-389">Az.ServiceFabric</span></span>
- <span data-ttu-id="cde94-390">Unterstützung für das Angeben des Zertifikats anhand des allgemeinen Namens und Fingerabdrucks</span><span class="sxs-lookup"><span data-stu-id="cde94-390">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="cde94-391">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="cde94-391">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="cde94-392">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="cde94-392">Az.SIgnalR</span></span>
- <span data-ttu-id="cde94-393">Allgemeine Verfügbarkeit für PowerShell-Cmdlets für SIgnalR</span><span class="sxs-lookup"><span data-stu-id="cde94-393">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="cde94-394">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cde94-394">Az.Sql</span></span>
- <span data-ttu-id="cde94-395">Neue Erkennungstypen Data_Exfiltration und Unsafe_Action zu Cmdlets für Bedrohungserkennung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-395">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="cde94-396">Dokumentationsbeispiele für Cmdlets für SQL-Überwachung aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-396">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="cde94-397">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="cde94-397">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="cde94-398">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cde94-398">Az.Storage</span></span>
- <span data-ttu-id="cde94-399">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="cde94-399">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="cde94-400">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cde94-400">Az.Websites</span></span>
- <span data-ttu-id="cde94-401">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="cde94-401">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="cde94-402">0.7.0 – Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="cde94-402">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="cde94-403">Allgemein</span><span class="sxs-lookup"><span data-stu-id="cde94-403">General</span></span>

* <span data-ttu-id="cde94-404">Geringe Änderungen für anstehenden Übergang von AzureRM zu Az</span><span class="sxs-lookup"><span data-stu-id="cde94-404">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="cde94-405">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cde94-405">Az.Compute</span></span>

* <span data-ttu-id="cde94-406">Unterstützung für UltraSSD und Katalogimages in einfachen Parametersätzen für `New-AzVm(ss)`-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="cde94-406">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="cde94-407">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cde94-407">Az.DataLakeStore</span></span>

* <span data-ttu-id="cde94-408">Nachgestellten Schrägstrich für die Domäne des ADLS-Kontos korrigiert</span><span class="sxs-lookup"><span data-stu-id="cde94-408">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="cde94-409">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="cde94-409">Az.FrontDoor</span></span>

* <span data-ttu-id="cde94-410">Einige fehlerhafte Links behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-410">Fixed some broken links</span></span>
    - <span data-ttu-id="cde94-411">In den Artikeln zu New-AzureRmFrontDoor und Set-AzureRmFrontDoor den Artikel-Link zum Cmdlet „New-AzureRmFrontDoorHealthProbeSettingObject“ korrigiert.</span><span class="sxs-lookup"><span data-stu-id="cde94-411">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="cde94-412">Im Artikel zu New-AzureRmFrontDoorManagedRuleObject den Artikel-Link zum Cmdlet „New-AzureRmFrontDoorRuleGroupOverrideObject“ korrigiert.</span><span class="sxs-lookup"><span data-stu-id="cde94-412">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="cde94-413">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cde94-413">Az.RecoveryServices</span></span>

* <span data-ttu-id="cde94-414">Clientseitige Validierungen für Wiederherstellungsvorgänge von Azure-Dateifreigaben hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="cde94-414">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="cde94-415">storageAccountName und storageAccountResourceGroupName für AFS-Wiederherstellung optional gemacht.</span><span class="sxs-lookup"><span data-stu-id="cde94-415">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="cde94-416">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cde94-416">Az.Resources</span></span>

* <span data-ttu-id="cde94-417">Fehlerbehebung für https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="cde94-417">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="cde94-418">Get-AzureRmRoleAssignment für die Verwendung des Abonnementbereichs aktualisiert, wenn dieser beim Anfordern von klassischen Administratoren angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="cde94-418">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="cde94-419">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cde94-419">Az.Sql</span></span>

* <span data-ttu-id="cde94-420">Geringe Änderungen für anstehenden Übergang von AzureRM zu Az</span><span class="sxs-lookup"><span data-stu-id="cde94-420">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="cde94-421">Problem mit der Verwendung von Get-AzureRmSqlDatabaseVulnerabilityAssessment mit .NET Core behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-421">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="cde94-422">Dokumentation mit Hilfemeldungen zu Cmdlets für die SQL-Überwachung geändert.</span><span class="sxs-lookup"><span data-stu-id="cde94-422">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="cde94-423">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cde94-423">Az.Storage</span></span>

* <span data-ttu-id="cde94-424">-EnableHierarchicalNamespace zu New-AzureRmStorageAccount hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-424">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="cde94-425">Problem behoben, bei dem für das Copy File-Cmdlet am Ziel kein Quellkontext wiederverwendet werden kann, wenn -DestContext nicht eingegeben wird</span><span class="sxs-lookup"><span data-stu-id="cde94-425">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="cde94-426">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="cde94-426">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="cde94-427">Unterstützung der Konfiguration von statischen Websites</span><span class="sxs-lookup"><span data-stu-id="cde94-427">Support Static Website configuration</span></span>
    - <span data-ttu-id="cde94-428">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="cde94-428">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="cde94-429">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="cde94-429">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="cde94-430">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cde94-430">Az.Websites</span></span>

* <span data-ttu-id="cde94-431">Set-AzureRmWebApp und Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="cde94-431">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="cde94-432">Neuen Parameter (-AzureStoragePath) zum Angeben von Azure Storage-Pfaden hinzugefügt, die in Windows- und Linux-Container-Apps bereitgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="cde94-432">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="cde94-433">Verwenden Sie die Ausgabe des neuen Cmdlets New-AzureRmWebAppAzureStoragePath als Parameter zum Festlegen der Azure Storage-Pfade.</span><span class="sxs-lookup"><span data-stu-id="cde94-433">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="cde94-434">0.6.1 – November 2018</span><span class="sxs-lookup"><span data-stu-id="cde94-434">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="cde94-435">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="cde94-435">Az.ApiManagement</span></span>
* <span data-ttu-id="cde94-436">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-436">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="cde94-437">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cde94-437">Az.Automation</span></span>
* <span data-ttu-id="cde94-438">Swagger-basierte Azure Automation-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="cde94-438">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="cde94-439">Cmdlets zur Updateverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-439">Added Update Management cmdlets</span></span>
* <span data-ttu-id="cde94-440">Cmdlets zur Quellcodeverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-440">Added Source Control cmdlets</span></span>
* <span data-ttu-id="cde94-441">Cmdlet „Remove-AzureRmAutomationHybridWorkerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-441">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="cde94-442">DSC-Befehl für die Knotenregistrierung korrigiert</span><span class="sxs-lookup"><span data-stu-id="cde94-442">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="cde94-443">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cde94-443">Az.Compute</span></span>
* <span data-ttu-id="cde94-444">Identitätsproblem für SystemAssigned-Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="cde94-444">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="cde94-445">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-445">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="cde94-446">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="cde94-446">Az.ContainerInstance</span></span>
* <span data-ttu-id="cde94-447">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-447">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="cde94-448">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="cde94-448">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="cde94-449">Beschreibung der Beispiele für Marketplace-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-449">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="cde94-450">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cde94-450">Az.Network</span></span>
* <span data-ttu-id="cde94-451">Folgende Cmdlets hinzugefügt: New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="cde94-451">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="cde94-452">ICMP wieder unterstützten AzureFirewall-Netzwerkprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-452">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="cde94-453">Cmdlet „Test-AzureRmNetworkWatcherConnectivity“ aktualisiert und Überprüfung für Ziel-ID, Adresse und Port hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-453">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="cde94-454">Probleme mit Arbeitsspeicherauslastung in der VirtualNetwork-Zuordnung behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-454">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="cde94-455">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="cde94-455">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="cde94-456">Problem beim Ändern der Richtlinie für eine geschützte Dateifreigabe behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-456">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="cde94-457">Richtlinienzeitzone in Großschreibung geändert</span><span class="sxs-lookup"><span data-stu-id="cde94-457">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="cde94-458">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="cde94-458">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="cde94-459">Korrigiertes Beispiel in „New-AzureRmRecoveryServicesAsrProtectableItem“</span><span class="sxs-lookup"><span data-stu-id="cde94-459">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="cde94-460">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-460">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="cde94-461">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="cde94-461">Az.Relay</span></span>
* <span data-ttu-id="cde94-462">Optionaler Parameter „-KeyValue“ zu Cmdlet „New-AzureRmRelayKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht</span><span class="sxs-lookup"><span data-stu-id="cde94-462">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="cde94-463">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cde94-463">Az.Resources</span></span>
* <span data-ttu-id="cde94-464">Hilfedokumentation für ressourcenidentitätsbezogene Parameter in `New-AzureRmPolicyAssignment` und `Set-AzureRmPolicyAssignment` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-464">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="cde94-465">Beispiel für „New-AzureRmPolicyDefinition“ hinzugefügt, das „-Metadata“ nutzt</span><span class="sxs-lookup"><span data-stu-id="cde94-465">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="cde94-466">Korrektur, um Beibehaltung von Groß-/Kleinschreibung in Tagschlüsseln in „NetStandard“ zu ermöglichen: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="cde94-466">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="cde94-467">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cde94-467">Az.ServiceFabric</span></span>
* <span data-ttu-id="cde94-468">Benachrichtigung über veraltete Elemente für anstehende wichtige Änderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-468">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="cde94-469">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cde94-469">Az.Sql</span></span>
* <span data-ttu-id="cde94-470">Neue Cmdlets für CRUD-Vorgänge in verwalteten Azure SQL-Datenbank-Instanzen und verwalteten Azure SQL-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-470">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="cde94-471">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="cde94-471">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="cde94-472">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="cde94-472">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="cde94-473">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="cde94-473">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="cde94-474">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="cde94-474">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="cde94-475">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="cde94-475">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="cde94-476">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="cde94-476">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="cde94-477">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="cde94-477">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="cde94-478">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="cde94-478">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="cde94-479">Erweiterte Verwaltung von Überwachungsrichtlinien auf einem Server oder in einer Datenbank aktiviert</span><span class="sxs-lookup"><span data-stu-id="cde94-479">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="cde94-480">Neuer Parameter (PredicateExpression) hinzugefügt, um die Filterung von Überwachungsprotokollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="cde94-480">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="cde94-481">Cmdlets wurden angepasst, sodass sie SQL-Clients anstelle von Legacyclients verwenden.</span><span class="sxs-lookup"><span data-stu-id="cde94-481">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="cde94-482">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="cde94-482">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="cde94-483">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="cde94-483">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="cde94-484">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="cde94-484">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="cde94-485">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="cde94-485">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="cde94-486">Problem bei Verwendung von „Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings“ mit festgelegtem Parameter für den Speicherkontonamen behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-486">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="cde94-487">0.5.0 – November 2018</span><span class="sxs-lookup"><span data-stu-id="cde94-487">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="cde94-488">Allgemein</span><span class="sxs-lookup"><span data-stu-id="cde94-488">General</span></span>
* <span data-ttu-id="cde94-489">Ressourcenvervollständigungen für viele Kern-Cmdlets hinzugefügt (diese ermöglichen das Durchlaufen von vorhandenen Ressourcennamen per TAB-TASTE, wenn Cmdlets interaktiv aufgerufen werden)</span><span class="sxs-lookup"><span data-stu-id="cde94-489">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="cde94-490">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="cde94-490">Az.Profile</span></span>
* <span data-ttu-id="cde94-491">Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="cde94-491">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="cde94-492">Parameter „TenantId“ im Cmdlet „Connect-AzAccount“ in „Tenant“ umbenannt und Alias für „TenantId“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-492">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="cde94-493">Beschreibung von „TenantId“ für „Connect-AzAccount“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="cde94-493">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="cde94-494">Fehlermeldung für fehlgeschlagene Anmeldung bei Angabe der Mandantendomäne korrigiert</span><span class="sxs-lookup"><span data-stu-id="cde94-494">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="cde94-495">Problem in Bezug auf Kontextnamenskonflikt für Konten ohne Abonnements im Mandanten behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-495">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="cde94-496">Problem mit DataLake-Endpunkten bei Verwendung von MSI behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-496">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="cde94-497">Problem behoben, das zur Auslösung von „Disconnect-AzAccount“ führte, wenn keine Verbindung bestand</span><span class="sxs-lookup"><span data-stu-id="cde94-497">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="cde94-498">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="cde94-498">Az.CognitiveServices</span></span>
* <span data-ttu-id="cde94-499">Vorgang „Get-AzCognitiveServicesAccountSkus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-499">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cde94-500">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cde94-500">Az.Compute</span></span>
* <span data-ttu-id="cde94-501">Cmdlets Add-AzVmssVMDataDisk und Remove-AzVmssVMDataDisk hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-501">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="cde94-502">„Get-AzVMImage“ zeigt „AutomaticOSUpgradeProperties“ an</span><span class="sxs-lookup"><span data-stu-id="cde94-502">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="cde94-503">Problem behoben, aufgrund dessen die Optionswerte „SetAzVMChefExtension -BootstrapOptions“ und „-JsonAttribute“ nicht im JSON-Format festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="cde94-503">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cde94-504">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cde94-504">Az.DataLakeStore</span></span>
* <span data-ttu-id="cde94-505">Aktualisierung des DataLake-Pakets auf 1.1.10</span><span class="sxs-lookup"><span data-stu-id="cde94-505">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="cde94-506">Standardmäßige Parallelität zu Multithreadvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-506">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="cde94-507">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="cde94-507">Az.Insights</span></span>
* <span data-ttu-id="cde94-508">Problem Nr. 7267 behoben (Bereich für automatische Skalierung)</span><span class="sxs-lookup"><span data-stu-id="cde94-508">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="cde94-509">Probleme beim Erstellen einer neuen Regel für die automatische Skalierung, aufgrund derer die aufgelisteten Parameter nicht richtig festgelegt wurden (Es wurde stets der Standardwert festgelegt.)</span><span class="sxs-lookup"><span data-stu-id="cde94-509">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="cde94-510">Problem Nr. 7513 behoben [Insights] „Set-AzDiagnosticSetting“ erfordert die explizite Angabe von Kategorien während der Erstellung der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="cde94-510">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="cde94-511">Nun erfordert das Cmdlet nicht die explizite Angabe der Kategorien, die während der Erstellung aktiviert werden sollen. Das bedeutet, es funktioniert wie dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="cde94-511">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cde94-512">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cde94-512">Az.Network</span></span>
* <span data-ttu-id="cde94-513">„PeeringType“ wurde geändert und ist nun ein erforderlicher Parameter für die folgenden Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="cde94-513">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="cde94-514">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="cde94-514">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="cde94-515">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="cde94-515">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="cde94-516">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="cde94-516">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="cde94-517">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="cde94-517">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="cde94-518">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="cde94-518">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="cde94-519">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="cde94-519">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="cde94-520">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="cde94-520">Az.PolicyInsights</span></span>
* <span data-ttu-id="cde94-521">Cmdlets für Richtlinienwartung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-521">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="cde94-522">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cde94-522">Az.Resources</span></span>
* <span data-ttu-id="cde94-523">Fehlerbehebung für https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="cde94-523">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="cde94-524">Zulassen der Auflistung von Ressourcen mithilfe des Parameters „-ResourceId“ für „Get-AzResource“</span><span class="sxs-lookup"><span data-stu-id="cde94-524">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="cde94-525">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="cde94-525">Az.ServiceBus</span></span>
* <span data-ttu-id="cde94-526">Schreibgeschützte Eigenschaft „MigrationState“ zu „PSServiceBusMigrationConfigurationAttributes“ hinzugefügt, was das Ermitteln des Migrationsstatus ermöglicht</span><span class="sxs-lookup"><span data-stu-id="cde94-526">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="cde94-527">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cde94-527">Az.ServiceFabric</span></span>
* <span data-ttu-id="cde94-528">Hinzufügen des Zertifikats zu Linux VMSS korrigiert</span><span class="sxs-lookup"><span data-stu-id="cde94-528">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="cde94-529">„Add-AzServiceFabricClusterCertificate“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="cde94-529">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="cde94-530">Verwenden des richtigen Fingerabdrucks aus dem neuen Zertifikat (Azure/service-fabric-issues#932)</span><span class="sxs-lookup"><span data-stu-id="cde94-530">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="cde94-531">Richtige Anzeige von Ausnahmen (Azure/service-fabric-issues#1054)</span><span class="sxs-lookup"><span data-stu-id="cde94-531">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="cde94-532">„Update-AzServiceFabricDurability“ korrigiert, um die Clusterkonfiguration zu aktualisieren, bevor der VMSS-Vorgang „CreateOrUpdate“ gestartet wird</span><span class="sxs-lookup"><span data-stu-id="cde94-532">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="cde94-533">0.4.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="cde94-533">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="cde94-534">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="cde94-534">Az.Profile</span></span>
* <span data-ttu-id="cde94-535">Problem mit „Get-AzSubscription“ in Cloud Shell behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-535">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="cde94-536">Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="cde94-536">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cde94-537">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cde94-537">Az.Compute</span></span>
* <span data-ttu-id="cde94-538">Neue Größen zur Whitelist von VM-Größen hinzugefügt, für die bei Verwendung des einfachen Parametersatzes für „New-AzVm“ der beschleunigte Netzwerkbetrieb aktiviert wird</span><span class="sxs-lookup"><span data-stu-id="cde94-538">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="cde94-539">ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="cde94-539">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cde94-540">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cde94-540">Az.DataLakeStore</span></span>
* <span data-ttu-id="cde94-541">Unterstützung für Regeln für virtuelle Netzwerke hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-541">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="cde94-542">Get-AzDataLakeStoreVirtualNetworkRule: Dient zum Abrufen oder Auflisten der Azure Data Lake Store-Regel für das virtuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="cde94-542">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="cde94-543">Add-AzDataLakeStoreVirtualNetworkRule: Fügt dem angegebenen Data Lake Store-Konto eine Regel für das virtuelle Netzwerk hinzu.</span><span class="sxs-lookup"><span data-stu-id="cde94-543">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="cde94-544">Set-AzDataLakeStoreVirtualNetworkRule: Ändert die angegebene Regel für das virtuelle Netzwerk in das angegebene Data Lake Store-Konto.</span><span class="sxs-lookup"><span data-stu-id="cde94-544">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="cde94-545">Remove-AzDataLakeStoreVirtualNetworkRule: Dient zum Löschen der Azure Data Lake Store-Regel für das virtuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="cde94-545">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cde94-546">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cde94-546">Az.Network</span></span>
* <span data-ttu-id="cde94-547">Cmdlet „Test-AzNetworkWatcherConnectivity“ aktualisiert, Protokollwert wird jetzt an Back-End übergeben.</span><span class="sxs-lookup"><span data-stu-id="cde94-547">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="cde94-548">ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="cde94-548">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="cde94-549">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cde94-549">Az.Resources</span></span>
* <span data-ttu-id="cde94-550">Problem behoben, aufgrund dessen „Get-AzRoleDefinition“ eine unverständliche Ausnahme auslöst (wenn das Standardprofil kein Abonnement enthält und kein Bereich festgelegt ist), indem im Szenario eine aussagekräftige Ausnahme hinzugefügt wurde.</span><span class="sxs-lookup"><span data-stu-id="cde94-550">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="cde94-551">Außerdem wurde der Standardparametersatz auf „RoleDefinitionNameParameterSet“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="cde94-551">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="cde94-552">0.3.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="cde94-552">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="cde94-553">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="cde94-553">Azure.Storage</span></span>
* <span data-ttu-id="cde94-554">Fehler beim Kopieren von Blobs/Dateien behoben, aufgrund dessen bei einem Metadatenproblem des Ziels keine Metadaten kopiert wurden</span><span class="sxs-lookup"><span data-stu-id="cde94-554">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="cde94-555">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="cde94-555">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="cde94-556">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="cde94-556">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="cde94-557">Der Abruf der Speicherressourcennutzung eines bestimmten Standorts wird jetzt unterstützt, und das Hinzufügen einer Warnmeldung für den Abruf der globalen Speicherressourcennutzung ist überflüssig.</span><span class="sxs-lookup"><span data-stu-id="cde94-557">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="cde94-558">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="cde94-558">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="cde94-559">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="cde94-559">Az.CognitiveServices</span></span>
* <span data-ttu-id="cde94-560">„Get-AzCognitiveServicesAccountSkus“ wird ohne vorhandenes Konto unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cde94-560">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cde94-561">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cde94-561">Az.Compute</span></span>
* <span data-ttu-id="cde94-562">Korrektur von „Get-AzVM -ResourceGroupName <rg>“, sodass ggf. mehr als 50 Ergebnisse zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="cde94-562">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="cde94-563">Der Cmdlet-Hilfe zu „New-AzVmss“ wurde ein Beispiel für „SimpleParameterSet“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="cde94-563">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="cde94-564">Tippfehler in der Azure Disk Encryption-Statusmeldung behoben</span><span class="sxs-lookup"><span data-stu-id="cde94-564">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="cde94-565">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="cde94-565">Az.DataFactoryV2</span></span>
* <span data-ttu-id="cde94-566">Die Version des ADF .Net-SDK wurde auf 2.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="cde94-566">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cde94-567">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cde94-567">Az.Network</span></span>
* <span data-ttu-id="cde94-568">NetworkProfile-Funktionalität wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="cde94-568">Added NetworkProfile functionality.</span></span> <span data-ttu-id="cde94-569">Neue Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-569">new cmdlets added</span></span>
    - <span data-ttu-id="cde94-570">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cde94-570">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="cde94-571">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cde94-571">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="cde94-572">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cde94-572">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="cde94-573">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cde94-573">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="cde94-574">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="cde94-574">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="cde94-575">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="cde94-575">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="cde94-576">Dienstzuordnungslink in Subnetzmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-576">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="cde94-577">Cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-577">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="cde94-578">Cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-578">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="cde94-579">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="cde94-579">Az.RedisCache</span></span>
* <span data-ttu-id="cde94-580">Künftig sind beliebige Zeichenfolgen als Größenparameter zulässig.</span><span class="sxs-lookup"><span data-stu-id="cde94-580">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="cde94-581">P5 in Popup „PSArgumentCompleter“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-581">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="cde94-582">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cde94-582">Az.Resources</span></span>
* <span data-ttu-id="cde94-583">Fehlender Parameter „-Mode“ zu „Set-AzPolicyDefinition“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="cde94-583">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="cde94-584">Cmdlet-Fehler bei „Get-AzProviderOperation“ für Vorgänge mit Ursprung behoben, der den Benutzer enthält</span><span class="sxs-lookup"><span data-stu-id="cde94-584">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="cde94-585">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cde94-585">Az.Sql</span></span>
* <span data-ttu-id="cde94-586">Problem behoben, aufgrund dessen einige Sicherungs-Cmdlets das aktuelle Azure-Abonnements nicht erkannt haben</span><span class="sxs-lookup"><span data-stu-id="cde94-586">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cde94-587">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cde94-587">Az.Websites</span></span>
* <span data-ttu-id="cde94-588">Neues Cmdlet „Get-AzWebAppContainerContinuousDeploymentUrl“ zum Abrufen der Webhook-URL von Continuous Deployment für Container</span><span class="sxs-lookup"><span data-stu-id="cde94-588">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="cde94-589">Neue Cmdlets „New-AzWebAppContainerPSSession“ und „Enter-WebAppContainerPSSession“ zum Initiieren einer PowerShell-Remotesitzung in einer Windows-Container-App</span><span class="sxs-lookup"><span data-stu-id="cde94-589">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="cde94-590">0.2.0 – September 2018</span><span class="sxs-lookup"><span data-stu-id="cde94-590">0.2.0 - September 2018</span></span>
 <span data-ttu-id="cde94-591">Erste Version</span><span class="sxs-lookup"><span data-stu-id="cde94-591">Initial Release</span></span>