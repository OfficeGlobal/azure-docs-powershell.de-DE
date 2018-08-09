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
ms.openlocfilehash: 3961f5c37869d0dc877b85bad535f399181040db
ms.sourcegitcommit: afae9f2f091b21ed07d5aec1c249cf859a8b89a4
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/09/2018
ms.locfileid: "39653490"
---
# <a name="release-notes"></a><span data-ttu-id="5a7ce-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="5a7ce-103">Release notes</span></span>

<span data-ttu-id="5a7ce-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="660---july-2018"></a><span data-ttu-id="5a7ce-105">6.6.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="5a7ce-105">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="5a7ce-106">Allgemein</span><span class="sxs-lookup"><span data-stu-id="5a7ce-106">General</span></span>
* <span data-ttu-id="5a7ce-107">Alle Hilfedateien aktualisiert, um vollständige Parametertypen und die richtigen Eingabe/Ausgabe-Typen einzuschließen.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-107">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="5a7ce-108">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5a7ce-108">AzureRM.Profile</span></span>
* <span data-ttu-id="5a7ce-109">Bibliothek „Common.Strategy“ aktualisiert, um überprüfen zu können, ob die aktuelle Konfiguration für eine Ressource mit der Zielressource kompatibel ist.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-109">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span> <span data-ttu-id="5a7ce-110">Standard ist immer „true“, einzelne Ressourcen können den Standard überschreiben.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-110">Default is always true, individual resources and overridet the default.</span></span>
* <span data-ttu-id="5a7ce-111">ps1xml-Typen zu „Common.Storage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-111">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="5a7ce-112">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="5a7ce-112">Azure.Storage</span></span>
* <span data-ttu-id="5a7ce-113">Unterstützung des Abrufs von Speicherkontext von „DefaultProfile“</span><span class="sxs-lookup"><span data-stu-id="5a7ce-113">Support get Storage Context from DefaulfProfile</span></span>
* <span data-ttu-id="5a7ce-114">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-114">Add Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="5a7ce-115">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5a7ce-115">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="5a7ce-116">Problem https://github.com/Azure/azure-powershell/issues/6370 behoben</span><span class="sxs-lookup"><span data-stu-id="5a7ce-116">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="5a7ce-117">Fehler in Automapper behoben, um „PsApiManagementApi“ in „ApiContract“ zu verschieben</span><span class="sxs-lookup"><span data-stu-id="5a7ce-117">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="5a7ce-118">Problem https://github.com/Azure/azure-powershell/issues/6515 behoben</span><span class="sxs-lookup"><span data-stu-id="5a7ce-118">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="5a7ce-119">Fehler in „File.Save“ behoben, um Überladung mit Codierungstyp zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="5a7ce-119">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="5a7ce-120">Problem https://github.com/Azure/azure-powershell/issues/6560 behoben</span><span class="sxs-lookup"><span data-stu-id="5a7ce-120">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="5a7ce-121">Upgrade auf Nuget-Version 4.0.3 durchgeführt, in der Musterausnahme in „apiId“ behoben wurde</span><span class="sxs-lookup"><span data-stu-id="5a7ce-121">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5a7ce-122">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5a7ce-122">AzureRM.Compute</span></span>
* <span data-ttu-id="5a7ce-123">Das Problem, aufgrund dessen beim Erstellen eines virtuellen Computers mithilfe von „DiskFileParameterSet“ in „New-AzureRmVm“ wegen einer Umbenennung des Speicherkontotyps „PremiumLRS“ ein Fehler auftrat, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-123">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="5a7ce-124">Cmdlet „Invoke-AzureRmVMRunCommand“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-124">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="5a7ce-125">„Get-AzureRmAvailabilitySet“ aktualisiert, um die Auflistung aller Verfügbarkeitsgruppen in einem Abonnement zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-125">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="5a7ce-126">(ResouceGroupName-Parameter ist jetzt optional.)</span><span class="sxs-lookup"><span data-stu-id="5a7ce-126">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="5a7ce-127">„SimpleParameterSet“ von „New-AzureRmVm“ aktualisiert, um Accelerated Networking auf kompatiblen virtuellen Computern zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-127">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="5a7ce-128">Einfacher Parametersatz „New-AzureRmVmss“ aktualisiert, sodass das Erstellen der VMSS fehlschlägt, wenn bereits ein benutzerdefinierter LB vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-128">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="5a7ce-129">Beispiel für „New-AzureRmDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-129">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="5a7ce-130">Beispiel für „New-AzureRmVM“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-130">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="5a7ce-131">Beschreibung für „Set-AzureRmVMOSDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-131">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="5a7ce-132">Beispiel 1 für „Set-AzureRmVMBginfoExtension“ aktualisiert, um Rechtschreibung und Präfix zu korrigieren.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-132">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="5a7ce-133">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="5a7ce-133">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="5a7ce-134">ADF .Net SDK-Version auf 1.1.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-134">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="5a7ce-135">Unterstützung der Freigabe der selbstgehosteten Integration Runtime über Data Factorys hinweg.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-135">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="5a7ce-136">Neuer Parameter „-SharedIntegrationRuntimeResourceId“ zu Cmdlet „Set-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-136">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="5a7ce-137">Neuer optionaler Parameter „-LinkedDataFactoryName“ zu Cmdlet „Remove-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-137">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="5a7ce-138">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5a7ce-138">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="5a7ce-139">DataPlane SDK-Version (Microsoft.Azure.DataLake.Store) auf 1.1.9 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-139">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="5a7ce-140">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="5a7ce-140">AzureRM.EventHub</span></span>
* <span data-ttu-id="5a7ce-141">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-141">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="5a7ce-142">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="5a7ce-142">AzureRM.Insights</span></span>
* <span data-ttu-id="5a7ce-143">Formatierung von „OutputType“ in Hilfedateien korrigiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-143">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="5a7ce-144">Verwendung von Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span><span class="sxs-lookup"><span data-stu-id="5a7ce-144">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="5a7ce-145">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5a7ce-145">AzureRM.KeyVault</span></span>
* <span data-ttu-id="5a7ce-146">Piping-Problem in „Set-AzureRmKeyVaultAccessPolicy“ behoben</span><span class="sxs-lookup"><span data-stu-id="5a7ce-146">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5a7ce-147">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5a7ce-147">AzureRM.Network</span></span>
* <span data-ttu-id="5a7ce-148">Beispiele für LoadBalancerInboundNatPoolConfig-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-148">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5a7ce-149">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5a7ce-149">AzureRM.Resources</span></span>
* <span data-ttu-id="5a7ce-150">Problem beim Angeben sowohl des Tag-Namens als auch des Werts für „Get-AzureRmResource“ behoben</span><span class="sxs-lookup"><span data-stu-id="5a7ce-150">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="5a7ce-151">Piping-Szenario mit „Set-AzureRmResource“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-151">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="5a7ce-152">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5a7ce-152">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="5a7ce-153">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-153">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="5a7ce-154">Einige Probleme behoben</span><span class="sxs-lookup"><span data-stu-id="5a7ce-154">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="5a7ce-155">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5a7ce-155">AzureRM.Sql</span></span>
* <span data-ttu-id="5a7ce-156">Unterstützung für Advanced Threat Protection für Server bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="5a7ce-156">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="5a7ce-157">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="5a7ce-157">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="5a7ce-158">Unterstützung für Sicherheitsrisikobewertung bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="5a7ce-158">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="5a7ce-159">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="5a7ce-159">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="5a7ce-160">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="5a7ce-160">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="5a7ce-161">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="5a7ce-161">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="5a7ce-162">Beispiel in „Remove-AzureRmSqlServerFirewallRule“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-162">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="5a7ce-163">Falsche Verarbeitung von „datetime“ für nicht US-basierte Kultur in „Get-AzureSqlSyncGroupLog“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-163">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="5a7ce-164">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="5a7ce-164">AzureRM.Storage</span></span>
* <span data-ttu-id="5a7ce-165">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-165">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="5a7ce-166">Cmdlet-Ausgabe von „StorageAccount“ in Tabellenansicht anzeigen</span><span class="sxs-lookup"><span data-stu-id="5a7ce-166">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="5a7ce-167">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5a7ce-167">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="5a7ce-168">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5a7ce-168">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="5a7ce-169">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5a7ce-169">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="5a7ce-170">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="5a7ce-170">AzureRM.Tags</span></span>
* <span data-ttu-id="5a7ce-171">Falsche Anweisung aus Tag-Cmdlet-Hilfe entfernt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-171">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="5a7ce-172">6.5.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="5a7ce-172">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="5a7ce-173">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5a7ce-173">AzureRM.Profile</span></span>
* <span data-ttu-id="5a7ce-174">Hilfe für „Get-AzureRmContextAutosaveSetting“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-174">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="5a7ce-175">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="5a7ce-175">Azure.Storage</span></span>
* <span data-ttu-id="5a7ce-176">Unterstützung des Blob- oder Dateiuploads mit lesegeschütztem SAS-Token</span><span class="sxs-lookup"><span data-stu-id="5a7ce-176">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="5a7ce-177">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="5a7ce-177">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="5a7ce-178">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="5a7ce-178">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="5a7ce-179">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="5a7ce-179">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="5a7ce-180">Erforderliche Eigenschaft „ResourceGroupName“ zu AS hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-180">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="5a7ce-181">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="5a7ce-181">AzureRM.Automation</span></span>
* <span data-ttu-id="5a7ce-182">Hilfe aktualisiert und Beispiel für „New-AzureRMAutomationSchedule“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-182">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5a7ce-183">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5a7ce-183">AzureRM.Compute</span></span>
* <span data-ttu-id="5a7ce-184">Parameter „-Tag“ zu „Update/New-AzureRmAvailabilitySet“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-184">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="5a7ce-185">Beispiel für „Add-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-185">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="5a7ce-186">Beispiele für „Remove-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-186">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="5a7ce-187">Hilfe für „Set-AzureRmVMAccessExtension“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-187">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="5a7ce-188">„SimpleParameterSet“ für „New-AzureRmVmss“ so aktualisiert, dass „SinglePlacementGroup“ standardmäßig auf „false“ festgelegt ist, und Switch-Parameter „SinglePlacementGroup“ hinzugefügt, der dem Benutzer das Erstellen der VMSS in einer einzelnen Platzierungsgruppe ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-188">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="5a7ce-189">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="5a7ce-189">AzureRM.EventHub</span></span>
* <span data-ttu-id="5a7ce-190">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSEventHubDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-190">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="5a7ce-191">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5a7ce-191">AzureRM.KeyVault</span></span>
* <span data-ttu-id="5a7ce-192">Fehlermeldung für „Set-AzureRmKeyVaultAccessPolicy“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-192">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="5a7ce-193">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="5a7ce-193">AzureRM.LogicApp</span></span>
* <span data-ttu-id="5a7ce-194">Fehler „Parametersatz konnte nicht aufgelöst werden“ in „New-AzureRmLogicApp“behoben</span><span class="sxs-lookup"><span data-stu-id="5a7ce-194">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5a7ce-195">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5a7ce-195">AzureRM.Network</span></span>
* <span data-ttu-id="5a7ce-196">Peering über mehrere virtuelle Netzwerke in mehreren Mandanten für „Set/Add-AzureRmVirtualNetworkPeering“ aktiviert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-196">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="5a7ce-197">Folgende Cmdlets für Application Gateway aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-197">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="5a7ce-198">New-AzureRmApplicationGateway: EnableFIPS-Flag und Zonenunterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-198">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="5a7ce-199">New-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-199">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="5a7ce-200">Set-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-200">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="5a7ce-201">RouteTable-Cmdlets mit aktueller Generatorversion erneut generiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-201">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="5a7ce-202">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="5a7ce-202">AzureRM.Relay</span></span>
* <span data-ttu-id="5a7ce-203">Markdowndateien aktualisiert, Problem mit Parametername in Beispiel behoben</span><span class="sxs-lookup"><span data-stu-id="5a7ce-203">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5a7ce-204">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5a7ce-204">AzureRM.Resources</span></span>
* <span data-ttu-id="5a7ce-205">Roleassignment- und roledefinition-Cmdlets aktualisiert:</span><span class="sxs-lookup"><span data-stu-id="5a7ce-205">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="5a7ce-206">Zusätzliche roledefinition-Aufrufe entfernt, die als Teil des Pagings durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-206">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="5a7ce-207">Get-AzureRmRoleAssignment-Cmdlet korrigiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-207">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="5a7ce-208">Befehlsparameterfunktion von „-ExpandPrincipalGroups“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-208">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="5a7ce-209">Problem mit „Get-AzureRmResource“ behoben, aufgrund dessen die Groß-/Kleinschreibung des Parameters „-ResourceType“ beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="5a7ce-209">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="5a7ce-210">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5a7ce-210">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="5a7ce-211">top- und skip-Parameter zu Listen-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-211">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="5a7ce-212">Cmdlets für die Migration von Standard- zu Premium-Namespace hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="5a7ce-212">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="5a7ce-213">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="5a7ce-213">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="5a7ce-214">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="5a7ce-214">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="5a7ce-215">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="5a7ce-215">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="5a7ce-216">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="5a7ce-216">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="5a7ce-217">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="5a7ce-217">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="5a7ce-218">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSServiceBusDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-218">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="5a7ce-219">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5a7ce-219">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="5a7ce-220">Beispiel für „New-AzureRmServiceFabricCluster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-220">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="5a7ce-221">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5a7ce-221">AzureRM.Sql</span></span>
* <span data-ttu-id="5a7ce-222">Neue Cmdlets für „Management.Sql“ hinzugefügt, um Kunden das Hinzufügen des TDE-Zertifikats zu einer SQL Server-Instanz oder einer verwalteten Instanz zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5a7ce-222">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="5a7ce-223">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="5a7ce-223">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="5a7ce-224">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="5a7ce-224">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="5a7ce-225">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="5a7ce-225">AzureRM.Websites</span></span>
* <span data-ttu-id="5a7ce-226">Wenn `Set-AzureRmWebApp -AssignIdentity` und `Set-AzureRmWebAppSlot -AssignIdentity` auf „false“ festgelegt sind, wird jetzt die Identity-Eigenschaft aus dem Websiteobjekt entfernt. Auch das Vorschau-Tag wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-226">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="5a7ce-227">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics`-Beispiel aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-227">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="5a7ce-228">Unterstützung von `Set-AzureRmWebApp -PhpVersion` als gültige PHP-Version eingestellt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-228">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="5a7ce-229">6.4.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="5a7ce-229">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="5a7ce-230">Allgemein</span><span class="sxs-lookup"><span data-stu-id="5a7ce-230">General</span></span>
* <span data-ttu-id="5a7ce-231">Formatierung von OutputType in Hilfedateien für die meisten Module korrigiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-231">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="5a7ce-232">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5a7ce-232">AzureRM.Profile</span></span>
* <span data-ttu-id="5a7ce-233">Attribut „Ps1Xml“ wurde den Standardausgabetypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-233">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5a7ce-234">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5a7ce-234">AzureRM.Compute</span></span>
* <span data-ttu-id="5a7ce-235">IP-Tag-Funktion für VMSS</span><span class="sxs-lookup"><span data-stu-id="5a7ce-235">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="5a7ce-236">Cmdlet „New-AzureRmVmssIpTagConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-236">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="5a7ce-237">IpTag-Parameter zu „New-AzureRmVmssIpConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-237">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="5a7ce-238">Funktion für automatisches Betriebssystemrollback für VMSS</span><span class="sxs-lookup"><span data-stu-id="5a7ce-238">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="5a7ce-239">DisableAutoRollback-Parameter zu „New-AzureRmVmssConfig“ und „Update-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-239">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="5a7ce-240">Funktion für Upgradeverlauf des Betriebssystems für VMSS</span><span class="sxs-lookup"><span data-stu-id="5a7ce-240">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="5a7ce-241">Switch-Parameter „OSUpgradeHistory“ zu „Get-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-241">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="5a7ce-242">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="5a7ce-242">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="5a7ce-243">Unterstützung für Katalog-ACLs über die folgenden Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="5a7ce-243">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="5a7ce-244">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="5a7ce-244">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="5a7ce-245">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="5a7ce-245">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="5a7ce-246">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="5a7ce-246">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="5a7ce-247">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5a7ce-247">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="5a7ce-248">Abbruchunterstützung und Nachverfolgung des Fortschritts für „Set-AzureRmDataLakeStoreItemAclEntry“, „Remove-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-248">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="5a7ce-249">Abbruchunterstützung „Export-AzureRmDataLakeStoreChildItemProperties“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-249">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="5a7ce-250">Leerung von Debugmeldungen für Cmdlets korrigiert, die rekursive Vorgänge durchführt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-250">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="5a7ce-251">Speicherort des Test von DataLake-Cmdlets korrigiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-251">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="5a7ce-252">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="5a7ce-252">AzureRM.EventHub</span></span>
* <span data-ttu-id="5a7ce-253">Optionaler Parameter „MaxCount“ zu Listenvorgangs-Cmdlets „Get-AzureRmEventHub“ und „Get-AzureRmEventHubConsumerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-253">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="5a7ce-254">Problem in Cmdlet „New-AzureRmEventHub“ behoben, aufgrund dessen beim Erstellen einer neuen EventHub-Instanz mindestens ein Parameter benötigt wurde.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-254">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="5a7ce-255">Standardparametersatz wurde bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-255">Provided Default Parameter set.</span></span>
* <span data-ttu-id="5a7ce-256">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmEventHubKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-256">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="5a7ce-257">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5a7ce-257">AzureRM.KeyVault</span></span>
* <span data-ttu-id="5a7ce-258">Problem behoben, aufgrund dessen von „Get-AzureRmKeyVault -Tag“ alle Ressourcen zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-258">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5a7ce-259">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5a7ce-259">AzureRM.Network</span></span>
* <span data-ttu-id="5a7ce-260">Neue SKUs für zonenredundante VirtualNetworkGateways-Instanzen verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="5a7ce-260">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="5a7ce-261">Neue Befehle für Funktion hinzugefügt: ExpressRoute-Partner-APIs über ARM</span><span class="sxs-lookup"><span data-stu-id="5a7ce-261">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="5a7ce-262">Get-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-262">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="5a7ce-263">Set-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-263">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="5a7ce-264">Add-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-264">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="5a7ce-265">Get-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-265">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="5a7ce-266">Remove-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-266">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="5a7ce-267">Get-AzureRMExpressRouteCrossConnectionArpTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-267">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="5a7ce-268">Get-AzureRMExpressRouteCrossConnectionRouteTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-268">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="5a7ce-269">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-269">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="5a7ce-270">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="5a7ce-270">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="5a7ce-271">Cmdlet „Get-AzureRmRecoveryServicesBackupStatus“ wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-271">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="5a7ce-272">Dieses Cmdlet überprüft anhand der ID eines virtuellen Computers, ob dieser durch einen Tresor im Abonnement geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-272">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="5a7ce-273">Wenn ein solcher Tresor vorhanden ist, gibt das Cmdlet die Tresordetails aus.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-273">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5a7ce-274">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5a7ce-274">AzureRM.Resources</span></span>
* <span data-ttu-id="5a7ce-275">Cmdlets vom Typ „Get-AzureRmPolicyAssignment“ aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="5a7ce-275">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="5a7ce-276">Unterstützung für das Auflisten von „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-276">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="5a7ce-277">Unterstützung für das Abrufen einzelner Arbeitsaufträge mit „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-277">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="5a7ce-278">Switches „-Effective“ und „-All“ zu Steuerparameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-278">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="5a7ce-279">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicyDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-279">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="5a7ce-280">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="5a7ce-280">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="5a7ce-281">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="5a7ce-281">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="5a7ce-282">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicySetDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-282">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="5a7ce-283">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="5a7ce-283">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="5a7ce-284">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="5a7ce-284">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="5a7ce-285">Unterstützung für KeyVault-Geheimnisverweis in Parametern hinzugefügt, wenn „TemplateParameterObject“ in „New-AzureRmResourceGroupDeployment“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5a7ce-285">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="5a7ce-286">Problem behoben, aufgrund dessen, der Parameter „-EndDate“ für „New-AzureRmADAppCredential“ ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="5a7ce-286">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="5a7ce-287">Problem behoben, aufgrund dessen „Add-AzureRmADGroupMember“ eine falsche URL für Anforderungen verwendete</span><span class="sxs-lookup"><span data-stu-id="5a7ce-287">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="5a7ce-288">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5a7ce-288">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="5a7ce-289">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmServiceBusKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-289">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="5a7ce-290">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5a7ce-290">AzureRM.Sql</span></span>
* <span data-ttu-id="5a7ce-291">Benutzerdefinierte Wiederherstellungspunkte für SQLDW in Hilfe zu „New-AzureRmSqlDatabaseRestorePoint“ erläutert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-291">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="5a7ce-292">Dokumentation von Parameter „-ComputeGeneration“ in mehreren Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-292">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="5a7ce-293">6.3.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="5a7ce-293">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="5a7ce-294">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5a7ce-294">AzureRM.Profile</span></span>
* <span data-ttu-id="5a7ce-295">Aktualisierte Fehlermeldungen für „Enable-AzureRmContextAutoSave“</span><span class="sxs-lookup"><span data-stu-id="5a7ce-295">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="5a7ce-296">Erstellen eines Kontexts für jedes Abonnement beim Ausführen von „Connect-AzureRmAccount“ ohne vorherigen Kontext</span><span class="sxs-lookup"><span data-stu-id="5a7ce-296">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="5a7ce-297">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="5a7ce-297">Azure.Storage</span></span>
* <span data-ttu-id="5a7ce-298">Zusätzliche Informationen zum Parameter „-Permissions“ in Hilfedateien</span><span class="sxs-lookup"><span data-stu-id="5a7ce-298">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5a7ce-299">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5a7ce-299">AzureRM.Compute</span></span>
* <span data-ttu-id="5a7ce-300">„Get-AzureRmVmDiskEncryptionStatus“ behebt ein Problem, das bei virtuellen Computern ohne Datenträger festgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-300">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="5a7ce-301">Version der Computeclientbibliothek aktualisiert, um folgende Cmdlets zu korrigieren:</span><span class="sxs-lookup"><span data-stu-id="5a7ce-301">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="5a7ce-302">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="5a7ce-302">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="5a7ce-303">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="5a7ce-303">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="5a7ce-304">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="5a7ce-304">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="5a7ce-305">Die folgenden Cmdlets wurden korrigiert, um die Vorgangs-ID und den Vorgangsstatus korrekt anzuzeigen:</span><span class="sxs-lookup"><span data-stu-id="5a7ce-305">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="5a7ce-306">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="5a7ce-306">Start-AzureRmVM</span></span>
    - <span data-ttu-id="5a7ce-307">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="5a7ce-307">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="5a7ce-308">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="5a7ce-308">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="5a7ce-309">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="5a7ce-309">Set-AzureRmVM</span></span>
    - <span data-ttu-id="5a7ce-310">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="5a7ce-310">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="5a7ce-311">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5a7ce-311">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="5a7ce-312">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="5a7ce-312">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="5a7ce-313">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="5a7ce-313">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="5a7ce-314">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5a7ce-314">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="5a7ce-315">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5a7ce-315">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="5a7ce-316">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5a7ce-316">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="5a7ce-317">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5a7ce-317">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="5a7ce-318">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="5a7ce-318">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="5a7ce-319">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="5a7ce-319">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="5a7ce-320">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="5a7ce-320">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="5a7ce-321">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="5a7ce-321">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="5a7ce-322">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="5a7ce-322">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="5a7ce-323">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="5a7ce-323">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="5a7ce-324">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="5a7ce-324">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="5a7ce-325">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="5a7ce-325">AzureRM.EventGrid</span></span>
