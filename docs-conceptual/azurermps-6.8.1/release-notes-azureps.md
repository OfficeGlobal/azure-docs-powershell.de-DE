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
ms.openlocfilehash: 6043d17df1b5e91521bad31e65372c10ee6a5c6a
ms.sourcegitcommit: dca906e73e943aac207cee23b79915773419c673
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/30/2018
ms.locfileid: "43250319"
---
# <a name="release-notes"></a><span data-ttu-id="dbceb-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="dbceb-103">Release notes</span></span>

<span data-ttu-id="dbceb-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="dbceb-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="680---august-2018"></a><span data-ttu-id="dbceb-105">6.8.0: August 2018</span><span class="sxs-lookup"><span data-stu-id="dbceb-105">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="dbceb-106">Allgemein</span><span class="sxs-lookup"><span data-stu-id="dbceb-106">General</span></span>
* <span data-ttu-id="dbceb-107">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="dbceb-107">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="dbceb-108">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="dbceb-108">AzureRM.Profile</span></span>
* <span data-ttu-id="dbceb-109">Ablaufeigenschaft zu Token hinzugefügt, die während „Connect-AzureRmAccount“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="dbceb-109">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="dbceb-110">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="dbceb-110">AzureRM.Compute</span></span>
* <span data-ttu-id="dbceb-111">Problem des fehlenden Ziels in der Fehlerausgabe behoben</span><span class="sxs-lookup"><span data-stu-id="dbceb-111">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="dbceb-112">Problem mit dem Speicherkontotyp für den virtuellen Computer mit verwaltetem Datenträgern behoben</span><span class="sxs-lookup"><span data-stu-id="dbceb-112">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="dbceb-113">AEM-Erweiterungs-Cmdlets für andere Umgebungen (etwa Azure China) korrigiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-113">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="dbceb-114">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="dbceb-114">AzureRM.IotHub</span></span>
* <span data-ttu-id="dbceb-115">Beispiele für „New-AzureRmIotHubExportDevices“ und „New-AzureRmIotHubImportDevices“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-115">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="dbceb-116">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="dbceb-116">AzureRM.Network</span></span>
* <span data-ttu-id="dbceb-117">Standarddarstellung von Modellen in Tabellenansicht geändert</span><span class="sxs-lookup"><span data-stu-id="dbceb-117">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="dbceb-118">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="dbceb-118">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="dbceb-119">Fehler in „Update-AzureRmPowerBIEmbeddedCapacity“ beim Skalieren der angehaltenen Kapazität behoben</span><span class="sxs-lookup"><span data-stu-id="dbceb-119">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="dbceb-120">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="dbceb-120">AzureRM.Resources</span></span>
* <span data-ttu-id="dbceb-121">Problem beim Erstellen der verwalteten Anwendung über Marketplace behoben</span><span class="sxs-lookup"><span data-stu-id="dbceb-121">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="dbceb-122">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="dbceb-122">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="dbceb-123">Fehlerbehebung</span><span class="sxs-lookup"><span data-stu-id="dbceb-123">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="dbceb-124">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="dbceb-124">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="dbceb-125">Unterstützung für Routingmethode „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="dbceb-125">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="dbceb-126">Neuer Parameter „MaxReturn“ für Routingtyp „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="dbceb-126">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="dbceb-127">Unterstützung für Subnetzroutingmethode</span><span class="sxs-lookup"><span data-stu-id="dbceb-127">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="dbceb-128">Unterstützung für IP-Adressbereiche (Subnetze) in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="dbceb-128">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="dbceb-129">Unterstützung für benutzerdefinierte Header in Profilen</span><span class="sxs-lookup"><span data-stu-id="dbceb-129">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="dbceb-130">Unterstützung für erwartete Statuscodebereiche in Profilen</span><span class="sxs-lookup"><span data-stu-id="dbceb-130">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="dbceb-131">Unterstützung für benutzerdefinierte Header in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="dbceb-131">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="dbceb-132">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="dbceb-132">AzureRM.Websites</span></span>
* <span data-ttu-id="dbceb-133">Das Problem, dass die Standardressourcengruppe falsch festgelegt wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="dbceb-133">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="dbceb-134">6.7.0: August 2018</span><span class="sxs-lookup"><span data-stu-id="dbceb-134">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="dbceb-135">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="dbceb-135">AzureRM.Profile</span></span>
* <span data-ttu-id="dbceb-136">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-136">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="dbceb-137">Benutzer-ID zum Standardkontextnamen hinzugefügt, um Kontextkonflikte zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="dbceb-137">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="dbceb-138">Probleme mit „Clear-AzureRmContext“ behoben, die Fehler beim Auswählen eines Kontexts verursacht haben (6398)</span><span class="sxs-lookup"><span data-stu-id="dbceb-138">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="dbceb-139">Ermöglicht, dass für „Connect-AzureRmAccount“ die Mandantendomäne an den Parameter „-TenantId“ übergeben wird</span><span class="sxs-lookup"><span data-stu-id="dbceb-139">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="dbceb-140">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="dbceb-140">Azure.Storage</span></span>
* <span data-ttu-id="dbceb-141">Begrenzung von 5 TB für das Kontingent der Azure-Dateifreigabe entfernt</span><span class="sxs-lookup"><span data-stu-id="dbceb-141">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="dbceb-142">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="dbceb-142">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="dbceb-143">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="dbceb-143">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="dbceb-144">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-144">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="dbceb-145">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="dbceb-145">Azure.AnalysisServices</span></span>
* <span data-ttu-id="dbceb-146">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-146">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="dbceb-147">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="dbceb-147">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="dbceb-148">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-148">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="dbceb-149">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="dbceb-149">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="dbceb-150">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-150">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="dbceb-151">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="dbceb-151">AzureRM.Automation</span></span>
* <span data-ttu-id="dbceb-152">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-152">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="dbceb-153">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="dbceb-153">AzureRM.Backup</span></span>
* <span data-ttu-id="dbceb-154">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-154">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="dbceb-155">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="dbceb-155">AzureRM.Batch</span></span>
* <span data-ttu-id="dbceb-156">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-156">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="dbceb-157">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="dbceb-157">AzureRM.Billing</span></span>
* <span data-ttu-id="dbceb-158">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-158">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="dbceb-159">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="dbceb-159">AzureRM.Cdn</span></span>
* <span data-ttu-id="dbceb-160">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-160">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="dbceb-161">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="dbceb-161">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="dbceb-162">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-162">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="dbceb-163">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="dbceb-163">AzureRM.Compute</span></span>
* <span data-ttu-id="dbceb-164">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-164">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="dbceb-165">EvictionPolicy-Parameter zu „New-AzureRmVmssConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-165">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="dbceb-166">Standort in „DiskFileParameterSet“ von „New-AzureRmVm“ angeben, wenn kein Ort angegeben ist</span><span class="sxs-lookup"><span data-stu-id="dbceb-166">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="dbceb-167">Parameterbeschreibung in „Save-AzureRmVMImage“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-167">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="dbceb-168">Cmdlet „Get-AzureRmVMDiskEncryptionStatus“ für bestimmte Szenarien im Zusammenhang mit einem Durchlauf korrigiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-168">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="dbceb-169">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="dbceb-169">AzureRM.Consumption</span></span>
* <span data-ttu-id="dbceb-170">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-170">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="dbceb-171">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="dbceb-171">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="dbceb-172">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-172">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="dbceb-173">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="dbceb-173">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="dbceb-174">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-174">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="dbceb-175">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="dbceb-175">AzureRM.DataFactories</span></span>
* <span data-ttu-id="dbceb-176">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-176">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="dbceb-177">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="dbceb-177">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="dbceb-178">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-178">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="dbceb-179">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="dbceb-179">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="dbceb-180">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-180">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="dbceb-181">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="dbceb-181">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="dbceb-182">Debuggen korrigiert, wenn „DebugPreference“ über die PowerShell-Befehlszeile festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="dbceb-182">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="dbceb-183">Beispiel für „Set-AzureRmDataLakeStoreItemAcl“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-183">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="dbceb-184">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="dbceb-184">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="dbceb-185">Beispiel für „Set-AzureRmDataLakeStoreItemAclEntry“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-185">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="dbceb-186">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="dbceb-186">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="dbceb-187">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-187">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="dbceb-188">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="dbceb-188">AzureRM.Dns</span></span>
* <span data-ttu-id="dbceb-189">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-189">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="dbceb-190">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="dbceb-190">AzureRM.EventGrid</span></span>
* <span data-ttu-id="dbceb-191">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-191">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="dbceb-192">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="dbceb-192">AzureRM.EventHub</span></span>
* <span data-ttu-id="dbceb-193">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-193">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="dbceb-194">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="dbceb-194">AzureRM.HDInsight</span></span>
* <span data-ttu-id="dbceb-195">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-195">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="dbceb-196">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="dbceb-196">AzureRM.Insights</span></span>
* <span data-ttu-id="dbceb-197">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-197">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="dbceb-198">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="dbceb-198">AzureRM.IotHub</span></span>
* <span data-ttu-id="dbceb-199">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-199">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="dbceb-200">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="dbceb-200">AzureRM.KeyVault</span></span>
* <span data-ttu-id="dbceb-201">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-201">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="dbceb-202">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="dbceb-202">AzureRM.LogicApp</span></span>
* <span data-ttu-id="dbceb-203">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-203">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="dbceb-204">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="dbceb-204">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="dbceb-205">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-205">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="dbceb-206">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="dbceb-206">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="dbceb-207">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-207">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="dbceb-208">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="dbceb-208">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="dbceb-209">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-209">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="dbceb-210">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="dbceb-210">AzureRM.Media</span></span>
* <span data-ttu-id="dbceb-211">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-211">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="dbceb-212">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="dbceb-212">AzureRM.Network</span></span>
* <span data-ttu-id="dbceb-213">Beispiel für „Set-AzureRmLocalNetworkGateway“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-213">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="dbceb-214">Beispiele und Beschreibungen für „Add-AzureRmVirtualNetworkGatewayIpConfig“, „Get-AzureRmVirtualNetworkGatewayConnectionSharedKey“ und „New-AzureRmVirtualNetworkGatewayConnection“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-214">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="dbceb-215">Beispiele für „Remove-AzureRmVirtualNetworkGatewayIpConfig“ und „Reset-AzureRmVirtualNetworkGateway“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-215">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="dbceb-216">Beispiel für „Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-216">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="dbceb-217">Beispiel für „Set-AzureRmVirtualNetworkGatewayConnectionSharedKey“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-217">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="dbceb-218">Beispiel für „Set-AzureRmVirtualNetworkGatewayConnection“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-218">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="dbceb-219">Cmdlets für „ApplicationSecurityGroup“, „RouteTable“ und „Usage“ mithilfe des aktuellen Code-Generators erneut erstellt</span><span class="sxs-lookup"><span data-stu-id="dbceb-219">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="dbceb-220">Deutlichere Formulierung der Fehlermeldung für „Get-AzureRmVirtualNetworkSubnetConfig“, wenn ein nicht vorhandenes Subnetz abgerufen wird</span><span class="sxs-lookup"><span data-stu-id="dbceb-220">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="dbceb-221">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="dbceb-221">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="dbceb-222">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-222">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="dbceb-223">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="dbceb-223">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="dbceb-224">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-224">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="dbceb-225">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="dbceb-225">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="dbceb-226">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-226">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="dbceb-227">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="dbceb-227">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="dbceb-228">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-228">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="dbceb-229">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="dbceb-229">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="dbceb-230">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-230">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="dbceb-231">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="dbceb-231">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="dbceb-232">Richtlinienfilter zum Cmdlet „Get-AzureRmRecoveryServicesBackItem“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="dbceb-232">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="dbceb-233">Der Befehl gibt die Liste der Sicherungselemente zurück, die durch die angegebene Richtlinien-ID geschützt sind.</span><span class="sxs-lookup"><span data-stu-id="dbceb-233">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="dbceb-234">„Microsoft.Azure.Management.RecoveryServices.Backup“ auf Version 3.0.0-preview aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-234">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="dbceb-235">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-235">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="dbceb-236">TargetResourceGroupName-Parameter zu „Restore-AzureRmRecoveryServicesBackupItem“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="dbceb-236">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="dbceb-237">Die Ressourcengruppe, in der die verwalteten Datenträger wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="dbceb-237">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="dbceb-238">Gilt für die Sicherung des virtuellen Computers mit verwalteten Datenträgern.</span><span class="sxs-lookup"><span data-stu-id="dbceb-238">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="dbceb-239">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="dbceb-239">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="dbceb-240">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-240">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="dbceb-241">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="dbceb-241">AzureRM.RedisCache</span></span>
* <span data-ttu-id="dbceb-242">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-242">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="dbceb-243">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="dbceb-243">AzureRM.Relay</span></span>
* <span data-ttu-id="dbceb-244">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-244">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="dbceb-245">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="dbceb-245">AzureRM.Resources</span></span>
* <span data-ttu-id="dbceb-246">Unterstützung der Vorlagenbereitstellung im Abonnementbereich.</span><span class="sxs-lookup"><span data-stu-id="dbceb-246">Support template deployment at subscription scope.</span></span> <span data-ttu-id="dbceb-247">Neue Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="dbceb-247">Add new Cmdlets:</span></span>
    - <span data-ttu-id="dbceb-248">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="dbceb-248">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="dbceb-249">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="dbceb-249">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="dbceb-250">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="dbceb-250">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="dbceb-251">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="dbceb-251">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="dbceb-252">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="dbceb-252">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="dbceb-253">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="dbceb-253">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="dbceb-254">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="dbceb-254">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="dbceb-255">Problem behoben, aufgrund dessen beim Übergeben eines Kontexts an „Set-AzureRmResource“ ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="dbceb-255">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="dbceb-256">Beispiel in „New-AzureRmResourceGroupDeployment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-256">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="dbceb-257">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-257">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="dbceb-258">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="dbceb-258">AzureRM.Scheduler</span></span>
