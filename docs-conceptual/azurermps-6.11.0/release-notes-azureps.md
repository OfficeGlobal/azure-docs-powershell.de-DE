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
ms.openlocfilehash: eec8b5960f787fa9ca1130b4f8b49c9d896aa99e
ms.sourcegitcommit: 5f946a535eccca0b3ddf3db8f617b32564a88938
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/25/2018
ms.locfileid: "50001506"
---
# <a name="release-notes"></a><span data-ttu-id="c78d0-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="c78d0-103">Release notes</span></span>

<span data-ttu-id="c78d0-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="c78d0-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="6110---october-2018"></a><span data-ttu-id="c78d0-105">6.11.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="c78d0-105">6.11.0 - October 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="c78d0-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c78d0-106">AzureRM.Profile</span></span>
* <span data-ttu-id="c78d0-107">Problem mit „Get-AzureRmSubscription“ in CloudShell behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-107">Fix issue with Get-AzureRmSubscription in CloudShell</span></span>
* <span data-ttu-id="c78d0-108">Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="c78d0-108">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="c78d0-109">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="c78d0-109">AzureRM.Backup</span></span>
* <span data-ttu-id="c78d0-110">Azure Backup-Cmdlets als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="c78d0-110">Deprecated Azure Backup cmdlets.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="c78d0-111">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c78d0-111">AzureRM.Compute</span></span>
* <span data-ttu-id="c78d0-112">Neue Größen zur Whitelist von VM-Größen hinzugefügt, für die bei Verwendung des einfachen Parametersatzes für „New-AzureRmVm“ der beschleunigte Netzwerkbetrieb aktiviert wird</span><span class="sxs-lookup"><span data-stu-id="c78d0-112">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzureRmVm'</span></span>
* <span data-ttu-id="c78d0-113">ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-113">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="c78d0-114">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78d0-114">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="c78d0-115">Unterstützung für Regeln für virtuelle Netzwerke hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-115">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="c78d0-116">Get-AzureRmDataLakeStoreVirtualNetworkRule: Ruft Regel für virtuelles Azure Data Lake Store-Netzwerk ab oder listet sie auf.</span><span class="sxs-lookup"><span data-stu-id="c78d0-116">Get-AzureRmDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="c78d0-117">Add-AzureRmDataLakeStoreVirtualNetworkRule: Fügt dem angegebenen Data Lake Store-Konto eine Regel für das virtuelle Netzwerk hinzu.</span><span class="sxs-lookup"><span data-stu-id="c78d0-117">Add-AzureRmDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="c78d0-118">Set-AzureRmDataLakeStoreVirtualNetworkRule: Ändert die angegebene Regel für das virtuelle Netzwerk im angegebenen Data Lake Store-Konto.</span><span class="sxs-lookup"><span data-stu-id="c78d0-118">Set-AzureRmDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="c78d0-119">Remove-AzureRmDataLakeStoreVirtualNetworkRule: Löscht eine Regel für das virtuelle Azure Data Lake Store-Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="c78d0-119">Remove-AzureRmDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="c78d0-120">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c78d0-120">AzureRM.Network</span></span>
* <span data-ttu-id="c78d0-121">Cmdlet „Test-AzureRmNetworkWatcherConnectivity“ aktualisiert, Protokollwert wird jetzt an Back-End übergeben.</span><span class="sxs-lookup"><span data-stu-id="c78d0-121">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="c78d0-122">ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-122">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="c78d0-123">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="c78d0-123">AzureRM.Resources</span></span>
* <span data-ttu-id="c78d0-124">Problem behoben, aufgrund dessen „Get-AzureRMRoleDefinition“ eine unverständliche Ausnahme auslöst (wenn das Standardprofil kein Abonnement enthält und kein Bereich festgelegt ist) indem im Szenario eine aussagekräftige Ausnahme hinzugefügt wurde.</span><span class="sxs-lookup"><span data-stu-id="c78d0-124">Fix isssue where Get-AzureRMRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="c78d0-125">Außerdem wurde der Standardparametersatz auf „RoleDefinitionNameParameterSet“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-125">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="6100---october-2018"></a><span data-ttu-id="c78d0-126">6.10.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="c78d0-126">6.10.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="c78d0-127">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="c78d0-127">Azure.Storage</span></span>
* <span data-ttu-id="c78d0-128">Fehler beim Kopieren von Blobs/Dateien behoben, aufgrund dessen bei einem Metadatenproblem des Ziels keine Metadaten kopiert wurden</span><span class="sxs-lookup"><span data-stu-id="c78d0-128">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="c78d0-129">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="c78d0-129">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="c78d0-130">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="c78d0-130">Start-AzureStorageFileCopy</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="c78d0-131">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c78d0-131">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="c78d0-132">„Get-AzureRmCognitiveServicesAccountSkus“ wird ohne vorhandenes Konto unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-132">Support Get-AzureRmCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="c78d0-133">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c78d0-133">AzureRM.Compute</span></span>
* <span data-ttu-id="c78d0-134">Korrektur von „Get-AzureRmVM -ResourceGroupName <rg>“ sodass ggf. mehr als 50 Ergebnisse zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="c78d0-134">Fix Get-AzureRmVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="c78d0-135">Der Cmdlet-Hilfe zu „New-AzureRmVmss“ wurde ein Beispiel für „SimpleParameterSet“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-135">Added an example of the 'SimpleParameterSet' to New-AzureRmVmss cmdlet help.</span></span>
* <span data-ttu-id="c78d0-136">Tippfehler in der Azure Disk Encryption-Statusmeldung behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-136">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="c78d0-137">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="c78d0-137">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="c78d0-138">Die Version des ADF .Net-SDK wurde auf 2.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="c78d0-138">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="c78d0-139">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c78d0-139">AzureRM.Network</span></span>
* <span data-ttu-id="c78d0-140">NetworkProfile-Funktionalität wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-140">Added NetworkProfile functionality.</span></span> <span data-ttu-id="c78d0-141">Neue Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-141">new cmdlets added</span></span>
    - <span data-ttu-id="c78d0-142">Get-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c78d0-142">Get-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="c78d0-143">New-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c78d0-143">New-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="c78d0-144">Remove-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c78d0-144">Remove-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="c78d0-145">Set-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c78d0-145">Set-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="c78d0-146">New-AzureRMContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-146">New-AzureRMContainerNicConfig</span></span>
    - <span data-ttu-id="c78d0-147">New-AzureRmContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-147">New-AzureRmContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="c78d0-148">Dienstzuordnungslink in Subnetzmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-148">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="c78d0-149">Cmdlets „New-AzureRmVirtualNetworkTap“, „Get-AzureRmVirtualNetworkTap“, „Set-AzureRmVirtualNetworkTap“, „Remove-AzureRmVirtualNetworkTap“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-149">Added cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span></span>