* <span data-ttu-id="5a7ce-326">ValidateNotNullOrEmpty-Überprüfungskonditionen für „SubjectBeginsWith“/„SubjectEndsWith“ im Cmdlet „Update-AzureRmEventGridSubscription“ wurden entfernt, um bei Bedarf die Änderung dieser Parameter in eine leere Zeichenfolge zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-326">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="5a7ce-327">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5a7ce-327">AzureRM.KeyVault</span></span>
* <span data-ttu-id="5a7ce-328">Ein Problem wurde behoben, aufgrund dessen bei Ausführung von „Get-AzureRmKeyVault -Tag“ keine Tags zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-328">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="5a7ce-329">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="5a7ce-329">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="5a7ce-330">Offizielle Veröffentlichung von Policy Insights-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="5a7ce-330">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="5a7ce-331">Verwendung der API-Version 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="5a7ce-331">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="5a7ce-332">„PolicyDefinitionReferenceId“ zu den Ergebnissen von „Get-AzureRmPolicyStateSummary“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-332">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="5a7ce-333">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="5a7ce-333">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="5a7ce-334">Parameter „-Vault“ zu den RecoveryServices.Backup-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-334">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="5a7ce-335">Bei der Übergabe wird dadurch das Cmdlet „Set-AzureRmRecoveryServicesContext“ außer Kraft gesetzt.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-335">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="5a7ce-336">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5a7ce-336">AzureRM.Sql</span></span>
* <span data-ttu-id="5a7ce-337">Aktualisiertes Beispiel in der Hilfedatei für „Get-AzureRmSqlDatabaseExpanded“</span><span class="sxs-lookup"><span data-stu-id="5a7ce-337">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="5a7ce-338">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="5a7ce-338">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="5a7ce-339">Hilfedatei für „Add-AzureRmTrafficManagerEndpointConfig“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5a7ce-339">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="5a7ce-340">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="5a7ce-340">AzureRM.Websites</span></span>
* <span data-ttu-id="5a7ce-341">„Set-AzureRmWebApp“ wurde aktualisiert, damit „AppSettings“ bei der Verwendung von „-AssignIdentity“ nicht außer Kraft gesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-341">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="5a7ce-342">„New-AzureRmWebAppSlot“ wurde aktualisiert, um „AppServicePlan“ als optionalen Parameter anzuerkennen</span><span class="sxs-lookup"><span data-stu-id="5a7ce-342">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="5a7ce-343">6.2.1: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="5a7ce-343">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="5a7ce-344">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="5a7ce-344">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="5a7ce-345">PSWorkspace-Modell aktualisiert, damit das Netzwerk „type“ als Parameter verwenden kann</span><span class="sxs-lookup"><span data-stu-id="5a7ce-345">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="5a7ce-346">6.2.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="5a7ce-346">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="5a7ce-347">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5a7ce-347">AzureRM.Profile</span></span>
* <span data-ttu-id="5a7ce-348">Beheben des Problems, aufgrund dessen Version 10.0.3 von Newtonsoft.Json beim Modulimport nicht geladen wurde</span><span class="sxs-lookup"><span data-stu-id="5a7ce-348">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5a7ce-349">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5a7ce-349">AzureRM.Compute</span></span>
* <span data-ttu-id="5a7ce-350">Feature zum Aktualisieren von virtuellen VMSS-Computern</span><span class="sxs-lookup"><span data-stu-id="5a7ce-350">VMSS VM Update feature</span></span>
    - <span data-ttu-id="5a7ce-351">Cmdlets „Update-AzureRmVmssVM“ und „New-AzureRmVMDataDisk“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-351">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="5a7ce-352">Fügen Sie den Parameter „VirtualMachineScaleSetVM“ zum Cmdlet „Add-AzureRmVMDataDisk“ hinzu, um das Hinzufügen eines Datenträgers zum virtuellen VMSS-Computer zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-352">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="5a7ce-353">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="5a7ce-353">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="5a7ce-354">Aktualisierung der ADF .Net SDK-Version auf 0.8.0-preview mit den folgenden Änderungen:</span><span class="sxs-lookup"><span data-stu-id="5a7ce-354">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="5a7ce-355">Vorgang zum Konfigurieren des Factoryrepositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-355">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="5a7ce-356">Der verknüpfte QuickBooks-Dienst wurde aktualisiert, um die Eigenschaften „consumerKey“ und „consumerSecret“ verfügbar zu machen.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-356">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="5a7ce-357">Aktualisierung verschiedener Modelltypen von „SecretBase“ auf „Object“</span><span class="sxs-lookup"><span data-stu-id="5a7ce-357">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="5a7ce-358">Blobereignisauslöser hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-358">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="5a7ce-359">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5a7ce-359">AzureRM.KeyVault</span></span>
