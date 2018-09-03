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
ms.sourcegitcommit: 9cb98f055a0525c2061f65149965d5e7c3e03ddc
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/30/2018
ms.locfileid: "43117517"
---
# <a name="release-notes"></a><span data-ttu-id="22e8e-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="22e8e-103">Release notes</span></span>

<span data-ttu-id="22e8e-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="22e8e-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="680---august-2018"></a><span data-ttu-id="22e8e-105">6.8.0: August 2018</span><span class="sxs-lookup"><span data-stu-id="22e8e-105">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="22e8e-106">Allgemein</span><span class="sxs-lookup"><span data-stu-id="22e8e-106">General</span></span>
* <span data-ttu-id="22e8e-107">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="22e8e-107">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="22e8e-108">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="22e8e-108">AzureRM.Profile</span></span>
* <span data-ttu-id="22e8e-109">Ablaufeigenschaft zu Token hinzugefügt, die während „Connect-AzureRmAccount“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="22e8e-109">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="22e8e-110">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="22e8e-110">AzureRM.Compute</span></span>
* <span data-ttu-id="22e8e-111">Problem des fehlenden Ziels in der Fehlerausgabe behoben</span><span class="sxs-lookup"><span data-stu-id="22e8e-111">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="22e8e-112">Problem mit dem Speicherkontotyp für den virtuellen Computer mit verwaltetem Datenträgern behoben</span><span class="sxs-lookup"><span data-stu-id="22e8e-112">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="22e8e-113">AEM-Erweiterungs-Cmdlets für andere Umgebungen (etwa Azure China) korrigiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-113">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="22e8e-114">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="22e8e-114">AzureRM.IotHub</span></span>
* <span data-ttu-id="22e8e-115">Beispiele für „New-AzureRmIotHubExportDevices“ und „New-AzureRmIotHubImportDevices“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-115">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="22e8e-116">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="22e8e-116">AzureRM.Network</span></span>
* <span data-ttu-id="22e8e-117">Standarddarstellung von Modellen in Tabellenansicht geändert</span><span class="sxs-lookup"><span data-stu-id="22e8e-117">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="22e8e-118">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="22e8e-118">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="22e8e-119">Fehler in „Update-AzureRmPowerBIEmbeddedCapacity“ beim Skalieren der angehaltenen Kapazität behoben</span><span class="sxs-lookup"><span data-stu-id="22e8e-119">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="22e8e-120">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="22e8e-120">AzureRM.Resources</span></span>
* <span data-ttu-id="22e8e-121">Problem beim Erstellen der verwalteten Anwendung über Marketplace behoben</span><span class="sxs-lookup"><span data-stu-id="22e8e-121">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="22e8e-122">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="22e8e-122">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="22e8e-123">Fehlerbehebung</span><span class="sxs-lookup"><span data-stu-id="22e8e-123">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="22e8e-124">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="22e8e-124">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="22e8e-125">Unterstützung für Routingmethode „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="22e8e-125">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="22e8e-126">Neuer Parameter „MaxReturn“ für Routingtyp „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="22e8e-126">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="22e8e-127">Unterstützung für Subnetzroutingmethode</span><span class="sxs-lookup"><span data-stu-id="22e8e-127">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="22e8e-128">Unterstützung für IP-Adressbereiche (Subnetze) in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="22e8e-128">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="22e8e-129">Unterstützung für benutzerdefinierte Header in Profilen</span><span class="sxs-lookup"><span data-stu-id="22e8e-129">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="22e8e-130">Unterstützung für erwartete Statuscodebereiche in Profilen</span><span class="sxs-lookup"><span data-stu-id="22e8e-130">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="22e8e-131">Unterstützung für benutzerdefinierte Header in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="22e8e-131">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="22e8e-132">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="22e8e-132">AzureRM.Websites</span></span>
* <span data-ttu-id="22e8e-133">Das Problem, dass die Standardressourcengruppe falsch festgelegt wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="22e8e-133">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="22e8e-134">6.7.0: August 2018</span><span class="sxs-lookup"><span data-stu-id="22e8e-134">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="22e8e-135">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="22e8e-135">AzureRM.Profile</span></span>
* <span data-ttu-id="22e8e-136">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-136">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="22e8e-137">Benutzer-ID zum Standardkontextnamen hinzugefügt, um Kontextkonflikte zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="22e8e-137">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="22e8e-138">Probleme mit „Clear-AzureRmContext“ behoben, die Fehler beim Auswählen eines Kontexts verursacht haben (6398)</span><span class="sxs-lookup"><span data-stu-id="22e8e-138">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="22e8e-139">Ermöglicht, dass für „Connect-AzureRmAccount“ die Mandantendomäne an den Parameter „-TenantId“ übergeben wird</span><span class="sxs-lookup"><span data-stu-id="22e8e-139">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="22e8e-140">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="22e8e-140">Azure.Storage</span></span>
* <span data-ttu-id="22e8e-141">Begrenzung von 5 TB für das Kontingent der Azure-Dateifreigabe entfernt</span><span class="sxs-lookup"><span data-stu-id="22e8e-141">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="22e8e-142">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="22e8e-142">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="22e8e-143">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="22e8e-143">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="22e8e-144">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-144">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="22e8e-145">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="22e8e-145">Azure.AnalysisServices</span></span>
* <span data-ttu-id="22e8e-146">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-146">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="22e8e-147">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="22e8e-147">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="22e8e-148">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-148">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="22e8e-149">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="22e8e-149">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="22e8e-150">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-150">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="22e8e-151">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="22e8e-151">AzureRM.Automation</span></span>
* <span data-ttu-id="22e8e-152">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-152">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="22e8e-153">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="22e8e-153">AzureRM.Backup</span></span>
* <span data-ttu-id="22e8e-154">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-154">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="22e8e-155">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="22e8e-155">AzureRM.Batch</span></span>
* <span data-ttu-id="22e8e-156">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-156">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="22e8e-157">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="22e8e-157">AzureRM.Billing</span></span>
* <span data-ttu-id="22e8e-158">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-158">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="22e8e-159">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="22e8e-159">AzureRM.Cdn</span></span>
* <span data-ttu-id="22e8e-160">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-160">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="22e8e-161">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="22e8e-161">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="22e8e-162">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-162">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="22e8e-163">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="22e8e-163">AzureRM.Compute</span></span>
* <span data-ttu-id="22e8e-164">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-164">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="22e8e-165">EvictionPolicy-Parameter zu „New-AzureRmVmssConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-165">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="22e8e-166">Standort in „DiskFileParameterSet“ von „New-AzureRmVm“ angeben, wenn kein Ort angegeben ist</span><span class="sxs-lookup"><span data-stu-id="22e8e-166">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="22e8e-167">Parameterbeschreibung in „Save-AzureRmVMImage“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-167">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="22e8e-168">Cmdlet „Get-AzureRmVMDiskEncryptionStatus“ für bestimmte Szenarien im Zusammenhang mit einem Durchlauf korrigiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-168">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="22e8e-169">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="22e8e-169">AzureRM.Consumption</span></span>
* <span data-ttu-id="22e8e-170">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-170">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="22e8e-171">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="22e8e-171">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="22e8e-172">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-172">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="22e8e-173">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="22e8e-173">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="22e8e-174">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-174">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="22e8e-175">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="22e8e-175">AzureRM.DataFactories</span></span>
* <span data-ttu-id="22e8e-176">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-176">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="22e8e-177">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="22e8e-177">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="22e8e-178">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-178">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="22e8e-179">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="22e8e-179">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="22e8e-180">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-180">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="22e8e-181">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="22e8e-181">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="22e8e-182">Debuggen korrigiert, wenn „DebugPreference“ über die PowerShell-Befehlszeile festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="22e8e-182">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="22e8e-183">Beispiel für „Set-AzureRmDataLakeStoreItemAcl“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-183">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="22e8e-184">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="22e8e-184">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="22e8e-185">Beispiel für „Set-AzureRmDataLakeStoreItemAclEntry“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-185">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="22e8e-186">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="22e8e-186">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="22e8e-187">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-187">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="22e8e-188">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="22e8e-188">AzureRM.Dns</span></span>
* <span data-ttu-id="22e8e-189">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-189">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="22e8e-190">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="22e8e-190">AzureRM.EventGrid</span></span>
* <span data-ttu-id="22e8e-191">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-191">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="22e8e-192">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="22e8e-192">AzureRM.EventHub</span></span>
* <span data-ttu-id="22e8e-193">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-193">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="22e8e-194">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="22e8e-194">AzureRM.HDInsight</span></span>
* <span data-ttu-id="22e8e-195">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-195">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="22e8e-196">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="22e8e-196">AzureRM.Insights</span></span>
* <span data-ttu-id="22e8e-197">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-197">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="22e8e-198">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="22e8e-198">AzureRM.IotHub</span></span>
* <span data-ttu-id="22e8e-199">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-199">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="22e8e-200">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="22e8e-200">AzureRM.KeyVault</span></span>
* <span data-ttu-id="22e8e-201">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-201">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="22e8e-202">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="22e8e-202">AzureRM.LogicApp</span></span>
* <span data-ttu-id="22e8e-203">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-203">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="22e8e-204">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="22e8e-204">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="22e8e-205">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-205">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="22e8e-206">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="22e8e-206">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="22e8e-207">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-207">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="22e8e-208">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="22e8e-208">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="22e8e-209">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-209">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="22e8e-210">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="22e8e-210">AzureRM.Media</span></span>
* <span data-ttu-id="22e8e-211">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-211">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="22e8e-212">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="22e8e-212">AzureRM.Network</span></span>
* <span data-ttu-id="22e8e-213">Beispiel für „Set-AzureRmLocalNetworkGateway“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-213">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="22e8e-214">Beispiele und Beschreibungen für „Add-AzureRmVirtualNetworkGatewayIpConfig“, „Get-AzureRmVirtualNetworkGatewayConnectionSharedKey“ und „New-AzureRmVirtualNetworkGatewayConnection“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-214">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="22e8e-215">Beispiele für „Remove-AzureRmVirtualNetworkGatewayIpConfig“ und „Reset-AzureRmVirtualNetworkGateway“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-215">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="22e8e-216">Beispiel für „Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-216">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="22e8e-217">Beispiel für „Set-AzureRmVirtualNetworkGatewayConnectionSharedKey“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-217">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="22e8e-218">Beispiel für „Set-AzureRmVirtualNetworkGatewayConnection“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-218">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="22e8e-219">Cmdlets für „ApplicationSecurityGroup“, „RouteTable“ und „Usage“ mithilfe des aktuellen Code-Generators erneut erstellt</span><span class="sxs-lookup"><span data-stu-id="22e8e-219">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="22e8e-220">Deutlichere Formulierung der Fehlermeldung für „Get-AzureRmVirtualNetworkSubnetConfig“, wenn ein nicht vorhandenes Subnetz abgerufen wird</span><span class="sxs-lookup"><span data-stu-id="22e8e-220">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="22e8e-221">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="22e8e-221">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="22e8e-222">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-222">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="22e8e-223">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="22e8e-223">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="22e8e-224">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-224">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="22e8e-225">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="22e8e-225">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="22e8e-226">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-226">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="22e8e-227">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="22e8e-227">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="22e8e-228">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-228">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="22e8e-229">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="22e8e-229">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="22e8e-230">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-230">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="22e8e-231">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="22e8e-231">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="22e8e-232">Richtlinienfilter zum Cmdlet „Get-AzureRmRecoveryServicesBackItem“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="22e8e-232">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="22e8e-233">Der Befehl gibt die Liste der Sicherungselemente zurück, die durch die angegebene Richtlinien-ID geschützt sind.</span><span class="sxs-lookup"><span data-stu-id="22e8e-233">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="22e8e-234">„Microsoft.Azure.Management.RecoveryServices.Backup“ auf Version 3.0.0-preview aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-234">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="22e8e-235">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-235">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="22e8e-236">TargetResourceGroupName-Parameter zu „Restore-AzureRmRecoveryServicesBackupItem“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="22e8e-236">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="22e8e-237">Die Ressourcengruppe, in der die verwalteten Datenträger wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="22e8e-237">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="22e8e-238">Gilt für die Sicherung des virtuellen Computers mit verwalteten Datenträgern.</span><span class="sxs-lookup"><span data-stu-id="22e8e-238">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="22e8e-239">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="22e8e-239">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="22e8e-240">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-240">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="22e8e-241">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="22e8e-241">AzureRM.RedisCache</span></span>
* <span data-ttu-id="22e8e-242">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-242">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="22e8e-243">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="22e8e-243">AzureRM.Relay</span></span>
* <span data-ttu-id="22e8e-244">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-244">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="22e8e-245">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="22e8e-245">AzureRM.Resources</span></span>
* <span data-ttu-id="22e8e-246">Unterstützung der Vorlagenbereitstellung im Abonnementbereich.</span><span class="sxs-lookup"><span data-stu-id="22e8e-246">Support template deployment at subscription scope.</span></span> <span data-ttu-id="22e8e-247">Neue Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="22e8e-247">Add new Cmdlets:</span></span>
    - <span data-ttu-id="22e8e-248">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="22e8e-248">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="22e8e-249">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="22e8e-249">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="22e8e-250">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="22e8e-250">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="22e8e-251">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="22e8e-251">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="22e8e-252">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="22e8e-252">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="22e8e-253">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="22e8e-253">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="22e8e-254">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="22e8e-254">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="22e8e-255">Problem behoben, aufgrund dessen beim Übergeben eines Kontexts an „Set-AzureRmResource“ ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="22e8e-255">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="22e8e-256">Beispiel in „New-AzureRmResourceGroupDeployment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-256">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="22e8e-257">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-257">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="22e8e-258">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="22e8e-258">AzureRM.Scheduler</span></span>