* <span data-ttu-id="c78d0-150">Cmdlets „Set-AzureRmNEtworkInterfaceTapConfig“, „Get-AzureRmNEtworkInterfaceTapConfig“, „Remove-AzureRmNEtworkInterfaceTapConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-150">Added cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="c78d0-151">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="c78d0-151">AzureRM.RedisCache</span></span>
* <span data-ttu-id="c78d0-152">Künftig sind beliebige Zeichenfolgen als Größenparameter zulässig.</span><span class="sxs-lookup"><span data-stu-id="c78d0-152">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="c78d0-153">P5 in Popup „PSArgumentCompleter“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-153">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="c78d0-154">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="c78d0-154">AzureRM.Resources</span></span>
* <span data-ttu-id="c78d0-155">Fehlender Parameter „-Mode“ zu „Set-AzureRmPolicyDefinition“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-155">Add missing -Mode parameter to Set-AzureRmPolicyDefinition</span></span>
* <span data-ttu-id="c78d0-156">Cmdlet-Fehler bei „Fix Get-AzureRmProviderOperation“ für Vorgänge mit Ursprung behoben, der den Benutzer enthält</span><span class="sxs-lookup"><span data-stu-id="c78d0-156">Fix Get-AzureRmProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="c78d0-157">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="c78d0-157">AzureRM.Sql</span></span>
* <span data-ttu-id="c78d0-158">Problem behoben, aufgrund dessen einige Sicherungs-Cmdlets das aktuelle Azure-Abonnements nicht erkannt haben</span><span class="sxs-lookup"><span data-stu-id="c78d0-158">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="c78d0-159">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="c78d0-159">AzureRM.Storage</span></span>
* <span data-ttu-id="c78d0-160">Der Abruf der Speicherressourcennutzung eines bestimmten Standorts wird jetzt unterstützt, und das Hinzufügen einer Warnmeldung für den Abruf der globalen Speicherressourcennutzung ist überflüssig.</span><span class="sxs-lookup"><span data-stu-id="c78d0-160">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="c78d0-161">Get-AzureRmStorageUsage</span><span class="sxs-lookup"><span data-stu-id="c78d0-161">Get-AzureRmStorageUsage</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="c78d0-162">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="c78d0-162">AzureRM.Websites</span></span>
* <span data-ttu-id="c78d0-163">Neues Cmdlet „Get-AzureRMWebAppContainerContinuousDeploymentUrl“ zum Abruf der Webhook-URL von Continuous Deployment für Container</span><span class="sxs-lookup"><span data-stu-id="c78d0-163">New Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="c78d0-164">Neue Cmdlets „New-AzureRMWebAppContainerPSSession“ und „Enter-WebAppContainerPSSession“ zum Initiieren einer PowerShell-Remotesitzung in einer Windows-Container-App</span><span class="sxs-lookup"><span data-stu-id="c78d0-164">New Cmdlets New-AzureRMWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="690---september-2018"></a><span data-ttu-id="c78d0-165">6.9.0 – September 2018</span><span class="sxs-lookup"><span data-stu-id="c78d0-165">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="c78d0-166">Allgemein</span><span class="sxs-lookup"><span data-stu-id="c78d0-166">General</span></span>
* <span data-ttu-id="c78d0-167">AzureRM.SignalR wurde dem Rollupmodul AzureRM hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-167">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="c78d0-168">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c78d0-168">AzureRM.Profile</span></span>
* <span data-ttu-id="c78d0-169">Kleinere Änderungen am allgemeinen Speichercode</span><span class="sxs-lookup"><span data-stu-id="c78d0-169">Minor changes to the storage common code</span></span>
* <span data-ttu-id="c78d0-170">Hilfedateien aktualisiert, um vollständige Parametertypen einzubinden.</span><span class="sxs-lookup"><span data-stu-id="c78d0-170">Updated help files to include full parameter types.</span></span>
- <span data-ttu-id="c78d0-171">„-ServicePrincipal“ im Parametersatz „ServicePrincipalCertificateWithSubscriptionId“ in nicht obligatorisch geändert</span><span class="sxs-lookup"><span data-stu-id="c78d0-171">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="c78d0-172">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="c78d0-172">Azure.Storage</span></span>
* <span data-ttu-id="c78d0-173">Unterstützung für die Erstellung des Speicherkontexts mit OAuth.</span><span class="sxs-lookup"><span data-stu-id="c78d0-173">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="c78d0-174">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="c78d0-174">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="c78d0-175">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="c78d0-175">AzureRM.Cdn</span></span>
* <span data-ttu-id="c78d0-176">Standard_Microsoft in SKU für CDN-Preise hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-176">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="c78d0-177">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c78d0-177">AzureRM.Compute</span></span>
* <span data-ttu-id="c78d0-178">Abhängigkeiten für Key Vault und Storage in allgemeine Abhängigkeiten verschieben</span><span class="sxs-lookup"><span data-stu-id="c78d0-178">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="c78d0-179">Unterstützung für weitere VM-Größen zu AEM-Cmdlets hinzufügen</span><span class="sxs-lookup"><span data-stu-id="c78d0-179">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="c78d0-180">Parameter „PublicIPPrefix“ zu „New-AzureRmVmssIpConfig“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="c78d0-180">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="c78d0-181">Parameter „ResourceId“ zu Cmdlet „Invoke-AzureRmVMRunCommand“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="c78d0-181">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="c78d0-182">Cmdlet „Invoke-AzureRmVmssVMRunCommand“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="c78d0-182">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="c78d0-183">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="c78d0-183">AzureRM.Dns</span></span>
* <span data-ttu-id="c78d0-184">Unterstützung für Aliaseintrag während der Erstellung des DNS-Eintrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-184">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="c78d0-185">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="c78d0-185">AzureRM.Insights</span></span>
* <span data-ttu-id="c78d0-186">Probleme #6833 und #7102 behoben (Bereich „Diagnoseeinstellungen“)</span><span class="sxs-lookup"><span data-stu-id="c78d0-186">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="c78d0-187">Probleme mit dem Standardnamen, also „service“, beim Erstellen und Auflisten/Abrufen von Diagnoseeinstellungen</span><span class="sxs-lookup"><span data-stu-id="c78d0-187">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="c78d0-188">Probleme beim Erstellen von Diagnoseeinstellungen mit Kategorien</span><span class="sxs-lookup"><span data-stu-id="c78d0-188">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="c78d0-189">Meldung zur Einstellung der Unterstützung für Metrikaggregationsintervall-Parameter</span><span class="sxs-lookup"><span data-stu-id="c78d0-189">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="c78d0-190">Aggregationsintervall-Parameter werden weiterhin akzeptiert (Änderung ohne Funktionsbeeinträchtigung), aber sie werden auf dem Back-End ignoriert, da nur PT1M gültig ist</span><span class="sxs-lookup"><span data-stu-id="c78d0-190">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="c78d0-191">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c78d0-191">AzureRM.Network</span></span>
* <span data-ttu-id="c78d0-192">Änderungen an LoadBalancer-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="c78d0-192">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="c78d0-193">LoadBalancerInboundNatPoolConfig: Parameter IdleTimeoutInMinutes, EnableFloatingIp und EnableTcpReset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-193">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="c78d0-194">LoadBalancerInboundNatRuleConfig: Parameter EnableTcpReset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-194">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="c78d0-195">LoadBalancerRuleConfig: Parameter EnableTcpReset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-195">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="c78d0-196">LoadBalancerProbeConfig: Unterstützung für Wert „Https“ für Parameter „Protocol“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-196">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="c78d0-197">Neue Befehle für neue Unterressource „OutboundRule“ von LoadBalancer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-197">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="c78d0-198">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-198">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="c78d0-199">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-199">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="c78d0-200">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-200">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="c78d0-201">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-201">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="c78d0-202">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-202">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="c78d0-203">Neue HostedWorkloads-Eigenschaft für PSNetworkInterface hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-203">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="c78d0-204">Neue Cmdlets für Feature: Azure Firewall über ARM</span><span class="sxs-lookup"><span data-stu-id="c78d0-204">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="c78d0-205">Get-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-205">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="c78d0-206">Set-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-206">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="c78d0-207">New-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-207">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="c78d0-208">Remove-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-208">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="c78d0-209">New-AzureRmFirewallApplicationRuleCollection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-209">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="c78d0-210">New-AzureRmFirewallApplicationRule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-210">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="c78d0-211">New-AzureRmFirewallNatRuleCollection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-211">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="c78d0-212">New-AzureRmFirewallNatRule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-212">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="c78d0-213">New-AzureRmFirewallNetworkRuleCollection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-213">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="c78d0-214">New-AzureRmFirewallNetworkRule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-214">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="c78d0-215">Unterstützung für vertrauenswürdiges Stammzertifikat und Konfiguration der automatischen Skalierung in Application Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-215">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="c78d0-216">Neue Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="c78d0-216">New Cmdlets added:</span></span>
      - <span data-ttu-id="c78d0-217">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="c78d0-217">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="c78d0-218">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="c78d0-218">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="c78d0-219">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="c78d0-219">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="c78d0-220">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="c78d0-220">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="c78d0-221">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="c78d0-221">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="c78d0-222">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="c78d0-222">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="c78d0-223">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="c78d0-223">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="c78d0-224">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="c78d0-224">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="c78d0-225">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="c78d0-225">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="c78d0-226">Cmdlets mit optionalem Parameter „-TrustedRootCertificate“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-226">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="c78d0-227">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="c78d0-227">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="c78d0-228">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="c78d0-228">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="c78d0-229">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="c78d0-229">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="c78d0-230">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="c78d0-230">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="c78d0-231">Cmdlets mit optionalem Parameter „-AutoscaleConfiguration“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-231">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="c78d0-232">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="c78d0-232">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="c78d0-233">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="c78d0-233">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="c78d0-234">Cmdlet für Schnittstellenendpunkt Get-AzureInterfaceEndpoint hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-234">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="c78d0-235">Unterstützung für mehrere Adresspräfixe in einem Subnetz hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-235">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="c78d0-236">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c78d0-236">Updated cmdlets:</span></span>
  - <span data-ttu-id="c78d0-237">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-237">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="c78d0-238">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-238">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="c78d0-239">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-239">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="c78d0-240">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-240">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="c78d0-241">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="c78d0-241">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="c78d0-242">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-242">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="c78d0-243">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-243">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="c78d0-244">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-244">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="c78d0-245">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="c78d0-245">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="c78d0-246">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="c78d0-246">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="c78d0-247">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="c78d0-247">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="c78d0-248">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-248">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="c78d0-249">New-AzureRmNetworkInterfaceIpConfig – Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-249">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="c78d0-250">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-250">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="c78d0-251">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-251">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="c78d0-252">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-252">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="c78d0-253">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-253">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="c78d0-254">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-254">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="c78d0-255">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="c78d0-255">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="c78d0-256">Cmdlets für die Subnetzdelegierung hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="c78d0-256">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="c78d0-257">New-AzureRmDelegation: Erstellt eine neue Delegierung, die einem Subnetz hinzugefügt werden kann</span><span class="sxs-lookup"><span data-stu-id="c78d0-257">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="c78d0-258">Remove-AzureRmDelegation: Nutzt ein Subnetz und entfernt den bereitgestellten Delegierungsnamen aus diesem Subnetz</span><span class="sxs-lookup"><span data-stu-id="c78d0-258">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="c78d0-259">Add-AzureRmDelegation: Nutzt ein Subnetz und fügt den angegebenen Dienstnamen diesem Subnetz als Delegierung hinzu</span><span class="sxs-lookup"><span data-stu-id="c78d0-259">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="c78d0-260">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="c78d0-260">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="c78d0-261">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="c78d0-261">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="c78d0-262">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="c78d0-262">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="c78d0-263">Unterstützung für verwalteten Datenträger</span><span class="sxs-lookup"><span data-stu-id="c78d0-263">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="c78d0-264">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="c78d0-264">AzureRM.RedisCache</span></span>