* <span data-ttu-id="5a7ce-360">Aktualisierung der Dokumentation mit Beispielausgabe</span><span class="sxs-lookup"><span data-stu-id="5a7ce-360">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="5a7ce-361">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5a7ce-361">AzureRM.Network</span></span>
* <span data-ttu-id="5a7ce-362">Aktivierung der Traffic Analytics-Parameter für Network Watcher-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="5a7ce-362">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5a7ce-363">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5a7ce-363">AzureRM.Resources</span></span>
* <span data-ttu-id="5a7ce-364">Behebung des Problems mit der Eigenschaft „Properties“ von PSResource-Objekten, die von „Get-AzureRmResource“ zurückgegeben wurden</span><span class="sxs-lookup"><span data-stu-id="5a7ce-364">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="5a7ce-365">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="5a7ce-365">AzureRM.Scheduler</span></span>
* <span data-ttu-id="5a7ce-366">Behebung des Problems, dass beim Aktualisieren von „ServiceBusQueueJob“ keine neuen Authentifizierungswerte festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="5a7ce-366">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="5a7ce-367">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5a7ce-367">AzureRM.Sql</span></span>
* <span data-ttu-id="5a7ce-368">Aktualisierung der folgenden Cmdlets mit dem optionalen LicenseType-Parameter</span><span class="sxs-lookup"><span data-stu-id="5a7ce-368">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="5a7ce-369">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="5a7ce-369">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="5a7ce-370">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="5a7ce-370">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="5a7ce-371">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="5a7ce-371">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="5a7ce-372">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="5a7ce-372">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="5a7ce-373">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="5a7ce-373">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="5a7ce-374">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="5a7ce-374">AzureRM.Websites</span></span>
* <span data-ttu-id="5a7ce-375">„New-AzureRMWebApp“ aktualisiert, um allgemeine Algorithmen aus der Strategiebibliothek zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-375">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="5a7ce-376">6.1.0 – Mai 2018</span><span class="sxs-lookup"><span data-stu-id="5a7ce-376">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="5a7ce-377">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5a7ce-377">AzureRM.Profile</span></span>
* <span data-ttu-id="5a7ce-378">Behebung eines Problems, durch das beim Ausführen von „Clear-AzureRmContext“ ein leerer Kontext mit dem Namen des vorherigen Standardkontexts beibehalten wurde und der Benutzer dadurch keinen neuen Kontext mit dem alten Namen erstellen konnte</span><span class="sxs-lookup"><span data-stu-id="5a7ce-378">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="5a7ce-379">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="5a7ce-379">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="5a7ce-380">Ermöglichung der Zuordnung von Gateways/Aufhebung der Gatewayzuordnung in AS</span><span class="sxs-lookup"><span data-stu-id="5a7ce-380">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="5a7ce-381">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5a7ce-381">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="5a7ce-382">Unterstützung für „ApiVersions“, „ApiReleases“ und „ApiRevisions“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-382">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="5a7ce-383">Unterstützung für ServiceFabric-Back-End hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-383">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="5a7ce-384">Unterstützung für Application Insights-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-384">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="5a7ce-385">Unterstützung für die Erkennung von SKUs vom Typ „Basic“ als gültige SKU des API Management-Diensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-385">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="5a7ce-386">Unterstützung hinzugefügt, damit Zertifikate, die von der privaten Zertifizierungsstelle ausgestellt wurden, als Stamm- oder ZS-Zertifikate installiert werden können</span><span class="sxs-lookup"><span data-stu-id="5a7ce-386">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="5a7ce-387">Unterstützung für die Akzeptierung benutzerdefinierter SSL-Zertifikate über KeyVault und mehrere Proxyhostnamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-387">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="5a7ce-388">Unterstützung für die verwaltete Dienstidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-388">Added support for MSI identity</span></span>
* <span data-ttu-id="5a7ce-389">Unterstützung für die Annahme von Richtlinien über URL hinzugefügt; HINWEIS: Folgende Cmdlets werden in einem zukünftigen Release als veraltet gekennzeichnet:</span><span class="sxs-lookup"><span data-stu-id="5a7ce-389">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="5a7ce-390">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="5a7ce-390">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="5a7ce-391">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="5a7ce-391">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="5a7ce-392">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="5a7ce-392">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="5a7ce-393">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="5a7ce-393">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="5a7ce-394">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="5a7ce-394">AzureRM.Batch</span></span>
* <span data-ttu-id="5a7ce-395">Veröffentlichung des neuen Cmdlets „Get-AzureBatchPoolNodeCounts“</span><span class="sxs-lookup"><span data-stu-id="5a7ce-395">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="5a7ce-396">Veröffentlichung des neuen Cmdlets „Start-AzureBatchComputeNodeServiceLogUpload“</span><span class="sxs-lookup"><span data-stu-id="5a7ce-396">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="5a7ce-397">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="5a7ce-397">AzureRM.Consumption</span></span>
* <span data-ttu-id="5a7ce-398">Hinzufügung neuer Parameter („Expand“, „ResourceGroup“, „InstanceName“, „InstanceId“, „Tags“ und „Top“) für das Cmdlet „Get-AzureRmConsumptionUsageDetail“</span><span class="sxs-lookup"><span data-stu-id="5a7ce-398">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="5a7ce-399">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5a7ce-399">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="5a7ce-400">Korrektur des Beispiels für „Export AzureRmDataLakeStoreChildItemProperties“</span><span class="sxs-lookup"><span data-stu-id="5a7ce-400">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="5a7ce-401">Korrektur der NULL-Parameterausnahme für rekursiven Fall in „Set-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="5a7ce-401">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="5a7ce-402">Korrektur der Hilfedateien für „Set-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ und „Remove-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="5a7ce-402">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="5a7ce-403">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5a7ce-403">AzureRM.Network</span></span>
* <span data-ttu-id="5a7ce-404">Erhöhung der Network SDK-Version von 18.0.0-preview auf 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="5a7ce-404">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="5a7ce-405">Cmdlet zum Erstellen der Protokollkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-405">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="5a7ce-406">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="5a7ce-406">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="5a7ce-407">Cmdlet zum Hinzufügen einer neuen Leitungsverbindung zu einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-407">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="5a7ce-408">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="5a7ce-408">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="5a7ce-409">Cmdlet zum Entfernen einer Leitungsverbindung aus einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-409">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="5a7ce-410">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="5a7ce-410">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="5a7ce-411">Cmdlet zum Abrufen einer Leitungsverbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5a7ce-411">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="5a7ce-412">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="5a7ce-412">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="5a7ce-413">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5a7ce-413">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="5a7ce-414">Verwendung der Serverauthentifizierung mit generierten Zertifikaten korrigiert (Problemnr. 5998)</span><span class="sxs-lookup"><span data-stu-id="5a7ce-414">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="5a7ce-415">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5a7ce-415">AzureRM.Sql</span></span>
* <span data-ttu-id="5a7ce-416">Überwachungscmdlets korrigiert, um das Entfernen von „AuditActions“ oder „AuditActionGroups“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5a7ce-416">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="5a7ce-417">Problem mit „Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy“ behoben, das beim Festlegen einer neuen flexiblen Aufbewahrungsrichtlinie zu folgendem Fehler führte: „Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-417">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="5a7ce-418">Please submit request with the new flexible retention policy“ (Das Konfigurieren einer langfristigen Aufbewahrungsrichtlinie mit Azure Recovery Service-Tresor und -Richtlinie wird nicht mehr unterstützt. Übermitteln Sie eine Anforderung mit der neuen flexiblen Aufbewahrungsrichtlinie.)</span><span class="sxs-lookup"><span data-stu-id="5a7ce-418">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="5a7ce-419">Aktualisierung aller Cmdlets für Azure SQL-Datenbank, für die Erstellung von Pools für elastische Datenbanken und für die Aktualisierung, sodass sie die neue Datenbank-API verwenden. Diese unterstützt die Sku-Eigenschaft für skalierungs- und tarifbezogene Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="5a7ce-419">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="5a7ce-420">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="5a7ce-420">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="5a7ce-421">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="5a7ce-421">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="5a7ce-422">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="5a7ce-422">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="5a7ce-423">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="5a7ce-423">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="5a7ce-424">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="5a7ce-424">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="5a7ce-425">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="5a7ce-425">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="5a7ce-426">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="5a7ce-426">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="5a7ce-427">Aktualisierung der Parameter für „Get-AzureRmTrafficManagerProfile“, sodass bei Verwendung des Parameters „-Name“ der Parameter „-ResourceGroupName“ erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="5a7ce-427">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>