* <span data-ttu-id="22e8e-259">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-259">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="22e8e-260">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="22e8e-260">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="22e8e-261">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-261">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="22e8e-262">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="22e8e-262">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="22e8e-263">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-263">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="22e8e-264">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="22e8e-264">AzureRM.Sql</span></span>
* <span data-ttu-id="22e8e-265">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-265">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="22e8e-266">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="22e8e-266">AzureRM.Storage</span></span>
* <span data-ttu-id="22e8e-267">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-267">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="22e8e-268">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="22e8e-268">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="22e8e-269">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-269">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="22e8e-270">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="22e8e-270">AzureRM.Tags</span></span>
* <span data-ttu-id="22e8e-271">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-271">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="22e8e-272">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="22e8e-272">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="22e8e-273">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-273">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="22e8e-274">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="22e8e-274">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="22e8e-275">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-275">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="22e8e-276">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="22e8e-276">AzureRM.Websites</span></span>
* <span data-ttu-id="22e8e-277">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-277">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="22e8e-278">6.6.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="22e8e-278">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="22e8e-279">Allgemein</span><span class="sxs-lookup"><span data-stu-id="22e8e-279">General</span></span>
* <span data-ttu-id="22e8e-280">Alle Hilfedateien aktualisiert, um vollständige Parametertypen und die richtigen Eingabe/Ausgabe-Typen einzuschließen.</span><span class="sxs-lookup"><span data-stu-id="22e8e-280">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="22e8e-281">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="22e8e-281">AzureRM.Profile</span></span>
* <span data-ttu-id="22e8e-282">Bibliothek „Common.Strategy“ aktualisiert, um überprüfen zu können, ob die aktuelle Konfiguration für eine Ressource mit der Zielressource kompatibel ist.</span><span class="sxs-lookup"><span data-stu-id="22e8e-282">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="22e8e-283">ps1xml-Typen zu „Common.Storage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-283">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="22e8e-284">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="22e8e-284">Azure.Storage</span></span>
* <span data-ttu-id="22e8e-285">Unterstützung zum Abrufen von Speicherkontext aus „DefaultProfile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-285">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="22e8e-286">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-286">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="22e8e-287">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="22e8e-287">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="22e8e-288">Problem https://github.com/Azure/azure-powershell/issues/6370 behoben</span><span class="sxs-lookup"><span data-stu-id="22e8e-288">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="22e8e-289">Fehler in Automapper behoben, um „PsApiManagementApi“ in „ApiContract“ zu verschieben</span><span class="sxs-lookup"><span data-stu-id="22e8e-289">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="22e8e-290">Problem https://github.com/Azure/azure-powershell/issues/6515 behoben</span><span class="sxs-lookup"><span data-stu-id="22e8e-290">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="22e8e-291">Fehler in „File.Save“ behoben, um Überladung mit Codierungstyp zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="22e8e-291">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="22e8e-292">Problem https://github.com/Azure/azure-powershell/issues/6560 behoben</span><span class="sxs-lookup"><span data-stu-id="22e8e-292">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="22e8e-293">Upgrade auf Nuget-Version 4.0.3 durchgeführt, in der Musterausnahme in „apiId“ behoben wurde</span><span class="sxs-lookup"><span data-stu-id="22e8e-293">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="22e8e-294">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="22e8e-294">AzureRM.Compute</span></span>
* <span data-ttu-id="22e8e-295">Das Problem, aufgrund dessen beim Erstellen eines virtuellen Computers mithilfe von „DiskFileParameterSet“ in „New-AzureRmVm“ wegen einer Umbenennung des Speicherkontotyps „PremiumLRS“ ein Fehler auftrat, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="22e8e-295">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="22e8e-296">Cmdlet „Invoke-AzureRmVMRunCommand“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-296">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="22e8e-297">„Get-AzureRmAvailabilitySet“ aktualisiert, um die Auflistung aller Verfügbarkeitsgruppen in einem Abonnement zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="22e8e-297">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="22e8e-298">(ResouceGroupName-Parameter ist jetzt optional.)</span><span class="sxs-lookup"><span data-stu-id="22e8e-298">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="22e8e-299">„SimpleParameterSet“ von „New-AzureRmVm“ aktualisiert, um Accelerated Networking auf kompatiblen virtuellen Computern zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="22e8e-299">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="22e8e-300">Einfacher Parametersatz „New-AzureRmVmss“ aktualisiert, sodass das Erstellen der VMSS fehlschlägt, wenn bereits ein benutzerdefinierter LB vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="22e8e-300">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="22e8e-301">Beispiel für „New-AzureRmDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-301">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="22e8e-302">Beispiel für „New-AzureRmVM“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-302">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="22e8e-303">Beschreibung für „Set-AzureRmVMOSDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-303">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="22e8e-304">Beispiel 1 für „Set-AzureRmVMBginfoExtension“ aktualisiert, um Rechtschreibung und Präfix zu korrigieren.</span><span class="sxs-lookup"><span data-stu-id="22e8e-304">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="22e8e-305">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="22e8e-305">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="22e8e-306">ADF .Net SDK-Version auf 1.1.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="22e8e-306">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="22e8e-307">Unterstützung der Freigabe der selbstgehosteten Integration Runtime über Data Factorys hinweg.</span><span class="sxs-lookup"><span data-stu-id="22e8e-307">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="22e8e-308">Neuer Parameter „-SharedIntegrationRuntimeResourceId“ zu Cmdlet „Set-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="22e8e-308">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="22e8e-309">Neuer optionaler Parameter „-LinkedDataFactoryName“ zu Cmdlet „Remove-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="22e8e-309">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="22e8e-310">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="22e8e-310">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="22e8e-311">DataPlane SDK-Version (Microsoft.Azure.DataLake.Store) auf 1.1.9 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-311">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="22e8e-312">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="22e8e-312">AzureRM.EventHub</span></span>
* <span data-ttu-id="22e8e-313">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-313">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="22e8e-314">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="22e8e-314">AzureRM.Insights</span></span>
* <span data-ttu-id="22e8e-315">Formatierung von „OutputType“ in Hilfedateien korrigiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-315">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="22e8e-316">Verwendung von Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span><span class="sxs-lookup"><span data-stu-id="22e8e-316">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="22e8e-317">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="22e8e-317">AzureRM.KeyVault</span></span>
* <span data-ttu-id="22e8e-318">Piping-Problem in „Set-AzureRmKeyVaultAccessPolicy“ behoben</span><span class="sxs-lookup"><span data-stu-id="22e8e-318">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="22e8e-319">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="22e8e-319">AzureRM.Network</span></span>
* <span data-ttu-id="22e8e-320">Beispiele für LoadBalancerInboundNatPoolConfig-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="22e8e-320">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="22e8e-321">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="22e8e-321">AzureRM.Resources</span></span>
* <span data-ttu-id="22e8e-322">Problem beim Angeben sowohl des Tag-Namens als auch des Werts für „Get-AzureRmResource“ behoben</span><span class="sxs-lookup"><span data-stu-id="22e8e-322">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="22e8e-323">Piping-Szenario mit „Set-AzureRmResource“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-323">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="22e8e-324">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="22e8e-324">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="22e8e-325">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-325">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="22e8e-326">Einige Probleme behoben</span><span class="sxs-lookup"><span data-stu-id="22e8e-326">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="22e8e-327">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="22e8e-327">AzureRM.Sql</span></span>
* <span data-ttu-id="22e8e-328">Unterstützung für Advanced Threat Protection für Server bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="22e8e-328">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="22e8e-329">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="22e8e-329">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="22e8e-330">Unterstützung für Sicherheitsrisikobewertung bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="22e8e-330">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="22e8e-331">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="22e8e-331">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="22e8e-332">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="22e8e-332">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="22e8e-333">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="22e8e-333">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="22e8e-334">Beispiel in „Remove-AzureRmSqlServerFirewallRule“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-334">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="22e8e-335">Falsche Verarbeitung von „datetime“ für nicht US-basierte Kultur in „Get-AzureSqlSyncGroupLog“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-335">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="22e8e-336">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="22e8e-336">AzureRM.Storage</span></span>
* <span data-ttu-id="22e8e-337">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-337">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="22e8e-338">Cmdlet-Ausgabe von „StorageAccount“ in Tabellenansicht anzeigen</span><span class="sxs-lookup"><span data-stu-id="22e8e-338">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="22e8e-339">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="22e8e-339">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="22e8e-340">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="22e8e-340">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="22e8e-341">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="22e8e-341">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="22e8e-342">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="22e8e-342">AzureRM.Tags</span></span>
* <span data-ttu-id="22e8e-343">Falsche Anweisung aus Tag-Cmdlet-Hilfe entfernt</span><span class="sxs-lookup"><span data-stu-id="22e8e-343">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="22e8e-344">6.5.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="22e8e-344">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="22e8e-345">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="22e8e-345">AzureRM.Profile</span></span>
* <span data-ttu-id="22e8e-346">Hilfe für „Get-AzureRmContextAutosaveSetting“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-346">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="22e8e-347">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="22e8e-347">Azure.Storage</span></span>
* <span data-ttu-id="22e8e-348">Unterstützung des Blob- oder Dateiuploads mit lesegeschütztem SAS-Token</span><span class="sxs-lookup"><span data-stu-id="22e8e-348">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="22e8e-349">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="22e8e-349">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="22e8e-350">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="22e8e-350">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="22e8e-351">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="22e8e-351">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="22e8e-352">Erforderliche Eigenschaft „ResourceGroupName“ zu AS hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="22e8e-352">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="22e8e-353">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="22e8e-353">AzureRM.Automation</span></span>
* <span data-ttu-id="22e8e-354">Hilfe aktualisiert und Beispiel für „New-AzureRMAutomationSchedule“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-354">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="22e8e-355">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="22e8e-355">AzureRM.Compute</span></span>
* <span data-ttu-id="22e8e-356">Parameter „-Tag“ zu „Update/New-AzureRmAvailabilitySet“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-356">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="22e8e-357">Beispiel für „Add-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-357">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="22e8e-358">Beispiele für „Remove-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-358">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="22e8e-359">Hilfe für „Set-AzureRmVMAccessExtension“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-359">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="22e8e-360">„SimpleParameterSet“ für „New-AzureRmVmss“ so aktualisiert, dass „SinglePlacementGroup“ standardmäßig auf „false“ festgelegt ist, und Switch-Parameter „SinglePlacementGroup“ hinzugefügt, der dem Benutzer das Erstellen der VMSS in einer einzelnen Platzierungsgruppe ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="22e8e-360">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="22e8e-361">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="22e8e-361">AzureRM.EventHub</span></span>
* <span data-ttu-id="22e8e-362">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSEventHubDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="22e8e-362">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="22e8e-363">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="22e8e-363">AzureRM.KeyVault</span></span>
* <span data-ttu-id="22e8e-364">Fehlermeldung für „Set-AzureRmKeyVaultAccessPolicy“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-364">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="22e8e-365">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="22e8e-365">AzureRM.LogicApp</span></span>
* <span data-ttu-id="22e8e-366">Fehler „Parametersatz konnte nicht aufgelöst werden“ in „New-AzureRmLogicApp“behoben</span><span class="sxs-lookup"><span data-stu-id="22e8e-366">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="22e8e-367">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="22e8e-367">AzureRM.Network</span></span>
* <span data-ttu-id="22e8e-368">Peering über mehrere virtuelle Netzwerke in mehreren Mandanten für „Set/Add-AzureRmVirtualNetworkPeering“ aktiviert</span><span class="sxs-lookup"><span data-stu-id="22e8e-368">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="22e8e-369">Folgende Cmdlets für Application Gateway aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-369">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="22e8e-370">New-AzureRmApplicationGateway: EnableFIPS-Flag und Zonenunterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-370">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="22e8e-371">New-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-371">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="22e8e-372">Set-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-372">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="22e8e-373">RouteTable-Cmdlets mit aktueller Generatorversion erneut generiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-373">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="22e8e-374">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="22e8e-374">AzureRM.Relay</span></span>
* <span data-ttu-id="22e8e-375">Markdowndateien aktualisiert, Problem mit Parametername in Beispiel behoben</span><span class="sxs-lookup"><span data-stu-id="22e8e-375">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="22e8e-376">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="22e8e-376">AzureRM.Resources</span></span>
* <span data-ttu-id="22e8e-377">Roleassignment- und roledefinition-Cmdlets aktualisiert:</span><span class="sxs-lookup"><span data-stu-id="22e8e-377">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="22e8e-378">Zusätzliche roledefinition-Aufrufe entfernt, die als Teil des Pagings durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="22e8e-378">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="22e8e-379">Get-AzureRmRoleAssignment-Cmdlet korrigiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-379">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="22e8e-380">Befehlsparameterfunktion von „-ExpandPrincipalGroups“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-380">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="22e8e-381">Problem mit „Get-AzureRmResource“ behoben, aufgrund dessen die Groß-/Kleinschreibung des Parameters „-ResourceType“ beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="22e8e-381">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="22e8e-382">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="22e8e-382">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="22e8e-383">top- und skip-Parameter zu Listen-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-383">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="22e8e-384">Cmdlets für die Migration von Standard- zu Premium-Namespace hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="22e8e-384">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="22e8e-385">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="22e8e-385">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="22e8e-386">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="22e8e-386">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="22e8e-387">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="22e8e-387">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="22e8e-388">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="22e8e-388">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="22e8e-389">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="22e8e-389">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="22e8e-390">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSServiceBusDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="22e8e-390">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="22e8e-391">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="22e8e-391">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="22e8e-392">Beispiel für „New-AzureRmServiceFabricCluster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-392">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="22e8e-393">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="22e8e-393">AzureRM.Sql</span></span>
* <span data-ttu-id="22e8e-394">Neue Cmdlets für „Management.Sql“ hinzugefügt, um Kunden das Hinzufügen des TDE-Zertifikats zu einer SQL Server-Instanz oder einer verwalteten Instanz zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="22e8e-394">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="22e8e-395">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="22e8e-395">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="22e8e-396">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="22e8e-396">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="22e8e-397">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="22e8e-397">AzureRM.Websites</span></span>
* <span data-ttu-id="22e8e-398">Wenn `Set-AzureRmWebApp -AssignIdentity` und `Set-AzureRmWebAppSlot -AssignIdentity` auf „false“ festgelegt sind, wird jetzt die Identity-Eigenschaft aus dem Websiteobjekt entfernt. Auch das Vorschau-Tag wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="22e8e-398">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="22e8e-399">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics`-Beispiel aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-399">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="22e8e-400">Unterstützung von `Set-AzureRmWebApp -PhpVersion` als gültige PHP-Version eingestellt</span><span class="sxs-lookup"><span data-stu-id="22e8e-400">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="22e8e-401">6.4.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="22e8e-401">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="22e8e-402">Allgemein</span><span class="sxs-lookup"><span data-stu-id="22e8e-402">General</span></span>
* <span data-ttu-id="22e8e-403">Formatierung von OutputType in Hilfedateien für die meisten Module korrigiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-403">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="22e8e-404">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="22e8e-404">AzureRM.Profile</span></span>
* <span data-ttu-id="22e8e-405">Attribut „Ps1Xml“ wurde den Standardausgabetypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-405">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="22e8e-406">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="22e8e-406">AzureRM.Compute</span></span>
* <span data-ttu-id="22e8e-407">IP-Tag-Funktion für VMSS</span><span class="sxs-lookup"><span data-stu-id="22e8e-407">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="22e8e-408">Cmdlet „New-AzureRmVmssIpTagConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-408">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="22e8e-409">IpTag-Parameter zu „New-AzureRmVmssIpConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-409">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="22e8e-410">Funktion für automatisches Betriebssystemrollback für VMSS</span><span class="sxs-lookup"><span data-stu-id="22e8e-410">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="22e8e-411">DisableAutoRollback-Parameter zu „New-AzureRmVmssConfig“ und „Update-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-411">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="22e8e-412">Funktion für Upgradeverlauf des Betriebssystems für VMSS</span><span class="sxs-lookup"><span data-stu-id="22e8e-412">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="22e8e-413">Switch-Parameter „OSUpgradeHistory“ zu „Get-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-413">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="22e8e-414">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="22e8e-414">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="22e8e-415">Unterstützung für Katalog-ACLs über die folgenden Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="22e8e-415">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="22e8e-416">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="22e8e-416">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="22e8e-417">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="22e8e-417">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="22e8e-418">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="22e8e-418">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="22e8e-419">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="22e8e-419">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="22e8e-420">Abbruchunterstützung und Nachverfolgung des Fortschritts für „Set-AzureRmDataLakeStoreItemAclEntry“, „Remove-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-420">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="22e8e-421">Abbruchunterstützung „Export-AzureRmDataLakeStoreChildItemProperties“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-421">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="22e8e-422">Leerung von Debugmeldungen für Cmdlets korrigiert, die rekursive Vorgänge durchführt</span><span class="sxs-lookup"><span data-stu-id="22e8e-422">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="22e8e-423">Speicherort des Test von DataLake-Cmdlets korrigiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-423">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="22e8e-424">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="22e8e-424">AzureRM.EventHub</span></span>
* <span data-ttu-id="22e8e-425">Optionaler Parameter „MaxCount“ zu Listenvorgangs-Cmdlets „Get-AzureRmEventHub“ und „Get-AzureRmEventHubConsumerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-425">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="22e8e-426">Problem in Cmdlet „New-AzureRmEventHub“ behoben, aufgrund dessen beim Erstellen einer neuen EventHub-Instanz mindestens ein Parameter benötigt wurde.</span><span class="sxs-lookup"><span data-stu-id="22e8e-426">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="22e8e-427">Standardparametersatz wurde bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="22e8e-427">Provided Default Parameter set.</span></span>
* <span data-ttu-id="22e8e-428">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmEventHubKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="22e8e-428">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="22e8e-429">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="22e8e-429">AzureRM.KeyVault</span></span>
* <span data-ttu-id="22e8e-430">Problem behoben, aufgrund dessen von „Get-AzureRmKeyVault -Tag“ alle Ressourcen zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="22e8e-430">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="22e8e-431">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="22e8e-431">AzureRM.Network</span></span>
* <span data-ttu-id="22e8e-432">Neue SKUs für zonenredundante VirtualNetworkGateways-Instanzen verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="22e8e-432">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="22e8e-433">Neue Befehle für Funktion hinzugefügt: ExpressRoute-Partner-APIs über ARM</span><span class="sxs-lookup"><span data-stu-id="22e8e-433">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="22e8e-434">Get-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-434">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="22e8e-435">Set-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-435">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="22e8e-436">Add-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-436">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="22e8e-437">Get-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-437">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="22e8e-438">Remove-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-438">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="22e8e-439">Get-AzureRMExpressRouteCrossConnectionArpTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-439">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="22e8e-440">Get-AzureRMExpressRouteCrossConnectionRouteTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-440">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="22e8e-441">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-441">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="22e8e-442">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="22e8e-442">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="22e8e-443">Cmdlet „Get-AzureRmRecoveryServicesBackupStatus“ wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="22e8e-443">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="22e8e-444">Dieses Cmdlet überprüft anhand der ID eines virtuellen Computers, ob dieser durch einen Tresor im Abonnement geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="22e8e-444">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="22e8e-445">Wenn ein solcher Tresor vorhanden ist, gibt das Cmdlet die Tresordetails aus.</span><span class="sxs-lookup"><span data-stu-id="22e8e-445">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="22e8e-446">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="22e8e-446">AzureRM.Resources</span></span>
* <span data-ttu-id="22e8e-447">Cmdlets vom Typ „Get-AzureRmPolicyAssignment“ aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="22e8e-447">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="22e8e-448">Unterstützung für das Auflisten von „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-448">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="22e8e-449">Unterstützung für das Abrufen einzelner Arbeitsaufträge mit „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-449">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="22e8e-450">Switches „-Effective“ und „-All“ zu Steuerparameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-450">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="22e8e-451">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicyDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-451">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="22e8e-452">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="22e8e-452">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="22e8e-453">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="22e8e-453">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="22e8e-454">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicySetDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-454">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="22e8e-455">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="22e8e-455">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="22e8e-456">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="22e8e-456">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="22e8e-457">Unterstützung für KeyVault-Geheimnisverweis in Parametern hinzugefügt, wenn „TemplateParameterObject“ in „New-AzureRmResourceGroupDeployment“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="22e8e-457">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="22e8e-458">Problem behoben, aufgrund dessen, der Parameter „-EndDate“ für „New-AzureRmADAppCredential“ ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="22e8e-458">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="22e8e-459">Problem behoben, aufgrund dessen „Add-AzureRmADGroupMember“ eine falsche URL für Anforderungen verwendete</span><span class="sxs-lookup"><span data-stu-id="22e8e-459">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="22e8e-460">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="22e8e-460">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="22e8e-461">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmServiceBusKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="22e8e-461">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="22e8e-462">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="22e8e-462">AzureRM.Sql</span></span>
* <span data-ttu-id="22e8e-463">Benutzerdefinierte Wiederherstellungspunkte für SQLDW in Hilfe zu „New-AzureRmSqlDatabaseRestorePoint“ erläutert</span><span class="sxs-lookup"><span data-stu-id="22e8e-463">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="22e8e-464">Dokumentation von Parameter „-ComputeGeneration“ in mehreren Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-464">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="22e8e-465">6.3.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="22e8e-465">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="22e8e-466">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="22e8e-466">AzureRM.Profile</span></span>
* <span data-ttu-id="22e8e-467">Aktualisierte Fehlermeldungen für „Enable-AzureRmContextAutoSave“</span><span class="sxs-lookup"><span data-stu-id="22e8e-467">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="22e8e-468">Erstellen eines Kontexts für jedes Abonnement beim Ausführen von „Connect-AzureRmAccount“ ohne vorherigen Kontext</span><span class="sxs-lookup"><span data-stu-id="22e8e-468">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="22e8e-469">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="22e8e-469">Azure.Storage</span></span>
* <span data-ttu-id="22e8e-470">Zusätzliche Informationen zum Parameter „-Permissions“ in Hilfedateien</span><span class="sxs-lookup"><span data-stu-id="22e8e-470">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="22e8e-471">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="22e8e-471">AzureRM.Compute</span></span>
* <span data-ttu-id="22e8e-472">„Get-AzureRmVmDiskEncryptionStatus“ behebt ein Problem, das bei virtuellen Computern ohne Datenträger festgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="22e8e-472">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="22e8e-473">Version der Computeclientbibliothek aktualisiert, um folgende Cmdlets zu korrigieren:</span><span class="sxs-lookup"><span data-stu-id="22e8e-473">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="22e8e-474">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="22e8e-474">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="22e8e-475">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="22e8e-475">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="22e8e-476">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="22e8e-476">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="22e8e-477">Die folgenden Cmdlets wurden korrigiert, um die Vorgangs-ID und den Vorgangsstatus korrekt anzuzeigen:</span><span class="sxs-lookup"><span data-stu-id="22e8e-477">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="22e8e-478">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="22e8e-478">Start-AzureRmVM</span></span>
    - <span data-ttu-id="22e8e-479">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="22e8e-479">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="22e8e-480">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="22e8e-480">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="22e8e-481">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="22e8e-481">Set-AzureRmVM</span></span>
    - <span data-ttu-id="22e8e-482">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="22e8e-482">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="22e8e-483">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="22e8e-483">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="22e8e-484">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="22e8e-484">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="22e8e-485">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="22e8e-485">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="22e8e-486">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="22e8e-486">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="22e8e-487">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="22e8e-487">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="22e8e-488">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="22e8e-488">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="22e8e-489">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="22e8e-489">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="22e8e-490">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="22e8e-490">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="22e8e-491">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="22e8e-491">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="22e8e-492">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="22e8e-492">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="22e8e-493">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="22e8e-493">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="22e8e-494">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="22e8e-494">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="22e8e-495">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="22e8e-495">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="22e8e-496">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="22e8e-496">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="22e8e-497">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="22e8e-497">AzureRM.EventGrid</span></span>
* <span data-ttu-id="22e8e-498">ValidateNotNullOrEmpty-Überprüfungskonditionen für „SubjectBeginsWith“/„SubjectEndsWith“ im Cmdlet „Update-AzureRmEventGridSubscription“ wurden entfernt, um bei Bedarf die Änderung dieser Parameter in eine leere Zeichenfolge zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="22e8e-498">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="22e8e-499">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="22e8e-499">AzureRM.KeyVault</span></span>
* <span data-ttu-id="22e8e-500">Ein Problem wurde behoben, aufgrund dessen bei Ausführung von „Get-AzureRmKeyVault -Tag“ keine Tags zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="22e8e-500">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="22e8e-501">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="22e8e-501">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="22e8e-502">Offizielle Veröffentlichung von Policy Insights-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="22e8e-502">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="22e8e-503">Verwendung der API-Version 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="22e8e-503">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="22e8e-504">„PolicyDefinitionReferenceId“ zu den Ergebnissen von „Get-AzureRmPolicyStateSummary“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-504">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="22e8e-505">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="22e8e-505">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="22e8e-506">Parameter „-Vault“ zu den RecoveryServices.Backup-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="22e8e-506">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="22e8e-507">Bei der Übergabe wird dadurch das Cmdlet „Set-AzureRmRecoveryServicesContext“ außer Kraft gesetzt.</span><span class="sxs-lookup"><span data-stu-id="22e8e-507">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="22e8e-508">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="22e8e-508">AzureRM.Sql</span></span>
* <span data-ttu-id="22e8e-509">Aktualisiertes Beispiel in der Hilfedatei für „Get-AzureRmSqlDatabaseExpanded“</span><span class="sxs-lookup"><span data-stu-id="22e8e-509">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="22e8e-510">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="22e8e-510">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="22e8e-511">Hilfedatei für „Add-AzureRmTrafficManagerEndpointConfig“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="22e8e-511">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="22e8e-512">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="22e8e-512">AzureRM.Websites</span></span>
* <span data-ttu-id="22e8e-513">„Set-AzureRmWebApp“ wurde aktualisiert, damit „AppSettings“ bei der Verwendung von „-AssignIdentity“ nicht außer Kraft gesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="22e8e-513">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="22e8e-514">„New-AzureRmWebAppSlot“ wurde aktualisiert, um „AppServicePlan“ als optionalen Parameter anzuerkennen</span><span class="sxs-lookup"><span data-stu-id="22e8e-514">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="22e8e-515">6.2.1: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="22e8e-515">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="22e8e-516">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="22e8e-516">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="22e8e-517">PSWorkspace-Modell aktualisiert, damit das Netzwerk „type“ als Parameter verwenden kann</span><span class="sxs-lookup"><span data-stu-id="22e8e-517">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="22e8e-518">6.2.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="22e8e-518">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="22e8e-519">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="22e8e-519">AzureRM.Profile</span></span>
* <span data-ttu-id="22e8e-520">Beheben des Problems, aufgrund dessen Version 10.0.3 von Newtonsoft.Json beim Modulimport nicht geladen wurde</span><span class="sxs-lookup"><span data-stu-id="22e8e-520">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="22e8e-521">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="22e8e-521">AzureRM.Compute</span></span>
* <span data-ttu-id="22e8e-522">Feature zum Aktualisieren von virtuellen VMSS-Computern</span><span class="sxs-lookup"><span data-stu-id="22e8e-522">VMSS VM Update feature</span></span>
    - <span data-ttu-id="22e8e-523">Cmdlets „Update-AzureRmVmssVM“ und „New-AzureRmVMDataDisk“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-523">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="22e8e-524">Fügen Sie den Parameter „VirtualMachineScaleSetVM“ zum Cmdlet „Add-AzureRmVMDataDisk“ hinzu, um das Hinzufügen eines Datenträgers zum virtuellen VMSS-Computer zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="22e8e-524">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="22e8e-525">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="22e8e-525">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="22e8e-526">Aktualisierung der ADF .Net SDK-Version auf 0.8.0-preview mit den folgenden Änderungen:</span><span class="sxs-lookup"><span data-stu-id="22e8e-526">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="22e8e-527">Vorgang zum Konfigurieren des Factoryrepositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-527">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="22e8e-528">Der verknüpfte QuickBooks-Dienst wurde aktualisiert, um die Eigenschaften „consumerKey“ und „consumerSecret“ verfügbar zu machen.</span><span class="sxs-lookup"><span data-stu-id="22e8e-528">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="22e8e-529">Aktualisierung verschiedener Modelltypen von „SecretBase“ auf „Object“</span><span class="sxs-lookup"><span data-stu-id="22e8e-529">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="22e8e-530">Blobereignisauslöser hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-530">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="22e8e-531">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="22e8e-531">AzureRM.KeyVault</span></span>
* <span data-ttu-id="22e8e-532">Aktualisierung der Dokumentation mit Beispielausgabe</span><span class="sxs-lookup"><span data-stu-id="22e8e-532">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="22e8e-533">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="22e8e-533">AzureRM.Network</span></span>
* <span data-ttu-id="22e8e-534">Aktivierung der Traffic Analytics-Parameter für Network Watcher-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="22e8e-534">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="22e8e-535">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="22e8e-535">AzureRM.Resources</span></span>
* <span data-ttu-id="22e8e-536">Behebung des Problems mit der Eigenschaft „Properties“ von PSResource-Objekten, die von „Get-AzureRmResource“ zurückgegeben wurden</span><span class="sxs-lookup"><span data-stu-id="22e8e-536">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="22e8e-537">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="22e8e-537">AzureRM.Scheduler</span></span>
* <span data-ttu-id="22e8e-538">Behebung des Problems, dass beim Aktualisieren von „ServiceBusQueueJob“ keine neuen Authentifizierungswerte festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="22e8e-538">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="22e8e-539">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="22e8e-539">AzureRM.Sql</span></span>
* <span data-ttu-id="22e8e-540">Aktualisierung der folgenden Cmdlets mit dem optionalen LicenseType-Parameter</span><span class="sxs-lookup"><span data-stu-id="22e8e-540">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="22e8e-541">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="22e8e-541">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="22e8e-542">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="22e8e-542">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="22e8e-543">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="22e8e-543">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="22e8e-544">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="22e8e-544">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="22e8e-545">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="22e8e-545">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="22e8e-546">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="22e8e-546">AzureRM.Websites</span></span>
* <span data-ttu-id="22e8e-547">„New-AzureRMWebApp“ aktualisiert, um allgemeine Algorithmen aus der Strategiebibliothek zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="22e8e-547">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="22e8e-548">6.1.0 – Mai 2018</span><span class="sxs-lookup"><span data-stu-id="22e8e-548">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="22e8e-549">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="22e8e-549">AzureRM.Profile</span></span>
* <span data-ttu-id="22e8e-550">Behebung eines Problems, durch das beim Ausführen von „Clear-AzureRmContext“ ein leerer Kontext mit dem Namen des vorherigen Standardkontexts beibehalten wurde und der Benutzer dadurch keinen neuen Kontext mit dem alten Namen erstellen konnte</span><span class="sxs-lookup"><span data-stu-id="22e8e-550">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="22e8e-551">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="22e8e-551">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="22e8e-552">Ermöglichung der Zuordnung von Gateways/Aufhebung der Gatewayzuordnung in AS</span><span class="sxs-lookup"><span data-stu-id="22e8e-552">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="22e8e-553">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="22e8e-553">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="22e8e-554">Unterstützung für „ApiVersions“, „ApiReleases“ und „ApiRevisions“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-554">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="22e8e-555">Unterstützung für ServiceFabric-Back-End hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-555">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="22e8e-556">Unterstützung für Application Insights-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-556">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="22e8e-557">Unterstützung für die Erkennung von SKUs vom Typ „Basic“ als gültige SKU des API Management-Diensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-557">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="22e8e-558">Unterstützung hinzugefügt, damit Zertifikate, die von der privaten Zertifizierungsstelle ausgestellt wurden, als Stamm- oder ZS-Zertifikate installiert werden können</span><span class="sxs-lookup"><span data-stu-id="22e8e-558">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="22e8e-559">Unterstützung für die Akzeptierung benutzerdefinierter SSL-Zertifikate über KeyVault und mehrere Proxyhostnamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-559">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="22e8e-560">Unterstützung für die verwaltete Dienstidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-560">Added support for MSI identity</span></span>
* <span data-ttu-id="22e8e-561">Unterstützung für die Annahme von Richtlinien über URL hinzugefügt; HINWEIS: Folgende Cmdlets werden in einem zukünftigen Release als veraltet gekennzeichnet:</span><span class="sxs-lookup"><span data-stu-id="22e8e-561">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="22e8e-562">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="22e8e-562">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="22e8e-563">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="22e8e-563">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="22e8e-564">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="22e8e-564">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="22e8e-565">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="22e8e-565">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="22e8e-566">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="22e8e-566">AzureRM.Batch</span></span>
* <span data-ttu-id="22e8e-567">Veröffentlichung des neuen Cmdlets „Get-AzureBatchPoolNodeCounts“</span><span class="sxs-lookup"><span data-stu-id="22e8e-567">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="22e8e-568">Veröffentlichung des neuen Cmdlets „Start-AzureBatchComputeNodeServiceLogUpload“</span><span class="sxs-lookup"><span data-stu-id="22e8e-568">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="22e8e-569">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="22e8e-569">AzureRM.Consumption</span></span>
* <span data-ttu-id="22e8e-570">Hinzufügung neuer Parameter („Expand“, „ResourceGroup“, „InstanceName“, „InstanceId“, „Tags“ und „Top“) für das Cmdlet „Get-AzureRmConsumptionUsageDetail“</span><span class="sxs-lookup"><span data-stu-id="22e8e-570">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="22e8e-571">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="22e8e-571">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="22e8e-572">Korrektur des Beispiels für „Export AzureRmDataLakeStoreChildItemProperties“</span><span class="sxs-lookup"><span data-stu-id="22e8e-572">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="22e8e-573">Korrektur der NULL-Parameterausnahme für rekursiven Fall in „Set-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="22e8e-573">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="22e8e-574">Korrektur der Hilfedateien für „Set-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ und „Remove-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="22e8e-574">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="22e8e-575">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="22e8e-575">AzureRM.Network</span></span>
* <span data-ttu-id="22e8e-576">Erhöhung der Network SDK-Version von 18.0.0-preview auf 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="22e8e-576">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="22e8e-577">Cmdlet zum Erstellen der Protokollkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-577">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="22e8e-578">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="22e8e-578">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="22e8e-579">Cmdlet zum Hinzufügen einer neuen Leitungsverbindung zu einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-579">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="22e8e-580">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="22e8e-580">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="22e8e-581">Cmdlet zum Entfernen einer Leitungsverbindung aus einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-581">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="22e8e-582">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="22e8e-582">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="22e8e-583">Cmdlet zum Abrufen einer Leitungsverbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="22e8e-583">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="22e8e-584">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="22e8e-584">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="22e8e-585">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="22e8e-585">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="22e8e-586">Verwendung der Serverauthentifizierung mit generierten Zertifikaten korrigiert (Problemnr. 5998)</span><span class="sxs-lookup"><span data-stu-id="22e8e-586">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="22e8e-587">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="22e8e-587">AzureRM.Sql</span></span>
* <span data-ttu-id="22e8e-588">Überwachungscmdlets korrigiert, um das Entfernen von „AuditActions“ oder „AuditActionGroups“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="22e8e-588">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="22e8e-589">Problem mit „Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy“ behoben, das beim Festlegen einer neuen flexiblen Aufbewahrungsrichtlinie zu folgendem Fehler führte: „Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span><span class="sxs-lookup"><span data-stu-id="22e8e-589">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="22e8e-590">Please submit request with the new flexible retention policy“ (Das Konfigurieren einer langfristigen Aufbewahrungsrichtlinie mit Azure Recovery Service-Tresor und -Richtlinie wird nicht mehr unterstützt. Übermitteln Sie eine Anforderung mit der neuen flexiblen Aufbewahrungsrichtlinie.)</span><span class="sxs-lookup"><span data-stu-id="22e8e-590">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="22e8e-591">Aktualisierung aller Cmdlets für Azure SQL-Datenbank, für die Erstellung von Pools für elastische Datenbanken und für die Aktualisierung, sodass sie die neue Datenbank-API verwenden. Diese unterstützt die Sku-Eigenschaft für skalierungs- und tarifbezogene Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="22e8e-591">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="22e8e-592">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="22e8e-592">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="22e8e-593">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="22e8e-593">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="22e8e-594">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="22e8e-594">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="22e8e-595">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="22e8e-595">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="22e8e-596">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="22e8e-596">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="22e8e-597">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="22e8e-597">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="22e8e-598">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="22e8e-598">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="22e8e-599">Aktualisierung der Parameter für „Get-AzureRmTrafficManagerProfile“, sodass bei Verwendung des Parameters „-Name“ der Parameter „-ResourceGroupName“ erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="22e8e-599">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