* <span data-ttu-id="c78d0-265">Insights-Abhängigkeit aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="c78d0-265">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="c78d0-266">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="c78d0-266">AzureRM.Resources</span></span>
* <span data-ttu-id="c78d0-267">New-AzureRmResourceGroupDeployment mit neuem Parameter „RollbackAction“ aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c78d0-267">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="c78d0-268">Unterstützung für OnErrorDeployment mit dem neuen Parameter hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="c78d0-268">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="c78d0-269">Unterstützung für verwaltete Identität in Richtlinienzuweisungen.</span><span class="sxs-lookup"><span data-stu-id="c78d0-269">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="c78d0-270">Parameter mit Standardwerten sind nicht mehr erforderlich, wenn eine Richtlinie mit „New-AzureRmPolicyAssignment“ zugewiesen wird</span><span class="sxs-lookup"><span data-stu-id="c78d0-270">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="c78d0-271">Neues Cmdlet „Get-AzureRmPolicyAlias“ zum Abrufen von Richtlinienaliasen hinzufügen</span><span class="sxs-lookup"><span data-stu-id="c78d0-271">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="c78d0-272">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c78d0-272">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="c78d0-273">Problem #7161 behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-273">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="c78d0-274">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="c78d0-274">AzureRM.SignalR</span></span>
* <span data-ttu-id="c78d0-275">SKU-Namen auf Free_F1 und Standard_S1 aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c78d0-275">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="c78d0-276">Versionsfeld zum PSSignalRResource-Objekt und Verbindungszeichenfolge zum PSSignalRKeys-Objekt hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="c78d0-276">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="c78d0-277">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="c78d0-277">AzureRM.Storage</span></span>
* <span data-ttu-id="c78d0-278">Unterstützung für Unveränderlichkeitsrichtlinie in AzureRm.Storage</span><span class="sxs-lookup"><span data-stu-id="c78d0-278">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="c78d0-279">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="c78d0-279">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="c78d0-280">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="c78d0-280">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="c78d0-281">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="c78d0-281">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="c78d0-282">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="c78d0-282">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="c78d0-283">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="c78d0-283">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="c78d0-284">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="c78d0-284">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="c78d0-285">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="c78d0-285">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="c78d0-286">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="c78d0-286">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="c78d0-287">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="c78d0-287">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="c78d0-288">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="c78d0-288">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="c78d0-289">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="c78d0-289">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="c78d0-290">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="c78d0-290">AzureRM.Websites</span></span>
* <span data-ttu-id="c78d0-291">Zwei neue Cmdlets hinzugefügt: Get-AzureRmDeletedWebApp und Restore-AzureRmDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="c78d0-291">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="c78d0-292">New-AzureRmAppServicePlan -HyperV-Switch für „App Service-Plan erstellen“ mit Windows-Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-292">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="c78d0-293">New-AzureRmWebApp/New-AzureRmWebAppSlot/Set-AzureRmWebApp/Set-AzureRmWebAppSlot: Neue Parameter (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) für die Erstellung und Verwaltung der Windows-Container-App hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-293">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="c78d0-294">6.8.1: August 2018</span><span class="sxs-lookup"><span data-stu-id="c78d0-294">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="c78d0-295">Allgemein</span><span class="sxs-lookup"><span data-stu-id="c78d0-295">General</span></span>
* <span data-ttu-id="c78d0-296">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="c78d0-296">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="c78d0-297">Allgemeine Laufzeitassemblys aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-297">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="c78d0-298">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c78d0-298">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="c78d0-299">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="c78d0-299">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="c78d0-300">Problem https://github.com/Azure/azure-powershell/issues/6603 behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-300">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="c78d0-301">Die Cmdlets „Import-AzureRmApiManagementApi“ und „\*-AzureRmApiManagementCertificate“ können jetzt relative Pfade verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="c78d0-301">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="c78d0-302">Problem https://github.com/Azure/azure-powershell/issues/6879 behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-302">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="c78d0-303">„CertificateInformation“ ist eine festlegbare Eigenschaft, die die ordnungsgemäße Funktionsweise des Cmdlets „Set-AzureRmApiManagement“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="c78d0-303">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="c78d0-304">Behoben durch Upgrade auf NuGet-Paket „4.0.4-preview“</span><span class="sxs-lookup"><span data-stu-id="c78d0-304">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="c78d0-305">Problem https://github.com/Azure/azure-powershell/issues/6853 behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-305">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="c78d0-306">OData-Filter für die Suche anhand des Namens korrigiert (Produkt)</span><span class="sxs-lookup"><span data-stu-id="c78d0-306">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="c78d0-307">Problem https://github.com/Azure/azure-powershell/issues/6814 behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-307">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="c78d0-308">OData-Filter für die Suche anhand des Namens korrigiert (API)</span><span class="sxs-lookup"><span data-stu-id="c78d0-308">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="c78d0-309">Unterstützung für AzureMonitor-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-309">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="c78d0-310">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c78d0-310">AzureRM.Compute</span></span>
* <span data-ttu-id="c78d0-311">Problem des fehlenden Ziels in der Fehlerausgabe behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-311">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="c78d0-312">Problem mit dem Speicherkontotyp für den virtuellen Computer mit verwaltetem Datenträgern behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-312">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="c78d0-313">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="c78d0-313">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="c78d0-314">AEM-Erweiterungs-Cmdlets für andere Umgebungen (etwa Azure China) korrigiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-314">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="c78d0-315">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c78d0-315">AzureRM.Network</span></span>
* <span data-ttu-id="c78d0-316">Standarddarstellung der Cmdlet-Ausgabe in Tabellenansicht geändert</span><span class="sxs-lookup"><span data-stu-id="c78d0-316">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="c78d0-317">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="c78d0-317">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="c78d0-318">Fehler in „Update-AzureRmPowerBIEmbeddedCapacity“ beim Skalieren der angehaltenen Kapazität behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-318">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="c78d0-319">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="c78d0-319">AzureRM.Resources</span></span>
* <span data-ttu-id="c78d0-320">Problem beim Erstellen verwalteter Anwendungen über Marketplace behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-320">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="c78d0-321">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c78d0-321">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="c78d0-322">Behobene Probleme</span><span class="sxs-lookup"><span data-stu-id="c78d0-322">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="c78d0-323">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c78d0-323">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="c78d0-324">Unterstützung für Routingmethode „MultiValue“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-324">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="c78d0-325">Neuer Parameter „MaxReturn“ für Routingtyp „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="c78d0-325">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="c78d0-326">Unterstützung für Subnetzroutingmethode hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-326">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="c78d0-327">Unterstützung für IP-Adressbereiche (Subnetze) in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="c78d0-327">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="c78d0-328">Unterstützung für benutzerdefinierte Header in Profilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-328">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="c78d0-329">Unterstützung für erwartete Statuscodebereiche in Profilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-329">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="c78d0-330">Unterstützung für benutzerdefinierte Header in Endpunkten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-330">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="c78d0-331">6.8.0: August 2018</span><span class="sxs-lookup"><span data-stu-id="c78d0-331">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="c78d0-332">Allgemein</span><span class="sxs-lookup"><span data-stu-id="c78d0-332">General</span></span>
* <span data-ttu-id="c78d0-333">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="c78d0-333">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="c78d0-334">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c78d0-334">AzureRM.Profile</span></span>
* <span data-ttu-id="c78d0-335">Ablaufeigenschaft zu Token hinzugefügt, die während „Connect-AzureRmAccount“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="c78d0-335">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="c78d0-336">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c78d0-336">AzureRM.Compute</span></span>
* <span data-ttu-id="c78d0-337">Problem des fehlenden Ziels in der Fehlerausgabe behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-337">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="c78d0-338">Problem mit dem Speicherkontotyp für den virtuellen Computer mit verwaltetem Datenträgern behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-338">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="c78d0-339">AEM-Erweiterungs-Cmdlets für andere Umgebungen (etwa Azure China) korrigiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-339">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="c78d0-340">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="c78d0-340">AzureRM.IotHub</span></span>
* <span data-ttu-id="c78d0-341">Beispiele für „New-AzureRmIotHubExportDevices“ und „New-AzureRmIotHubImportDevices“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-341">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="c78d0-342">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c78d0-342">AzureRM.Network</span></span>
* <span data-ttu-id="c78d0-343">Standarddarstellung von Modellen in Tabellenansicht geändert</span><span class="sxs-lookup"><span data-stu-id="c78d0-343">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="c78d0-344">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="c78d0-344">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="c78d0-345">Fehler in „Update-AzureRmPowerBIEmbeddedCapacity“ beim Skalieren der angehaltenen Kapazität behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-345">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="c78d0-346">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="c78d0-346">AzureRM.Resources</span></span>
* <span data-ttu-id="c78d0-347">Problem beim Erstellen der verwalteten Anwendung über Marketplace behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-347">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="c78d0-348">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c78d0-348">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="c78d0-349">Fehlerbehebung</span><span class="sxs-lookup"><span data-stu-id="c78d0-349">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="c78d0-350">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c78d0-350">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="c78d0-351">Unterstützung für Routingmethode „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="c78d0-351">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="c78d0-352">Neuer Parameter „MaxReturn“ für Routingtyp „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="c78d0-352">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="c78d0-353">Unterstützung für Subnetzroutingmethode</span><span class="sxs-lookup"><span data-stu-id="c78d0-353">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="c78d0-354">Unterstützung für IP-Adressbereiche (Subnetze) in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="c78d0-354">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="c78d0-355">Unterstützung für benutzerdefinierte Header in Profilen</span><span class="sxs-lookup"><span data-stu-id="c78d0-355">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="c78d0-356">Unterstützung für erwartete Statuscodebereiche in Profilen</span><span class="sxs-lookup"><span data-stu-id="c78d0-356">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="c78d0-357">Unterstützung für benutzerdefinierte Header in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="c78d0-357">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="c78d0-358">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="c78d0-358">AzureRM.Websites</span></span>
* <span data-ttu-id="c78d0-359">Das Problem, dass die Standardressourcengruppe falsch festgelegt wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="c78d0-359">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="c78d0-360">6.7.0: August 2018</span><span class="sxs-lookup"><span data-stu-id="c78d0-360">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="c78d0-361">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c78d0-361">AzureRM.Profile</span></span>
* <span data-ttu-id="c78d0-362">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-362">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="c78d0-363">Benutzer-ID zum Standardkontextnamen hinzugefügt, um Kontextkonflikte zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="c78d0-363">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="c78d0-364">Probleme mit „Clear-AzureRmContext“ behoben, die Fehler beim Auswählen eines Kontexts verursacht haben (6398)</span><span class="sxs-lookup"><span data-stu-id="c78d0-364">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="c78d0-365">Ermöglicht, dass für „Connect-AzureRmAccount“ die Mandantendomäne an den Parameter „-TenantId“ übergeben wird</span><span class="sxs-lookup"><span data-stu-id="c78d0-365">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="c78d0-366">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="c78d0-366">Azure.Storage</span></span>
* <span data-ttu-id="c78d0-367">Begrenzung von 5 TB für das Kontingent der Azure-Dateifreigabe entfernt</span><span class="sxs-lookup"><span data-stu-id="c78d0-367">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="c78d0-368">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="c78d0-368">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="c78d0-369">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c78d0-369">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="c78d0-370">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-370">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="c78d0-371">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c78d0-371">Azure.AnalysisServices</span></span>
* <span data-ttu-id="c78d0-372">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-372">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="c78d0-373">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c78d0-373">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="c78d0-374">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-374">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="c78d0-375">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="c78d0-375">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="c78d0-376">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-376">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="c78d0-377">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="c78d0-377">AzureRM.Automation</span></span>
* <span data-ttu-id="c78d0-378">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-378">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="c78d0-379">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="c78d0-379">AzureRM.Backup</span></span>
* <span data-ttu-id="c78d0-380">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-380">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="c78d0-381">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="c78d0-381">AzureRM.Batch</span></span>
* <span data-ttu-id="c78d0-382">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-382">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="c78d0-383">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="c78d0-383">AzureRM.Billing</span></span>
* <span data-ttu-id="c78d0-384">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-384">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="c78d0-385">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="c78d0-385">AzureRM.Cdn</span></span>
* <span data-ttu-id="c78d0-386">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-386">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="c78d0-387">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c78d0-387">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="c78d0-388">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-388">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="c78d0-389">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c78d0-389">AzureRM.Compute</span></span>
* <span data-ttu-id="c78d0-390">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-390">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="c78d0-391">EvictionPolicy-Parameter zu „New-AzureRmVmssConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-391">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="c78d0-392">Standort in „DiskFileParameterSet“ von „New-AzureRmVm“ angeben, wenn kein Ort angegeben ist</span><span class="sxs-lookup"><span data-stu-id="c78d0-392">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="c78d0-393">Parameterbeschreibung in „Save-AzureRmVMImage“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-393">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="c78d0-394">Cmdlet „Get-AzureRmVMDiskEncryptionStatus“ für bestimmte Szenarien im Zusammenhang mit einem Durchlauf korrigiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-394">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="c78d0-395">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="c78d0-395">AzureRM.Consumption</span></span>
* <span data-ttu-id="c78d0-396">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-396">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="c78d0-397">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="c78d0-397">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="c78d0-398">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-398">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="c78d0-399">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="c78d0-399">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="c78d0-400">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-400">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="c78d0-401">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="c78d0-401">AzureRM.DataFactories</span></span>
* <span data-ttu-id="c78d0-402">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-402">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="c78d0-403">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="c78d0-403">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="c78d0-404">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-404">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="c78d0-405">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="c78d0-405">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="c78d0-406">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-406">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="c78d0-407">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78d0-407">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="c78d0-408">Debuggen korrigiert, wenn „DebugPreference“ über die PowerShell-Befehlszeile festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="c78d0-408">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="c78d0-409">Beispiel für „Set-AzureRmDataLakeStoreItemAcl“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-409">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="c78d0-410">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="c78d0-410">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="c78d0-411">Beispiel für „Set-AzureRmDataLakeStoreItemAclEntry“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-411">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="c78d0-412">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="c78d0-412">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="c78d0-413">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-413">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="c78d0-414">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="c78d0-414">AzureRM.Dns</span></span>
* <span data-ttu-id="c78d0-415">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-415">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="c78d0-416">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c78d0-416">AzureRM.EventGrid</span></span>
* <span data-ttu-id="c78d0-417">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-417">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="c78d0-418">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="c78d0-418">AzureRM.EventHub</span></span>
* <span data-ttu-id="c78d0-419">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-419">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="c78d0-420">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c78d0-420">AzureRM.HDInsight</span></span>
* <span data-ttu-id="c78d0-421">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-421">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="c78d0-422">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="c78d0-422">AzureRM.Insights</span></span>
* <span data-ttu-id="c78d0-423">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-423">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="c78d0-424">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="c78d0-424">AzureRM.IotHub</span></span>
* <span data-ttu-id="c78d0-425">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-425">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="c78d0-426">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78d0-426">AzureRM.KeyVault</span></span>
* <span data-ttu-id="c78d0-427">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-427">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="c78d0-428">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c78d0-428">AzureRM.LogicApp</span></span>
* <span data-ttu-id="c78d0-429">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-429">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="c78d0-430">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="c78d0-430">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="c78d0-431">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-431">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="c78d0-432">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="c78d0-432">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="c78d0-433">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-433">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="c78d0-434">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="c78d0-434">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="c78d0-435">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-435">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="c78d0-436">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="c78d0-436">AzureRM.Media</span></span>
* <span data-ttu-id="c78d0-437">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-437">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="c78d0-438">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c78d0-438">AzureRM.Network</span></span>
* <span data-ttu-id="c78d0-439">Beispiel für „Set-AzureRmLocalNetworkGateway“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-439">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="c78d0-440">Beispiele und Beschreibungen für „Add-AzureRmVirtualNetworkGatewayIpConfig“, „Get-AzureRmVirtualNetworkGatewayConnectionSharedKey“ und „New-AzureRmVirtualNetworkGatewayConnection“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-440">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="c78d0-441">Beispiele für „Remove-AzureRmVirtualNetworkGatewayIpConfig“ und „Reset-AzureRmVirtualNetworkGateway“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-441">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="c78d0-442">Beispiel für „Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-442">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="c78d0-443">Beispiel für „Set-AzureRmVirtualNetworkGatewayConnectionSharedKey“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-443">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="c78d0-444">Beispiel für „Set-AzureRmVirtualNetworkGatewayConnection“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-444">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="c78d0-445">Cmdlets für „ApplicationSecurityGroup“, „RouteTable“ und „Usage“ mithilfe des aktuellen Code-Generators erneut erstellt</span><span class="sxs-lookup"><span data-stu-id="c78d0-445">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="c78d0-446">Deutlichere Formulierung der Fehlermeldung für „Get-AzureRmVirtualNetworkSubnetConfig“, wenn ein nicht vorhandenes Subnetz abgerufen wird</span><span class="sxs-lookup"><span data-stu-id="c78d0-446">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="c78d0-447">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="c78d0-447">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="c78d0-448">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-448">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="c78d0-449">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c78d0-449">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="c78d0-450">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-450">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="c78d0-451">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c78d0-451">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="c78d0-452">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-452">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="c78d0-453">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="c78d0-453">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="c78d0-454">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-454">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="c78d0-455">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78d0-455">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="c78d0-456">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-456">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="c78d0-457">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="c78d0-457">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="c78d0-458">Richtlinienfilter zum Cmdlet „Get-AzureRmRecoveryServicesBackItem“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-458">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="c78d0-459">Der Befehl gibt die Liste der Sicherungselemente zurück, die durch die angegebene Richtlinien-ID geschützt sind.</span><span class="sxs-lookup"><span data-stu-id="c78d0-459">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="c78d0-460">„Microsoft.Azure.Management.RecoveryServices.Backup“ auf Version 3.0.0-preview aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-460">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="c78d0-461">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-461">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="c78d0-462">TargetResourceGroupName-Parameter zu „Restore-AzureRmRecoveryServicesBackupItem“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-462">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="c78d0-463">Die Ressourcengruppe, in der die verwalteten Datenträger wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="c78d0-463">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="c78d0-464">Gilt für die Sicherung des virtuellen Computers mit verwalteten Datenträgern.</span><span class="sxs-lookup"><span data-stu-id="c78d0-464">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="c78d0-465">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="c78d0-465">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="c78d0-466">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-466">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="c78d0-467">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="c78d0-467">AzureRM.RedisCache</span></span>
* <span data-ttu-id="c78d0-468">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-468">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="c78d0-469">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="c78d0-469">AzureRM.Relay</span></span>
* <span data-ttu-id="c78d0-470">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-470">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="c78d0-471">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="c78d0-471">AzureRM.Resources</span></span>
* <span data-ttu-id="c78d0-472">Unterstützung der Vorlagenbereitstellung im Abonnementbereich.</span><span class="sxs-lookup"><span data-stu-id="c78d0-472">Support template deployment at subscription scope.</span></span> <span data-ttu-id="c78d0-473">Neue Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="c78d0-473">Add new Cmdlets:</span></span>
    - <span data-ttu-id="c78d0-474">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="c78d0-474">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="c78d0-475">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="c78d0-475">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="c78d0-476">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="c78d0-476">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="c78d0-477">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="c78d0-477">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="c78d0-478">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="c78d0-478">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="c78d0-479">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="c78d0-479">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="c78d0-480">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="c78d0-480">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="c78d0-481">Problem behoben, aufgrund dessen beim Übergeben eines Kontexts an „Set-AzureRmResource“ ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="c78d0-481">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="c78d0-482">Beispiel in „New-AzureRmResourceGroupDeployment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-482">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="c78d0-483">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-483">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="c78d0-484">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="c78d0-484">AzureRM.Scheduler</span></span>
