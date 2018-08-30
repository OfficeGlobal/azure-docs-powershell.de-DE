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
ms.openlocfilehash: 340c1d2d28e1b97cdd2ec98033361eb00b4302da
ms.sourcegitcommit: 72086f8d368ec84bd403e802305acfc336c08978
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/14/2018
ms.locfileid: "43018974"
---
# <a name="release-notes"></a><span data-ttu-id="795b5-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="795b5-103">Release notes</span></span>

<span data-ttu-id="795b5-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="795b5-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="660---july-2018"></a><span data-ttu-id="795b5-105">6.6.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="795b5-105">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="795b5-106">Allgemein</span><span class="sxs-lookup"><span data-stu-id="795b5-106">General</span></span>
* <span data-ttu-id="795b5-107">Alle Hilfedateien aktualisiert, um vollständige Parametertypen und die richtigen Eingabe/Ausgabe-Typen einzuschließen.</span><span class="sxs-lookup"><span data-stu-id="795b5-107">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="795b5-108">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="795b5-108">AzureRM.Profile</span></span>
* <span data-ttu-id="795b5-109">Bibliothek „Common.Strategy“ aktualisiert, um überprüfen zu können, ob die aktuelle Konfiguration für eine Ressource mit der Zielressource kompatibel ist.</span><span class="sxs-lookup"><span data-stu-id="795b5-109">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="795b5-110">ps1xml-Typen zu „Common.Storage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-110">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="795b5-111">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="795b5-111">Azure.Storage</span></span>
* <span data-ttu-id="795b5-112">Unterstützung zum Abrufen von Speicherkontext aus „DefaultProfile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-112">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="795b5-113">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-113">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="795b5-114">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="795b5-114">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="795b5-115">Problem https://github.com/Azure/azure-powershell/issues/6370 behoben</span><span class="sxs-lookup"><span data-stu-id="795b5-115">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="795b5-116">Fehler in Automapper behoben, um „PsApiManagementApi“ in „ApiContract“ zu verschieben</span><span class="sxs-lookup"><span data-stu-id="795b5-116">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="795b5-117">Problem https://github.com/Azure/azure-powershell/issues/6515 behoben</span><span class="sxs-lookup"><span data-stu-id="795b5-117">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="795b5-118">Fehler in „File.Save“ behoben, um Überladung mit Codierungstyp zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="795b5-118">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="795b5-119">Problem https://github.com/Azure/azure-powershell/issues/6560 behoben</span><span class="sxs-lookup"><span data-stu-id="795b5-119">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="795b5-120">Upgrade auf Nuget-Version 4.0.3 durchgeführt, in der Musterausnahme in „apiId“ behoben wurde</span><span class="sxs-lookup"><span data-stu-id="795b5-120">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="795b5-121">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="795b5-121">AzureRM.Compute</span></span>
* <span data-ttu-id="795b5-122">Das Problem, aufgrund dessen beim Erstellen eines virtuellen Computers mithilfe von „DiskFileParameterSet“ in „New-AzureRmVm“ wegen einer Umbenennung des Speicherkontotyps „PremiumLRS“ ein Fehler auftrat, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="795b5-122">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="795b5-123">Cmdlet „Invoke-AzureRmVMRunCommand“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="795b5-123">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="795b5-124">„Get-AzureRmAvailabilitySet“ aktualisiert, um die Auflistung aller Verfügbarkeitsgruppen in einem Abonnement zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="795b5-124">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="795b5-125">(ResouceGroupName-Parameter ist jetzt optional.)</span><span class="sxs-lookup"><span data-stu-id="795b5-125">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="795b5-126">„SimpleParameterSet“ von „New-AzureRmVm“ aktualisiert, um Accelerated Networking auf kompatiblen virtuellen Computern zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="795b5-126">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="795b5-127">Einfacher Parametersatz „New-AzureRmVmss“ aktualisiert, sodass das Erstellen der VMSS fehlschlägt, wenn bereits ein benutzerdefinierter LB vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="795b5-127">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="795b5-128">Beispiel für „New-AzureRmDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="795b5-128">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="795b5-129">Beispiel für „New-AzureRmVM“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-129">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="795b5-130">Beschreibung für „Set-AzureRmVMOSDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="795b5-130">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="795b5-131">Beispiel 1 für „Set-AzureRmVMBginfoExtension“ aktualisiert, um Rechtschreibung und Präfix zu korrigieren.</span><span class="sxs-lookup"><span data-stu-id="795b5-131">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="795b5-132">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="795b5-132">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="795b5-133">ADF .Net SDK-Version auf 1.1.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="795b5-133">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="795b5-134">Unterstützung der Freigabe der selbstgehosteten Integration Runtime über Data Factorys hinweg.</span><span class="sxs-lookup"><span data-stu-id="795b5-134">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="795b5-135">Neuer Parameter „-SharedIntegrationRuntimeResourceId“ zu Cmdlet „Set-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="795b5-135">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="795b5-136">Neuer optionaler Parameter „-LinkedDataFactoryName“ zu Cmdlet „Remove-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="795b5-136">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="795b5-137">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="795b5-137">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="795b5-138">DataPlane SDK-Version (Microsoft.Azure.DataLake.Store) auf 1.1.9 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="795b5-138">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="795b5-139">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="795b5-139">AzureRM.EventHub</span></span>
* <span data-ttu-id="795b5-140">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="795b5-140">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="795b5-141">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="795b5-141">AzureRM.Insights</span></span>
* <span data-ttu-id="795b5-142">Formatierung von „OutputType“ in Hilfedateien korrigiert</span><span class="sxs-lookup"><span data-stu-id="795b5-142">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="795b5-143">Verwendung von Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span><span class="sxs-lookup"><span data-stu-id="795b5-143">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="795b5-144">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="795b5-144">AzureRM.KeyVault</span></span>
* <span data-ttu-id="795b5-145">Piping-Problem in „Set-AzureRmKeyVaultAccessPolicy“ behoben</span><span class="sxs-lookup"><span data-stu-id="795b5-145">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="795b5-146">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="795b5-146">AzureRM.Network</span></span>
* <span data-ttu-id="795b5-147">Beispiele für LoadBalancerInboundNatPoolConfig-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="795b5-147">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="795b5-148">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="795b5-148">AzureRM.Resources</span></span>
* <span data-ttu-id="795b5-149">Problem beim Angeben sowohl des Tag-Namens als auch des Werts für „Get-AzureRmResource“ behoben</span><span class="sxs-lookup"><span data-stu-id="795b5-149">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="795b5-150">Piping-Szenario mit „Set-AzureRmResource“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="795b5-150">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="795b5-151">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="795b5-151">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="795b5-152">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="795b5-152">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="795b5-153">Einige Probleme behoben</span><span class="sxs-lookup"><span data-stu-id="795b5-153">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="795b5-154">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="795b5-154">AzureRM.Sql</span></span>
* <span data-ttu-id="795b5-155">Unterstützung für Advanced Threat Protection für Server bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="795b5-155">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="795b5-156">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="795b5-156">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="795b5-157">Unterstützung für Sicherheitsrisikobewertung bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="795b5-157">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="795b5-158">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="795b5-158">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="795b5-159">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="795b5-159">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="795b5-160">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="795b5-160">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="795b5-161">Beispiel in „Remove-AzureRmSqlServerFirewallRule“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="795b5-161">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="795b5-162">Falsche Verarbeitung von „datetime“ für nicht US-basierte Kultur in „Get-AzureSqlSyncGroupLog“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="795b5-162">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="795b5-163">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="795b5-163">AzureRM.Storage</span></span>
* <span data-ttu-id="795b5-164">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-164">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="795b5-165">Cmdlet-Ausgabe von „StorageAccount“ in Tabellenansicht anzeigen</span><span class="sxs-lookup"><span data-stu-id="795b5-165">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="795b5-166">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="795b5-166">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="795b5-167">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="795b5-167">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="795b5-168">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="795b5-168">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="795b5-169">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="795b5-169">AzureRM.Tags</span></span>
* <span data-ttu-id="795b5-170">Falsche Anweisung aus Tag-Cmdlet-Hilfe entfernt</span><span class="sxs-lookup"><span data-stu-id="795b5-170">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="795b5-171">6.5.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="795b5-171">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="795b5-172">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="795b5-172">AzureRM.Profile</span></span>
* <span data-ttu-id="795b5-173">Hilfe für „Get-AzureRmContextAutosaveSetting“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="795b5-173">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="795b5-174">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="795b5-174">Azure.Storage</span></span>
* <span data-ttu-id="795b5-175">Unterstützung des Blob- oder Dateiuploads mit lesegeschütztem SAS-Token</span><span class="sxs-lookup"><span data-stu-id="795b5-175">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="795b5-176">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="795b5-176">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="795b5-177">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="795b5-177">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="795b5-178">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="795b5-178">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="795b5-179">Erforderliche Eigenschaft „ResourceGroupName“ zu AS hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="795b5-179">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="795b5-180">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="795b5-180">AzureRM.Automation</span></span>
* <span data-ttu-id="795b5-181">Hilfe aktualisiert und Beispiel für „New-AzureRMAutomationSchedule“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-181">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="795b5-182">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="795b5-182">AzureRM.Compute</span></span>
* <span data-ttu-id="795b5-183">Parameter „-Tag“ zu „Update/New-AzureRmAvailabilitySet“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-183">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="795b5-184">Beispiel für „Add-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-184">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="795b5-185">Beispiele für „Remove-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-185">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="795b5-186">Hilfe für „Set-AzureRmVMAccessExtension“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="795b5-186">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="795b5-187">„SimpleParameterSet“ für „New-AzureRmVmss“ so aktualisiert, dass „SinglePlacementGroup“ standardmäßig auf „false“ festgelegt ist, und Switch-Parameter „SinglePlacementGroup“ hinzugefügt, der dem Benutzer das Erstellen der VMSS in einer einzelnen Platzierungsgruppe ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="795b5-187">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="795b5-188">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="795b5-188">AzureRM.EventHub</span></span>
* <span data-ttu-id="795b5-189">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSEventHubDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="795b5-189">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="795b5-190">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="795b5-190">AzureRM.KeyVault</span></span>
* <span data-ttu-id="795b5-191">Fehlermeldung für „Set-AzureRmKeyVaultAccessPolicy“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="795b5-191">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="795b5-192">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="795b5-192">AzureRM.LogicApp</span></span>
* <span data-ttu-id="795b5-193">Fehler „Parametersatz konnte nicht aufgelöst werden“ in „New-AzureRmLogicApp“behoben</span><span class="sxs-lookup"><span data-stu-id="795b5-193">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="795b5-194">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="795b5-194">AzureRM.Network</span></span>
* <span data-ttu-id="795b5-195">Peering über mehrere virtuelle Netzwerke in mehreren Mandanten für „Set/Add-AzureRmVirtualNetworkPeering“ aktiviert</span><span class="sxs-lookup"><span data-stu-id="795b5-195">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="795b5-196">Folgende Cmdlets für Application Gateway aktualisiert</span><span class="sxs-lookup"><span data-stu-id="795b5-196">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="795b5-197">New-AzureRmApplicationGateway: EnableFIPS-Flag und Zonenunterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-197">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="795b5-198">New-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-198">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="795b5-199">Set-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-199">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="795b5-200">RouteTable-Cmdlets mit aktueller Generatorversion erneut generiert</span><span class="sxs-lookup"><span data-stu-id="795b5-200">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="795b5-201">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="795b5-201">AzureRM.Relay</span></span>
* <span data-ttu-id="795b5-202">Markdowndateien aktualisiert, Problem mit Parametername in Beispiel behoben</span><span class="sxs-lookup"><span data-stu-id="795b5-202">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="795b5-203">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="795b5-203">AzureRM.Resources</span></span>
* <span data-ttu-id="795b5-204">Roleassignment- und roledefinition-Cmdlets aktualisiert:</span><span class="sxs-lookup"><span data-stu-id="795b5-204">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="795b5-205">Zusätzliche roledefinition-Aufrufe entfernt, die als Teil des Pagings durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="795b5-205">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="795b5-206">Get-AzureRmRoleAssignment-Cmdlet korrigiert</span><span class="sxs-lookup"><span data-stu-id="795b5-206">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="795b5-207">Befehlsparameterfunktion von „-ExpandPrincipalGroups“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="795b5-207">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="795b5-208">Problem mit „Get-AzureRmResource“ behoben, aufgrund dessen die Groß-/Kleinschreibung des Parameters „-ResourceType“ beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="795b5-208">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="795b5-209">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="795b5-209">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="795b5-210">top- und skip-Parameter zu Listen-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-210">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="795b5-211">Cmdlets für die Migration von Standard- zu Premium-Namespace hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="795b5-211">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="795b5-212">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="795b5-212">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="795b5-213">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="795b5-213">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="795b5-214">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="795b5-214">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="795b5-215">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="795b5-215">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="795b5-216">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="795b5-216">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="795b5-217">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSServiceBusDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="795b5-217">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="795b5-218">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="795b5-218">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="795b5-219">Beispiel für „New-AzureRmServiceFabricCluster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-219">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="795b5-220">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="795b5-220">AzureRM.Sql</span></span>
* <span data-ttu-id="795b5-221">Neue Cmdlets für „Management.Sql“ hinzugefügt, um Kunden das Hinzufügen des TDE-Zertifikats zu einer SQL Server-Instanz oder einer verwalteten Instanz zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="795b5-221">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="795b5-222">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="795b5-222">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="795b5-223">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="795b5-223">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="795b5-224">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="795b5-224">AzureRM.Websites</span></span>
* <span data-ttu-id="795b5-225">Wenn `Set-AzureRmWebApp -AssignIdentity` und `Set-AzureRmWebAppSlot -AssignIdentity` auf „false“ festgelegt sind, wird jetzt die Identity-Eigenschaft aus dem Websiteobjekt entfernt. Auch das Vorschau-Tag wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="795b5-225">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="795b5-226">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics`-Beispiel aktualisiert</span><span class="sxs-lookup"><span data-stu-id="795b5-226">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="795b5-227">Unterstützung von `Set-AzureRmWebApp -PhpVersion` als gültige PHP-Version eingestellt</span><span class="sxs-lookup"><span data-stu-id="795b5-227">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="795b5-228">6.4.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="795b5-228">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="795b5-229">Allgemein</span><span class="sxs-lookup"><span data-stu-id="795b5-229">General</span></span>
* <span data-ttu-id="795b5-230">Formatierung von OutputType in Hilfedateien für die meisten Module korrigiert</span><span class="sxs-lookup"><span data-stu-id="795b5-230">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="795b5-231">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="795b5-231">AzureRM.Profile</span></span>
* <span data-ttu-id="795b5-232">Attribut „Ps1Xml“ wurde den Standardausgabetypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-232">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="795b5-233">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="795b5-233">AzureRM.Compute</span></span>
* <span data-ttu-id="795b5-234">IP-Tag-Funktion für VMSS</span><span class="sxs-lookup"><span data-stu-id="795b5-234">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="795b5-235">Cmdlet „New-AzureRmVmssIpTagConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-235">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="795b5-236">IpTag-Parameter zu „New-AzureRmVmssIpConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-236">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="795b5-237">Funktion für automatisches Betriebssystemrollback für VMSS</span><span class="sxs-lookup"><span data-stu-id="795b5-237">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="795b5-238">DisableAutoRollback-Parameter zu „New-AzureRmVmssConfig“ und „Update-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-238">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="795b5-239">Funktion für Upgradeverlauf des Betriebssystems für VMSS</span><span class="sxs-lookup"><span data-stu-id="795b5-239">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="795b5-240">Switch-Parameter „OSUpgradeHistory“ zu „Get-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-240">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="795b5-241">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="795b5-241">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="795b5-242">Unterstützung für Katalog-ACLs über die folgenden Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="795b5-242">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="795b5-243">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="795b5-243">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="795b5-244">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="795b5-244">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="795b5-245">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="795b5-245">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="795b5-246">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="795b5-246">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="795b5-247">Abbruchunterstützung und Nachverfolgung des Fortschritts für „Set-AzureRmDataLakeStoreItemAclEntry“, „Remove-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-247">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="795b5-248">Abbruchunterstützung „Export-AzureRmDataLakeStoreChildItemProperties“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-248">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="795b5-249">Leerung von Debugmeldungen für Cmdlets korrigiert, die rekursive Vorgänge durchführt</span><span class="sxs-lookup"><span data-stu-id="795b5-249">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="795b5-250">Speicherort des Test von DataLake-Cmdlets korrigiert</span><span class="sxs-lookup"><span data-stu-id="795b5-250">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="795b5-251">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="795b5-251">AzureRM.EventHub</span></span>
* <span data-ttu-id="795b5-252">Optionaler Parameter „MaxCount“ zu Listenvorgangs-Cmdlets „Get-AzureRmEventHub“ und „Get-AzureRmEventHubConsumerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-252">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="795b5-253">Problem in Cmdlet „New-AzureRmEventHub“ behoben, aufgrund dessen beim Erstellen einer neuen EventHub-Instanz mindestens ein Parameter benötigt wurde.</span><span class="sxs-lookup"><span data-stu-id="795b5-253">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="795b5-254">Standardparametersatz wurde bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="795b5-254">Provided Default Parameter set.</span></span>
* <span data-ttu-id="795b5-255">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmEventHubKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="795b5-255">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="795b5-256">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="795b5-256">AzureRM.KeyVault</span></span>
* <span data-ttu-id="795b5-257">Problem behoben, aufgrund dessen von „Get-AzureRmKeyVault -Tag“ alle Ressourcen zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="795b5-257">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="795b5-258">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="795b5-258">AzureRM.Network</span></span>
* <span data-ttu-id="795b5-259">Neue SKUs für zonenredundante VirtualNetworkGateways-Instanzen verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="795b5-259">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="795b5-260">Neue Befehle für Funktion hinzugefügt: ExpressRoute-Partner-APIs über ARM</span><span class="sxs-lookup"><span data-stu-id="795b5-260">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="795b5-261">Get-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-261">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="795b5-262">Set-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-262">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="795b5-263">Add-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-263">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="795b5-264">Get-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-264">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="795b5-265">Remove-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-265">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="795b5-266">Get-AzureRMExpressRouteCrossConnectionArpTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-266">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="795b5-267">Get-AzureRMExpressRouteCrossConnectionRouteTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-267">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="795b5-268">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-268">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="795b5-269">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="795b5-269">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="795b5-270">Cmdlet „Get-AzureRmRecoveryServicesBackupStatus“ wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="795b5-270">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="795b5-271">Dieses Cmdlet überprüft anhand der ID eines virtuellen Computers, ob dieser durch einen Tresor im Abonnement geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="795b5-271">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="795b5-272">Wenn ein solcher Tresor vorhanden ist, gibt das Cmdlet die Tresordetails aus.</span><span class="sxs-lookup"><span data-stu-id="795b5-272">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="795b5-273">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="795b5-273">AzureRM.Resources</span></span>
* <span data-ttu-id="795b5-274">Cmdlets vom Typ „Get-AzureRmPolicyAssignment“ aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="795b5-274">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="795b5-275">Unterstützung für das Auflisten von „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-275">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="795b5-276">Unterstützung für das Abrufen einzelner Arbeitsaufträge mit „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-276">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="795b5-277">Switches „-Effective“ und „-All“ zu Steuerparameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-277">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="795b5-278">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicyDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="795b5-278">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="795b5-279">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="795b5-279">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="795b5-280">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="795b5-280">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="795b5-281">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicySetDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="795b5-281">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="795b5-282">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="795b5-282">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="795b5-283">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="795b5-283">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="795b5-284">Unterstützung für KeyVault-Geheimnisverweis in Parametern hinzugefügt, wenn „TemplateParameterObject“ in „New-AzureRmResourceGroupDeployment“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="795b5-284">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="795b5-285">Problem behoben, aufgrund dessen, der Parameter „-EndDate“ für „New-AzureRmADAppCredential“ ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="795b5-285">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="795b5-286">Problem behoben, aufgrund dessen „Add-AzureRmADGroupMember“ eine falsche URL für Anforderungen verwendete</span><span class="sxs-lookup"><span data-stu-id="795b5-286">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="795b5-287">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="795b5-287">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="795b5-288">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmServiceBusKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="795b5-288">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="795b5-289">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="795b5-289">AzureRM.Sql</span></span>
* <span data-ttu-id="795b5-290">Benutzerdefinierte Wiederherstellungspunkte für SQLDW in Hilfe zu „New-AzureRmSqlDatabaseRestorePoint“ erläutert</span><span class="sxs-lookup"><span data-stu-id="795b5-290">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="795b5-291">Dokumentation von Parameter „-ComputeGeneration“ in mehreren Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="795b5-291">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="795b5-292">6.3.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="795b5-292">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="795b5-293">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="795b5-293">AzureRM.Profile</span></span>
* <span data-ttu-id="795b5-294">Aktualisierte Fehlermeldungen für „Enable-AzureRmContextAutoSave“</span><span class="sxs-lookup"><span data-stu-id="795b5-294">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="795b5-295">Erstellen eines Kontexts für jedes Abonnement beim Ausführen von „Connect-AzureRmAccount“ ohne vorherigen Kontext</span><span class="sxs-lookup"><span data-stu-id="795b5-295">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="795b5-296">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="795b5-296">Azure.Storage</span></span>
* <span data-ttu-id="795b5-297">Zusätzliche Informationen zum Parameter „-Permissions“ in Hilfedateien</span><span class="sxs-lookup"><span data-stu-id="795b5-297">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="795b5-298">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="795b5-298">AzureRM.Compute</span></span>
* <span data-ttu-id="795b5-299">„Get-AzureRmVmDiskEncryptionStatus“ behebt ein Problem, das bei virtuellen Computern ohne Datenträger festgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="795b5-299">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="795b5-300">Version der Computeclientbibliothek aktualisiert, um folgende Cmdlets zu korrigieren:</span><span class="sxs-lookup"><span data-stu-id="795b5-300">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="795b5-301">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="795b5-301">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="795b5-302">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="795b5-302">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="795b5-303">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="795b5-303">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="795b5-304">Die folgenden Cmdlets wurden korrigiert, um die Vorgangs-ID und den Vorgangsstatus korrekt anzuzeigen:</span><span class="sxs-lookup"><span data-stu-id="795b5-304">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="795b5-305">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="795b5-305">Start-AzureRmVM</span></span>
    - <span data-ttu-id="795b5-306">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="795b5-306">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="795b5-307">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="795b5-307">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="795b5-308">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="795b5-308">Set-AzureRmVM</span></span>
    - <span data-ttu-id="795b5-309">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="795b5-309">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="795b5-310">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="795b5-310">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="795b5-311">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="795b5-311">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="795b5-312">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="795b5-312">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="795b5-313">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="795b5-313">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="795b5-314">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="795b5-314">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="795b5-315">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="795b5-315">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="795b5-316">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="795b5-316">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="795b5-317">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="795b5-317">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="795b5-318">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="795b5-318">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="795b5-319">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="795b5-319">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="795b5-320">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="795b5-320">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="795b5-321">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="795b5-321">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="795b5-322">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="795b5-322">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="795b5-323">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="795b5-323">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="795b5-324">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="795b5-324">AzureRM.EventGrid</span></span>
* <span data-ttu-id="795b5-325">ValidateNotNullOrEmpty-Überprüfungskonditionen für „SubjectBeginsWith“/„SubjectEndsWith“ im Cmdlet „Update-AzureRmEventGridSubscription“ wurden entfernt, um bei Bedarf die Änderung dieser Parameter in eine leere Zeichenfolge zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="795b5-325">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="795b5-326">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="795b5-326">AzureRM.KeyVault</span></span>
* <span data-ttu-id="795b5-327">Ein Problem wurde behoben, aufgrund dessen bei Ausführung von „Get-AzureRmKeyVault -Tag“ keine Tags zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="795b5-327">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="795b5-328">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="795b5-328">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="795b5-329">Offizielle Veröffentlichung von Policy Insights-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="795b5-329">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="795b5-330">Verwendung der API-Version 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="795b5-330">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="795b5-331">„PolicyDefinitionReferenceId“ zu den Ergebnissen von „Get-AzureRmPolicyStateSummary“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-331">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="795b5-332">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="795b5-332">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="795b5-333">Parameter „-Vault“ zu den RecoveryServices.Backup-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="795b5-333">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="795b5-334">Bei der Übergabe wird dadurch das Cmdlet „Set-AzureRmRecoveryServicesContext“ außer Kraft gesetzt.</span><span class="sxs-lookup"><span data-stu-id="795b5-334">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="795b5-335">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="795b5-335">AzureRM.Sql</span></span>
* <span data-ttu-id="795b5-336">Aktualisiertes Beispiel in der Hilfedatei für „Get-AzureRmSqlDatabaseExpanded“</span><span class="sxs-lookup"><span data-stu-id="795b5-336">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="795b5-337">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="795b5-337">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="795b5-338">Hilfedatei für „Add-AzureRmTrafficManagerEndpointConfig“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="795b5-338">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="795b5-339">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="795b5-339">AzureRM.Websites</span></span>
* <span data-ttu-id="795b5-340">„Set-AzureRmWebApp“ wurde aktualisiert, damit „AppSettings“ bei der Verwendung von „-AssignIdentity“ nicht außer Kraft gesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="795b5-340">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="795b5-341">„New-AzureRmWebAppSlot“ wurde aktualisiert, um „AppServicePlan“ als optionalen Parameter anzuerkennen</span><span class="sxs-lookup"><span data-stu-id="795b5-341">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="795b5-342">6.2.1: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="795b5-342">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="795b5-343">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="795b5-343">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="795b5-344">PSWorkspace-Modell aktualisiert, damit das Netzwerk „type“ als Parameter verwenden kann</span><span class="sxs-lookup"><span data-stu-id="795b5-344">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="795b5-345">6.2.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="795b5-345">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="795b5-346">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="795b5-346">AzureRM.Profile</span></span>
* <span data-ttu-id="795b5-347">Beheben des Problems, aufgrund dessen Version 10.0.3 von Newtonsoft.Json beim Modulimport nicht geladen wurde</span><span class="sxs-lookup"><span data-stu-id="795b5-347">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="795b5-348">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="795b5-348">AzureRM.Compute</span></span>
* <span data-ttu-id="795b5-349">Feature zum Aktualisieren von virtuellen VMSS-Computern</span><span class="sxs-lookup"><span data-stu-id="795b5-349">VMSS VM Update feature</span></span>
    - <span data-ttu-id="795b5-350">Cmdlets „Update-AzureRmVmssVM“ und „New-AzureRmVMDataDisk“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-350">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="795b5-351">Fügen Sie den Parameter „VirtualMachineScaleSetVM“ zum Cmdlet „Add-AzureRmVMDataDisk“ hinzu, um das Hinzufügen eines Datenträgers zum virtuellen VMSS-Computer zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="795b5-351">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="795b5-352">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="795b5-352">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="795b5-353">Aktualisierung der ADF .Net SDK-Version auf 0.8.0-preview mit den folgenden Änderungen:</span><span class="sxs-lookup"><span data-stu-id="795b5-353">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="795b5-354">Vorgang zum Konfigurieren des Factoryrepositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-354">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="795b5-355">Der verknüpfte QuickBooks-Dienst wurde aktualisiert, um die Eigenschaften „consumerKey“ und „consumerSecret“ verfügbar zu machen.</span><span class="sxs-lookup"><span data-stu-id="795b5-355">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="795b5-356">Aktualisierung verschiedener Modelltypen von „SecretBase“ auf „Object“</span><span class="sxs-lookup"><span data-stu-id="795b5-356">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="795b5-357">Blobereignisauslöser hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-357">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="795b5-358">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="795b5-358">AzureRM.KeyVault</span></span>
* <span data-ttu-id="795b5-359">Aktualisierung der Dokumentation mit Beispielausgabe</span><span class="sxs-lookup"><span data-stu-id="795b5-359">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="795b5-360">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="795b5-360">AzureRM.Network</span></span>
* <span data-ttu-id="795b5-361">Aktivierung der Traffic Analytics-Parameter für Network Watcher-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="795b5-361">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="795b5-362">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="795b5-362">AzureRM.Resources</span></span>
* <span data-ttu-id="795b5-363">Behebung des Problems mit der Eigenschaft „Properties“ von PSResource-Objekten, die von „Get-AzureRmResource“ zurückgegeben wurden</span><span class="sxs-lookup"><span data-stu-id="795b5-363">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="795b5-364">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="795b5-364">AzureRM.Scheduler</span></span>
* <span data-ttu-id="795b5-365">Behebung des Problems, dass beim Aktualisieren von „ServiceBusQueueJob“ keine neuen Authentifizierungswerte festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="795b5-365">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="795b5-366">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="795b5-366">AzureRM.Sql</span></span>
* <span data-ttu-id="795b5-367">Aktualisierung der folgenden Cmdlets mit dem optionalen LicenseType-Parameter</span><span class="sxs-lookup"><span data-stu-id="795b5-367">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="795b5-368">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="795b5-368">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="795b5-369">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="795b5-369">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="795b5-370">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="795b5-370">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="795b5-371">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="795b5-371">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="795b5-372">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="795b5-372">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="795b5-373">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="795b5-373">AzureRM.Websites</span></span>
* <span data-ttu-id="795b5-374">„New-AzureRMWebApp“ aktualisiert, um allgemeine Algorithmen aus der Strategiebibliothek zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="795b5-374">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="795b5-375">6.1.0 – Mai 2018</span><span class="sxs-lookup"><span data-stu-id="795b5-375">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="795b5-376">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="795b5-376">AzureRM.Profile</span></span>
* <span data-ttu-id="795b5-377">Behebung eines Problems, durch das beim Ausführen von „Clear-AzureRmContext“ ein leerer Kontext mit dem Namen des vorherigen Standardkontexts beibehalten wurde und der Benutzer dadurch keinen neuen Kontext mit dem alten Namen erstellen konnte</span><span class="sxs-lookup"><span data-stu-id="795b5-377">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="795b5-378">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="795b5-378">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="795b5-379">Ermöglichung der Zuordnung von Gateways/Aufhebung der Gatewayzuordnung in AS</span><span class="sxs-lookup"><span data-stu-id="795b5-379">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="795b5-380">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="795b5-380">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="795b5-381">Unterstützung für „ApiVersions“, „ApiReleases“ und „ApiRevisions“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-381">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="795b5-382">Unterstützung für ServiceFabric-Back-End hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-382">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="795b5-383">Unterstützung für Application Insights-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-383">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="795b5-384">Unterstützung für die Erkennung von SKUs vom Typ „Basic“ als gültige SKU des API Management-Diensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-384">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="795b5-385">Unterstützung hinzugefügt, damit Zertifikate, die von der privaten Zertifizierungsstelle ausgestellt wurden, als Stamm- oder ZS-Zertifikate installiert werden können</span><span class="sxs-lookup"><span data-stu-id="795b5-385">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="795b5-386">Unterstützung für die Akzeptierung benutzerdefinierter SSL-Zertifikate über KeyVault und mehrere Proxyhostnamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-386">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="795b5-387">Unterstützung für die verwaltete Dienstidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-387">Added support for MSI identity</span></span>
* <span data-ttu-id="795b5-388">Unterstützung für die Annahme von Richtlinien über URL hinzugefügt; HINWEIS: Folgende Cmdlets werden in einem zukünftigen Release als veraltet gekennzeichnet:</span><span class="sxs-lookup"><span data-stu-id="795b5-388">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="795b5-389">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="795b5-389">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="795b5-390">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="795b5-390">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="795b5-391">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="795b5-391">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="795b5-392">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="795b5-392">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="795b5-393">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="795b5-393">AzureRM.Batch</span></span>
* <span data-ttu-id="795b5-394">Veröffentlichung des neuen Cmdlets „Get-AzureBatchPoolNodeCounts“</span><span class="sxs-lookup"><span data-stu-id="795b5-394">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="795b5-395">Veröffentlichung des neuen Cmdlets „Start-AzureBatchComputeNodeServiceLogUpload“</span><span class="sxs-lookup"><span data-stu-id="795b5-395">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="795b5-396">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="795b5-396">AzureRM.Consumption</span></span>
* <span data-ttu-id="795b5-397">Hinzufügung neuer Parameter („Expand“, „ResourceGroup“, „InstanceName“, „InstanceId“, „Tags“ und „Top“) für das Cmdlet „Get-AzureRmConsumptionUsageDetail“</span><span class="sxs-lookup"><span data-stu-id="795b5-397">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="795b5-398">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="795b5-398">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="795b5-399">Korrektur des Beispiels für „Export AzureRmDataLakeStoreChildItemProperties“</span><span class="sxs-lookup"><span data-stu-id="795b5-399">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="795b5-400">Korrektur der NULL-Parameterausnahme für rekursiven Fall in „Set-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="795b5-400">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="795b5-401">Korrektur der Hilfedateien für „Set-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ und „Remove-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="795b5-401">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="795b5-402">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="795b5-402">AzureRM.Network</span></span>
* <span data-ttu-id="795b5-403">Erhöhung der Network SDK-Version von 18.0.0-preview auf 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="795b5-403">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="795b5-404">Cmdlet zum Erstellen der Protokollkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-404">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="795b5-405">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="795b5-405">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="795b5-406">Cmdlet zum Hinzufügen einer neuen Leitungsverbindung zu einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-406">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="795b5-407">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="795b5-407">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="795b5-408">Cmdlet zum Entfernen einer Leitungsverbindung aus einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-408">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="795b5-409">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="795b5-409">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="795b5-410">Cmdlet zum Abrufen einer Leitungsverbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="795b5-410">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="795b5-411">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="795b5-411">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="795b5-412">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="795b5-412">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="795b5-413">Verwendung der Serverauthentifizierung mit generierten Zertifikaten korrigiert (Problemnr. 5998)</span><span class="sxs-lookup"><span data-stu-id="795b5-413">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="795b5-414">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="795b5-414">AzureRM.Sql</span></span>
* <span data-ttu-id="795b5-415">Überwachungscmdlets korrigiert, um das Entfernen von „AuditActions“ oder „AuditActionGroups“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="795b5-415">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="795b5-416">Problem mit „Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy“ behoben, das beim Festlegen einer neuen flexiblen Aufbewahrungsrichtlinie zu folgendem Fehler führte: „Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span><span class="sxs-lookup"><span data-stu-id="795b5-416">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="795b5-417">Please submit request with the new flexible retention policy“ (Das Konfigurieren einer langfristigen Aufbewahrungsrichtlinie mit Azure Recovery Service-Tresor und -Richtlinie wird nicht mehr unterstützt. Übermitteln Sie eine Anforderung mit der neuen flexiblen Aufbewahrungsrichtlinie.)</span><span class="sxs-lookup"><span data-stu-id="795b5-417">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="795b5-418">Aktualisierung aller Cmdlets für Azure SQL-Datenbank, für die Erstellung von Pools für elastische Datenbanken und für die Aktualisierung, sodass sie die neue Datenbank-API verwenden. Diese unterstützt die Sku-Eigenschaft für skalierungs- und tarifbezogene Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="795b5-418">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="795b5-419">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="795b5-419">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="795b5-420">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="795b5-420">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="795b5-421">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="795b5-421">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="795b5-422">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="795b5-422">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="795b5-423">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="795b5-423">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="795b5-424">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="795b5-424">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="795b5-425">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="795b5-425">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="795b5-426">Aktualisierung der Parameter für „Get-AzureRmTrafficManagerProfile“, sodass bei Verwendung des Parameters „-Name“ der Parameter „-ResourceGroupName“ erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="795b5-426">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
