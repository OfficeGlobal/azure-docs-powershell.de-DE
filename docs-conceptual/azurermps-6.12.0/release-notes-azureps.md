---
title: Azure PowerShell-Änderungsprotokoll | Microsoft-Dokumentation
description: Hierbei handelt es sich um einen Verlauf der Änderungen, die in der neuesten Version an Azure PowerShell vorgenommen wurden.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 08/28/2018
ms.openlocfilehash: 8a7b184ed06eb078956229fa67d02840014e3aaf
ms.sourcegitcommit: 4afdba3cd7e1d348876ce59f3503fdcd258f79ab
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/15/2018
ms.locfileid: "51574531"
---
# <a name="release-notes"></a><span data-ttu-id="755dd-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="755dd-103">Release notes</span></span>

<span data-ttu-id="755dd-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="755dd-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="6120---november-2018"></a><span data-ttu-id="755dd-105">6.12.0: November 2018</span><span class="sxs-lookup"><span data-stu-id="755dd-105">6.12.0 - November 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="755dd-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="755dd-106">AzureRM.Profile</span></span>
* <span data-ttu-id="755dd-107">Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="755dd-107">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="755dd-108">Parameter „TenantId“ im Cmdlet „Connect-AzureRmAccount“ in „Tenant“ umbenannt und Alias für „TenantId“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-108">Rename param TenantId in cmdlet Connect-AzureRmAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="755dd-109">Beschreibung von „TenantId“ für „Connect-AzureRmAccount“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-109">Updated TenantId description for Connect-AzureRmAccount</span></span>
* <span data-ttu-id="755dd-110">Fehlermeldung für fehlgeschlagene Anmeldung bei Angabe der Mandantendomäne korrigiert</span><span class="sxs-lookup"><span data-stu-id="755dd-110">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="755dd-111">Problem in Bezug auf Kontextnamenskonflikt für Konten ohne Abonnements im Mandanten behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-111">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="755dd-112">Problem mit DataLake-Endpunkten bei Verwendung von MSI behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-112">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="755dd-113">Problem behoben, das zur Auslösung von „Disconnect-AzureRmAccount“ führte, wenn keine Verbindung bestand</span><span class="sxs-lookup"><span data-stu-id="755dd-113">Fix issue where 'Disconnect-AzureRmAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azurermautomation"></a><span data-ttu-id="755dd-114">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="755dd-114">AzureRM.Automation</span></span>
* <span data-ttu-id="755dd-115">DLL-Dateiname des Cmdlets in „Microsoft.Azure.Commands.Automation.dll“ umbenannt</span><span class="sxs-lookup"><span data-stu-id="755dd-115">Renamed cmdlet DLL filename to Microsoft.Azure.Commands.Automation.dll</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="755dd-116">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="755dd-116">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="755dd-117">Vorgang „Get-AzureRmCognitiveServicesAccountSkus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-117">Add Get-AzureRmCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="755dd-118">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="755dd-118">AzureRM.Compute</span></span>
* <span data-ttu-id="755dd-119">Cmdlets „Add-AzureRmVmssVMDataDisk“ und „Remove-AzureRmVmssVMDataDisk“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-119">Add Add-AzureRmVmssVMDataDisk and Remove-AzureRmVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="755dd-120">„Get-AzureRmVMImage“ zeigt „AutomaticOSUpgradeProperties“ an.</span><span class="sxs-lookup"><span data-stu-id="755dd-120">Get-AzureRmVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="755dd-121">Problem behoben, aufgrund dessen die Optionswerte „SetAzureRmVMChefExtension -BootstrapOptions“ und „-JsonAttribute“ nicht im JSON-Format festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="755dd-121">Fixed SetAzureRmVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="755dd-122">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="755dd-122">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="755dd-123">Aktualisierung des DataLake-Pakets auf 1.1.10</span><span class="sxs-lookup"><span data-stu-id="755dd-123">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="755dd-124">Standardmäßige Parallelität zu Multithreadvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-124">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="755dd-125">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="755dd-125">AzureRM.Insights</span></span>
* <span data-ttu-id="755dd-126">Problem Nr. 7267 behoben (Bereich für automatische Skalierung)</span><span class="sxs-lookup"><span data-stu-id="755dd-126">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="755dd-127">Probleme beim Erstellen einer neuen Regel für die automatische Skalierung, aufgrund derer die aufgelisteten Parameter nicht richtig festgelegt wurden (Es wurde stets der Standardwert festgelegt.)</span><span class="sxs-lookup"><span data-stu-id="755dd-127">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="755dd-128">Problem Nr. 7513 behoben [Insights] „Set-AzureRMDiagnosticSetting“ erfordert die explizite Angabe von Kategorien während der Erstellung der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="755dd-128">Fixed issue #7513 [Insights] Set-AzureRMDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="755dd-129">Nun erfordert das Cmdlet nicht die explizite Angabe der Kategorien, die während der Erstellung aktiviert werden sollen. Das bedeutet, es funktioniert wie dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="755dd-129">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="755dd-130">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="755dd-130">AzureRM.Network</span></span>
* <span data-ttu-id="755dd-131">„PeeringType“ wurde geändert und ist nun ein erforderlicher Parameter für die folgenden Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="755dd-131">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="755dd-132">Get-AzureRmExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="755dd-132">Get-AzureRmExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="755dd-133">Get-AzureRmExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="755dd-133">Get-AzureRmExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="755dd-134">Get-AzureRmExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="755dd-134">Get-AzureRmExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="755dd-135">Get-AzureRMExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="755dd-135">Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="755dd-136">Get-AzureRMExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="755dd-136">Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="755dd-137">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="755dd-137">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="755dd-138">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="755dd-138">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="755dd-139">Cmdlets für Richtlinienwartung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-139">Added policy remediation cmdlets</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="755dd-140">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="755dd-140">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="755dd-141">Unterstützung für Azure-Dateifreigaben in Wiederherstellungsdiensten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-141">Added support for azure file shares in recovery services.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="755dd-142">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="755dd-142">AzureRM.Resources</span></span>
* <span data-ttu-id="755dd-143">Fehlerbehebung für https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="755dd-143">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="755dd-144">Zulassen der Auflistung von Ressourcen mithilfe des Parameters „-ResourceId“ für „Get-AzureRmResource“</span><span class="sxs-lookup"><span data-stu-id="755dd-144">Allow listing resources using the '-ResourceId' parameter for 'Get-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="755dd-145">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="755dd-145">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="755dd-146">Schreibgeschützte Eigenschaft „MigrationState“ zu „PSServiceBusMigrationConfigurationAttributes“ hinzugefügt, was das Ermitteln des Migrationsstatus ermöglicht</span><span class="sxs-lookup"><span data-stu-id="755dd-146">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="755dd-147">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="755dd-147">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="755dd-148">Hinzufügen des Zertifikats zu Linux VMSS korrigiert</span><span class="sxs-lookup"><span data-stu-id="755dd-148">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="755dd-149">„Add-AzureRmServiceFabricClusterCertificate“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="755dd-149">Fix 'Add-AzureRmServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="755dd-150">Verwenden des richtigen Fingerabdrucks aus dem neuen Zertifikat (Azure/service-fabric-issues#932)</span><span class="sxs-lookup"><span data-stu-id="755dd-150">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="755dd-151">Richtige Anzeige von Ausnahmen (Azure/service-fabric-issues#1054)</span><span class="sxs-lookup"><span data-stu-id="755dd-151">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="755dd-152">„Update-AzureRmServiceFabricDurability“ korrigiert, um die Clusterkonfiguration zu aktualisieren, bevor der VMSS-Vorgang „CreateOrUpdate“ gestartet wird</span><span class="sxs-lookup"><span data-stu-id="755dd-152">Fix 'Update-AzureRmServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="6110---october-2018"></a><span data-ttu-id="755dd-153">6.11.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="755dd-153">6.11.0 - October 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="755dd-154">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="755dd-154">AzureRM.Profile</span></span>
* <span data-ttu-id="755dd-155">Problem mit „Get-AzureRmSubscription“ in CloudShell behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-155">Fix issue with Get-AzureRmSubscription in CloudShell</span></span>
* <span data-ttu-id="755dd-156">Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="755dd-156">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="755dd-157">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="755dd-157">AzureRM.Backup</span></span>
* <span data-ttu-id="755dd-158">Azure Backup-Cmdlets als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="755dd-158">Deprecated Azure Backup cmdlets.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="755dd-159">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="755dd-159">AzureRM.Compute</span></span>
* <span data-ttu-id="755dd-160">Neue Größen zur Whitelist von VM-Größen hinzugefügt, für die bei Verwendung des einfachen Parametersatzes für „New-AzureRmVm“ der beschleunigte Netzwerkbetrieb aktiviert wird</span><span class="sxs-lookup"><span data-stu-id="755dd-160">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzureRmVm'</span></span>
* <span data-ttu-id="755dd-161">ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="755dd-161">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="755dd-162">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="755dd-162">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="755dd-163">Unterstützung für Regeln für virtuelle Netzwerke hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-163">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="755dd-164">Get-AzureRmDataLakeStoreVirtualNetworkRule: Ruft Regel für virtuelles Azure Data Lake Store-Netzwerk ab oder listet sie auf.</span><span class="sxs-lookup"><span data-stu-id="755dd-164">Get-AzureRmDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="755dd-165">Add-AzureRmDataLakeStoreVirtualNetworkRule: Fügt dem angegebenen Data Lake Store-Konto eine Regel für das virtuelle Netzwerk hinzu.</span><span class="sxs-lookup"><span data-stu-id="755dd-165">Add-AzureRmDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="755dd-166">Set-AzureRmDataLakeStoreVirtualNetworkRule: Ändert die angegebene Regel für das virtuelle Netzwerk im angegebenen Data Lake Store-Konto.</span><span class="sxs-lookup"><span data-stu-id="755dd-166">Set-AzureRmDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="755dd-167">Remove-AzureRmDataLakeStoreVirtualNetworkRule: Löscht eine Regel für das virtuelle Azure Data Lake Store-Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="755dd-167">Remove-AzureRmDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="755dd-168">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="755dd-168">AzureRM.Network</span></span>
* <span data-ttu-id="755dd-169">Cmdlet „Test-AzureRmNetworkWatcherConnectivity“ aktualisiert, Protokollwert wird jetzt an Back-End übergeben.</span><span class="sxs-lookup"><span data-stu-id="755dd-169">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="755dd-170">ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="755dd-170">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="755dd-171">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="755dd-171">AzureRM.Resources</span></span>
* <span data-ttu-id="755dd-172">Problem behoben, aufgrund dessen „Get-AzureRMRoleDefinition“ eine unverständliche Ausnahme auslöst (wenn das Standardprofil kein Abonnement enthält und kein Bereich festgelegt ist) indem im Szenario eine aussagekräftige Ausnahme hinzugefügt wurde.</span><span class="sxs-lookup"><span data-stu-id="755dd-172">Fix isssue where Get-AzureRMRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="755dd-173">Außerdem wurde der Standardparametersatz auf „RoleDefinitionNameParameterSet“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="755dd-173">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="6100---october-2018"></a><span data-ttu-id="755dd-174">6.10.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="755dd-174">6.10.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="755dd-175">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="755dd-175">Azure.Storage</span></span>
* <span data-ttu-id="755dd-176">Fehler beim Kopieren von Blobs/Dateien behoben, aufgrund dessen bei einem Metadatenproblem des Ziels keine Metadaten kopiert wurden</span><span class="sxs-lookup"><span data-stu-id="755dd-176">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="755dd-177">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="755dd-177">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="755dd-178">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="755dd-178">Start-AzureStorageFileCopy</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="755dd-179">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="755dd-179">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="755dd-180">„Get-AzureRmCognitiveServicesAccountSkus“ wird ohne vorhandenes Konto unterstützt.</span><span class="sxs-lookup"><span data-stu-id="755dd-180">Support Get-AzureRmCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="755dd-181">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="755dd-181">AzureRM.Compute</span></span>
* <span data-ttu-id="755dd-182">Korrektur von „Get-AzureRmVM -ResourceGroupName <rg>“ sodass ggf. mehr als 50 Ergebnisse zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="755dd-182">Fix Get-AzureRmVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="755dd-183">Der Cmdlet-Hilfe zu „New-AzureRmVmss“ wurde ein Beispiel für „SimpleParameterSet“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="755dd-183">Added an example of the 'SimpleParameterSet' to New-AzureRmVmss cmdlet help.</span></span>
* <span data-ttu-id="755dd-184">Tippfehler in der Azure Disk Encryption-Statusmeldung behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-184">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="755dd-185">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="755dd-185">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="755dd-186">Die Version des ADF .Net-SDK wurde auf 2.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="755dd-186">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="755dd-187">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="755dd-187">AzureRM.Network</span></span>
* <span data-ttu-id="755dd-188">NetworkProfile-Funktionalität wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="755dd-188">Added NetworkProfile functionality.</span></span> <span data-ttu-id="755dd-189">Neue Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-189">new cmdlets added</span></span>
    - <span data-ttu-id="755dd-190">Get-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="755dd-190">Get-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="755dd-191">New-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="755dd-191">New-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="755dd-192">Remove-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="755dd-192">Remove-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="755dd-193">Set-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="755dd-193">Set-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="755dd-194">New-AzureRMContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-194">New-AzureRMContainerNicConfig</span></span>
    - <span data-ttu-id="755dd-195">New-AzureRmContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-195">New-AzureRmContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="755dd-196">Dienstzuordnungslink in Subnetzmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-196">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="755dd-197">Cmdlets „New-AzureRmVirtualNetworkTap“, „Get-AzureRmVirtualNetworkTap“, „Set-AzureRmVirtualNetworkTap“, „Remove-AzureRmVirtualNetworkTap“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-197">Added cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span></span>
* <span data-ttu-id="755dd-198">Cmdlets „Set-AzureRmNEtworkInterfaceTapConfig“, „Get-AzureRmNEtworkInterfaceTapConfig“, „Remove-AzureRmNEtworkInterfaceTapConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-198">Added cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="755dd-199">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="755dd-199">AzureRM.RedisCache</span></span>
* <span data-ttu-id="755dd-200">Künftig sind beliebige Zeichenfolgen als Größenparameter zulässig.</span><span class="sxs-lookup"><span data-stu-id="755dd-200">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="755dd-201">P5 in Popup „PSArgumentCompleter“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-201">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="755dd-202">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="755dd-202">AzureRM.Resources</span></span>
* <span data-ttu-id="755dd-203">Fehlender Parameter „-Mode“ zu „Set-AzureRmPolicyDefinition“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-203">Add missing -Mode parameter to Set-AzureRmPolicyDefinition</span></span>
* <span data-ttu-id="755dd-204">Cmdlet-Fehler bei „Fix Get-AzureRmProviderOperation“ für Vorgänge mit Ursprung behoben, der den Benutzer enthält</span><span class="sxs-lookup"><span data-stu-id="755dd-204">Fix Get-AzureRmProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="755dd-205">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="755dd-205">AzureRM.Sql</span></span>
* <span data-ttu-id="755dd-206">Problem behoben, aufgrund dessen einige Sicherungs-Cmdlets das aktuelle Azure-Abonnements nicht erkannt haben</span><span class="sxs-lookup"><span data-stu-id="755dd-206">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="755dd-207">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="755dd-207">AzureRM.Storage</span></span>
* <span data-ttu-id="755dd-208">Der Abruf der Speicherressourcennutzung eines bestimmten Standorts wird jetzt unterstützt, und das Hinzufügen einer Warnmeldung für den Abruf der globalen Speicherressourcennutzung ist überflüssig.</span><span class="sxs-lookup"><span data-stu-id="755dd-208">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="755dd-209">Get-AzureRmStorageUsage</span><span class="sxs-lookup"><span data-stu-id="755dd-209">Get-AzureRmStorageUsage</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="755dd-210">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="755dd-210">AzureRM.Websites</span></span>
* <span data-ttu-id="755dd-211">Neues Cmdlet „Get-AzureRMWebAppContainerContinuousDeploymentUrl“ zum Abruf der Webhook-URL von Continuous Deployment für Container</span><span class="sxs-lookup"><span data-stu-id="755dd-211">New Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="755dd-212">Neue Cmdlets „New-AzureRMWebAppContainerPSSession“ und „Enter-WebAppContainerPSSession“ zum Initiieren einer PowerShell-Remotesitzung in einer Windows-Container-App</span><span class="sxs-lookup"><span data-stu-id="755dd-212">New Cmdlets New-AzureRMWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="690---september-2018"></a><span data-ttu-id="755dd-213">6.9.0 – September 2018</span><span class="sxs-lookup"><span data-stu-id="755dd-213">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="755dd-214">Allgemein</span><span class="sxs-lookup"><span data-stu-id="755dd-214">General</span></span>
* <span data-ttu-id="755dd-215">AzureRM.SignalR wurde dem Rollupmodul AzureRM hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-215">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="755dd-216">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="755dd-216">AzureRM.Profile</span></span>
* <span data-ttu-id="755dd-217">Kleinere Änderungen am allgemeinen Speichercode</span><span class="sxs-lookup"><span data-stu-id="755dd-217">Minor changes to the storage common code</span></span>
* <span data-ttu-id="755dd-218">Hilfedateien aktualisiert, um vollständige Parametertypen einzubinden.</span><span class="sxs-lookup"><span data-stu-id="755dd-218">Updated help files to include full parameter types.</span></span>
* <span data-ttu-id="755dd-219">„-ServicePrincipal“ im Parametersatz „ServicePrincipalCertificateWithSubscriptionId“ in nicht obligatorisch geändert</span><span class="sxs-lookup"><span data-stu-id="755dd-219">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="755dd-220">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="755dd-220">Azure.Storage</span></span>
* <span data-ttu-id="755dd-221">Unterstützung für die Erstellung des Speicherkontexts mit OAuth.</span><span class="sxs-lookup"><span data-stu-id="755dd-221">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="755dd-222">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="755dd-222">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="755dd-223">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="755dd-223">AzureRM.Cdn</span></span>
* <span data-ttu-id="755dd-224">Standard_Microsoft in SKU für CDN-Preise hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="755dd-224">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="755dd-225">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="755dd-225">AzureRM.Compute</span></span>
* <span data-ttu-id="755dd-226">Abhängigkeiten für Key Vault und Storage in allgemeine Abhängigkeiten verschieben</span><span class="sxs-lookup"><span data-stu-id="755dd-226">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="755dd-227">Unterstützung für weitere VM-Größen zu AEM-Cmdlets hinzufügen</span><span class="sxs-lookup"><span data-stu-id="755dd-227">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="755dd-228">Parameter „PublicIPPrefix“ zu „New-AzureRmVmssIpConfig“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="755dd-228">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="755dd-229">Parameter „ResourceId“ zu Cmdlet „Invoke-AzureRmVMRunCommand“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="755dd-229">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="755dd-230">Cmdlet „Invoke-AzureRmVmssVMRunCommand“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="755dd-230">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="755dd-231">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="755dd-231">AzureRM.Dns</span></span>
* <span data-ttu-id="755dd-232">Unterstützung für Aliaseintrag während der Erstellung des DNS-Eintrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-232">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="755dd-233">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="755dd-233">AzureRM.Insights</span></span>
* <span data-ttu-id="755dd-234">Probleme #6833 und #7102 behoben (Bereich „Diagnoseeinstellungen“)</span><span class="sxs-lookup"><span data-stu-id="755dd-234">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="755dd-235">Probleme mit dem Standardnamen, also „service“, beim Erstellen und Auflisten/Abrufen von Diagnoseeinstellungen</span><span class="sxs-lookup"><span data-stu-id="755dd-235">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="755dd-236">Probleme beim Erstellen von Diagnoseeinstellungen mit Kategorien</span><span class="sxs-lookup"><span data-stu-id="755dd-236">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="755dd-237">Meldung zur Einstellung der Unterstützung für Metrikaggregationsintervall-Parameter</span><span class="sxs-lookup"><span data-stu-id="755dd-237">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="755dd-238">Aggregationsintervall-Parameter werden weiterhin akzeptiert (Änderung ohne Funktionsbeeinträchtigung), aber sie werden auf dem Back-End ignoriert, da nur PT1M gültig ist</span><span class="sxs-lookup"><span data-stu-id="755dd-238">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="755dd-239">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="755dd-239">AzureRM.Network</span></span>
* <span data-ttu-id="755dd-240">Änderungen an LoadBalancer-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="755dd-240">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="755dd-241">LoadBalancerInboundNatPoolConfig: Parameter IdleTimeoutInMinutes, EnableFloatingIp und EnableTcpReset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-241">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="755dd-242">LoadBalancerInboundNatRuleConfig: Parameter EnableTcpReset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-242">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="755dd-243">LoadBalancerRuleConfig: Parameter EnableTcpReset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-243">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="755dd-244">LoadBalancerProbeConfig: Unterstützung für Wert „Https“ für Parameter „Protocol“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-244">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="755dd-245">Neue Befehle für neue Unterressource „OutboundRule“ von LoadBalancer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-245">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="755dd-246">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-246">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="755dd-247">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-247">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="755dd-248">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-248">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="755dd-249">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-249">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="755dd-250">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-250">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="755dd-251">Neue HostedWorkloads-Eigenschaft für PSNetworkInterface hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-251">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="755dd-252">Neue Cmdlets für Feature: Azure Firewall über ARM</span><span class="sxs-lookup"><span data-stu-id="755dd-252">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="755dd-253">Get-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-253">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="755dd-254">Set-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-254">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="755dd-255">New-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-255">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="755dd-256">Remove-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-256">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="755dd-257">New-AzureRmFirewallApplicationRuleCollection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-257">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="755dd-258">New-AzureRmFirewallApplicationRule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-258">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="755dd-259">New-AzureRmFirewallNatRuleCollection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-259">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="755dd-260">New-AzureRmFirewallNatRule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-260">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="755dd-261">New-AzureRmFirewallNetworkRuleCollection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-261">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="755dd-262">New-AzureRmFirewallNetworkRule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-262">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="755dd-263">Unterstützung für vertrauenswürdiges Stammzertifikat und Konfiguration der automatischen Skalierung in Application Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-263">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="755dd-264">Neue Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="755dd-264">New Cmdlets added:</span></span>
      - <span data-ttu-id="755dd-265">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="755dd-265">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="755dd-266">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="755dd-266">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="755dd-267">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="755dd-267">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="755dd-268">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="755dd-268">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="755dd-269">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="755dd-269">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="755dd-270">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="755dd-270">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="755dd-271">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="755dd-271">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="755dd-272">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="755dd-272">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="755dd-273">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="755dd-273">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="755dd-274">Cmdlets mit optionalem Parameter „-TrustedRootCertificate“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-274">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="755dd-275">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="755dd-275">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="755dd-276">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="755dd-276">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="755dd-277">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="755dd-277">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="755dd-278">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="755dd-278">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="755dd-279">Cmdlets mit optionalem Parameter „-AutoscaleConfiguration“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-279">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="755dd-280">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="755dd-280">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="755dd-281">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="755dd-281">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="755dd-282">Cmdlet für Schnittstellenendpunkt Get-AzureInterfaceEndpoint hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-282">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="755dd-283">Unterstützung für mehrere Adresspräfixe in einem Subnetz hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="755dd-283">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="755dd-284">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="755dd-284">Updated cmdlets:</span></span>
  - <span data-ttu-id="755dd-285">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-285">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="755dd-286">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-286">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="755dd-287">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-287">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="755dd-288">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-288">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="755dd-289">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="755dd-289">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="755dd-290">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-290">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="755dd-291">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-291">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="755dd-292">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-292">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="755dd-293">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="755dd-293">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="755dd-294">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="755dd-294">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="755dd-295">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="755dd-295">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="755dd-296">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-296">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="755dd-297">New-AzureRmNetworkInterfaceIpConfig – Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-297">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="755dd-298">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-298">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="755dd-299">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-299">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="755dd-300">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-300">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="755dd-301">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-301">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="755dd-302">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-302">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="755dd-303">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="755dd-303">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="755dd-304">Cmdlets für die Subnetzdelegierung hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="755dd-304">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="755dd-305">New-AzureRmDelegation: Erstellt eine neue Delegierung, die einem Subnetz hinzugefügt werden kann</span><span class="sxs-lookup"><span data-stu-id="755dd-305">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="755dd-306">Remove-AzureRmDelegation: Nutzt ein Subnetz und entfernt den bereitgestellten Delegierungsnamen aus diesem Subnetz</span><span class="sxs-lookup"><span data-stu-id="755dd-306">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="755dd-307">Add-AzureRmDelegation: Nutzt ein Subnetz und fügt den angegebenen Dienstnamen diesem Subnetz als Delegierung hinzu</span><span class="sxs-lookup"><span data-stu-id="755dd-307">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="755dd-308">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="755dd-308">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="755dd-309">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="755dd-309">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="755dd-310">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="755dd-310">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="755dd-311">Unterstützung für verwalteten Datenträger</span><span class="sxs-lookup"><span data-stu-id="755dd-311">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="755dd-312">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="755dd-312">AzureRM.RedisCache</span></span>
* <span data-ttu-id="755dd-313">Insights-Abhängigkeit aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="755dd-313">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="755dd-314">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="755dd-314">AzureRM.Resources</span></span>
* <span data-ttu-id="755dd-315">New-AzureRmResourceGroupDeployment mit neuem Parameter „RollbackAction“ aktualisieren</span><span class="sxs-lookup"><span data-stu-id="755dd-315">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="755dd-316">Unterstützung für OnErrorDeployment mit dem neuen Parameter hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="755dd-316">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="755dd-317">Unterstützung für verwaltete Identität in Richtlinienzuweisungen.</span><span class="sxs-lookup"><span data-stu-id="755dd-317">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="755dd-318">Parameter mit Standardwerten sind nicht mehr erforderlich, wenn eine Richtlinie mit „New-AzureRmPolicyAssignment“ zugewiesen wird</span><span class="sxs-lookup"><span data-stu-id="755dd-318">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="755dd-319">Neues Cmdlet „Get-AzureRmPolicyAlias“ zum Abrufen von Richtlinienaliasen hinzufügen</span><span class="sxs-lookup"><span data-stu-id="755dd-319">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="755dd-320">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="755dd-320">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="755dd-321">Problem #7161 behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-321">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="755dd-322">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="755dd-322">AzureRM.SignalR</span></span>
* <span data-ttu-id="755dd-323">SKU-Namen auf Free_F1 und Standard_S1 aktualisieren</span><span class="sxs-lookup"><span data-stu-id="755dd-323">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="755dd-324">Versionsfeld zum PSSignalRResource-Objekt und Verbindungszeichenfolge zum PSSignalRKeys-Objekt hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="755dd-324">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="755dd-325">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="755dd-325">AzureRM.Storage</span></span>
* <span data-ttu-id="755dd-326">Unterstützung für Unveränderlichkeitsrichtlinie in AzureRm.Storage</span><span class="sxs-lookup"><span data-stu-id="755dd-326">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="755dd-327">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="755dd-327">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="755dd-328">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="755dd-328">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="755dd-329">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="755dd-329">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="755dd-330">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="755dd-330">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="755dd-331">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="755dd-331">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="755dd-332">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="755dd-332">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="755dd-333">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="755dd-333">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="755dd-334">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="755dd-334">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="755dd-335">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="755dd-335">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="755dd-336">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="755dd-336">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="755dd-337">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="755dd-337">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="755dd-338">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="755dd-338">AzureRM.Websites</span></span>
* <span data-ttu-id="755dd-339">Zwei neue Cmdlets hinzugefügt: Get-AzureRmDeletedWebApp und Restore-AzureRmDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="755dd-339">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="755dd-340">New-AzureRmAppServicePlan -HyperV-Switch für „App Service-Plan erstellen“ mit Windows-Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-340">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="755dd-341">New-AzureRmWebApp/New-AzureRmWebAppSlot/Set-AzureRmWebApp/Set-AzureRmWebAppSlot: Neue Parameter (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) für die Erstellung und Verwaltung der Windows-Container-App hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-341">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="755dd-342">6.8.1: August 2018</span><span class="sxs-lookup"><span data-stu-id="755dd-342">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="755dd-343">Allgemein</span><span class="sxs-lookup"><span data-stu-id="755dd-343">General</span></span>
* <span data-ttu-id="755dd-344">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="755dd-344">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="755dd-345">Allgemeine Laufzeitassemblys aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-345">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="755dd-346">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="755dd-346">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="755dd-347">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="755dd-347">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="755dd-348">Problem https://github.com/Azure/azure-powershell/issues/6603 behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-348">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="755dd-349">Die Cmdlets „Import-AzureRmApiManagementApi“ und „\*-AzureRmApiManagementCertificate“ können jetzt relative Pfade verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="755dd-349">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="755dd-350">Problem https://github.com/Azure/azure-powershell/issues/6879 behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-350">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="755dd-351">„CertificateInformation“ ist eine festlegbare Eigenschaft, die die ordnungsgemäße Funktionsweise des Cmdlets „Set-AzureRmApiManagement“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="755dd-351">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="755dd-352">Behoben durch Upgrade auf NuGet-Paket „4.0.4-preview“</span><span class="sxs-lookup"><span data-stu-id="755dd-352">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="755dd-353">Problem https://github.com/Azure/azure-powershell/issues/6853 behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-353">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="755dd-354">OData-Filter für die Suche anhand des Namens korrigiert (Produkt)</span><span class="sxs-lookup"><span data-stu-id="755dd-354">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="755dd-355">Problem https://github.com/Azure/azure-powershell/issues/6814 behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-355">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="755dd-356">OData-Filter für die Suche anhand des Namens korrigiert (API)</span><span class="sxs-lookup"><span data-stu-id="755dd-356">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="755dd-357">Unterstützung für AzureMonitor-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-357">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="755dd-358">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="755dd-358">AzureRM.Compute</span></span>
* <span data-ttu-id="755dd-359">Problem des fehlenden Ziels in der Fehlerausgabe behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-359">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="755dd-360">Problem mit dem Speicherkontotyp für den virtuellen Computer mit verwaltetem Datenträgern behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-360">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="755dd-361">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="755dd-361">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="755dd-362">AEM-Erweiterungs-Cmdlets für andere Umgebungen (etwa Azure China) korrigiert</span><span class="sxs-lookup"><span data-stu-id="755dd-362">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="755dd-363">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="755dd-363">AzureRM.Network</span></span>
* <span data-ttu-id="755dd-364">Standarddarstellung der Cmdlet-Ausgabe in Tabellenansicht geändert</span><span class="sxs-lookup"><span data-stu-id="755dd-364">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="755dd-365">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="755dd-365">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="755dd-366">Fehler in „Update-AzureRmPowerBIEmbeddedCapacity“ beim Skalieren der angehaltenen Kapazität behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-366">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="755dd-367">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="755dd-367">AzureRM.Resources</span></span>
* <span data-ttu-id="755dd-368">Problem beim Erstellen verwalteter Anwendungen über Marketplace behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-368">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="755dd-369">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="755dd-369">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="755dd-370">Behobene Probleme</span><span class="sxs-lookup"><span data-stu-id="755dd-370">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="755dd-371">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="755dd-371">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="755dd-372">Unterstützung für Routingmethode „MultiValue“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-372">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="755dd-373">Neuer Parameter „MaxReturn“ für Routingtyp „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="755dd-373">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="755dd-374">Unterstützung für Subnetzroutingmethode hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-374">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="755dd-375">Unterstützung für IP-Adressbereiche (Subnetze) in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="755dd-375">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="755dd-376">Unterstützung für benutzerdefinierte Header in Profilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-376">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="755dd-377">Unterstützung für erwartete Statuscodebereiche in Profilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-377">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="755dd-378">Unterstützung für benutzerdefinierte Header in Endpunkten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-378">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="755dd-379">6.8.0: August 2018</span><span class="sxs-lookup"><span data-stu-id="755dd-379">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="755dd-380">Allgemein</span><span class="sxs-lookup"><span data-stu-id="755dd-380">General</span></span>
* <span data-ttu-id="755dd-381">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="755dd-381">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="755dd-382">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="755dd-382">AzureRM.Profile</span></span>
* <span data-ttu-id="755dd-383">Ablaufeigenschaft zu Token hinzugefügt, die während „Connect-AzureRmAccount“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="755dd-383">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="755dd-384">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="755dd-384">AzureRM.Compute</span></span>
* <span data-ttu-id="755dd-385">Problem des fehlenden Ziels in der Fehlerausgabe behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-385">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="755dd-386">Problem mit dem Speicherkontotyp für den virtuellen Computer mit verwaltetem Datenträgern behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-386">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="755dd-387">AEM-Erweiterungs-Cmdlets für andere Umgebungen (etwa Azure China) korrigiert</span><span class="sxs-lookup"><span data-stu-id="755dd-387">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="755dd-388">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="755dd-388">AzureRM.IotHub</span></span>
* <span data-ttu-id="755dd-389">Beispiele für „New-AzureRmIotHubExportDevices“ und „New-AzureRmIotHubImportDevices“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="755dd-389">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="755dd-390">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="755dd-390">AzureRM.Network</span></span>
* <span data-ttu-id="755dd-391">Standarddarstellung von Modellen in Tabellenansicht geändert</span><span class="sxs-lookup"><span data-stu-id="755dd-391">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="755dd-392">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="755dd-392">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="755dd-393">Fehler in „Update-AzureRmPowerBIEmbeddedCapacity“ beim Skalieren der angehaltenen Kapazität behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-393">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="755dd-394">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="755dd-394">AzureRM.Resources</span></span>
* <span data-ttu-id="755dd-395">Problem beim Erstellen der verwalteten Anwendung über Marketplace behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-395">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="755dd-396">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="755dd-396">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="755dd-397">Fehlerbehebung</span><span class="sxs-lookup"><span data-stu-id="755dd-397">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="755dd-398">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="755dd-398">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="755dd-399">Unterstützung für Routingmethode „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="755dd-399">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="755dd-400">Neuer Parameter „MaxReturn“ für Routingtyp „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="755dd-400">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="755dd-401">Unterstützung für Subnetzroutingmethode</span><span class="sxs-lookup"><span data-stu-id="755dd-401">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="755dd-402">Unterstützung für IP-Adressbereiche (Subnetze) in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="755dd-402">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="755dd-403">Unterstützung für benutzerdefinierte Header in Profilen</span><span class="sxs-lookup"><span data-stu-id="755dd-403">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="755dd-404">Unterstützung für erwartete Statuscodebereiche in Profilen</span><span class="sxs-lookup"><span data-stu-id="755dd-404">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="755dd-405">Unterstützung für benutzerdefinierte Header in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="755dd-405">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="755dd-406">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="755dd-406">AzureRM.Websites</span></span>
* <span data-ttu-id="755dd-407">Das Problem, dass die Standardressourcengruppe falsch festgelegt wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="755dd-407">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="755dd-408">6.7.0: August 2018</span><span class="sxs-lookup"><span data-stu-id="755dd-408">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="755dd-409">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="755dd-409">AzureRM.Profile</span></span>
* <span data-ttu-id="755dd-410">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-410">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="755dd-411">Benutzer-ID zum Standardkontextnamen hinzugefügt, um Kontextkonflikte zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="755dd-411">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="755dd-412">Probleme mit „Clear-AzureRmContext“ behoben, die Fehler beim Auswählen eines Kontexts verursacht haben (6398)</span><span class="sxs-lookup"><span data-stu-id="755dd-412">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="755dd-413">Ermöglicht, dass für „Connect-AzureRmAccount“ die Mandantendomäne an den Parameter „-TenantId“ übergeben wird</span><span class="sxs-lookup"><span data-stu-id="755dd-413">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="755dd-414">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="755dd-414">Azure.Storage</span></span>
* <span data-ttu-id="755dd-415">Begrenzung von 5 TB für das Kontingent der Azure-Dateifreigabe entfernt</span><span class="sxs-lookup"><span data-stu-id="755dd-415">Remove the 5TB limitation for Azure File Share quota</span></span>
* <span data-ttu-id="755dd-416">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="755dd-416">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="755dd-417">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="755dd-417">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="755dd-418">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-418">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="755dd-419">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="755dd-419">Azure.AnalysisServices</span></span>
* <span data-ttu-id="755dd-420">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-420">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="755dd-421">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="755dd-421">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="755dd-422">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-422">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="755dd-423">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="755dd-423">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="755dd-424">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-424">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="755dd-425">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="755dd-425">AzureRM.Automation</span></span>
* <span data-ttu-id="755dd-426">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-426">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="755dd-427">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="755dd-427">AzureRM.Backup</span></span>
* <span data-ttu-id="755dd-428">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-428">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="755dd-429">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="755dd-429">AzureRM.Batch</span></span>
* <span data-ttu-id="755dd-430">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-430">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="755dd-431">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="755dd-431">AzureRM.Billing</span></span>
* <span data-ttu-id="755dd-432">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-432">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="755dd-433">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="755dd-433">AzureRM.Cdn</span></span>
* <span data-ttu-id="755dd-434">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-434">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="755dd-435">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="755dd-435">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="755dd-436">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-436">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="755dd-437">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="755dd-437">AzureRM.Compute</span></span>
* <span data-ttu-id="755dd-438">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-438">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="755dd-439">EvictionPolicy-Parameter zu „New-AzureRmVmssConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-439">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="755dd-440">Standort in „DiskFileParameterSet“ von „New-AzureRmVm“ angeben, wenn kein Ort angegeben ist</span><span class="sxs-lookup"><span data-stu-id="755dd-440">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="755dd-441">Parameterbeschreibung in „Save-AzureRmVMImage“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="755dd-441">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="755dd-442">Cmdlet „Get-AzureRmVMDiskEncryptionStatus“ für bestimmte Szenarien im Zusammenhang mit einem Durchlauf korrigiert</span><span class="sxs-lookup"><span data-stu-id="755dd-442">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="755dd-443">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="755dd-443">AzureRM.Consumption</span></span>
* <span data-ttu-id="755dd-444">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-444">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="755dd-445">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="755dd-445">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="755dd-446">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-446">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="755dd-447">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="755dd-447">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="755dd-448">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-448">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="755dd-449">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="755dd-449">AzureRM.DataFactories</span></span>
* <span data-ttu-id="755dd-450">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-450">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="755dd-451">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="755dd-451">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="755dd-452">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-452">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="755dd-453">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="755dd-453">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="755dd-454">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-454">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="755dd-455">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="755dd-455">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="755dd-456">Debuggen korrigiert, wenn „DebugPreference“ über die PowerShell-Befehlszeile festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="755dd-456">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="755dd-457">Beispiel für „Set-AzureRmDataLakeStoreItemAcl“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-457">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="755dd-458">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="755dd-458">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="755dd-459">Beispiel für „Set-AzureRmDataLakeStoreItemAclEntry“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-459">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="755dd-460">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="755dd-460">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="755dd-461">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-461">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="755dd-462">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="755dd-462">AzureRM.Dns</span></span>
* <span data-ttu-id="755dd-463">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-463">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="755dd-464">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="755dd-464">AzureRM.EventGrid</span></span>
* <span data-ttu-id="755dd-465">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-465">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="755dd-466">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="755dd-466">AzureRM.EventHub</span></span>
* <span data-ttu-id="755dd-467">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-467">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="755dd-468">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="755dd-468">AzureRM.HDInsight</span></span>
* <span data-ttu-id="755dd-469">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-469">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="755dd-470">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="755dd-470">AzureRM.Insights</span></span>
* <span data-ttu-id="755dd-471">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-471">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="755dd-472">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="755dd-472">AzureRM.IotHub</span></span>
* <span data-ttu-id="755dd-473">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-473">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="755dd-474">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="755dd-474">AzureRM.KeyVault</span></span>
* <span data-ttu-id="755dd-475">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-475">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="755dd-476">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="755dd-476">AzureRM.LogicApp</span></span>
* <span data-ttu-id="755dd-477">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-477">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="755dd-478">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="755dd-478">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="755dd-479">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-479">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="755dd-480">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="755dd-480">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="755dd-481">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-481">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="755dd-482">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="755dd-482">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="755dd-483">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-483">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="755dd-484">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="755dd-484">AzureRM.Media</span></span>
* <span data-ttu-id="755dd-485">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-485">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="755dd-486">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="755dd-486">AzureRM.Network</span></span>
* <span data-ttu-id="755dd-487">Beispiel für „Set-AzureRmLocalNetworkGateway“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-487">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="755dd-488">Beispiele und Beschreibungen für „Add-AzureRmVirtualNetworkGatewayIpConfig“, „Get-AzureRmVirtualNetworkGatewayConnectionSharedKey“ und „New-AzureRmVirtualNetworkGatewayConnection“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-488">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="755dd-489">Beispiele für „Remove-AzureRmVirtualNetworkGatewayIpConfig“ und „Reset-AzureRmVirtualNetworkGateway“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-489">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="755dd-490">Beispiel für „Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-490">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="755dd-491">Beispiel für „Set-AzureRmVirtualNetworkGatewayConnectionSharedKey“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-491">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="755dd-492">Beispiel für „Set-AzureRmVirtualNetworkGatewayConnection“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-492">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="755dd-493">Cmdlets für „ApplicationSecurityGroup“, „RouteTable“ und „Usage“ mithilfe des aktuellen Code-Generators erneut erstellt</span><span class="sxs-lookup"><span data-stu-id="755dd-493">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="755dd-494">Deutlichere Formulierung der Fehlermeldung für „Get-AzureRmVirtualNetworkSubnetConfig“, wenn ein nicht vorhandenes Subnetz abgerufen wird</span><span class="sxs-lookup"><span data-stu-id="755dd-494">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="755dd-495">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="755dd-495">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="755dd-496">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-496">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="755dd-497">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="755dd-497">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="755dd-498">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-498">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="755dd-499">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="755dd-499">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="755dd-500">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-500">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="755dd-501">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="755dd-501">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="755dd-502">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-502">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="755dd-503">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="755dd-503">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="755dd-504">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-504">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="755dd-505">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="755dd-505">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="755dd-506">Richtlinienfilter zum Cmdlet „Get-AzureRmRecoveryServicesBackItem“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="755dd-506">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="755dd-507">Der Befehl gibt die Liste der Sicherungselemente zurück, die durch die angegebene Richtlinien-ID geschützt sind.</span><span class="sxs-lookup"><span data-stu-id="755dd-507">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="755dd-508">„Microsoft.Azure.Management.RecoveryServices.Backup“ auf Version 3.0.0-preview aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-508">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="755dd-509">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-509">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="755dd-510">TargetResourceGroupName-Parameter zu „Restore-AzureRmRecoveryServicesBackupItem“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="755dd-510">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="755dd-511">Die Ressourcengruppe, in der die verwalteten Datenträger wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="755dd-511">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="755dd-512">Gilt für die Sicherung des virtuellen Computers mit verwalteten Datenträgern.</span><span class="sxs-lookup"><span data-stu-id="755dd-512">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="755dd-513">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="755dd-513">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="755dd-514">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-514">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="755dd-515">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="755dd-515">AzureRM.RedisCache</span></span>
* <span data-ttu-id="755dd-516">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-516">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="755dd-517">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="755dd-517">AzureRM.Relay</span></span>
* <span data-ttu-id="755dd-518">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-518">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="755dd-519">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="755dd-519">AzureRM.Resources</span></span>
* <span data-ttu-id="755dd-520">Unterstützung der Vorlagenbereitstellung im Abonnementbereich.</span><span class="sxs-lookup"><span data-stu-id="755dd-520">Support template deployment at subscription scope.</span></span> <span data-ttu-id="755dd-521">Neue Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="755dd-521">Add new Cmdlets:</span></span>
    - <span data-ttu-id="755dd-522">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="755dd-522">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="755dd-523">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="755dd-523">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="755dd-524">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="755dd-524">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="755dd-525">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="755dd-525">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="755dd-526">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="755dd-526">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="755dd-527">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="755dd-527">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="755dd-528">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="755dd-528">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="755dd-529">Problem behoben, aufgrund dessen beim Übergeben eines Kontexts an „Set-AzureRmResource“ ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="755dd-529">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="755dd-530">Beispiel in „New-AzureRmResourceGroupDeployment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="755dd-530">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="755dd-531">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-531">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="755dd-532">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="755dd-532">AzureRM.Scheduler</span></span>
* <span data-ttu-id="755dd-533">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-533">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="755dd-534">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="755dd-534">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="755dd-535">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-535">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="755dd-536">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="755dd-536">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="755dd-537">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-537">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="755dd-538">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="755dd-538">AzureRM.Sql</span></span>
* <span data-ttu-id="755dd-539">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-539">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="755dd-540">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="755dd-540">AzureRM.Storage</span></span>
* <span data-ttu-id="755dd-541">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-541">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="755dd-542">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="755dd-542">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="755dd-543">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-543">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="755dd-544">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="755dd-544">AzureRM.Tags</span></span>
* <span data-ttu-id="755dd-545">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-545">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="755dd-546">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="755dd-546">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="755dd-547">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-547">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="755dd-548">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="755dd-548">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="755dd-549">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-549">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="755dd-550">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="755dd-550">AzureRM.Websites</span></span>
* <span data-ttu-id="755dd-551">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-551">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="755dd-552">6.6.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="755dd-552">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="755dd-553">Allgemein</span><span class="sxs-lookup"><span data-stu-id="755dd-553">General</span></span>
* <span data-ttu-id="755dd-554">Alle Hilfedateien aktualisiert, um vollständige Parametertypen und die richtigen Eingabe/Ausgabe-Typen einzuschließen.</span><span class="sxs-lookup"><span data-stu-id="755dd-554">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="755dd-555">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="755dd-555">AzureRM.Profile</span></span>
* <span data-ttu-id="755dd-556">Bibliothek „Common.Strategy“ aktualisiert, um überprüfen zu können, ob die aktuelle Konfiguration für eine Ressource mit der Zielressource kompatibel ist.</span><span class="sxs-lookup"><span data-stu-id="755dd-556">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="755dd-557">ps1xml-Typen zu „Common.Storage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-557">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="755dd-558">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="755dd-558">Azure.Storage</span></span>
* <span data-ttu-id="755dd-559">Unterstützung zum Abrufen von Speicherkontext aus „DefaultProfile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-559">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="755dd-560">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-560">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="755dd-561">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="755dd-561">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="755dd-562">Problem https://github.com/Azure/azure-powershell/issues/6370 behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-562">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="755dd-563">Fehler in Automapper behoben, um „PsApiManagementApi“ in „ApiContract“ zu verschieben</span><span class="sxs-lookup"><span data-stu-id="755dd-563">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="755dd-564">Problem https://github.com/Azure/azure-powershell/issues/6515 behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-564">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="755dd-565">Fehler in „File.Save“ behoben, um Überladung mit Codierungstyp zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="755dd-565">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="755dd-566">Problem https://github.com/Azure/azure-powershell/issues/6560 behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-566">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="755dd-567">Upgrade auf Nuget-Version 4.0.3 durchgeführt, in der Musterausnahme in „apiId“ behoben wurde</span><span class="sxs-lookup"><span data-stu-id="755dd-567">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="755dd-568">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="755dd-568">AzureRM.Compute</span></span>
* <span data-ttu-id="755dd-569">Das Problem, aufgrund dessen beim Erstellen eines virtuellen Computers mithilfe von „DiskFileParameterSet“ in „New-AzureRmVm“ wegen einer Umbenennung des Speicherkontotyps „PremiumLRS“ ein Fehler auftrat, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="755dd-569">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="755dd-570">Cmdlet „Invoke-AzureRmVMRunCommand“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="755dd-570">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="755dd-571">„Get-AzureRmAvailabilitySet“ aktualisiert, um die Auflistung aller Verfügbarkeitsgruppen in einem Abonnement zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="755dd-571">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="755dd-572">(ResouceGroupName-Parameter ist jetzt optional.)</span><span class="sxs-lookup"><span data-stu-id="755dd-572">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="755dd-573">„SimpleParameterSet“ von „New-AzureRmVm“ aktualisiert, um Accelerated Networking auf kompatiblen virtuellen Computern zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="755dd-573">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="755dd-574">Einfacher Parametersatz „New-AzureRmVmss“ aktualisiert, sodass das Erstellen der VMSS fehlschlägt, wenn bereits ein benutzerdefinierter LB vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="755dd-574">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="755dd-575">Beispiel für „New-AzureRmDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-575">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="755dd-576">Beispiel für „New-AzureRmVM“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-576">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="755dd-577">Beschreibung für „Set-AzureRmVMOSDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-577">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="755dd-578">Beispiel 1 für „Set-AzureRmVMBginfoExtension“ aktualisiert, um Rechtschreibung und Präfix zu korrigieren.</span><span class="sxs-lookup"><span data-stu-id="755dd-578">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="755dd-579">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="755dd-579">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="755dd-580">ADF .Net SDK-Version auf 1.1.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="755dd-580">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="755dd-581">Unterstützung der Freigabe der selbstgehosteten Integration Runtime über Data Factorys hinweg.</span><span class="sxs-lookup"><span data-stu-id="755dd-581">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="755dd-582">Neuer Parameter „-SharedIntegrationRuntimeResourceId“ zu Cmdlet „Set-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="755dd-582">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="755dd-583">Neuer optionaler Parameter „-LinkedDataFactoryName“ zu Cmdlet „Remove-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="755dd-583">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="755dd-584">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="755dd-584">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="755dd-585">DataPlane SDK-Version (Microsoft.Azure.DataLake.Store) auf 1.1.9 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-585">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="755dd-586">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="755dd-586">AzureRM.EventHub</span></span>
* <span data-ttu-id="755dd-587">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-587">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="755dd-588">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="755dd-588">AzureRM.Insights</span></span>
* <span data-ttu-id="755dd-589">Formatierung von „OutputType“ in Hilfedateien korrigiert</span><span class="sxs-lookup"><span data-stu-id="755dd-589">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="755dd-590">Verwendung von Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span><span class="sxs-lookup"><span data-stu-id="755dd-590">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="755dd-591">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="755dd-591">AzureRM.KeyVault</span></span>
* <span data-ttu-id="755dd-592">Piping-Problem in „Set-AzureRmKeyVaultAccessPolicy“ behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-592">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="755dd-593">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="755dd-593">AzureRM.Network</span></span>
* <span data-ttu-id="755dd-594">Beispiele für LoadBalancerInboundNatPoolConfig-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="755dd-594">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="755dd-595">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="755dd-595">AzureRM.Resources</span></span>
* <span data-ttu-id="755dd-596">Problem beim Angeben sowohl des Tag-Namens als auch des Werts für „Get-AzureRmResource“ behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-596">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="755dd-597">Piping-Szenario mit „Set-AzureRmResource“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="755dd-597">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="755dd-598">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="755dd-598">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="755dd-599">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-599">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="755dd-600">Einige Probleme behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-600">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="755dd-601">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="755dd-601">AzureRM.Sql</span></span>
* <span data-ttu-id="755dd-602">Unterstützung für Advanced Threat Protection für Server bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="755dd-602">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="755dd-603">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="755dd-603">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="755dd-604">Unterstützung für Sicherheitsrisikobewertung bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="755dd-604">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="755dd-605">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="755dd-605">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="755dd-606">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="755dd-606">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="755dd-607">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="755dd-607">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="755dd-608">Beispiel in „Remove-AzureRmSqlServerFirewallRule“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="755dd-608">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="755dd-609">Falsche Verarbeitung von „datetime“ für nicht US-basierte Kultur in „Get-AzureSqlSyncGroupLog“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="755dd-609">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="755dd-610">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="755dd-610">AzureRM.Storage</span></span>
* <span data-ttu-id="755dd-611">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-611">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="755dd-612">Cmdlet-Ausgabe von „StorageAccount“ in Tabellenansicht anzeigen</span><span class="sxs-lookup"><span data-stu-id="755dd-612">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="755dd-613">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="755dd-613">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="755dd-614">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="755dd-614">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="755dd-615">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="755dd-615">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="755dd-616">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="755dd-616">AzureRM.Tags</span></span>
* <span data-ttu-id="755dd-617">Falsche Anweisung aus Tag-Cmdlet-Hilfe entfernt</span><span class="sxs-lookup"><span data-stu-id="755dd-617">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="755dd-618">6.5.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="755dd-618">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="755dd-619">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="755dd-619">AzureRM.Profile</span></span>
* <span data-ttu-id="755dd-620">Hilfe für „Get-AzureRmContextAutosaveSetting“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-620">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="755dd-621">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="755dd-621">Azure.Storage</span></span>
* <span data-ttu-id="755dd-622">Unterstützung des Blob- oder Dateiuploads mit lesegeschütztem SAS-Token</span><span class="sxs-lookup"><span data-stu-id="755dd-622">Support Upload Blob or File with write only Sas token</span></span>
* <span data-ttu-id="755dd-623">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="755dd-623">Set-AzureStorageBlobContent</span></span>
* <span data-ttu-id="755dd-624">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="755dd-624">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="755dd-625">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="755dd-625">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="755dd-626">Erforderliche Eigenschaft „ResourceGroupName“ zu AS hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="755dd-626">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="755dd-627">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="755dd-627">AzureRM.Automation</span></span>
* <span data-ttu-id="755dd-628">Hilfe aktualisiert und Beispiel für „New-AzureRMAutomationSchedule“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-628">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="755dd-629">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="755dd-629">AzureRM.Compute</span></span>
* <span data-ttu-id="755dd-630">Parameter „-Tag“ zu „Update/New-AzureRmAvailabilitySet“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-630">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="755dd-631">Beispiel für „Add-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-631">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="755dd-632">Beispiele für „Remove-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-632">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="755dd-633">Hilfe für „Set-AzureRmVMAccessExtension“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-633">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="755dd-634">„SimpleParameterSet“ für „New-AzureRmVmss“ so aktualisiert, dass „SinglePlacementGroup“ standardmäßig auf „false“ festgelegt ist, und Switch-Parameter „SinglePlacementGroup“ hinzugefügt, der dem Benutzer das Erstellen der VMSS in einer einzelnen Platzierungsgruppe ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="755dd-634">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="755dd-635">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="755dd-635">AzureRM.EventHub</span></span>
* <span data-ttu-id="755dd-636">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSEventHubDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="755dd-636">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="755dd-637">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="755dd-637">AzureRM.KeyVault</span></span>
* <span data-ttu-id="755dd-638">Fehlermeldung für „Set-AzureRmKeyVaultAccessPolicy“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-638">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="755dd-639">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="755dd-639">AzureRM.LogicApp</span></span>
* <span data-ttu-id="755dd-640">Fehler „Parametersatz konnte nicht aufgelöst werden“ in „New-AzureRmLogicApp“behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-640">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="755dd-641">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="755dd-641">AzureRM.Network</span></span>
* <span data-ttu-id="755dd-642">Peering über mehrere virtuelle Netzwerke in mehreren Mandanten für „Set/Add-AzureRmVirtualNetworkPeering“ aktiviert</span><span class="sxs-lookup"><span data-stu-id="755dd-642">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="755dd-643">Folgende Cmdlets für Application Gateway aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-643">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="755dd-644">New-AzureRmApplicationGateway: EnableFIPS-Flag und Zonenunterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-644">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="755dd-645">New-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-645">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="755dd-646">Set-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-646">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="755dd-647">RouteTable-Cmdlets mit aktueller Generatorversion erneut generiert</span><span class="sxs-lookup"><span data-stu-id="755dd-647">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="755dd-648">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="755dd-648">AzureRM.Relay</span></span>
* <span data-ttu-id="755dd-649">Markdowndateien aktualisiert, Problem mit Parametername in Beispiel behoben</span><span class="sxs-lookup"><span data-stu-id="755dd-649">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="755dd-650">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="755dd-650">AzureRM.Resources</span></span>
* <span data-ttu-id="755dd-651">Roleassignment- und roledefinition-Cmdlets aktualisiert:</span><span class="sxs-lookup"><span data-stu-id="755dd-651">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="755dd-652">Zusätzliche roledefinition-Aufrufe entfernt, die als Teil des Pagings durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="755dd-652">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="755dd-653">Get-AzureRmRoleAssignment-Cmdlet korrigiert</span><span class="sxs-lookup"><span data-stu-id="755dd-653">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="755dd-654">Befehlsparameterfunktion von „-ExpandPrincipalGroups“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="755dd-654">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="755dd-655">Problem mit „Get-AzureRmResource“ behoben, aufgrund dessen die Groß-/Kleinschreibung des Parameters „-ResourceType“ beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="755dd-655">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="755dd-656">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="755dd-656">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="755dd-657">top- und skip-Parameter zu Listen-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-657">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="755dd-658">Cmdlets für die Migration von Standard- zu Premium-Namespace hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="755dd-658">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="755dd-659">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="755dd-659">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="755dd-660">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="755dd-660">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="755dd-661">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="755dd-661">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="755dd-662">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="755dd-662">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="755dd-663">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="755dd-663">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="755dd-664">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSServiceBusDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="755dd-664">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="755dd-665">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="755dd-665">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="755dd-666">Beispiel für „New-AzureRmServiceFabricCluster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-666">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="755dd-667">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="755dd-667">AzureRM.Sql</span></span>
* <span data-ttu-id="755dd-668">Neue Cmdlets für „Management.Sql“ hinzugefügt, um Kunden das Hinzufügen des TDE-Zertifikats zu einer SQL Server-Instanz oder einer verwalteten Instanz zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="755dd-668">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="755dd-669">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="755dd-669">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="755dd-670">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="755dd-670">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="755dd-671">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="755dd-671">AzureRM.Websites</span></span>
* <span data-ttu-id="755dd-672">Wenn `Set-AzureRmWebApp -AssignIdentity` und `Set-AzureRmWebAppSlot -AssignIdentity` auf „false“ festgelegt sind, wird jetzt die Identity-Eigenschaft aus dem Websiteobjekt entfernt. Auch das Vorschau-Tag wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="755dd-672">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="755dd-673">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics`-Beispiel aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-673">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="755dd-674">Unterstützung von `Set-AzureRmWebApp -PhpVersion` als gültige PHP-Version eingestellt</span><span class="sxs-lookup"><span data-stu-id="755dd-674">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="755dd-675">6.4.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="755dd-675">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="755dd-676">Allgemein</span><span class="sxs-lookup"><span data-stu-id="755dd-676">General</span></span>
* <span data-ttu-id="755dd-677">Formatierung von OutputType in Hilfedateien für die meisten Module korrigiert</span><span class="sxs-lookup"><span data-stu-id="755dd-677">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="755dd-678">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="755dd-678">AzureRM.Profile</span></span>
* <span data-ttu-id="755dd-679">Attribut „Ps1Xml“ wurde den Standardausgabetypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-679">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="755dd-680">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="755dd-680">AzureRM.Compute</span></span>
* <span data-ttu-id="755dd-681">IP-Tag-Funktion für VMSS</span><span class="sxs-lookup"><span data-stu-id="755dd-681">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="755dd-682">Cmdlet „New-AzureRmVmssIpTagConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-682">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="755dd-683">IpTag-Parameter zu „New-AzureRmVmssIpConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-683">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="755dd-684">Funktion für automatisches Betriebssystemrollback für VMSS</span><span class="sxs-lookup"><span data-stu-id="755dd-684">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="755dd-685">DisableAutoRollback-Parameter zu „New-AzureRmVmssConfig“ und „Update-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-685">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="755dd-686">Funktion für Upgradeverlauf des Betriebssystems für VMSS</span><span class="sxs-lookup"><span data-stu-id="755dd-686">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="755dd-687">Switch-Parameter „OSUpgradeHistory“ zu „Get-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-687">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="755dd-688">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="755dd-688">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="755dd-689">Unterstützung für Katalog-ACLs über die folgenden Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="755dd-689">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="755dd-690">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="755dd-690">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="755dd-691">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="755dd-691">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="755dd-692">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="755dd-692">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="755dd-693">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="755dd-693">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="755dd-694">Abbruchunterstützung und Nachverfolgung des Fortschritts für „Set-AzureRmDataLakeStoreItemAclEntry“, „Remove-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-694">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="755dd-695">Abbruchunterstützung „Export-AzureRmDataLakeStoreChildItemProperties“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-695">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="755dd-696">Leerung von Debugmeldungen für Cmdlets korrigiert, die rekursive Vorgänge durchführt</span><span class="sxs-lookup"><span data-stu-id="755dd-696">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="755dd-697">Speicherort des Test von DataLake-Cmdlets korrigiert</span><span class="sxs-lookup"><span data-stu-id="755dd-697">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="755dd-698">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="755dd-698">AzureRM.EventHub</span></span>
* <span data-ttu-id="755dd-699">Optionaler Parameter „MaxCount“ zu Listenvorgangs-Cmdlets „Get-AzureRmEventHub“ und „Get-AzureRmEventHubConsumerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-699">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="755dd-700">Problem in Cmdlet „New-AzureRmEventHub“ behoben, aufgrund dessen beim Erstellen einer neuen EventHub-Instanz mindestens ein Parameter benötigt wurde.</span><span class="sxs-lookup"><span data-stu-id="755dd-700">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="755dd-701">Standardparametersatz wurde bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="755dd-701">Provided Default Parameter set.</span></span>
* <span data-ttu-id="755dd-702">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmEventHubKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="755dd-702">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="755dd-703">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="755dd-703">AzureRM.KeyVault</span></span>
* <span data-ttu-id="755dd-704">Problem behoben, aufgrund dessen von „Get-AzureRmKeyVault -Tag“ alle Ressourcen zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="755dd-704">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="755dd-705">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="755dd-705">AzureRM.Network</span></span>
* <span data-ttu-id="755dd-706">Neue SKUs für zonenredundante VirtualNetworkGateways-Instanzen verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="755dd-706">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="755dd-707">Neue Befehle für Funktion hinzugefügt: ExpressRoute-Partner-APIs über ARM</span><span class="sxs-lookup"><span data-stu-id="755dd-707">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="755dd-708">Get-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-708">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="755dd-709">Set-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-709">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="755dd-710">Add-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-710">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="755dd-711">Get-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-711">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="755dd-712">Remove-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-712">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="755dd-713">Get-AzureRMExpressRouteCrossConnectionArpTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-713">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="755dd-714">Get-AzureRMExpressRouteCrossConnectionRouteTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-714">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="755dd-715">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-715">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="755dd-716">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="755dd-716">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="755dd-717">Cmdlet „Get-AzureRmRecoveryServicesBackupStatus“ wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="755dd-717">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="755dd-718">Dieses Cmdlet überprüft anhand der ID eines virtuellen Computers, ob dieser durch einen Tresor im Abonnement geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="755dd-718">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="755dd-719">Wenn ein solcher Tresor vorhanden ist, gibt das Cmdlet die Tresordetails aus.</span><span class="sxs-lookup"><span data-stu-id="755dd-719">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="755dd-720">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="755dd-720">AzureRM.Resources</span></span>
* <span data-ttu-id="755dd-721">Cmdlets vom Typ „Get-AzureRmPolicyAssignment“ aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="755dd-721">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="755dd-722">Unterstützung für das Auflisten von „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-722">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="755dd-723">Unterstützung für das Abrufen einzelner Arbeitsaufträge mit „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-723">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="755dd-724">Switches „-Effective“ und „-All“ zu Steuerparameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-724">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="755dd-725">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicyDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-725">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="755dd-726">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="755dd-726">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="755dd-727">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="755dd-727">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="755dd-728">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicySetDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-728">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="755dd-729">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="755dd-729">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="755dd-730">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="755dd-730">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="755dd-731">Unterstützung für KeyVault-Geheimnisverweis in Parametern hinzugefügt, wenn „TemplateParameterObject“ in „New-AzureRmResourceGroupDeployment“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="755dd-731">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="755dd-732">Problem behoben, aufgrund dessen, der Parameter „-EndDate“ für „New-AzureRmADAppCredential“ ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="755dd-732">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="755dd-733">Problem behoben, aufgrund dessen „Add-AzureRmADGroupMember“ eine falsche URL für Anforderungen verwendete</span><span class="sxs-lookup"><span data-stu-id="755dd-733">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="755dd-734">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="755dd-734">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="755dd-735">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmServiceBusKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="755dd-735">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="755dd-736">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="755dd-736">AzureRM.Sql</span></span>
* <span data-ttu-id="755dd-737">Benutzerdefinierte Wiederherstellungspunkte für SQLDW in Hilfe zu „New-AzureRmSqlDatabaseRestorePoint“ erläutert</span><span class="sxs-lookup"><span data-stu-id="755dd-737">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="755dd-738">Dokumentation von Parameter „-ComputeGeneration“ in mehreren Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-738">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="755dd-739">6.3.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="755dd-739">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="755dd-740">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="755dd-740">AzureRM.Profile</span></span>
* <span data-ttu-id="755dd-741">Aktualisierte Fehlermeldungen für „Enable-AzureRmContextAutoSave“</span><span class="sxs-lookup"><span data-stu-id="755dd-741">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="755dd-742">Erstellen eines Kontexts für jedes Abonnement beim Ausführen von „Connect-AzureRmAccount“ ohne vorherigen Kontext</span><span class="sxs-lookup"><span data-stu-id="755dd-742">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="755dd-743">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="755dd-743">Azure.Storage</span></span>
* <span data-ttu-id="755dd-744">Zusätzliche Informationen zum Parameter „-Permissions“ in Hilfedateien</span><span class="sxs-lookup"><span data-stu-id="755dd-744">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="755dd-745">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="755dd-745">AzureRM.Compute</span></span>
* <span data-ttu-id="755dd-746">„Get-AzureRmVmDiskEncryptionStatus“ behebt ein Problem, das bei virtuellen Computern ohne Datenträger festgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="755dd-746">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="755dd-747">Version der Computeclientbibliothek aktualisiert, um folgende Cmdlets zu korrigieren:</span><span class="sxs-lookup"><span data-stu-id="755dd-747">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="755dd-748">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="755dd-748">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="755dd-749">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="755dd-749">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="755dd-750">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="755dd-750">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="755dd-751">Die folgenden Cmdlets wurden korrigiert, um die Vorgangs-ID und den Vorgangsstatus korrekt anzuzeigen:</span><span class="sxs-lookup"><span data-stu-id="755dd-751">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="755dd-752">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="755dd-752">Start-AzureRmVM</span></span>
    - <span data-ttu-id="755dd-753">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="755dd-753">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="755dd-754">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="755dd-754">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="755dd-755">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="755dd-755">Set-AzureRmVM</span></span>
    - <span data-ttu-id="755dd-756">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="755dd-756">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="755dd-757">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="755dd-757">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="755dd-758">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="755dd-758">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="755dd-759">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="755dd-759">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="755dd-760">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="755dd-760">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="755dd-761">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="755dd-761">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="755dd-762">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="755dd-762">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="755dd-763">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="755dd-763">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="755dd-764">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="755dd-764">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="755dd-765">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="755dd-765">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="755dd-766">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="755dd-766">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="755dd-767">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="755dd-767">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="755dd-768">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="755dd-768">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="755dd-769">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="755dd-769">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="755dd-770">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="755dd-770">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="755dd-771">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="755dd-771">AzureRM.EventGrid</span></span>
* <span data-ttu-id="755dd-772">ValidateNotNullOrEmpty-Überprüfungskonditionen für „SubjectBeginsWith“/„SubjectEndsWith“ im Cmdlet „Update-AzureRmEventGridSubscription“ wurden entfernt, um bei Bedarf die Änderung dieser Parameter in eine leere Zeichenfolge zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="755dd-772">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="755dd-773">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="755dd-773">AzureRM.KeyVault</span></span>
* <span data-ttu-id="755dd-774">Ein Problem wurde behoben, aufgrund dessen bei Ausführung von „Get-AzureRmKeyVault -Tag“ keine Tags zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="755dd-774">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="755dd-775">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="755dd-775">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="755dd-776">Offizielle Veröffentlichung von Policy Insights-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="755dd-776">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="755dd-777">Verwendung der API-Version 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="755dd-777">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="755dd-778">„PolicyDefinitionReferenceId“ zu den Ergebnissen von „Get-AzureRmPolicyStateSummary“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-778">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="755dd-779">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="755dd-779">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="755dd-780">Parameter „-Vault“ zu den RecoveryServices.Backup-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="755dd-780">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="755dd-781">Bei der Übergabe wird dadurch das Cmdlet „Set-AzureRmRecoveryServicesContext“ außer Kraft gesetzt.</span><span class="sxs-lookup"><span data-stu-id="755dd-781">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="755dd-782">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="755dd-782">AzureRM.Sql</span></span>
* <span data-ttu-id="755dd-783">Aktualisiertes Beispiel in der Hilfedatei für „Get-AzureRmSqlDatabaseExpanded“</span><span class="sxs-lookup"><span data-stu-id="755dd-783">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="755dd-784">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="755dd-784">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="755dd-785">Hilfedatei für „Add-AzureRmTrafficManagerEndpointConfig“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="755dd-785">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="755dd-786">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="755dd-786">AzureRM.Websites</span></span>
* <span data-ttu-id="755dd-787">„Set-AzureRmWebApp“ wurde aktualisiert, damit „AppSettings“ bei der Verwendung von „-AssignIdentity“ nicht außer Kraft gesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="755dd-787">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="755dd-788">„New-AzureRmWebAppSlot“ wurde aktualisiert, um „AppServicePlan“ als optionalen Parameter anzuerkennen</span><span class="sxs-lookup"><span data-stu-id="755dd-788">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="755dd-789">6.2.1: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="755dd-789">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="755dd-790">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="755dd-790">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="755dd-791">PSWorkspace-Modell aktualisiert, damit das Netzwerk „type“ als Parameter verwenden kann</span><span class="sxs-lookup"><span data-stu-id="755dd-791">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="755dd-792">6.2.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="755dd-792">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="755dd-793">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="755dd-793">AzureRM.Profile</span></span>
* <span data-ttu-id="755dd-794">Beheben des Problems, aufgrund dessen Version 10.0.3 von Newtonsoft.Json beim Modulimport nicht geladen wurde</span><span class="sxs-lookup"><span data-stu-id="755dd-794">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="755dd-795">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="755dd-795">AzureRM.Compute</span></span>
* <span data-ttu-id="755dd-796">Feature zum Aktualisieren von virtuellen VMSS-Computern</span><span class="sxs-lookup"><span data-stu-id="755dd-796">VMSS VM Update feature</span></span>
    - <span data-ttu-id="755dd-797">Cmdlets „Update-AzureRmVmssVM“ und „New-AzureRmVMDataDisk“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-797">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="755dd-798">Fügen Sie den Parameter „VirtualMachineScaleSetVM“ zum Cmdlet „Add-AzureRmVMDataDisk“ hinzu, um das Hinzufügen eines Datenträgers zum virtuellen VMSS-Computer zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="755dd-798">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="755dd-799">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="755dd-799">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="755dd-800">Aktualisierung der ADF .Net SDK-Version auf 0.8.0-preview mit den folgenden Änderungen:</span><span class="sxs-lookup"><span data-stu-id="755dd-800">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="755dd-801">Vorgang zum Konfigurieren des Factoryrepositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-801">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="755dd-802">Der verknüpfte QuickBooks-Dienst wurde aktualisiert, um die Eigenschaften „consumerKey“ und „consumerSecret“ verfügbar zu machen.</span><span class="sxs-lookup"><span data-stu-id="755dd-802">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="755dd-803">Aktualisierung verschiedener Modelltypen von „SecretBase“ auf „Object“</span><span class="sxs-lookup"><span data-stu-id="755dd-803">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="755dd-804">Blobereignisauslöser hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-804">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="755dd-805">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="755dd-805">AzureRM.KeyVault</span></span>
* <span data-ttu-id="755dd-806">Aktualisierung der Dokumentation mit Beispielausgabe</span><span class="sxs-lookup"><span data-stu-id="755dd-806">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="755dd-807">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="755dd-807">AzureRM.Network</span></span>
* <span data-ttu-id="755dd-808">Aktivierung der Traffic Analytics-Parameter für Network Watcher-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="755dd-808">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="755dd-809">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="755dd-809">AzureRM.Resources</span></span>
* <span data-ttu-id="755dd-810">Behebung des Problems mit der Eigenschaft „Properties“ von PSResource-Objekten, die von „Get-AzureRmResource“ zurückgegeben wurden</span><span class="sxs-lookup"><span data-stu-id="755dd-810">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="755dd-811">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="755dd-811">AzureRM.Scheduler</span></span>
* <span data-ttu-id="755dd-812">Behebung des Problems, dass beim Aktualisieren von „ServiceBusQueueJob“ keine neuen Authentifizierungswerte festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="755dd-812">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="755dd-813">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="755dd-813">AzureRM.Sql</span></span>
* <span data-ttu-id="755dd-814">Aktualisierung der folgenden Cmdlets mit dem optionalen LicenseType-Parameter</span><span class="sxs-lookup"><span data-stu-id="755dd-814">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="755dd-815">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="755dd-815">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="755dd-816">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="755dd-816">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="755dd-817">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="755dd-817">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="755dd-818">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="755dd-818">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="755dd-819">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="755dd-819">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="755dd-820">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="755dd-820">AzureRM.Websites</span></span>
* <span data-ttu-id="755dd-821">„New-AzureRMWebApp“ aktualisiert, um allgemeine Algorithmen aus der Strategiebibliothek zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="755dd-821">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="755dd-822">6.1.0 – Mai 2018</span><span class="sxs-lookup"><span data-stu-id="755dd-822">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="755dd-823">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="755dd-823">AzureRM.Profile</span></span>
* <span data-ttu-id="755dd-824">Behebung eines Problems, durch das beim Ausführen von „Clear-AzureRmContext“ ein leerer Kontext mit dem Namen des vorherigen Standardkontexts beibehalten wurde und der Benutzer dadurch keinen neuen Kontext mit dem alten Namen erstellen konnte</span><span class="sxs-lookup"><span data-stu-id="755dd-824">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="755dd-825">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="755dd-825">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="755dd-826">Ermöglichung der Zuordnung von Gateways/Aufhebung der Gatewayzuordnung in AS</span><span class="sxs-lookup"><span data-stu-id="755dd-826">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="755dd-827">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="755dd-827">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="755dd-828">Unterstützung für „ApiVersions“, „ApiReleases“ und „ApiRevisions“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-828">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="755dd-829">Unterstützung für ServiceFabric-Back-End hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-829">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="755dd-830">Unterstützung für Application Insights-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-830">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="755dd-831">Unterstützung für die Erkennung von SKUs vom Typ „Basic“ als gültige SKU des API Management-Diensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-831">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="755dd-832">Unterstützung hinzugefügt, damit Zertifikate, die von der privaten Zertifizierungsstelle ausgestellt wurden, als Stamm- oder ZS-Zertifikate installiert werden können</span><span class="sxs-lookup"><span data-stu-id="755dd-832">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="755dd-833">Unterstützung für die Akzeptierung benutzerdefinierter SSL-Zertifikate über KeyVault und mehrere Proxyhostnamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-833">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="755dd-834">Unterstützung für die verwaltete Dienstidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-834">Added support for MSI identity</span></span>
* <span data-ttu-id="755dd-835">Unterstützung für die Annahme von Richtlinien über URL hinzugefügt; HINWEIS: Folgende Cmdlets werden in einem zukünftigen Release als veraltet gekennzeichnet:</span><span class="sxs-lookup"><span data-stu-id="755dd-835">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="755dd-836">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="755dd-836">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="755dd-837">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="755dd-837">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="755dd-838">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="755dd-838">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="755dd-839">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="755dd-839">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="755dd-840">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="755dd-840">AzureRM.Batch</span></span>
* <span data-ttu-id="755dd-841">Veröffentlichung des neuen Cmdlets „Get-AzureBatchPoolNodeCounts“</span><span class="sxs-lookup"><span data-stu-id="755dd-841">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="755dd-842">Veröffentlichung des neuen Cmdlets „Start-AzureBatchComputeNodeServiceLogUpload“</span><span class="sxs-lookup"><span data-stu-id="755dd-842">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="755dd-843">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="755dd-843">AzureRM.Consumption</span></span>
* <span data-ttu-id="755dd-844">Hinzufügung neuer Parameter („Expand“, „ResourceGroup“, „InstanceName“, „InstanceId“, „Tags“ und „Top“) für das Cmdlet „Get-AzureRmConsumptionUsageDetail“</span><span class="sxs-lookup"><span data-stu-id="755dd-844">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="755dd-845">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="755dd-845">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="755dd-846">Korrektur des Beispiels für „Export AzureRmDataLakeStoreChildItemProperties“</span><span class="sxs-lookup"><span data-stu-id="755dd-846">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="755dd-847">Korrektur der NULL-Parameterausnahme für rekursiven Fall in „Set-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="755dd-847">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="755dd-848">Korrektur der Hilfedateien für „Set-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ und „Remove-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="755dd-848">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="755dd-849">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="755dd-849">AzureRM.Network</span></span>
* <span data-ttu-id="755dd-850">Erhöhung der Network SDK-Version von 18.0.0-preview auf 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="755dd-850">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="755dd-851">Cmdlet zum Erstellen der Protokollkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-851">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="755dd-852">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="755dd-852">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="755dd-853">Cmdlet zum Hinzufügen einer neuen Leitungsverbindung zu einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-853">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="755dd-854">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-854">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="755dd-855">Cmdlet zum Entfernen einer Leitungsverbindung aus einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-855">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="755dd-856">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-856">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="755dd-857">Cmdlet zum Abrufen einer Leitungsverbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="755dd-857">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="755dd-858">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="755dd-858">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="755dd-859">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="755dd-859">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="755dd-860">Verwendung der Serverauthentifizierung mit generierten Zertifikaten korrigiert (Problemnr. 5998)</span><span class="sxs-lookup"><span data-stu-id="755dd-860">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="755dd-861">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="755dd-861">AzureRM.Sql</span></span>
* <span data-ttu-id="755dd-862">Überwachungscmdlets korrigiert, um das Entfernen von „AuditActions“ oder „AuditActionGroups“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="755dd-862">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="755dd-863">Problem mit „Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy“ behoben, das beim Festlegen einer neuen flexiblen Aufbewahrungsrichtlinie zu folgendem Fehler führte: „Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span><span class="sxs-lookup"><span data-stu-id="755dd-863">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="755dd-864">Please submit request with the new flexible retention policy“ (Das Konfigurieren einer langfristigen Aufbewahrungsrichtlinie mit Azure Recovery Service-Tresor und -Richtlinie wird nicht mehr unterstützt. Übermitteln Sie eine Anforderung mit der neuen flexiblen Aufbewahrungsrichtlinie.)</span><span class="sxs-lookup"><span data-stu-id="755dd-864">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="755dd-865">Aktualisierung aller Cmdlets für Azure SQL-Datenbank, für die Erstellung von Pools für elastische Datenbanken und für die Aktualisierung, sodass sie die neue Datenbank-API verwenden. Diese unterstützt die Sku-Eigenschaft für skalierungs- und tarifbezogene Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="755dd-865">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="755dd-866">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="755dd-866">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="755dd-867">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="755dd-867">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="755dd-868">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="755dd-868">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="755dd-869">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="755dd-869">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="755dd-870">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="755dd-870">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="755dd-871">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="755dd-871">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="755dd-872">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="755dd-872">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="755dd-873">Aktualisierung der Parameter für „Get-AzureRmTrafficManagerProfile“, sodass bei Verwendung des Parameters „-Name“ der Parameter „-ResourceGroupName“ erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="755dd-873">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