* <span data-ttu-id="c78d0-485">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-485">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="c78d0-486">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c78d0-486">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="c78d0-487">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-487">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="c78d0-488">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c78d0-488">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="c78d0-489">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-489">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="c78d0-490">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="c78d0-490">AzureRM.Sql</span></span>
* <span data-ttu-id="c78d0-491">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-491">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="c78d0-492">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="c78d0-492">AzureRM.Storage</span></span>
* <span data-ttu-id="c78d0-493">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-493">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="c78d0-494">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="c78d0-494">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="c78d0-495">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-495">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="c78d0-496">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="c78d0-496">AzureRM.Tags</span></span>
* <span data-ttu-id="c78d0-497">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-497">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="c78d0-498">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c78d0-498">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="c78d0-499">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-499">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="c78d0-500">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="c78d0-500">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="c78d0-501">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-501">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="c78d0-502">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="c78d0-502">AzureRM.Websites</span></span>
* <span data-ttu-id="c78d0-503">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-503">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="c78d0-504">6.6.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="c78d0-504">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="c78d0-505">Allgemein</span><span class="sxs-lookup"><span data-stu-id="c78d0-505">General</span></span>
* <span data-ttu-id="c78d0-506">Alle Hilfedateien aktualisiert, um vollständige Parametertypen und die richtigen Eingabe/Ausgabe-Typen einzuschließen.</span><span class="sxs-lookup"><span data-stu-id="c78d0-506">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="c78d0-507">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c78d0-507">AzureRM.Profile</span></span>
* <span data-ttu-id="c78d0-508">Bibliothek „Common.Strategy“ aktualisiert, um überprüfen zu können, ob die aktuelle Konfiguration für eine Ressource mit der Zielressource kompatibel ist.</span><span class="sxs-lookup"><span data-stu-id="c78d0-508">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="c78d0-509">ps1xml-Typen zu „Common.Storage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-509">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="c78d0-510">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="c78d0-510">Azure.Storage</span></span>
* <span data-ttu-id="c78d0-511">Unterstützung zum Abrufen von Speicherkontext aus „DefaultProfile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-511">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="c78d0-512">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-512">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="c78d0-513">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c78d0-513">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="c78d0-514">Problem https://github.com/Azure/azure-powershell/issues/6370 behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-514">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="c78d0-515">Fehler in Automapper behoben, um „PsApiManagementApi“ in „ApiContract“ zu verschieben</span><span class="sxs-lookup"><span data-stu-id="c78d0-515">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="c78d0-516">Problem https://github.com/Azure/azure-powershell/issues/6515 behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-516">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="c78d0-517">Fehler in „File.Save“ behoben, um Überladung mit Codierungstyp zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="c78d0-517">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="c78d0-518">Problem https://github.com/Azure/azure-powershell/issues/6560 behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-518">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="c78d0-519">Upgrade auf Nuget-Version 4.0.3 durchgeführt, in der Musterausnahme in „apiId“ behoben wurde</span><span class="sxs-lookup"><span data-stu-id="c78d0-519">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="c78d0-520">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c78d0-520">AzureRM.Compute</span></span>
* <span data-ttu-id="c78d0-521">Das Problem, aufgrund dessen beim Erstellen eines virtuellen Computers mithilfe von „DiskFileParameterSet“ in „New-AzureRmVm“ wegen einer Umbenennung des Speicherkontotyps „PremiumLRS“ ein Fehler auftrat, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="c78d0-521">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="c78d0-522">Cmdlet „Invoke-AzureRmVMRunCommand“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-522">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="c78d0-523">„Get-AzureRmAvailabilitySet“ aktualisiert, um die Auflistung aller Verfügbarkeitsgruppen in einem Abonnement zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="c78d0-523">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="c78d0-524">(ResouceGroupName-Parameter ist jetzt optional.)</span><span class="sxs-lookup"><span data-stu-id="c78d0-524">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="c78d0-525">„SimpleParameterSet“ von „New-AzureRmVm“ aktualisiert, um Accelerated Networking auf kompatiblen virtuellen Computern zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="c78d0-525">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="c78d0-526">Einfacher Parametersatz „New-AzureRmVmss“ aktualisiert, sodass das Erstellen der VMSS fehlschlägt, wenn bereits ein benutzerdefinierter LB vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="c78d0-526">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="c78d0-527">Beispiel für „New-AzureRmDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-527">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="c78d0-528">Beispiel für „New-AzureRmVM“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-528">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="c78d0-529">Beschreibung für „Set-AzureRmVMOSDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-529">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="c78d0-530">Beispiel 1 für „Set-AzureRmVMBginfoExtension“ aktualisiert, um Rechtschreibung und Präfix zu korrigieren.</span><span class="sxs-lookup"><span data-stu-id="c78d0-530">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="c78d0-531">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="c78d0-531">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="c78d0-532">ADF .Net SDK-Version auf 1.1.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="c78d0-532">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="c78d0-533">Unterstützung der Freigabe der selbstgehosteten Integration Runtime über Data Factorys hinweg.</span><span class="sxs-lookup"><span data-stu-id="c78d0-533">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="c78d0-534">Neuer Parameter „-SharedIntegrationRuntimeResourceId“ zu Cmdlet „Set-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-534">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="c78d0-535">Neuer optionaler Parameter „-LinkedDataFactoryName“ zu Cmdlet „Remove-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-535">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="c78d0-536">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78d0-536">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="c78d0-537">DataPlane SDK-Version (Microsoft.Azure.DataLake.Store) auf 1.1.9 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-537">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="c78d0-538">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="c78d0-538">AzureRM.EventHub</span></span>
* <span data-ttu-id="c78d0-539">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-539">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="c78d0-540">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="c78d0-540">AzureRM.Insights</span></span>
* <span data-ttu-id="c78d0-541">Formatierung von „OutputType“ in Hilfedateien korrigiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-541">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="c78d0-542">Verwendung von Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span><span class="sxs-lookup"><span data-stu-id="c78d0-542">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="c78d0-543">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78d0-543">AzureRM.KeyVault</span></span>
* <span data-ttu-id="c78d0-544">Piping-Problem in „Set-AzureRmKeyVaultAccessPolicy“ behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-544">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="c78d0-545">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c78d0-545">AzureRM.Network</span></span>
* <span data-ttu-id="c78d0-546">Beispiele für LoadBalancerInboundNatPoolConfig-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-546">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="c78d0-547">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="c78d0-547">AzureRM.Resources</span></span>
* <span data-ttu-id="c78d0-548">Problem beim Angeben sowohl des Tag-Namens als auch des Werts für „Get-AzureRmResource“ behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-548">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="c78d0-549">Piping-Szenario mit „Set-AzureRmResource“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-549">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="c78d0-550">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c78d0-550">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="c78d0-551">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-551">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="c78d0-552">Einige Probleme behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-552">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="c78d0-553">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="c78d0-553">AzureRM.Sql</span></span>
* <span data-ttu-id="c78d0-554">Unterstützung für Advanced Threat Protection für Server bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="c78d0-554">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="c78d0-555">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c78d0-555">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="c78d0-556">Unterstützung für Sicherheitsrisikobewertung bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="c78d0-556">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="c78d0-557">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="c78d0-557">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="c78d0-558">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="c78d0-558">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="c78d0-559">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="c78d0-559">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="c78d0-560">Beispiel in „Remove-AzureRmSqlServerFirewallRule“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-560">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="c78d0-561">Falsche Verarbeitung von „datetime“ für nicht US-basierte Kultur in „Get-AzureSqlSyncGroupLog“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-561">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="c78d0-562">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="c78d0-562">AzureRM.Storage</span></span>
* <span data-ttu-id="c78d0-563">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-563">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="c78d0-564">Cmdlet-Ausgabe von „StorageAccount“ in Tabellenansicht anzeigen</span><span class="sxs-lookup"><span data-stu-id="c78d0-564">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="c78d0-565">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c78d0-565">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="c78d0-566">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c78d0-566">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="c78d0-567">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c78d0-567">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="c78d0-568">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="c78d0-568">AzureRM.Tags</span></span>
* <span data-ttu-id="c78d0-569">Falsche Anweisung aus Tag-Cmdlet-Hilfe entfernt</span><span class="sxs-lookup"><span data-stu-id="c78d0-569">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="c78d0-570">6.5.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="c78d0-570">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="c78d0-571">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c78d0-571">AzureRM.Profile</span></span>
* <span data-ttu-id="c78d0-572">Hilfe für „Get-AzureRmContextAutosaveSetting“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-572">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="c78d0-573">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="c78d0-573">Azure.Storage</span></span>
* <span data-ttu-id="c78d0-574">Unterstützung des Blob- oder Dateiuploads mit lesegeschütztem SAS-Token</span><span class="sxs-lookup"><span data-stu-id="c78d0-574">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="c78d0-575">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="c78d0-575">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="c78d0-576">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="c78d0-576">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="c78d0-577">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c78d0-577">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="c78d0-578">Erforderliche Eigenschaft „ResourceGroupName“ zu AS hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-578">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="c78d0-579">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="c78d0-579">AzureRM.Automation</span></span>
* <span data-ttu-id="c78d0-580">Hilfe aktualisiert und Beispiel für „New-AzureRMAutomationSchedule“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-580">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="c78d0-581">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c78d0-581">AzureRM.Compute</span></span>
* <span data-ttu-id="c78d0-582">Parameter „-Tag“ zu „Update/New-AzureRmAvailabilitySet“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-582">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="c78d0-583">Beispiel für „Add-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-583">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="c78d0-584">Beispiele für „Remove-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-584">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="c78d0-585">Hilfe für „Set-AzureRmVMAccessExtension“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-585">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="c78d0-586">„SimpleParameterSet“ für „New-AzureRmVmss“ so aktualisiert, dass „SinglePlacementGroup“ standardmäßig auf „false“ festgelegt ist, und Switch-Parameter „SinglePlacementGroup“ hinzugefügt, der dem Benutzer das Erstellen der VMSS in einer einzelnen Platzierungsgruppe ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="c78d0-586">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="c78d0-587">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="c78d0-587">AzureRM.EventHub</span></span>
* <span data-ttu-id="c78d0-588">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSEventHubDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="c78d0-588">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="c78d0-589">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78d0-589">AzureRM.KeyVault</span></span>
* <span data-ttu-id="c78d0-590">Fehlermeldung für „Set-AzureRmKeyVaultAccessPolicy“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-590">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="c78d0-591">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c78d0-591">AzureRM.LogicApp</span></span>
* <span data-ttu-id="c78d0-592">Fehler „Parametersatz konnte nicht aufgelöst werden“ in „New-AzureRmLogicApp“behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-592">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="c78d0-593">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c78d0-593">AzureRM.Network</span></span>
* <span data-ttu-id="c78d0-594">Peering über mehrere virtuelle Netzwerke in mehreren Mandanten für „Set/Add-AzureRmVirtualNetworkPeering“ aktiviert</span><span class="sxs-lookup"><span data-stu-id="c78d0-594">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="c78d0-595">Folgende Cmdlets für Application Gateway aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-595">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="c78d0-596">New-AzureRmApplicationGateway: EnableFIPS-Flag und Zonenunterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-596">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="c78d0-597">New-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-597">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="c78d0-598">Set-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-598">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="c78d0-599">RouteTable-Cmdlets mit aktueller Generatorversion erneut generiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-599">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="c78d0-600">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="c78d0-600">AzureRM.Relay</span></span>
* <span data-ttu-id="c78d0-601">Markdowndateien aktualisiert, Problem mit Parametername in Beispiel behoben</span><span class="sxs-lookup"><span data-stu-id="c78d0-601">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="c78d0-602">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="c78d0-602">AzureRM.Resources</span></span>
* <span data-ttu-id="c78d0-603">Roleassignment- und roledefinition-Cmdlets aktualisiert:</span><span class="sxs-lookup"><span data-stu-id="c78d0-603">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="c78d0-604">Zusätzliche roledefinition-Aufrufe entfernt, die als Teil des Pagings durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="c78d0-604">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="c78d0-605">Get-AzureRmRoleAssignment-Cmdlet korrigiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-605">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="c78d0-606">Befehlsparameterfunktion von „-ExpandPrincipalGroups“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-606">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="c78d0-607">Problem mit „Get-AzureRmResource“ behoben, aufgrund dessen die Groß-/Kleinschreibung des Parameters „-ResourceType“ beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="c78d0-607">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="c78d0-608">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c78d0-608">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="c78d0-609">top- und skip-Parameter zu Listen-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-609">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="c78d0-610">Cmdlets für die Migration von Standard- zu Premium-Namespace hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="c78d0-610">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="c78d0-611">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="c78d0-611">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="c78d0-612">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="c78d0-612">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="c78d0-613">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="c78d0-613">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="c78d0-614">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="c78d0-614">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="c78d0-615">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="c78d0-615">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="c78d0-616">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSServiceBusDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="c78d0-616">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="c78d0-617">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c78d0-617">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="c78d0-618">Beispiel für „New-AzureRmServiceFabricCluster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-618">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="c78d0-619">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="c78d0-619">AzureRM.Sql</span></span>
* <span data-ttu-id="c78d0-620">Neue Cmdlets für „Management.Sql“ hinzugefügt, um Kunden das Hinzufügen des TDE-Zertifikats zu einer SQL Server-Instanz oder einer verwalteten Instanz zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="c78d0-620">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="c78d0-621">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="c78d0-621">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="c78d0-622">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="c78d0-622">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="c78d0-623">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="c78d0-623">AzureRM.Websites</span></span>
* <span data-ttu-id="c78d0-624">Wenn `Set-AzureRmWebApp -AssignIdentity` und `Set-AzureRmWebAppSlot -AssignIdentity` auf „false“ festgelegt sind, wird jetzt die Identity-Eigenschaft aus dem Websiteobjekt entfernt. Auch das Vorschau-Tag wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-624">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="c78d0-625">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics`-Beispiel aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-625">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="c78d0-626">Unterstützung von `Set-AzureRmWebApp -PhpVersion` als gültige PHP-Version eingestellt</span><span class="sxs-lookup"><span data-stu-id="c78d0-626">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="c78d0-627">6.4.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="c78d0-627">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="c78d0-628">Allgemein</span><span class="sxs-lookup"><span data-stu-id="c78d0-628">General</span></span>
* <span data-ttu-id="c78d0-629">Formatierung von OutputType in Hilfedateien für die meisten Module korrigiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-629">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="c78d0-630">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c78d0-630">AzureRM.Profile</span></span>
* <span data-ttu-id="c78d0-631">Attribut „Ps1Xml“ wurde den Standardausgabetypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-631">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="c78d0-632">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c78d0-632">AzureRM.Compute</span></span>
* <span data-ttu-id="c78d0-633">IP-Tag-Funktion für VMSS</span><span class="sxs-lookup"><span data-stu-id="c78d0-633">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="c78d0-634">Cmdlet „New-AzureRmVmssIpTagConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-634">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="c78d0-635">IpTag-Parameter zu „New-AzureRmVmssIpConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-635">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="c78d0-636">Funktion für automatisches Betriebssystemrollback für VMSS</span><span class="sxs-lookup"><span data-stu-id="c78d0-636">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="c78d0-637">DisableAutoRollback-Parameter zu „New-AzureRmVmssConfig“ und „Update-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-637">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="c78d0-638">Funktion für Upgradeverlauf des Betriebssystems für VMSS</span><span class="sxs-lookup"><span data-stu-id="c78d0-638">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="c78d0-639">Switch-Parameter „OSUpgradeHistory“ zu „Get-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-639">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="c78d0-640">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="c78d0-640">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="c78d0-641">Unterstützung für Katalog-ACLs über die folgenden Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="c78d0-641">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="c78d0-642">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="c78d0-642">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="c78d0-643">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="c78d0-643">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="c78d0-644">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="c78d0-644">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="c78d0-645">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78d0-645">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="c78d0-646">Abbruchunterstützung und Nachverfolgung des Fortschritts für „Set-AzureRmDataLakeStoreItemAclEntry“, „Remove-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-646">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="c78d0-647">Abbruchunterstützung „Export-AzureRmDataLakeStoreChildItemProperties“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-647">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="c78d0-648">Leerung von Debugmeldungen für Cmdlets korrigiert, die rekursive Vorgänge durchführt</span><span class="sxs-lookup"><span data-stu-id="c78d0-648">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="c78d0-649">Speicherort des Test von DataLake-Cmdlets korrigiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-649">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="c78d0-650">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="c78d0-650">AzureRM.EventHub</span></span>
* <span data-ttu-id="c78d0-651">Optionaler Parameter „MaxCount“ zu Listenvorgangs-Cmdlets „Get-AzureRmEventHub“ und „Get-AzureRmEventHubConsumerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-651">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="c78d0-652">Problem in Cmdlet „New-AzureRmEventHub“ behoben, aufgrund dessen beim Erstellen einer neuen EventHub-Instanz mindestens ein Parameter benötigt wurde.</span><span class="sxs-lookup"><span data-stu-id="c78d0-652">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="c78d0-653">Standardparametersatz wurde bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-653">Provided Default Parameter set.</span></span>
* <span data-ttu-id="c78d0-654">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmEventHubKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="c78d0-654">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="c78d0-655">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78d0-655">AzureRM.KeyVault</span></span>
* <span data-ttu-id="c78d0-656">Problem behoben, aufgrund dessen von „Get-AzureRmKeyVault -Tag“ alle Ressourcen zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="c78d0-656">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="c78d0-657">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c78d0-657">AzureRM.Network</span></span>
* <span data-ttu-id="c78d0-658">Neue SKUs für zonenredundante VirtualNetworkGateways-Instanzen verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="c78d0-658">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="c78d0-659">Neue Befehle für Funktion hinzugefügt: ExpressRoute-Partner-APIs über ARM</span><span class="sxs-lookup"><span data-stu-id="c78d0-659">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="c78d0-660">Get-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-660">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="c78d0-661">Set-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-661">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="c78d0-662">Add-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-662">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="c78d0-663">Get-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-663">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="c78d0-664">Remove-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-664">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="c78d0-665">Get-AzureRMExpressRouteCrossConnectionArpTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-665">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="c78d0-666">Get-AzureRMExpressRouteCrossConnectionRouteTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-666">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="c78d0-667">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-667">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="c78d0-668">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="c78d0-668">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="c78d0-669">Cmdlet „Get-AzureRmRecoveryServicesBackupStatus“ wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-669">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="c78d0-670">Dieses Cmdlet überprüft anhand der ID eines virtuellen Computers, ob dieser durch einen Tresor im Abonnement geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="c78d0-670">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="c78d0-671">Wenn ein solcher Tresor vorhanden ist, gibt das Cmdlet die Tresordetails aus.</span><span class="sxs-lookup"><span data-stu-id="c78d0-671">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="c78d0-672">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="c78d0-672">AzureRM.Resources</span></span>
* <span data-ttu-id="c78d0-673">Cmdlets vom Typ „Get-AzureRmPolicyAssignment“ aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="c78d0-673">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="c78d0-674">Unterstützung für das Auflisten von „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-674">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="c78d0-675">Unterstützung für das Abrufen einzelner Arbeitsaufträge mit „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-675">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="c78d0-676">Switches „-Effective“ und „-All“ zu Steuerparameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-676">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="c78d0-677">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicyDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-677">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="c78d0-678">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="c78d0-678">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="c78d0-679">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="c78d0-679">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="c78d0-680">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicySetDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-680">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="c78d0-681">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="c78d0-681">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="c78d0-682">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="c78d0-682">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="c78d0-683">Unterstützung für KeyVault-Geheimnisverweis in Parametern hinzugefügt, wenn „TemplateParameterObject“ in „New-AzureRmResourceGroupDeployment“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="c78d0-683">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="c78d0-684">Problem behoben, aufgrund dessen, der Parameter „-EndDate“ für „New-AzureRmADAppCredential“ ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="c78d0-684">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="c78d0-685">Problem behoben, aufgrund dessen „Add-AzureRmADGroupMember“ eine falsche URL für Anforderungen verwendete</span><span class="sxs-lookup"><span data-stu-id="c78d0-685">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="c78d0-686">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c78d0-686">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="c78d0-687">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmServiceBusKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="c78d0-687">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="c78d0-688">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="c78d0-688">AzureRM.Sql</span></span>
* <span data-ttu-id="c78d0-689">Benutzerdefinierte Wiederherstellungspunkte für SQLDW in Hilfe zu „New-AzureRmSqlDatabaseRestorePoint“ erläutert</span><span class="sxs-lookup"><span data-stu-id="c78d0-689">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="c78d0-690">Dokumentation von Parameter „-ComputeGeneration“ in mehreren Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-690">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="c78d0-691">6.3.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="c78d0-691">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="c78d0-692">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c78d0-692">AzureRM.Profile</span></span>
* <span data-ttu-id="c78d0-693">Aktualisierte Fehlermeldungen für „Enable-AzureRmContextAutoSave“</span><span class="sxs-lookup"><span data-stu-id="c78d0-693">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="c78d0-694">Erstellen eines Kontexts für jedes Abonnement beim Ausführen von „Connect-AzureRmAccount“ ohne vorherigen Kontext</span><span class="sxs-lookup"><span data-stu-id="c78d0-694">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="c78d0-695">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="c78d0-695">Azure.Storage</span></span>
* <span data-ttu-id="c78d0-696">Zusätzliche Informationen zum Parameter „-Permissions“ in Hilfedateien</span><span class="sxs-lookup"><span data-stu-id="c78d0-696">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="c78d0-697">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c78d0-697">AzureRM.Compute</span></span>
* <span data-ttu-id="c78d0-698">„Get-AzureRmVmDiskEncryptionStatus“ behebt ein Problem, das bei virtuellen Computern ohne Datenträger festgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="c78d0-698">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="c78d0-699">Version der Computeclientbibliothek aktualisiert, um folgende Cmdlets zu korrigieren:</span><span class="sxs-lookup"><span data-stu-id="c78d0-699">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="c78d0-700">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="c78d0-700">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="c78d0-701">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="c78d0-701">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="c78d0-702">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="c78d0-702">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="c78d0-703">Die folgenden Cmdlets wurden korrigiert, um die Vorgangs-ID und den Vorgangsstatus korrekt anzuzeigen:</span><span class="sxs-lookup"><span data-stu-id="c78d0-703">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="c78d0-704">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="c78d0-704">Start-AzureRmVM</span></span>
    - <span data-ttu-id="c78d0-705">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="c78d0-705">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="c78d0-706">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="c78d0-706">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="c78d0-707">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="c78d0-707">Set-AzureRmVM</span></span>
    - <span data-ttu-id="c78d0-708">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="c78d0-708">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="c78d0-709">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="c78d0-709">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="c78d0-710">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="c78d0-710">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="c78d0-711">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="c78d0-711">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="c78d0-712">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="c78d0-712">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="c78d0-713">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="c78d0-713">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="c78d0-714">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="c78d0-714">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="c78d0-715">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="c78d0-715">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="c78d0-716">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="c78d0-716">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="c78d0-717">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="c78d0-717">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="c78d0-718">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="c78d0-718">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="c78d0-719">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="c78d0-719">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="c78d0-720">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="c78d0-720">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="c78d0-721">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="c78d0-721">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="c78d0-722">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="c78d0-722">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="c78d0-723">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c78d0-723">AzureRM.EventGrid</span></span>