* <span data-ttu-id="dbceb-259">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-259">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="dbceb-260">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="dbceb-260">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="dbceb-261">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-261">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="dbceb-262">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="dbceb-262">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="dbceb-263">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-263">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="dbceb-264">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="dbceb-264">AzureRM.Sql</span></span>
* <span data-ttu-id="dbceb-265">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-265">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="dbceb-266">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="dbceb-266">AzureRM.Storage</span></span>
* <span data-ttu-id="dbceb-267">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-267">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="dbceb-268">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="dbceb-268">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="dbceb-269">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-269">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="dbceb-270">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="dbceb-270">AzureRM.Tags</span></span>
* <span data-ttu-id="dbceb-271">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-271">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="dbceb-272">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="dbceb-272">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="dbceb-273">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-273">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="dbceb-274">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="dbceb-274">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="dbceb-275">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-275">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="dbceb-276">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="dbceb-276">AzureRM.Websites</span></span>
* <span data-ttu-id="dbceb-277">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-277">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="dbceb-278">6.6.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="dbceb-278">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="dbceb-279">Allgemein</span><span class="sxs-lookup"><span data-stu-id="dbceb-279">General</span></span>
* <span data-ttu-id="dbceb-280">Alle Hilfedateien aktualisiert, um vollständige Parametertypen und die richtigen Eingabe/Ausgabe-Typen einzuschließen.</span><span class="sxs-lookup"><span data-stu-id="dbceb-280">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="dbceb-281">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="dbceb-281">AzureRM.Profile</span></span>
* <span data-ttu-id="dbceb-282">Bibliothek „Common.Strategy“ aktualisiert, um überprüfen zu können, ob die aktuelle Konfiguration für eine Ressource mit der Zielressource kompatibel ist.</span><span class="sxs-lookup"><span data-stu-id="dbceb-282">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="dbceb-283">ps1xml-Typen zu „Common.Storage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-283">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="dbceb-284">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="dbceb-284">Azure.Storage</span></span>
* <span data-ttu-id="dbceb-285">Unterstützung zum Abrufen von Speicherkontext aus „DefaultProfile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-285">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="dbceb-286">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-286">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="dbceb-287">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="dbceb-287">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="dbceb-288">Problem https://github.com/Azure/azure-powershell/issues/6370 behoben</span><span class="sxs-lookup"><span data-stu-id="dbceb-288">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="dbceb-289">Fehler in Automapper behoben, um „PsApiManagementApi“ in „ApiContract“ zu verschieben</span><span class="sxs-lookup"><span data-stu-id="dbceb-289">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="dbceb-290">Problem https://github.com/Azure/azure-powershell/issues/6515 behoben</span><span class="sxs-lookup"><span data-stu-id="dbceb-290">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="dbceb-291">Fehler in „File.Save“ behoben, um Überladung mit Codierungstyp zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="dbceb-291">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="dbceb-292">Problem https://github.com/Azure/azure-powershell/issues/6560 behoben</span><span class="sxs-lookup"><span data-stu-id="dbceb-292">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="dbceb-293">Upgrade auf Nuget-Version 4.0.3 durchgeführt, in der Musterausnahme in „apiId“ behoben wurde</span><span class="sxs-lookup"><span data-stu-id="dbceb-293">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="dbceb-294">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="dbceb-294">AzureRM.Compute</span></span>
* <span data-ttu-id="dbceb-295">Das Problem, aufgrund dessen beim Erstellen eines virtuellen Computers mithilfe von „DiskFileParameterSet“ in „New-AzureRmVm“ wegen einer Umbenennung des Speicherkontotyps „PremiumLRS“ ein Fehler auftrat, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="dbceb-295">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="dbceb-296">Cmdlet „Invoke-AzureRmVMRunCommand“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-296">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="dbceb-297">„Get-AzureRmAvailabilitySet“ aktualisiert, um die Auflistung aller Verfügbarkeitsgruppen in einem Abonnement zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="dbceb-297">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="dbceb-298">(ResouceGroupName-Parameter ist jetzt optional.)</span><span class="sxs-lookup"><span data-stu-id="dbceb-298">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="dbceb-299">„SimpleParameterSet“ von „New-AzureRmVm“ aktualisiert, um Accelerated Networking auf kompatiblen virtuellen Computern zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="dbceb-299">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="dbceb-300">Einfacher Parametersatz „New-AzureRmVmss“ aktualisiert, sodass das Erstellen der VMSS fehlschlägt, wenn bereits ein benutzerdefinierter LB vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="dbceb-300">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="dbceb-301">Beispiel für „New-AzureRmDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-301">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="dbceb-302">Beispiel für „New-AzureRmVM“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-302">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="dbceb-303">Beschreibung für „Set-AzureRmVMOSDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-303">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="dbceb-304">Beispiel 1 für „Set-AzureRmVMBginfoExtension“ aktualisiert, um Rechtschreibung und Präfix zu korrigieren.</span><span class="sxs-lookup"><span data-stu-id="dbceb-304">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="dbceb-305">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="dbceb-305">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="dbceb-306">ADF .Net SDK-Version auf 1.1.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="dbceb-306">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="dbceb-307">Unterstützung der Freigabe der selbstgehosteten Integration Runtime über Data Factorys hinweg.</span><span class="sxs-lookup"><span data-stu-id="dbceb-307">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="dbceb-308">Neuer Parameter „-SharedIntegrationRuntimeResourceId“ zu Cmdlet „Set-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="dbceb-308">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="dbceb-309">Neuer optionaler Parameter „-LinkedDataFactoryName“ zu Cmdlet „Remove-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="dbceb-309">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="dbceb-310">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="dbceb-310">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="dbceb-311">DataPlane SDK-Version (Microsoft.Azure.DataLake.Store) auf 1.1.9 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-311">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="dbceb-312">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="dbceb-312">AzureRM.EventHub</span></span>
* <span data-ttu-id="dbceb-313">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-313">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="dbceb-314">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="dbceb-314">AzureRM.Insights</span></span>
* <span data-ttu-id="dbceb-315">Formatierung von „OutputType“ in Hilfedateien korrigiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-315">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="dbceb-316">Verwendung von Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span><span class="sxs-lookup"><span data-stu-id="dbceb-316">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="dbceb-317">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="dbceb-317">AzureRM.KeyVault</span></span>
* <span data-ttu-id="dbceb-318">Piping-Problem in „Set-AzureRmKeyVaultAccessPolicy“ behoben</span><span class="sxs-lookup"><span data-stu-id="dbceb-318">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="dbceb-319">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="dbceb-319">AzureRM.Network</span></span>
* <span data-ttu-id="dbceb-320">Beispiele für LoadBalancerInboundNatPoolConfig-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="dbceb-320">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="dbceb-321">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="dbceb-321">AzureRM.Resources</span></span>
* <span data-ttu-id="dbceb-322">Problem beim Angeben sowohl des Tag-Namens als auch des Werts für „Get-AzureRmResource“ behoben</span><span class="sxs-lookup"><span data-stu-id="dbceb-322">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="dbceb-323">Piping-Szenario mit „Set-AzureRmResource“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-323">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="dbceb-324">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="dbceb-324">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="dbceb-325">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-325">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="dbceb-326">Einige Probleme behoben</span><span class="sxs-lookup"><span data-stu-id="dbceb-326">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="dbceb-327">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="dbceb-327">AzureRM.Sql</span></span>
* <span data-ttu-id="dbceb-328">Unterstützung für Advanced Threat Protection für Server bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="dbceb-328">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="dbceb-329">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="dbceb-329">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="dbceb-330">Unterstützung für Sicherheitsrisikobewertung bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="dbceb-330">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="dbceb-331">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="dbceb-331">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="dbceb-332">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="dbceb-332">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="dbceb-333">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="dbceb-333">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="dbceb-334">Beispiel in „Remove-AzureRmSqlServerFirewallRule“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-334">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="dbceb-335">Falsche Verarbeitung von „datetime“ für nicht US-basierte Kultur in „Get-AzureSqlSyncGroupLog“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-335">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="dbceb-336">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="dbceb-336">AzureRM.Storage</span></span>
* <span data-ttu-id="dbceb-337">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-337">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="dbceb-338">Cmdlet-Ausgabe von „StorageAccount“ in Tabellenansicht anzeigen</span><span class="sxs-lookup"><span data-stu-id="dbceb-338">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="dbceb-339">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="dbceb-339">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="dbceb-340">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="dbceb-340">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="dbceb-341">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="dbceb-341">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="dbceb-342">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="dbceb-342">AzureRM.Tags</span></span>
* <span data-ttu-id="dbceb-343">Falsche Anweisung aus Tag-Cmdlet-Hilfe entfernt</span><span class="sxs-lookup"><span data-stu-id="dbceb-343">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="dbceb-344">6.5.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="dbceb-344">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="dbceb-345">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="dbceb-345">AzureRM.Profile</span></span>
* <span data-ttu-id="dbceb-346">Hilfe für „Get-AzureRmContextAutosaveSetting“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-346">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="dbceb-347">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="dbceb-347">Azure.Storage</span></span>
* <span data-ttu-id="dbceb-348">Unterstützung des Blob- oder Dateiuploads mit lesegeschütztem SAS-Token</span><span class="sxs-lookup"><span data-stu-id="dbceb-348">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="dbceb-349">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="dbceb-349">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="dbceb-350">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="dbceb-350">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="dbceb-351">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="dbceb-351">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="dbceb-352">Erforderliche Eigenschaft „ResourceGroupName“ zu AS hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="dbceb-352">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="dbceb-353">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="dbceb-353">AzureRM.Automation</span></span>
* <span data-ttu-id="dbceb-354">Hilfe aktualisiert und Beispiel für „New-AzureRMAutomationSchedule“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-354">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="dbceb-355">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="dbceb-355">AzureRM.Compute</span></span>
* <span data-ttu-id="dbceb-356">Parameter „-Tag“ zu „Update/New-AzureRmAvailabilitySet“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-356">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="dbceb-357">Beispiel für „Add-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-357">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="dbceb-358">Beispiele für „Remove-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-358">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="dbceb-359">Hilfe für „Set-AzureRmVMAccessExtension“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-359">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="dbceb-360">„SimpleParameterSet“ für „New-AzureRmVmss“ so aktualisiert, dass „SinglePlacementGroup“ standardmäßig auf „false“ festgelegt ist, und Switch-Parameter „SinglePlacementGroup“ hinzugefügt, der dem Benutzer das Erstellen der VMSS in einer einzelnen Platzierungsgruppe ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="dbceb-360">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="dbceb-361">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="dbceb-361">AzureRM.EventHub</span></span>
* <span data-ttu-id="dbceb-362">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSEventHubDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="dbceb-362">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="dbceb-363">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="dbceb-363">AzureRM.KeyVault</span></span>
* <span data-ttu-id="dbceb-364">Fehlermeldung für „Set-AzureRmKeyVaultAccessPolicy“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-364">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="dbceb-365">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="dbceb-365">AzureRM.LogicApp</span></span>
* <span data-ttu-id="dbceb-366">Fehler „Parametersatz konnte nicht aufgelöst werden“ in „New-AzureRmLogicApp“behoben</span><span class="sxs-lookup"><span data-stu-id="dbceb-366">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="dbceb-367">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="dbceb-367">AzureRM.Network</span></span>
* <span data-ttu-id="dbceb-368">Peering über mehrere virtuelle Netzwerke in mehreren Mandanten für „Set/Add-AzureRmVirtualNetworkPeering“ aktiviert</span><span class="sxs-lookup"><span data-stu-id="dbceb-368">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="dbceb-369">Folgende Cmdlets für Application Gateway aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-369">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="dbceb-370">New-AzureRmApplicationGateway: EnableFIPS-Flag und Zonenunterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-370">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="dbceb-371">New-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-371">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="dbceb-372">Set-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-372">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="dbceb-373">RouteTable-Cmdlets mit aktueller Generatorversion erneut generiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-373">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="dbceb-374">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="dbceb-374">AzureRM.Relay</span></span>
* <span data-ttu-id="dbceb-375">Markdowndateien aktualisiert, Problem mit Parametername in Beispiel behoben</span><span class="sxs-lookup"><span data-stu-id="dbceb-375">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="dbceb-376">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="dbceb-376">AzureRM.Resources</span></span>
* <span data-ttu-id="dbceb-377">Roleassignment- und roledefinition-Cmdlets aktualisiert:</span><span class="sxs-lookup"><span data-stu-id="dbceb-377">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="dbceb-378">Zusätzliche roledefinition-Aufrufe entfernt, die als Teil des Pagings durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="dbceb-378">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="dbceb-379">Get-AzureRmRoleAssignment-Cmdlet korrigiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-379">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="dbceb-380">Befehlsparameterfunktion von „-ExpandPrincipalGroups“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-380">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="dbceb-381">Problem mit „Get-AzureRmResource“ behoben, aufgrund dessen die Groß-/Kleinschreibung des Parameters „-ResourceType“ beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="dbceb-381">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="dbceb-382">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="dbceb-382">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="dbceb-383">top- und skip-Parameter zu Listen-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-383">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="dbceb-384">Cmdlets für die Migration von Standard- zu Premium-Namespace hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="dbceb-384">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="dbceb-385">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="dbceb-385">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="dbceb-386">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="dbceb-386">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="dbceb-387">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="dbceb-387">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="dbceb-388">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="dbceb-388">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="dbceb-389">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="dbceb-389">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="dbceb-390">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSServiceBusDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="dbceb-390">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="dbceb-391">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="dbceb-391">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="dbceb-392">Beispiel für „New-AzureRmServiceFabricCluster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-392">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="dbceb-393">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="dbceb-393">AzureRM.Sql</span></span>
* <span data-ttu-id="dbceb-394">Neue Cmdlets für „Management.Sql“ hinzugefügt, um Kunden das Hinzufügen des TDE-Zertifikats zu einer SQL Server-Instanz oder einer verwalteten Instanz zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="dbceb-394">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="dbceb-395">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="dbceb-395">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="dbceb-396">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="dbceb-396">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="dbceb-397">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="dbceb-397">AzureRM.Websites</span></span>
* <span data-ttu-id="dbceb-398">Wenn `Set-AzureRmWebApp -AssignIdentity` und `Set-AzureRmWebAppSlot -AssignIdentity` auf „false“ festgelegt sind, wird jetzt die Identity-Eigenschaft aus dem Websiteobjekt entfernt. Auch das Vorschau-Tag wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="dbceb-398">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="dbceb-399">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics`-Beispiel aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-399">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="dbceb-400">Unterstützung von `Set-AzureRmWebApp -PhpVersion` als gültige PHP-Version eingestellt</span><span class="sxs-lookup"><span data-stu-id="dbceb-400">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="dbceb-401">6.4.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="dbceb-401">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="dbceb-402">Allgemein</span><span class="sxs-lookup"><span data-stu-id="dbceb-402">General</span></span>
* <span data-ttu-id="dbceb-403">Formatierung von OutputType in Hilfedateien für die meisten Module korrigiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-403">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="dbceb-404">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="dbceb-404">AzureRM.Profile</span></span>
* <span data-ttu-id="dbceb-405">Attribut „Ps1Xml“ wurde den Standardausgabetypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-405">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="dbceb-406">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="dbceb-406">AzureRM.Compute</span></span>
* <span data-ttu-id="dbceb-407">IP-Tag-Funktion für VMSS</span><span class="sxs-lookup"><span data-stu-id="dbceb-407">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="dbceb-408">Cmdlet „New-AzureRmVmssIpTagConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-408">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="dbceb-409">IpTag-Parameter zu „New-AzureRmVmssIpConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-409">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="dbceb-410">Funktion für automatisches Betriebssystemrollback für VMSS</span><span class="sxs-lookup"><span data-stu-id="dbceb-410">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="dbceb-411">DisableAutoRollback-Parameter zu „New-AzureRmVmssConfig“ und „Update-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-411">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="dbceb-412">Funktion für Upgradeverlauf des Betriebssystems für VMSS</span><span class="sxs-lookup"><span data-stu-id="dbceb-412">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="dbceb-413">Switch-Parameter „OSUpgradeHistory“ zu „Get-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-413">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="dbceb-414">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="dbceb-414">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="dbceb-415">Unterstützung für Katalog-ACLs über die folgenden Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="dbceb-415">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="dbceb-416">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="dbceb-416">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="dbceb-417">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="dbceb-417">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="dbceb-418">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="dbceb-418">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="dbceb-419">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="dbceb-419">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="dbceb-420">Abbruchunterstützung und Nachverfolgung des Fortschritts für „Set-AzureRmDataLakeStoreItemAclEntry“, „Remove-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-420">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="dbceb-421">Abbruchunterstützung „Export-AzureRmDataLakeStoreChildItemProperties“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-421">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="dbceb-422">Leerung von Debugmeldungen für Cmdlets korrigiert, die rekursive Vorgänge durchführt</span><span class="sxs-lookup"><span data-stu-id="dbceb-422">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="dbceb-423">Speicherort des Test von DataLake-Cmdlets korrigiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-423">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="dbceb-424">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="dbceb-424">AzureRM.EventHub</span></span>
* <span data-ttu-id="dbceb-425">Optionaler Parameter „MaxCount“ zu Listenvorgangs-Cmdlets „Get-AzureRmEventHub“ und „Get-AzureRmEventHubConsumerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-425">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="dbceb-426">Problem in Cmdlet „New-AzureRmEventHub“ behoben, aufgrund dessen beim Erstellen einer neuen EventHub-Instanz mindestens ein Parameter benötigt wurde.</span><span class="sxs-lookup"><span data-stu-id="dbceb-426">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="dbceb-427">Standardparametersatz wurde bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="dbceb-427">Provided Default Parameter set.</span></span>
* <span data-ttu-id="dbceb-428">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmEventHubKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="dbceb-428">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="dbceb-429">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="dbceb-429">AzureRM.KeyVault</span></span>
* <span data-ttu-id="dbceb-430">Problem behoben, aufgrund dessen von „Get-AzureRmKeyVault -Tag“ alle Ressourcen zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="dbceb-430">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="dbceb-431">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="dbceb-431">AzureRM.Network</span></span>
* <span data-ttu-id="dbceb-432">Neue SKUs für zonenredundante VirtualNetworkGateways-Instanzen verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="dbceb-432">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="dbceb-433">Neue Befehle für Funktion hinzugefügt: ExpressRoute-Partner-APIs über ARM</span><span class="sxs-lookup"><span data-stu-id="dbceb-433">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="dbceb-434">Get-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-434">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="dbceb-435">Set-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-435">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="dbceb-436">Add-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-436">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="dbceb-437">Get-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-437">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="dbceb-438">Remove-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-438">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="dbceb-439">Get-AzureRMExpressRouteCrossConnectionArpTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-439">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="dbceb-440">Get-AzureRMExpressRouteCrossConnectionRouteTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-440">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="dbceb-441">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-441">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="dbceb-442">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="dbceb-442">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="dbceb-443">Cmdlet „Get-AzureRmRecoveryServicesBackupStatus“ wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="dbceb-443">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="dbceb-444">Dieses Cmdlet überprüft anhand der ID eines virtuellen Computers, ob dieser durch einen Tresor im Abonnement geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="dbceb-444">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="dbceb-445">Wenn ein solcher Tresor vorhanden ist, gibt das Cmdlet die Tresordetails aus.</span><span class="sxs-lookup"><span data-stu-id="dbceb-445">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="dbceb-446">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="dbceb-446">AzureRM.Resources</span></span>
* <span data-ttu-id="dbceb-447">Cmdlets vom Typ „Get-AzureRmPolicyAssignment“ aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="dbceb-447">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="dbceb-448">Unterstützung für das Auflisten von „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-448">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="dbceb-449">Unterstützung für das Abrufen einzelner Arbeitsaufträge mit „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-449">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="dbceb-450">Switches „-Effective“ und „-All“ zu Steuerparameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-450">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="dbceb-451">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicyDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-451">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="dbceb-452">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="dbceb-452">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="dbceb-453">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="dbceb-453">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="dbceb-454">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicySetDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-454">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="dbceb-455">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="dbceb-455">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="dbceb-456">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="dbceb-456">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="dbceb-457">Unterstützung für KeyVault-Geheimnisverweis in Parametern hinzugefügt, wenn „TemplateParameterObject“ in „New-AzureRmResourceGroupDeployment“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="dbceb-457">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="dbceb-458">Problem behoben, aufgrund dessen, der Parameter „-EndDate“ für „New-AzureRmADAppCredential“ ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="dbceb-458">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="dbceb-459">Problem behoben, aufgrund dessen „Add-AzureRmADGroupMember“ eine falsche URL für Anforderungen verwendete</span><span class="sxs-lookup"><span data-stu-id="dbceb-459">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="dbceb-460">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="dbceb-460">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="dbceb-461">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmServiceBusKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="dbceb-461">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="dbceb-462">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="dbceb-462">AzureRM.Sql</span></span>
* <span data-ttu-id="dbceb-463">Benutzerdefinierte Wiederherstellungspunkte für SQLDW in Hilfe zu „New-AzureRmSqlDatabaseRestorePoint“ erläutert</span><span class="sxs-lookup"><span data-stu-id="dbceb-463">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="dbceb-464">Dokumentation von Parameter „-ComputeGeneration“ in mehreren Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-464">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="dbceb-465">6.3.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="dbceb-465">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="dbceb-466">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="dbceb-466">AzureRM.Profile</span></span>
* <span data-ttu-id="dbceb-467">Aktualisierte Fehlermeldungen für „Enable-AzureRmContextAutoSave“</span><span class="sxs-lookup"><span data-stu-id="dbceb-467">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="dbceb-468">Erstellen eines Kontexts für jedes Abonnement beim Ausführen von „Connect-AzureRmAccount“ ohne vorherigen Kontext</span><span class="sxs-lookup"><span data-stu-id="dbceb-468">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="dbceb-469">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="dbceb-469">Azure.Storage</span></span>
* <span data-ttu-id="dbceb-470">Zusätzliche Informationen zum Parameter „-Permissions“ in Hilfedateien</span><span class="sxs-lookup"><span data-stu-id="dbceb-470">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="dbceb-471">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="dbceb-471">AzureRM.Compute</span></span>
* <span data-ttu-id="dbceb-472">„Get-AzureRmVmDiskEncryptionStatus“ behebt ein Problem, das bei virtuellen Computern ohne Datenträger festgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="dbceb-472">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="dbceb-473">Version der Computeclientbibliothek aktualisiert, um folgende Cmdlets zu korrigieren:</span><span class="sxs-lookup"><span data-stu-id="dbceb-473">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="dbceb-474">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="dbceb-474">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="dbceb-475">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="dbceb-475">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="dbceb-476">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="dbceb-476">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="dbceb-477">Die folgenden Cmdlets wurden korrigiert, um die Vorgangs-ID und den Vorgangsstatus korrekt anzuzeigen:</span><span class="sxs-lookup"><span data-stu-id="dbceb-477">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="dbceb-478">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="dbceb-478">Start-AzureRmVM</span></span>
    - <span data-ttu-id="dbceb-479">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="dbceb-479">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="dbceb-480">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="dbceb-480">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="dbceb-481">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="dbceb-481">Set-AzureRmVM</span></span>
    - <span data-ttu-id="dbceb-482">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="dbceb-482">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="dbceb-483">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="dbceb-483">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="dbceb-484">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="dbceb-484">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="dbceb-485">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="dbceb-485">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="dbceb-486">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="dbceb-486">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="dbceb-487">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="dbceb-487">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="dbceb-488">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="dbceb-488">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="dbceb-489">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="dbceb-489">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="dbceb-490">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="dbceb-490">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="dbceb-491">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="dbceb-491">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="dbceb-492">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="dbceb-492">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="dbceb-493">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="dbceb-493">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="dbceb-494">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="dbceb-494">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="dbceb-495">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="dbceb-495">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="dbceb-496">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="dbceb-496">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="dbceb-497">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="dbceb-497">AzureRM.EventGrid</span></span>
* <span data-ttu-id="dbceb-498">ValidateNotNullOrEmpty-Überprüfungskonditionen für „SubjectBeginsWith“/„SubjectEndsWith“ im Cmdlet „Update-AzureRmEventGridSubscription“ wurden entfernt, um bei Bedarf die Änderung dieser Parameter in eine leere Zeichenfolge zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="dbceb-498">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="dbceb-499">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="dbceb-499">AzureRM.KeyVault</span></span>
* <span data-ttu-id="dbceb-500">Ein Problem wurde behoben, aufgrund dessen bei Ausführung von „Get-AzureRmKeyVault -Tag“ keine Tags zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="dbceb-500">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="dbceb-501">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="dbceb-501">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="dbceb-502">Offizielle Veröffentlichung von Policy Insights-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="dbceb-502">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="dbceb-503">Verwendung der API-Version 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="dbceb-503">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="dbceb-504">„PolicyDefinitionReferenceId“ zu den Ergebnissen von „Get-AzureRmPolicyStateSummary“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-504">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="dbceb-505">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="dbceb-505">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="dbceb-506">Parameter „-Vault“ zu den RecoveryServices.Backup-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="dbceb-506">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="dbceb-507">Bei der Übergabe wird dadurch das Cmdlet „Set-AzureRmRecoveryServicesContext“ außer Kraft gesetzt.</span><span class="sxs-lookup"><span data-stu-id="dbceb-507">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="dbceb-508">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="dbceb-508">AzureRM.Sql</span></span>
* <span data-ttu-id="dbceb-509">Aktualisiertes Beispiel in der Hilfedatei für „Get-AzureRmSqlDatabaseExpanded“</span><span class="sxs-lookup"><span data-stu-id="dbceb-509">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="dbceb-510">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="dbceb-510">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="dbceb-511">Hilfedatei für „Add-AzureRmTrafficManagerEndpointConfig“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="dbceb-511">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="dbceb-512">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="dbceb-512">AzureRM.Websites</span></span>
* <span data-ttu-id="dbceb-513">„Set-AzureRmWebApp“ wurde aktualisiert, damit „AppSettings“ bei der Verwendung von „-AssignIdentity“ nicht außer Kraft gesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="dbceb-513">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="dbceb-514">„New-AzureRmWebAppSlot“ wurde aktualisiert, um „AppServicePlan“ als optionalen Parameter anzuerkennen</span><span class="sxs-lookup"><span data-stu-id="dbceb-514">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="dbceb-515">6.2.1: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="dbceb-515">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="dbceb-516">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="dbceb-516">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="dbceb-517">PSWorkspace-Modell aktualisiert, damit das Netzwerk „type“ als Parameter verwenden kann</span><span class="sxs-lookup"><span data-stu-id="dbceb-517">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="dbceb-518">6.2.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="dbceb-518">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="dbceb-519">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="dbceb-519">AzureRM.Profile</span></span>
* <span data-ttu-id="dbceb-520">Beheben des Problems, aufgrund dessen Version 10.0.3 von Newtonsoft.Json beim Modulimport nicht geladen wurde</span><span class="sxs-lookup"><span data-stu-id="dbceb-520">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="dbceb-521">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="dbceb-521">AzureRM.Compute</span></span>
* <span data-ttu-id="dbceb-522">Feature zum Aktualisieren von virtuellen VMSS-Computern</span><span class="sxs-lookup"><span data-stu-id="dbceb-522">VMSS VM Update feature</span></span>
    - <span data-ttu-id="dbceb-523">Cmdlets „Update-AzureRmVmssVM“ und „New-AzureRmVMDataDisk“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-523">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="dbceb-524">Fügen Sie den Parameter „VirtualMachineScaleSetVM“ zum Cmdlet „Add-AzureRmVMDataDisk“ hinzu, um das Hinzufügen eines Datenträgers zum virtuellen VMSS-Computer zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="dbceb-524">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="dbceb-525">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="dbceb-525">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="dbceb-526">Aktualisierung der ADF .Net SDK-Version auf 0.8.0-preview mit den folgenden Änderungen:</span><span class="sxs-lookup"><span data-stu-id="dbceb-526">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="dbceb-527">Vorgang zum Konfigurieren des Factoryrepositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-527">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="dbceb-528">Der verknüpfte QuickBooks-Dienst wurde aktualisiert, um die Eigenschaften „consumerKey“ und „consumerSecret“ verfügbar zu machen.</span><span class="sxs-lookup"><span data-stu-id="dbceb-528">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="dbceb-529">Aktualisierung verschiedener Modelltypen von „SecretBase“ auf „Object“</span><span class="sxs-lookup"><span data-stu-id="dbceb-529">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="dbceb-530">Blobereignisauslöser hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-530">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="dbceb-531">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="dbceb-531">AzureRM.KeyVault</span></span>
* <span data-ttu-id="dbceb-532">Aktualisierung der Dokumentation mit Beispielausgabe</span><span class="sxs-lookup"><span data-stu-id="dbceb-532">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="dbceb-533">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="dbceb-533">AzureRM.Network</span></span>
* <span data-ttu-id="dbceb-534">Aktivierung der Traffic Analytics-Parameter für Network Watcher-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="dbceb-534">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="dbceb-535">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="dbceb-535">AzureRM.Resources</span></span>
* <span data-ttu-id="dbceb-536">Behebung des Problems mit der Eigenschaft „Properties“ von PSResource-Objekten, die von „Get-AzureRmResource“ zurückgegeben wurden</span><span class="sxs-lookup"><span data-stu-id="dbceb-536">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="dbceb-537">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="dbceb-537">AzureRM.Scheduler</span></span>
* <span data-ttu-id="dbceb-538">Behebung des Problems, dass beim Aktualisieren von „ServiceBusQueueJob“ keine neuen Authentifizierungswerte festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="dbceb-538">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="dbceb-539">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="dbceb-539">AzureRM.Sql</span></span>
* <span data-ttu-id="dbceb-540">Aktualisierung der folgenden Cmdlets mit dem optionalen LicenseType-Parameter</span><span class="sxs-lookup"><span data-stu-id="dbceb-540">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="dbceb-541">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="dbceb-541">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="dbceb-542">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="dbceb-542">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="dbceb-543">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="dbceb-543">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="dbceb-544">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="dbceb-544">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="dbceb-545">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="dbceb-545">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="dbceb-546">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="dbceb-546">AzureRM.Websites</span></span>
* <span data-ttu-id="dbceb-547">„New-AzureRMWebApp“ aktualisiert, um allgemeine Algorithmen aus der Strategiebibliothek zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="dbceb-547">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="dbceb-548">6.1.0 – Mai 2018</span><span class="sxs-lookup"><span data-stu-id="dbceb-548">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="dbceb-549">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="dbceb-549">AzureRM.Profile</span></span>
* <span data-ttu-id="dbceb-550">Behebung eines Problems, durch das beim Ausführen von „Clear-AzureRmContext“ ein leerer Kontext mit dem Namen des vorherigen Standardkontexts beibehalten wurde und der Benutzer dadurch keinen neuen Kontext mit dem alten Namen erstellen konnte</span><span class="sxs-lookup"><span data-stu-id="dbceb-550">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="dbceb-551">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="dbceb-551">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="dbceb-552">Ermöglichung der Zuordnung von Gateways/Aufhebung der Gatewayzuordnung in AS</span><span class="sxs-lookup"><span data-stu-id="dbceb-552">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="dbceb-553">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="dbceb-553">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="dbceb-554">Unterstützung für „ApiVersions“, „ApiReleases“ und „ApiRevisions“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-554">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="dbceb-555">Unterstützung für ServiceFabric-Back-End hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-555">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="dbceb-556">Unterstützung für Application Insights-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-556">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="dbceb-557">Unterstützung für die Erkennung von SKUs vom Typ „Basic“ als gültige SKU des API Management-Diensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-557">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="dbceb-558">Unterstützung hinzugefügt, damit Zertifikate, die von der privaten Zertifizierungsstelle ausgestellt wurden, als Stamm- oder ZS-Zertifikate installiert werden können</span><span class="sxs-lookup"><span data-stu-id="dbceb-558">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="dbceb-559">Unterstützung für die Akzeptierung benutzerdefinierter SSL-Zertifikate über KeyVault und mehrere Proxyhostnamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-559">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="dbceb-560">Unterstützung für die verwaltete Dienstidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-560">Added support for MSI identity</span></span>
* <span data-ttu-id="dbceb-561">Unterstützung für die Annahme von Richtlinien über URL hinzugefügt; HINWEIS: Folgende Cmdlets werden in einem zukünftigen Release als veraltet gekennzeichnet:</span><span class="sxs-lookup"><span data-stu-id="dbceb-561">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="dbceb-562">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="dbceb-562">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="dbceb-563">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="dbceb-563">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="dbceb-564">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="dbceb-564">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="dbceb-565">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="dbceb-565">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="dbceb-566">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="dbceb-566">AzureRM.Batch</span></span>
* <span data-ttu-id="dbceb-567">Veröffentlichung des neuen Cmdlets „Get-AzureBatchPoolNodeCounts“</span><span class="sxs-lookup"><span data-stu-id="dbceb-567">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="dbceb-568">Veröffentlichung des neuen Cmdlets „Start-AzureBatchComputeNodeServiceLogUpload“</span><span class="sxs-lookup"><span data-stu-id="dbceb-568">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="dbceb-569">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="dbceb-569">AzureRM.Consumption</span></span>
* <span data-ttu-id="dbceb-570">Hinzufügung neuer Parameter („Expand“, „ResourceGroup“, „InstanceName“, „InstanceId“, „Tags“ und „Top“) für das Cmdlet „Get-AzureRmConsumptionUsageDetail“</span><span class="sxs-lookup"><span data-stu-id="dbceb-570">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="dbceb-571">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="dbceb-571">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="dbceb-572">Korrektur des Beispiels für „Export AzureRmDataLakeStoreChildItemProperties“</span><span class="sxs-lookup"><span data-stu-id="dbceb-572">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="dbceb-573">Korrektur der NULL-Parameterausnahme für rekursiven Fall in „Set-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="dbceb-573">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="dbceb-574">Korrektur der Hilfedateien für „Set-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ und „Remove-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="dbceb-574">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="dbceb-575">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="dbceb-575">AzureRM.Network</span></span>
* <span data-ttu-id="dbceb-576">Erhöhung der Network SDK-Version von 18.0.0-preview auf 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="dbceb-576">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="dbceb-577">Cmdlet zum Erstellen der Protokollkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-577">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="dbceb-578">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="dbceb-578">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="dbceb-579">Cmdlet zum Hinzufügen einer neuen Leitungsverbindung zu einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-579">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="dbceb-580">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="dbceb-580">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="dbceb-581">Cmdlet zum Entfernen einer Leitungsverbindung aus einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-581">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="dbceb-582">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="dbceb-582">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="dbceb-583">Cmdlet zum Abrufen einer Leitungsverbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="dbceb-583">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="dbceb-584">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="dbceb-584">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="dbceb-585">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="dbceb-585">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="dbceb-586">Verwendung der Serverauthentifizierung mit generierten Zertifikaten korrigiert (Problemnr. 5998)</span><span class="sxs-lookup"><span data-stu-id="dbceb-586">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="dbceb-587">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="dbceb-587">AzureRM.Sql</span></span>
* <span data-ttu-id="dbceb-588">Überwachungscmdlets korrigiert, um das Entfernen von „AuditActions“ oder „AuditActionGroups“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="dbceb-588">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="dbceb-589">Problem mit „Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy“ behoben, das beim Festlegen einer neuen flexiblen Aufbewahrungsrichtlinie zu folgendem Fehler führte: „Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span><span class="sxs-lookup"><span data-stu-id="dbceb-589">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="dbceb-590">Please submit request with the new flexible retention policy“ (Das Konfigurieren einer langfristigen Aufbewahrungsrichtlinie mit Azure Recovery Service-Tresor und -Richtlinie wird nicht mehr unterstützt. Übermitteln Sie eine Anforderung mit der neuen flexiblen Aufbewahrungsrichtlinie.)</span><span class="sxs-lookup"><span data-stu-id="dbceb-590">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="dbceb-591">Aktualisierung aller Cmdlets für Azure SQL-Datenbank, für die Erstellung von Pools für elastische Datenbanken und für die Aktualisierung, sodass sie die neue Datenbank-API verwenden. Diese unterstützt die Sku-Eigenschaft für skalierungs- und tarifbezogene Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="dbceb-591">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="dbceb-592">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="dbceb-592">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="dbceb-593">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="dbceb-593">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="dbceb-594">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="dbceb-594">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="dbceb-595">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="dbceb-595">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="dbceb-596">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="dbceb-596">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="dbceb-597">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="dbceb-597">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="dbceb-598">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="dbceb-598">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="dbceb-599">Aktualisierung der Parameter für „Get-AzureRmTrafficManagerProfile“, sodass bei Verwendung des Parameters „-Name“ der Parameter „-ResourceGroupName“ erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="dbceb-599">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