* <span data-ttu-id="c78d0-724">ValidateNotNullOrEmpty-Überprüfungskonditionen für „SubjectBeginsWith“/„SubjectEndsWith“ im Cmdlet „Update-AzureRmEventGridSubscription“ wurden entfernt, um bei Bedarf die Änderung dieser Parameter in eine leere Zeichenfolge zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="c78d0-724">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="c78d0-725">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78d0-725">AzureRM.KeyVault</span></span>
* <span data-ttu-id="c78d0-726">Ein Problem wurde behoben, aufgrund dessen bei Ausführung von „Get-AzureRmKeyVault -Tag“ keine Tags zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="c78d0-726">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="c78d0-727">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c78d0-727">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="c78d0-728">Offizielle Veröffentlichung von Policy Insights-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="c78d0-728">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="c78d0-729">Verwendung der API-Version 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="c78d0-729">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="c78d0-730">„PolicyDefinitionReferenceId“ zu den Ergebnissen von „Get-AzureRmPolicyStateSummary“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-730">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="c78d0-731">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="c78d0-731">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="c78d0-732">Parameter „-Vault“ zu den RecoveryServices.Backup-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-732">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="c78d0-733">Bei der Übergabe wird dadurch das Cmdlet „Set-AzureRmRecoveryServicesContext“ außer Kraft gesetzt.</span><span class="sxs-lookup"><span data-stu-id="c78d0-733">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="c78d0-734">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="c78d0-734">AzureRM.Sql</span></span>
* <span data-ttu-id="c78d0-735">Aktualisiertes Beispiel in der Hilfedatei für „Get-AzureRmSqlDatabaseExpanded“</span><span class="sxs-lookup"><span data-stu-id="c78d0-735">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="c78d0-736">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c78d0-736">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="c78d0-737">Hilfedatei für „Add-AzureRmTrafficManagerEndpointConfig“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c78d0-737">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="c78d0-738">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="c78d0-738">AzureRM.Websites</span></span>
* <span data-ttu-id="c78d0-739">„Set-AzureRmWebApp“ wurde aktualisiert, damit „AppSettings“ bei der Verwendung von „-AssignIdentity“ nicht außer Kraft gesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="c78d0-739">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="c78d0-740">„New-AzureRmWebAppSlot“ wurde aktualisiert, um „AppServicePlan“ als optionalen Parameter anzuerkennen</span><span class="sxs-lookup"><span data-stu-id="c78d0-740">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="c78d0-741">6.2.1: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="c78d0-741">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="c78d0-742">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c78d0-742">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="c78d0-743">PSWorkspace-Modell aktualisiert, damit das Netzwerk „type“ als Parameter verwenden kann</span><span class="sxs-lookup"><span data-stu-id="c78d0-743">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="c78d0-744">6.2.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="c78d0-744">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="c78d0-745">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c78d0-745">AzureRM.Profile</span></span>
* <span data-ttu-id="c78d0-746">Beheben des Problems, aufgrund dessen Version 10.0.3 von Newtonsoft.Json beim Modulimport nicht geladen wurde</span><span class="sxs-lookup"><span data-stu-id="c78d0-746">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="c78d0-747">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c78d0-747">AzureRM.Compute</span></span>
* <span data-ttu-id="c78d0-748">Feature zum Aktualisieren von virtuellen VMSS-Computern</span><span class="sxs-lookup"><span data-stu-id="c78d0-748">VMSS VM Update feature</span></span>
    - <span data-ttu-id="c78d0-749">Cmdlets „Update-AzureRmVmssVM“ und „New-AzureRmVMDataDisk“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-749">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="c78d0-750">Fügen Sie den Parameter „VirtualMachineScaleSetVM“ zum Cmdlet „Add-AzureRmVMDataDisk“ hinzu, um das Hinzufügen eines Datenträgers zum virtuellen VMSS-Computer zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="c78d0-750">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="c78d0-751">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="c78d0-751">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="c78d0-752">Aktualisierung der ADF .Net SDK-Version auf 0.8.0-preview mit den folgenden Änderungen:</span><span class="sxs-lookup"><span data-stu-id="c78d0-752">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="c78d0-753">Vorgang zum Konfigurieren des Factoryrepositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-753">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="c78d0-754">Der verknüpfte QuickBooks-Dienst wurde aktualisiert, um die Eigenschaften „consumerKey“ und „consumerSecret“ verfügbar zu machen.</span><span class="sxs-lookup"><span data-stu-id="c78d0-754">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="c78d0-755">Aktualisierung verschiedener Modelltypen von „SecretBase“ auf „Object“</span><span class="sxs-lookup"><span data-stu-id="c78d0-755">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="c78d0-756">Blobereignisauslöser hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-756">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="c78d0-757">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78d0-757">AzureRM.KeyVault</span></span>
* <span data-ttu-id="c78d0-758">Aktualisierung der Dokumentation mit Beispielausgabe</span><span class="sxs-lookup"><span data-stu-id="c78d0-758">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="c78d0-759">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c78d0-759">AzureRM.Network</span></span>
* <span data-ttu-id="c78d0-760">Aktivierung der Traffic Analytics-Parameter für Network Watcher-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="c78d0-760">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="c78d0-761">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="c78d0-761">AzureRM.Resources</span></span>
* <span data-ttu-id="c78d0-762">Behebung des Problems mit der Eigenschaft „Properties“ von PSResource-Objekten, die von „Get-AzureRmResource“ zurückgegeben wurden</span><span class="sxs-lookup"><span data-stu-id="c78d0-762">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="c78d0-763">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="c78d0-763">AzureRM.Scheduler</span></span>
* <span data-ttu-id="c78d0-764">Behebung des Problems, dass beim Aktualisieren von „ServiceBusQueueJob“ keine neuen Authentifizierungswerte festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="c78d0-764">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="c78d0-765">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="c78d0-765">AzureRM.Sql</span></span>
* <span data-ttu-id="c78d0-766">Aktualisierung der folgenden Cmdlets mit dem optionalen LicenseType-Parameter</span><span class="sxs-lookup"><span data-stu-id="c78d0-766">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="c78d0-767">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="c78d0-767">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="c78d0-768">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="c78d0-768">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="c78d0-769">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="c78d0-769">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="c78d0-770">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="c78d0-770">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="c78d0-771">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="c78d0-771">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="c78d0-772">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="c78d0-772">AzureRM.Websites</span></span>
* <span data-ttu-id="c78d0-773">„New-AzureRMWebApp“ aktualisiert, um allgemeine Algorithmen aus der Strategiebibliothek zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="c78d0-773">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="c78d0-774">6.1.0 – Mai 2018</span><span class="sxs-lookup"><span data-stu-id="c78d0-774">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="c78d0-775">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c78d0-775">AzureRM.Profile</span></span>
* <span data-ttu-id="c78d0-776">Behebung eines Problems, durch das beim Ausführen von „Clear-AzureRmContext“ ein leerer Kontext mit dem Namen des vorherigen Standardkontexts beibehalten wurde und der Benutzer dadurch keinen neuen Kontext mit dem alten Namen erstellen konnte</span><span class="sxs-lookup"><span data-stu-id="c78d0-776">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="c78d0-777">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c78d0-777">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="c78d0-778">Ermöglichung der Zuordnung von Gateways/Aufhebung der Gatewayzuordnung in AS</span><span class="sxs-lookup"><span data-stu-id="c78d0-778">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="c78d0-779">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c78d0-779">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="c78d0-780">Unterstützung für „ApiVersions“, „ApiReleases“ und „ApiRevisions“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-780">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="c78d0-781">Unterstützung für ServiceFabric-Back-End hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-781">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="c78d0-782">Unterstützung für Application Insights-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-782">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="c78d0-783">Unterstützung für die Erkennung von SKUs vom Typ „Basic“ als gültige SKU des API Management-Diensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-783">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="c78d0-784">Unterstützung hinzugefügt, damit Zertifikate, die von der privaten Zertifizierungsstelle ausgestellt wurden, als Stamm- oder ZS-Zertifikate installiert werden können</span><span class="sxs-lookup"><span data-stu-id="c78d0-784">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="c78d0-785">Unterstützung für die Akzeptierung benutzerdefinierter SSL-Zertifikate über KeyVault und mehrere Proxyhostnamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-785">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="c78d0-786">Unterstützung für die verwaltete Dienstidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-786">Added support for MSI identity</span></span>
* <span data-ttu-id="c78d0-787">Unterstützung für die Annahme von Richtlinien über URL hinzugefügt; HINWEIS: Folgende Cmdlets werden in einem zukünftigen Release als veraltet gekennzeichnet:</span><span class="sxs-lookup"><span data-stu-id="c78d0-787">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="c78d0-788">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="c78d0-788">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="c78d0-789">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="c78d0-789">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="c78d0-790">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="c78d0-790">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="c78d0-791">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="c78d0-791">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="c78d0-792">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="c78d0-792">AzureRM.Batch</span></span>
* <span data-ttu-id="c78d0-793">Veröffentlichung des neuen Cmdlets „Get-AzureBatchPoolNodeCounts“</span><span class="sxs-lookup"><span data-stu-id="c78d0-793">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="c78d0-794">Veröffentlichung des neuen Cmdlets „Start-AzureBatchComputeNodeServiceLogUpload“</span><span class="sxs-lookup"><span data-stu-id="c78d0-794">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="c78d0-795">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="c78d0-795">AzureRM.Consumption</span></span>
* <span data-ttu-id="c78d0-796">Hinzufügung neuer Parameter („Expand“, „ResourceGroup“, „InstanceName“, „InstanceId“, „Tags“ und „Top“) für das Cmdlet „Get-AzureRmConsumptionUsageDetail“</span><span class="sxs-lookup"><span data-stu-id="c78d0-796">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="c78d0-797">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78d0-797">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="c78d0-798">Korrektur des Beispiels für „Export AzureRmDataLakeStoreChildItemProperties“</span><span class="sxs-lookup"><span data-stu-id="c78d0-798">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="c78d0-799">Korrektur der NULL-Parameterausnahme für rekursiven Fall in „Set-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="c78d0-799">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="c78d0-800">Korrektur der Hilfedateien für „Set-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ und „Remove-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="c78d0-800">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="c78d0-801">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c78d0-801">AzureRM.Network</span></span>
* <span data-ttu-id="c78d0-802">Erhöhung der Network SDK-Version von 18.0.0-preview auf 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="c78d0-802">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="c78d0-803">Cmdlet zum Erstellen der Protokollkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-803">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="c78d0-804">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="c78d0-804">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="c78d0-805">Cmdlet zum Hinzufügen einer neuen Leitungsverbindung zu einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-805">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="c78d0-806">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-806">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="c78d0-807">Cmdlet zum Entfernen einer Leitungsverbindung aus einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-807">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="c78d0-808">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-808">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="c78d0-809">Cmdlet zum Abrufen einer Leitungsverbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c78d0-809">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="c78d0-810">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="c78d0-810">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="c78d0-811">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c78d0-811">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="c78d0-812">Verwendung der Serverauthentifizierung mit generierten Zertifikaten korrigiert (Problemnr. 5998)</span><span class="sxs-lookup"><span data-stu-id="c78d0-812">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="c78d0-813">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="c78d0-813">AzureRM.Sql</span></span>
* <span data-ttu-id="c78d0-814">Überwachungscmdlets korrigiert, um das Entfernen von „AuditActions“ oder „AuditActionGroups“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="c78d0-814">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="c78d0-815">Problem mit „Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy“ behoben, das beim Festlegen einer neuen flexiblen Aufbewahrungsrichtlinie zu folgendem Fehler führte: „Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span><span class="sxs-lookup"><span data-stu-id="c78d0-815">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="c78d0-816">Please submit request with the new flexible retention policy“ (Das Konfigurieren einer langfristigen Aufbewahrungsrichtlinie mit Azure Recovery Service-Tresor und -Richtlinie wird nicht mehr unterstützt. Übermitteln Sie eine Anforderung mit der neuen flexiblen Aufbewahrungsrichtlinie.)</span><span class="sxs-lookup"><span data-stu-id="c78d0-816">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="c78d0-817">Aktualisierung aller Cmdlets für Azure SQL-Datenbank, für die Erstellung von Pools für elastische Datenbanken und für die Aktualisierung, sodass sie die neue Datenbank-API verwenden. Diese unterstützt die Sku-Eigenschaft für skalierungs- und tarifbezogene Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="c78d0-817">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="c78d0-818">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c78d0-818">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="c78d0-819">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="c78d0-819">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="c78d0-820">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="c78d0-820">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="c78d0-821">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="c78d0-821">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="c78d0-822">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="c78d0-822">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="c78d0-823">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="c78d0-823">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="c78d0-824">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c78d0-824">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="c78d0-825">Aktualisierung der Parameter für „Get-AzureRmTrafficManagerProfile“, sodass bei Verwendung des Parameters „-Name“ der Parameter „-ResourceGroupName“ erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="c78d0-825">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
