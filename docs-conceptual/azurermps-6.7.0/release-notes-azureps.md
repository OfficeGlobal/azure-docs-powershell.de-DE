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
ms.openlocfilehash: 2a6e20137f12ae9317c7eeed330a2433774e1ea9
ms.sourcegitcommit: 7df99dc139e93a8a4e6d5b1a27968857588d75dd
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/16/2018
ms.locfileid: "40106757"
---
# <a name="release-notes"></a><span data-ttu-id="04ad9-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="04ad9-103">Release notes</span></span>

<span data-ttu-id="04ad9-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="04ad9-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="670---august-2018"></a><span data-ttu-id="04ad9-105">6.7.0: August 2018</span><span class="sxs-lookup"><span data-stu-id="04ad9-105">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="04ad9-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="04ad9-106">AzureRM.Profile</span></span>
* <span data-ttu-id="04ad9-107">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-107">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="04ad9-108">Benutzer-ID zum Standardkontextnamen hinzugefügt, um Kontextkonflikte zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="04ad9-108">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="04ad9-109">Probleme mit „Clear-AzureRmContext“ behoben, die Fehler beim Auswählen eines Kontexts verursacht haben (6398)</span><span class="sxs-lookup"><span data-stu-id="04ad9-109">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="04ad9-110">Ermöglicht, dass für „Connect-AzureRmAccount“ die Mandantendomäne an den Parameter „-TenantId“ übergeben wird</span><span class="sxs-lookup"><span data-stu-id="04ad9-110">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="04ad9-111">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="04ad9-111">Azure.Storage</span></span>
* <span data-ttu-id="04ad9-112">Begrenzung von 5 TB für das Kontingent der Azure-Dateifreigabe entfernt</span><span class="sxs-lookup"><span data-stu-id="04ad9-112">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="04ad9-113">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="04ad9-113">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="04ad9-114">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="04ad9-114">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="04ad9-115">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-115">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="04ad9-116">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="04ad9-116">Azure.AnalysisServices</span></span>
* <span data-ttu-id="04ad9-117">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-117">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="04ad9-118">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="04ad9-118">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="04ad9-119">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-119">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="04ad9-120">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="04ad9-120">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="04ad9-121">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-121">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="04ad9-122">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="04ad9-122">AzureRM.Automation</span></span>
* <span data-ttu-id="04ad9-123">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-123">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="04ad9-124">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="04ad9-124">AzureRM.Backup</span></span>
* <span data-ttu-id="04ad9-125">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-125">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="04ad9-126">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="04ad9-126">AzureRM.Batch</span></span>
* <span data-ttu-id="04ad9-127">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-127">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="04ad9-128">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="04ad9-128">AzureRM.Billing</span></span>
* <span data-ttu-id="04ad9-129">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-129">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="04ad9-130">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="04ad9-130">AzureRM.Cdn</span></span>
* <span data-ttu-id="04ad9-131">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-131">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="04ad9-132">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="04ad9-132">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="04ad9-133">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-133">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="04ad9-134">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="04ad9-134">AzureRM.Compute</span></span>
* <span data-ttu-id="04ad9-135">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-135">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="04ad9-136">EvictionPolicy-Parameter zu „New-AzureRmVmssConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-136">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="04ad9-137">Standort in „DiskFileParameterSet“ von „New-AzureRmVm“ angeben, wenn kein Ort angegeben ist</span><span class="sxs-lookup"><span data-stu-id="04ad9-137">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="04ad9-138">Parameterbeschreibung in „Save-AzureRmVMImage“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-138">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="04ad9-139">Cmdlet „Get-AzureRmVMDiskEncryptionStatus“ für bestimmte Szenarien im Zusammenhang mit einem Durchlauf korrigiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-139">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="04ad9-140">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="04ad9-140">AzureRM.Consumption</span></span>
* <span data-ttu-id="04ad9-141">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-141">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="04ad9-142">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="04ad9-142">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="04ad9-143">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-143">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="04ad9-144">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="04ad9-144">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="04ad9-145">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-145">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="04ad9-146">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="04ad9-146">AzureRM.DataFactories</span></span>
* <span data-ttu-id="04ad9-147">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-147">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="04ad9-148">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="04ad9-148">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="04ad9-149">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-149">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="04ad9-150">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="04ad9-150">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="04ad9-151">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-151">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="04ad9-152">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="04ad9-152">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="04ad9-153">Debuggen korrigiert, wenn „DebugPreference“ über die PowerShell-Befehlszeile festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="04ad9-153">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="04ad9-154">Beispiel für „Set-AzureRmDataLakeStoreItemAcl“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-154">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="04ad9-155">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-155">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="04ad9-156">Beispiel für „Set-AzureRmDataLakeStoreItemAclEntry“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-156">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="04ad9-157">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="04ad9-157">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="04ad9-158">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-158">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="04ad9-159">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="04ad9-159">AzureRM.Dns</span></span>
* <span data-ttu-id="04ad9-160">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-160">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="04ad9-161">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="04ad9-161">AzureRM.EventGrid</span></span>
* <span data-ttu-id="04ad9-162">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-162">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="04ad9-163">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="04ad9-163">AzureRM.EventHub</span></span>
* <span data-ttu-id="04ad9-164">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-164">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="04ad9-165">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="04ad9-165">AzureRM.HDInsight</span></span>
* <span data-ttu-id="04ad9-166">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-166">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="04ad9-167">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="04ad9-167">AzureRM.Insights</span></span>
* <span data-ttu-id="04ad9-168">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-168">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="04ad9-169">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="04ad9-169">AzureRM.IotHub</span></span>
* <span data-ttu-id="04ad9-170">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-170">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="04ad9-171">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="04ad9-171">AzureRM.KeyVault</span></span>
* <span data-ttu-id="04ad9-172">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-172">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="04ad9-173">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="04ad9-173">AzureRM.LogicApp</span></span>
* <span data-ttu-id="04ad9-174">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-174">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="04ad9-175">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="04ad9-175">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="04ad9-176">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-176">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="04ad9-177">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="04ad9-177">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="04ad9-178">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-178">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="04ad9-179">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="04ad9-179">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="04ad9-180">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-180">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="04ad9-181">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="04ad9-181">AzureRM.Media</span></span>
* <span data-ttu-id="04ad9-182">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-182">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="04ad9-183">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="04ad9-183">AzureRM.Network</span></span>
* <span data-ttu-id="04ad9-184">Beispiel für „Set-AzureRmLocalNetworkGateway“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-184">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="04ad9-185">Beispiele und Beschreibungen für „Add-AzureRmVirtualNetworkGatewayIpConfig“, „Get-AzureRmVirtualNetworkGatewayConnectionSharedKey“ und „New-AzureRmVirtualNetworkGatewayConnection“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-185">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="04ad9-186">Beispiele für „Remove-AzureRmVirtualNetworkGatewayIpConfig“ und „Reset-AzureRmVirtualNetworkGateway“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-186">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="04ad9-187">Beispiel für „Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-187">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="04ad9-188">Beispiel für „Set-AzureRmVirtualNetworkGatewayConnectionSharedKey“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-188">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="04ad9-189">Beispiel für „Set-AzureRmVirtualNetworkGatewayConnection“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-189">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="04ad9-190">Cmdlets für „ApplicationSecurityGroup“, „RouteTable“ und „Usage“ mithilfe des aktuellen Code-Generators erneut erstellt</span><span class="sxs-lookup"><span data-stu-id="04ad9-190">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="04ad9-191">Deutlichere Formulierung der Fehlermeldung für „Get-AzureRmVirtualNetworkSubnetConfig“, wenn ein nicht vorhandenes Subnetz abgerufen wird</span><span class="sxs-lookup"><span data-stu-id="04ad9-191">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="04ad9-192">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="04ad9-192">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="04ad9-193">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-193">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="04ad9-194">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="04ad9-194">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="04ad9-195">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-195">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="04ad9-196">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="04ad9-196">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="04ad9-197">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-197">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="04ad9-198">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="04ad9-198">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="04ad9-199">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-199">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="04ad9-200">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="04ad9-200">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="04ad9-201">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="04ad9-201">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="04ad9-202">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="04ad9-202">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="04ad9-203">Richtlinienfilter zum Cmdlet „Get-AzureRmRecoveryServicesBackItem“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="04ad9-203">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="04ad9-204">Der Befehl gibt die Liste der Sicherungselemente zurück, die durch die angegebene Richtlinien-ID geschützt sind.</span><span class="sxs-lookup"><span data-stu-id="04ad9-204">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="04ad9-205">„Microsoft.Azure.Management.RecoveryServices.Backup“ auf Version 3.0.0-preview aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-205">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="04ad9-206">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-206">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="04ad9-207">TargetResourceGroupName-Parameter zu „Restore-AzureRmRecoveryServicesBackupItem“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="04ad9-207">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="04ad9-208">Die Ressourcengruppe, in der die verwalteten Datenträger wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="04ad9-208">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="04ad9-209">Gilt für die Sicherung des virtuellen Computers mit verwalteten Datenträgern.</span><span class="sxs-lookup"><span data-stu-id="04ad9-209">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="04ad9-210">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="04ad9-210">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="04ad9-211">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-211">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="04ad9-212">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="04ad9-212">AzureRM.RedisCache</span></span>
* <span data-ttu-id="04ad9-213">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-213">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="04ad9-214">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="04ad9-214">AzureRM.Relay</span></span>
* <span data-ttu-id="04ad9-215">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-215">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="04ad9-216">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="04ad9-216">AzureRM.Resources</span></span>
* <span data-ttu-id="04ad9-217">Unterstützung der Vorlagenbereitstellung im Abonnementbereich.</span><span class="sxs-lookup"><span data-stu-id="04ad9-217">Support template deployment at subscription scope.</span></span> <span data-ttu-id="04ad9-218">Neue Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="04ad9-218">Add new Cmdlets:</span></span>
    - <span data-ttu-id="04ad9-219">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="04ad9-219">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="04ad9-220">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="04ad9-220">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="04ad9-221">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="04ad9-221">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="04ad9-222">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="04ad9-222">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="04ad9-223">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="04ad9-223">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="04ad9-224">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="04ad9-224">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="04ad9-225">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="04ad9-225">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="04ad9-226">Problem behoben, aufgrund dessen beim Übergeben eines Kontexts an „Set-AzureRmResource“ ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="04ad9-226">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="04ad9-227">Beispiel in „New-AzureRmResourceGroupDeployment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-227">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="04ad9-228">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-228">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="04ad9-229">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="04ad9-229">AzureRM.Scheduler</span></span>
* <span data-ttu-id="04ad9-230">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-230">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="04ad9-231">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="04ad9-231">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="04ad9-232">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-232">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="04ad9-233">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="04ad9-233">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="04ad9-234">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-234">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="04ad9-235">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="04ad9-235">AzureRM.Sql</span></span>
* <span data-ttu-id="04ad9-236">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-236">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="04ad9-237">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="04ad9-237">AzureRM.Storage</span></span>
* <span data-ttu-id="04ad9-238">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-238">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="04ad9-239">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="04ad9-239">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="04ad9-240">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-240">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="04ad9-241">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="04ad9-241">AzureRM.Tags</span></span>
* <span data-ttu-id="04ad9-242">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-242">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="04ad9-243">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="04ad9-243">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="04ad9-244">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-244">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="04ad9-245">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="04ad9-245">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="04ad9-246">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-246">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="04ad9-247">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="04ad9-247">AzureRM.Websites</span></span>
* <span data-ttu-id="04ad9-248">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-248">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="04ad9-249">6.6.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="04ad9-249">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="04ad9-250">Allgemein</span><span class="sxs-lookup"><span data-stu-id="04ad9-250">General</span></span>
* <span data-ttu-id="04ad9-251">Alle Hilfedateien aktualisiert, um vollständige Parametertypen und die richtigen Eingabe/Ausgabe-Typen einzuschließen.</span><span class="sxs-lookup"><span data-stu-id="04ad9-251">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="04ad9-252">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="04ad9-252">AzureRM.Profile</span></span>
* <span data-ttu-id="04ad9-253">Bibliothek „Common.Strategy“ aktualisiert, um überprüfen zu können, ob die aktuelle Konfiguration für eine Ressource mit der Zielressource kompatibel ist.</span><span class="sxs-lookup"><span data-stu-id="04ad9-253">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="04ad9-254">ps1xml-Typen zu „Common.Storage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-254">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="04ad9-255">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="04ad9-255">Azure.Storage</span></span>
* <span data-ttu-id="04ad9-256">Unterstützung zum Abrufen von Speicherkontext aus „DefaultProfile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-256">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="04ad9-257">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-257">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="04ad9-258">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="04ad9-258">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="04ad9-259">Problem https://github.com/Azure/azure-powershell/issues/6370 behoben</span><span class="sxs-lookup"><span data-stu-id="04ad9-259">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="04ad9-260">Fehler in Automapper behoben, um „PsApiManagementApi“ in „ApiContract“ zu verschieben</span><span class="sxs-lookup"><span data-stu-id="04ad9-260">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="04ad9-261">Problem https://github.com/Azure/azure-powershell/issues/6515 behoben</span><span class="sxs-lookup"><span data-stu-id="04ad9-261">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="04ad9-262">Fehler in „File.Save“ behoben, um Überladung mit Codierungstyp zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="04ad9-262">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="04ad9-263">Problem https://github.com/Azure/azure-powershell/issues/6560 behoben</span><span class="sxs-lookup"><span data-stu-id="04ad9-263">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="04ad9-264">Upgrade auf Nuget-Version 4.0.3 durchgeführt, in der Musterausnahme in „apiId“ behoben wurde</span><span class="sxs-lookup"><span data-stu-id="04ad9-264">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="04ad9-265">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="04ad9-265">AzureRM.Compute</span></span>
* <span data-ttu-id="04ad9-266">Das Problem, aufgrund dessen beim Erstellen eines virtuellen Computers mithilfe von „DiskFileParameterSet“ in „New-AzureRmVm“ wegen einer Umbenennung des Speicherkontotyps „PremiumLRS“ ein Fehler auftrat, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="04ad9-266">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="04ad9-267">Cmdlet „Invoke-AzureRmVMRunCommand“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-267">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="04ad9-268">„Get-AzureRmAvailabilitySet“ aktualisiert, um die Auflistung aller Verfügbarkeitsgruppen in einem Abonnement zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="04ad9-268">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="04ad9-269">(ResouceGroupName-Parameter ist jetzt optional.)</span><span class="sxs-lookup"><span data-stu-id="04ad9-269">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="04ad9-270">„SimpleParameterSet“ von „New-AzureRmVm“ aktualisiert, um Accelerated Networking auf kompatiblen virtuellen Computern zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="04ad9-270">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="04ad9-271">Einfacher Parametersatz „New-AzureRmVmss“ aktualisiert, sodass das Erstellen der VMSS fehlschlägt, wenn bereits ein benutzerdefinierter LB vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="04ad9-271">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="04ad9-272">Beispiel für „New-AzureRmDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-272">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="04ad9-273">Beispiel für „New-AzureRmVM“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-273">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="04ad9-274">Beschreibung für „Set-AzureRmVMOSDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-274">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="04ad9-275">Beispiel 1 für „Set-AzureRmVMBginfoExtension“ aktualisiert, um Rechtschreibung und Präfix zu korrigieren.</span><span class="sxs-lookup"><span data-stu-id="04ad9-275">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="04ad9-276">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="04ad9-276">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="04ad9-277">ADF .Net SDK-Version auf 1.1.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="04ad9-277">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="04ad9-278">Unterstützung der Freigabe der selbstgehosteten Integration Runtime über Data Factorys hinweg.</span><span class="sxs-lookup"><span data-stu-id="04ad9-278">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="04ad9-279">Neuer Parameter „-SharedIntegrationRuntimeResourceId“ zu Cmdlet „Set-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="04ad9-279">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="04ad9-280">Neuer optionaler Parameter „-LinkedDataFactoryName“ zu Cmdlet „Remove-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="04ad9-280">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="04ad9-281">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="04ad9-281">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="04ad9-282">DataPlane SDK-Version (Microsoft.Azure.DataLake.Store) auf 1.1.9 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-282">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="04ad9-283">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="04ad9-283">AzureRM.EventHub</span></span>
* <span data-ttu-id="04ad9-284">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-284">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="04ad9-285">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="04ad9-285">AzureRM.Insights</span></span>
* <span data-ttu-id="04ad9-286">Formatierung von „OutputType“ in Hilfedateien korrigiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-286">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="04ad9-287">Verwendung von Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span><span class="sxs-lookup"><span data-stu-id="04ad9-287">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="04ad9-288">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="04ad9-288">AzureRM.KeyVault</span></span>
* <span data-ttu-id="04ad9-289">Piping-Problem in „Set-AzureRmKeyVaultAccessPolicy“ behoben</span><span class="sxs-lookup"><span data-stu-id="04ad9-289">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="04ad9-290">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="04ad9-290">AzureRM.Network</span></span>
* <span data-ttu-id="04ad9-291">Beispiele für LoadBalancerInboundNatPoolConfig-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="04ad9-291">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="04ad9-292">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="04ad9-292">AzureRM.Resources</span></span>
* <span data-ttu-id="04ad9-293">Problem beim Angeben sowohl des Tag-Namens als auch des Werts für „Get-AzureRmResource“ behoben</span><span class="sxs-lookup"><span data-stu-id="04ad9-293">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="04ad9-294">Piping-Szenario mit „Set-AzureRmResource“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-294">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="04ad9-295">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="04ad9-295">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="04ad9-296">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-296">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="04ad9-297">Einige Probleme behoben</span><span class="sxs-lookup"><span data-stu-id="04ad9-297">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="04ad9-298">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="04ad9-298">AzureRM.Sql</span></span>
* <span data-ttu-id="04ad9-299">Unterstützung für Advanced Threat Protection für Server bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="04ad9-299">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="04ad9-300">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="04ad9-300">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="04ad9-301">Unterstützung für Sicherheitsrisikobewertung bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="04ad9-301">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="04ad9-302">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="04ad9-302">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="04ad9-303">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="04ad9-303">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="04ad9-304">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="04ad9-304">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="04ad9-305">Beispiel in „Remove-AzureRmSqlServerFirewallRule“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-305">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="04ad9-306">Falsche Verarbeitung von „datetime“ für nicht US-basierte Kultur in „Get-AzureSqlSyncGroupLog“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-306">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="04ad9-307">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="04ad9-307">AzureRM.Storage</span></span>
* <span data-ttu-id="04ad9-308">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-308">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="04ad9-309">Cmdlet-Ausgabe von „StorageAccount“ in Tabellenansicht anzeigen</span><span class="sxs-lookup"><span data-stu-id="04ad9-309">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="04ad9-310">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="04ad9-310">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="04ad9-311">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="04ad9-311">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="04ad9-312">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="04ad9-312">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="04ad9-313">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="04ad9-313">AzureRM.Tags</span></span>
* <span data-ttu-id="04ad9-314">Falsche Anweisung aus Tag-Cmdlet-Hilfe entfernt</span><span class="sxs-lookup"><span data-stu-id="04ad9-314">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="04ad9-315">6.5.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="04ad9-315">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="04ad9-316">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="04ad9-316">AzureRM.Profile</span></span>
* <span data-ttu-id="04ad9-317">Hilfe für „Get-AzureRmContextAutosaveSetting“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-317">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="04ad9-318">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="04ad9-318">Azure.Storage</span></span>
* <span data-ttu-id="04ad9-319">Unterstützung des Blob- oder Dateiuploads mit lesegeschütztem SAS-Token</span><span class="sxs-lookup"><span data-stu-id="04ad9-319">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="04ad9-320">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="04ad9-320">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="04ad9-321">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="04ad9-321">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="04ad9-322">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="04ad9-322">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="04ad9-323">Erforderliche Eigenschaft „ResourceGroupName“ zu AS hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="04ad9-323">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="04ad9-324">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="04ad9-324">AzureRM.Automation</span></span>
* <span data-ttu-id="04ad9-325">Hilfe aktualisiert und Beispiel für „New-AzureRMAutomationSchedule“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-325">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="04ad9-326">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="04ad9-326">AzureRM.Compute</span></span>
* <span data-ttu-id="04ad9-327">Parameter „-Tag“ zu „Update/New-AzureRmAvailabilitySet“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-327">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="04ad9-328">Beispiel für „Add-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-328">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="04ad9-329">Beispiele für „Remove-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-329">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="04ad9-330">Hilfe für „Set-AzureRmVMAccessExtension“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-330">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="04ad9-331">„SimpleParameterSet“ für „New-AzureRmVmss“ so aktualisiert, dass „SinglePlacementGroup“ standardmäßig auf „false“ festgelegt ist, und Switch-Parameter „SinglePlacementGroup“ hinzugefügt, der dem Benutzer das Erstellen der VMSS in einer einzelnen Platzierungsgruppe ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="04ad9-331">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="04ad9-332">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="04ad9-332">AzureRM.EventHub</span></span>
* <span data-ttu-id="04ad9-333">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSEventHubDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="04ad9-333">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="04ad9-334">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="04ad9-334">AzureRM.KeyVault</span></span>
* <span data-ttu-id="04ad9-335">Fehlermeldung für „Set-AzureRmKeyVaultAccessPolicy“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-335">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="04ad9-336">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="04ad9-336">AzureRM.LogicApp</span></span>
* <span data-ttu-id="04ad9-337">Fehler „Parametersatz konnte nicht aufgelöst werden“ in „New-AzureRmLogicApp“behoben</span><span class="sxs-lookup"><span data-stu-id="04ad9-337">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="04ad9-338">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="04ad9-338">AzureRM.Network</span></span>
* <span data-ttu-id="04ad9-339">Peering über mehrere virtuelle Netzwerke in mehreren Mandanten für „Set/Add-AzureRmVirtualNetworkPeering“ aktiviert</span><span class="sxs-lookup"><span data-stu-id="04ad9-339">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="04ad9-340">Folgende Cmdlets für Application Gateway aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-340">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="04ad9-341">New-AzureRmApplicationGateway: EnableFIPS-Flag und Zonenunterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-341">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="04ad9-342">New-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-342">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="04ad9-343">Set-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-343">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="04ad9-344">RouteTable-Cmdlets mit aktueller Generatorversion erneut generiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-344">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="04ad9-345">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="04ad9-345">AzureRM.Relay</span></span>
* <span data-ttu-id="04ad9-346">Markdowndateien aktualisiert, Problem mit Parametername in Beispiel behoben</span><span class="sxs-lookup"><span data-stu-id="04ad9-346">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="04ad9-347">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="04ad9-347">AzureRM.Resources</span></span>
* <span data-ttu-id="04ad9-348">Roleassignment- und roledefinition-Cmdlets aktualisiert:</span><span class="sxs-lookup"><span data-stu-id="04ad9-348">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="04ad9-349">Zusätzliche roledefinition-Aufrufe entfernt, die als Teil des Pagings durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="04ad9-349">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="04ad9-350">Get-AzureRmRoleAssignment-Cmdlet korrigiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-350">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="04ad9-351">Befehlsparameterfunktion von „-ExpandPrincipalGroups“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-351">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="04ad9-352">Problem mit „Get-AzureRmResource“ behoben, aufgrund dessen die Groß-/Kleinschreibung des Parameters „-ResourceType“ beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="04ad9-352">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="04ad9-353">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="04ad9-353">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="04ad9-354">top- und skip-Parameter zu Listen-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-354">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="04ad9-355">Cmdlets für die Migration von Standard- zu Premium-Namespace hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="04ad9-355">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="04ad9-356">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="04ad9-356">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="04ad9-357">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="04ad9-357">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="04ad9-358">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="04ad9-358">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="04ad9-359">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="04ad9-359">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="04ad9-360">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="04ad9-360">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="04ad9-361">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSServiceBusDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="04ad9-361">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="04ad9-362">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="04ad9-362">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="04ad9-363">Beispiel für „New-AzureRmServiceFabricCluster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-363">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="04ad9-364">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="04ad9-364">AzureRM.Sql</span></span>
* <span data-ttu-id="04ad9-365">Neue Cmdlets für „Management.Sql“ hinzugefügt, um Kunden das Hinzufügen des TDE-Zertifikats zu einer SQL Server-Instanz oder einer verwalteten Instanz zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="04ad9-365">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="04ad9-366">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="04ad9-366">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="04ad9-367">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="04ad9-367">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="04ad9-368">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="04ad9-368">AzureRM.Websites</span></span>
* <span data-ttu-id="04ad9-369">Wenn `Set-AzureRmWebApp -AssignIdentity` und `Set-AzureRmWebAppSlot -AssignIdentity` auf „false“ festgelegt sind, wird jetzt die Identity-Eigenschaft aus dem Websiteobjekt entfernt. Auch das Vorschau-Tag wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="04ad9-369">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="04ad9-370">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics`-Beispiel aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-370">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="04ad9-371">Unterstützung von `Set-AzureRmWebApp -PhpVersion` als gültige PHP-Version eingestellt</span><span class="sxs-lookup"><span data-stu-id="04ad9-371">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="04ad9-372">6.4.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="04ad9-372">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="04ad9-373">Allgemein</span><span class="sxs-lookup"><span data-stu-id="04ad9-373">General</span></span>
* <span data-ttu-id="04ad9-374">Formatierung von OutputType in Hilfedateien für die meisten Module korrigiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-374">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="04ad9-375">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="04ad9-375">AzureRM.Profile</span></span>
* <span data-ttu-id="04ad9-376">Attribut „Ps1Xml“ wurde den Standardausgabetypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-376">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="04ad9-377">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="04ad9-377">AzureRM.Compute</span></span>
* <span data-ttu-id="04ad9-378">IP-Tag-Funktion für VMSS</span><span class="sxs-lookup"><span data-stu-id="04ad9-378">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="04ad9-379">Cmdlet „New-AzureRmVmssIpTagConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-379">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="04ad9-380">IpTag-Parameter zu „New-AzureRmVmssIpConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-380">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="04ad9-381">Funktion für automatisches Betriebssystemrollback für VMSS</span><span class="sxs-lookup"><span data-stu-id="04ad9-381">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="04ad9-382">DisableAutoRollback-Parameter zu „New-AzureRmVmssConfig“ und „Update-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-382">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="04ad9-383">Funktion für Upgradeverlauf des Betriebssystems für VMSS</span><span class="sxs-lookup"><span data-stu-id="04ad9-383">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="04ad9-384">Switch-Parameter „OSUpgradeHistory“ zu „Get-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-384">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="04ad9-385">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="04ad9-385">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="04ad9-386">Unterstützung für Katalog-ACLs über die folgenden Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="04ad9-386">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="04ad9-387">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="04ad9-387">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="04ad9-388">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="04ad9-388">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="04ad9-389">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="04ad9-389">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="04ad9-390">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="04ad9-390">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="04ad9-391">Abbruchunterstützung und Nachverfolgung des Fortschritts für „Set-AzureRmDataLakeStoreItemAclEntry“, „Remove-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-391">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="04ad9-392">Abbruchunterstützung „Export-AzureRmDataLakeStoreChildItemProperties“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-392">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="04ad9-393">Leerung von Debugmeldungen für Cmdlets korrigiert, die rekursive Vorgänge durchführt</span><span class="sxs-lookup"><span data-stu-id="04ad9-393">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="04ad9-394">Speicherort des Test von DataLake-Cmdlets korrigiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-394">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="04ad9-395">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="04ad9-395">AzureRM.EventHub</span></span>
* <span data-ttu-id="04ad9-396">Optionaler Parameter „MaxCount“ zu Listenvorgangs-Cmdlets „Get-AzureRmEventHub“ und „Get-AzureRmEventHubConsumerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-396">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="04ad9-397">Problem in Cmdlet „New-AzureRmEventHub“ behoben, aufgrund dessen beim Erstellen einer neuen EventHub-Instanz mindestens ein Parameter benötigt wurde.</span><span class="sxs-lookup"><span data-stu-id="04ad9-397">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="04ad9-398">Standardparametersatz wurde bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="04ad9-398">Provided Default Parameter set.</span></span>
* <span data-ttu-id="04ad9-399">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmEventHubKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="04ad9-399">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="04ad9-400">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="04ad9-400">AzureRM.KeyVault</span></span>
* <span data-ttu-id="04ad9-401">Problem behoben, aufgrund dessen von „Get-AzureRmKeyVault -Tag“ alle Ressourcen zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="04ad9-401">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="04ad9-402">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="04ad9-402">AzureRM.Network</span></span>
* <span data-ttu-id="04ad9-403">Neue SKUs für zonenredundante VirtualNetworkGateways-Instanzen verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="04ad9-403">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="04ad9-404">Neue Befehle für Funktion hinzugefügt: ExpressRoute-Partner-APIs über ARM</span><span class="sxs-lookup"><span data-stu-id="04ad9-404">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="04ad9-405">Get-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-405">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="04ad9-406">Set-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-406">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="04ad9-407">Add-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-407">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="04ad9-408">Get-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-408">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="04ad9-409">Remove-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-409">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="04ad9-410">Get-AzureRMExpressRouteCrossConnectionArpTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-410">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="04ad9-411">Get-AzureRMExpressRouteCrossConnectionRouteTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-411">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="04ad9-412">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-412">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="04ad9-413">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="04ad9-413">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="04ad9-414">Cmdlet „Get-AzureRmRecoveryServicesBackupStatus“ wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="04ad9-414">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="04ad9-415">Dieses Cmdlet überprüft anhand der ID eines virtuellen Computers, ob dieser durch einen Tresor im Abonnement geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="04ad9-415">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="04ad9-416">Wenn ein solcher Tresor vorhanden ist, gibt das Cmdlet die Tresordetails aus.</span><span class="sxs-lookup"><span data-stu-id="04ad9-416">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="04ad9-417">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="04ad9-417">AzureRM.Resources</span></span>
* <span data-ttu-id="04ad9-418">Cmdlets vom Typ „Get-AzureRmPolicyAssignment“ aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="04ad9-418">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="04ad9-419">Unterstützung für das Auflisten von „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-419">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="04ad9-420">Unterstützung für das Abrufen einzelner Arbeitsaufträge mit „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-420">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="04ad9-421">Switches „-Effective“ und „-All“ zu Steuerparameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-421">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="04ad9-422">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicyDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-422">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="04ad9-423">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="04ad9-423">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="04ad9-424">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="04ad9-424">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="04ad9-425">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicySetDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-425">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="04ad9-426">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="04ad9-426">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="04ad9-427">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="04ad9-427">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="04ad9-428">Unterstützung für KeyVault-Geheimnisverweis in Parametern hinzugefügt, wenn „TemplateParameterObject“ in „New-AzureRmResourceGroupDeployment“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="04ad9-428">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="04ad9-429">Problem behoben, aufgrund dessen, der Parameter „-EndDate“ für „New-AzureRmADAppCredential“ ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="04ad9-429">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="04ad9-430">Problem behoben, aufgrund dessen „Add-AzureRmADGroupMember“ eine falsche URL für Anforderungen verwendete</span><span class="sxs-lookup"><span data-stu-id="04ad9-430">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="04ad9-431">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="04ad9-431">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="04ad9-432">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmServiceBusKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="04ad9-432">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="04ad9-433">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="04ad9-433">AzureRM.Sql</span></span>
* <span data-ttu-id="04ad9-434">Benutzerdefinierte Wiederherstellungspunkte für SQLDW in Hilfe zu „New-AzureRmSqlDatabaseRestorePoint“ erläutert</span><span class="sxs-lookup"><span data-stu-id="04ad9-434">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="04ad9-435">Dokumentation von Parameter „-ComputeGeneration“ in mehreren Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-435">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="04ad9-436">6.3.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="04ad9-436">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="04ad9-437">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="04ad9-437">AzureRM.Profile</span></span>
* <span data-ttu-id="04ad9-438">Aktualisierte Fehlermeldungen für „Enable-AzureRmContextAutoSave“</span><span class="sxs-lookup"><span data-stu-id="04ad9-438">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="04ad9-439">Erstellen eines Kontexts für jedes Abonnement beim Ausführen von „Connect-AzureRmAccount“ ohne vorherigen Kontext</span><span class="sxs-lookup"><span data-stu-id="04ad9-439">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="04ad9-440">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="04ad9-440">Azure.Storage</span></span>
* <span data-ttu-id="04ad9-441">Zusätzliche Informationen zum Parameter „-Permissions“ in Hilfedateien</span><span class="sxs-lookup"><span data-stu-id="04ad9-441">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="04ad9-442">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="04ad9-442">AzureRM.Compute</span></span>
* <span data-ttu-id="04ad9-443">„Get-AzureRmVmDiskEncryptionStatus“ behebt ein Problem, das bei virtuellen Computern ohne Datenträger festgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="04ad9-443">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="04ad9-444">Version der Computeclientbibliothek aktualisiert, um folgende Cmdlets zu korrigieren:</span><span class="sxs-lookup"><span data-stu-id="04ad9-444">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="04ad9-445">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="04ad9-445">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="04ad9-446">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="04ad9-446">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="04ad9-447">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="04ad9-447">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="04ad9-448">Die folgenden Cmdlets wurden korrigiert, um die Vorgangs-ID und den Vorgangsstatus korrekt anzuzeigen:</span><span class="sxs-lookup"><span data-stu-id="04ad9-448">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="04ad9-449">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="04ad9-449">Start-AzureRmVM</span></span>
    - <span data-ttu-id="04ad9-450">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="04ad9-450">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="04ad9-451">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="04ad9-451">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="04ad9-452">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="04ad9-452">Set-AzureRmVM</span></span>
    - <span data-ttu-id="04ad9-453">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="04ad9-453">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="04ad9-454">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="04ad9-454">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="04ad9-455">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="04ad9-455">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="04ad9-456">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="04ad9-456">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="04ad9-457">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="04ad9-457">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="04ad9-458">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="04ad9-458">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="04ad9-459">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="04ad9-459">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="04ad9-460">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="04ad9-460">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="04ad9-461">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="04ad9-461">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="04ad9-462">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="04ad9-462">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="04ad9-463">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="04ad9-463">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="04ad9-464">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="04ad9-464">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="04ad9-465">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="04ad9-465">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="04ad9-466">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="04ad9-466">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="04ad9-467">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="04ad9-467">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="04ad9-468">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="04ad9-468">AzureRM.EventGrid</span></span>
* <span data-ttu-id="04ad9-469">ValidateNotNullOrEmpty-Überprüfungskonditionen für „SubjectBeginsWith“/„SubjectEndsWith“ im Cmdlet „Update-AzureRmEventGridSubscription“ wurden entfernt, um bei Bedarf die Änderung dieser Parameter in eine leere Zeichenfolge zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="04ad9-469">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="04ad9-470">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="04ad9-470">AzureRM.KeyVault</span></span>
* <span data-ttu-id="04ad9-471">Ein Problem wurde behoben, aufgrund dessen bei Ausführung von „Get-AzureRmKeyVault -Tag“ keine Tags zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="04ad9-471">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="04ad9-472">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="04ad9-472">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="04ad9-473">Offizielle Veröffentlichung von Policy Insights-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="04ad9-473">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="04ad9-474">Verwendung der API-Version 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="04ad9-474">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="04ad9-475">„PolicyDefinitionReferenceId“ zu den Ergebnissen von „Get-AzureRmPolicyStateSummary“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-475">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="04ad9-476">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="04ad9-476">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="04ad9-477">Parameter „-Vault“ zu den RecoveryServices.Backup-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="04ad9-477">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="04ad9-478">Bei der Übergabe wird dadurch das Cmdlet „Set-AzureRmRecoveryServicesContext“ außer Kraft gesetzt.</span><span class="sxs-lookup"><span data-stu-id="04ad9-478">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="04ad9-479">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="04ad9-479">AzureRM.Sql</span></span>
* <span data-ttu-id="04ad9-480">Aktualisiertes Beispiel in der Hilfedatei für „Get-AzureRmSqlDatabaseExpanded“</span><span class="sxs-lookup"><span data-stu-id="04ad9-480">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="04ad9-481">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="04ad9-481">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="04ad9-482">Hilfedatei für „Add-AzureRmTrafficManagerEndpointConfig“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="04ad9-482">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="04ad9-483">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="04ad9-483">AzureRM.Websites</span></span>
* <span data-ttu-id="04ad9-484">„Set-AzureRmWebApp“ wurde aktualisiert, damit „AppSettings“ bei der Verwendung von „-AssignIdentity“ nicht außer Kraft gesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="04ad9-484">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="04ad9-485">„New-AzureRmWebAppSlot“ wurde aktualisiert, um „AppServicePlan“ als optionalen Parameter anzuerkennen</span><span class="sxs-lookup"><span data-stu-id="04ad9-485">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="04ad9-486">6.2.1: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="04ad9-486">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="04ad9-487">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="04ad9-487">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="04ad9-488">PSWorkspace-Modell aktualisiert, damit das Netzwerk „type“ als Parameter verwenden kann</span><span class="sxs-lookup"><span data-stu-id="04ad9-488">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="04ad9-489">6.2.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="04ad9-489">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="04ad9-490">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="04ad9-490">AzureRM.Profile</span></span>
* <span data-ttu-id="04ad9-491">Beheben des Problems, aufgrund dessen Version 10.0.3 von Newtonsoft.Json beim Modulimport nicht geladen wurde</span><span class="sxs-lookup"><span data-stu-id="04ad9-491">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="04ad9-492">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="04ad9-492">AzureRM.Compute</span></span>
* <span data-ttu-id="04ad9-493">Feature zum Aktualisieren von virtuellen VMSS-Computern</span><span class="sxs-lookup"><span data-stu-id="04ad9-493">VMSS VM Update feature</span></span>
    - <span data-ttu-id="04ad9-494">Cmdlets „Update-AzureRmVmssVM“ und „New-AzureRmVMDataDisk“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-494">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="04ad9-495">Fügen Sie den Parameter „VirtualMachineScaleSetVM“ zum Cmdlet „Add-AzureRmVMDataDisk“ hinzu, um das Hinzufügen eines Datenträgers zum virtuellen VMSS-Computer zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="04ad9-495">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="04ad9-496">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="04ad9-496">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="04ad9-497">Aktualisierung der ADF .Net SDK-Version auf 0.8.0-preview mit den folgenden Änderungen:</span><span class="sxs-lookup"><span data-stu-id="04ad9-497">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="04ad9-498">Vorgang zum Konfigurieren des Factoryrepositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-498">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="04ad9-499">Der verknüpfte QuickBooks-Dienst wurde aktualisiert, um die Eigenschaften „consumerKey“ und „consumerSecret“ verfügbar zu machen.</span><span class="sxs-lookup"><span data-stu-id="04ad9-499">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="04ad9-500">Aktualisierung verschiedener Modelltypen von „SecretBase“ auf „Object“</span><span class="sxs-lookup"><span data-stu-id="04ad9-500">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="04ad9-501">Blobereignisauslöser hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-501">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="04ad9-502">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="04ad9-502">AzureRM.KeyVault</span></span>
* <span data-ttu-id="04ad9-503">Aktualisierung der Dokumentation mit Beispielausgabe</span><span class="sxs-lookup"><span data-stu-id="04ad9-503">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="04ad9-504">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="04ad9-504">AzureRM.Network</span></span>
* <span data-ttu-id="04ad9-505">Aktivierung der Traffic Analytics-Parameter für Network Watcher-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="04ad9-505">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="04ad9-506">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="04ad9-506">AzureRM.Resources</span></span>
* <span data-ttu-id="04ad9-507">Behebung des Problems mit der Eigenschaft „Properties“ von PSResource-Objekten, die von „Get-AzureRmResource“ zurückgegeben wurden</span><span class="sxs-lookup"><span data-stu-id="04ad9-507">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="04ad9-508">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="04ad9-508">AzureRM.Scheduler</span></span>
* <span data-ttu-id="04ad9-509">Behebung des Problems, dass beim Aktualisieren von „ServiceBusQueueJob“ keine neuen Authentifizierungswerte festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="04ad9-509">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="04ad9-510">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="04ad9-510">AzureRM.Sql</span></span>
* <span data-ttu-id="04ad9-511">Aktualisierung der folgenden Cmdlets mit dem optionalen LicenseType-Parameter</span><span class="sxs-lookup"><span data-stu-id="04ad9-511">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="04ad9-512">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="04ad9-512">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="04ad9-513">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="04ad9-513">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="04ad9-514">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="04ad9-514">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="04ad9-515">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="04ad9-515">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="04ad9-516">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="04ad9-516">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="04ad9-517">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="04ad9-517">AzureRM.Websites</span></span>
* <span data-ttu-id="04ad9-518">„New-AzureRMWebApp“ aktualisiert, um allgemeine Algorithmen aus der Strategiebibliothek zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="04ad9-518">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="04ad9-519">6.1.0 – Mai 2018</span><span class="sxs-lookup"><span data-stu-id="04ad9-519">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="04ad9-520">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="04ad9-520">AzureRM.Profile</span></span>
* <span data-ttu-id="04ad9-521">Behebung eines Problems, durch das beim Ausführen von „Clear-AzureRmContext“ ein leerer Kontext mit dem Namen des vorherigen Standardkontexts beibehalten wurde und der Benutzer dadurch keinen neuen Kontext mit dem alten Namen erstellen konnte</span><span class="sxs-lookup"><span data-stu-id="04ad9-521">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="04ad9-522">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="04ad9-522">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="04ad9-523">Ermöglichung der Zuordnung von Gateways/Aufhebung der Gatewayzuordnung in AS</span><span class="sxs-lookup"><span data-stu-id="04ad9-523">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="04ad9-524">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="04ad9-524">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="04ad9-525">Unterstützung für „ApiVersions“, „ApiReleases“ und „ApiRevisions“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-525">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="04ad9-526">Unterstützung für ServiceFabric-Back-End hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-526">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="04ad9-527">Unterstützung für Application Insights-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-527">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="04ad9-528">Unterstützung für die Erkennung von SKUs vom Typ „Basic“ als gültige SKU des API Management-Diensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-528">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="04ad9-529">Unterstützung hinzugefügt, damit Zertifikate, die von der privaten Zertifizierungsstelle ausgestellt wurden, als Stamm- oder ZS-Zertifikate installiert werden können</span><span class="sxs-lookup"><span data-stu-id="04ad9-529">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="04ad9-530">Unterstützung für die Akzeptierung benutzerdefinierter SSL-Zertifikate über KeyVault und mehrere Proxyhostnamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-530">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="04ad9-531">Unterstützung für die verwaltete Dienstidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-531">Added support for MSI identity</span></span>
* <span data-ttu-id="04ad9-532">Unterstützung für die Annahme von Richtlinien über URL hinzugefügt; HINWEIS: Folgende Cmdlets werden in einem zukünftigen Release als veraltet gekennzeichnet:</span><span class="sxs-lookup"><span data-stu-id="04ad9-532">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="04ad9-533">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="04ad9-533">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="04ad9-534">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="04ad9-534">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="04ad9-535">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="04ad9-535">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="04ad9-536">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="04ad9-536">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="04ad9-537">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="04ad9-537">AzureRM.Batch</span></span>
* <span data-ttu-id="04ad9-538">Veröffentlichung des neuen Cmdlets „Get-AzureBatchPoolNodeCounts“</span><span class="sxs-lookup"><span data-stu-id="04ad9-538">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="04ad9-539">Veröffentlichung des neuen Cmdlets „Start-AzureBatchComputeNodeServiceLogUpload“</span><span class="sxs-lookup"><span data-stu-id="04ad9-539">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="04ad9-540">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="04ad9-540">AzureRM.Consumption</span></span>
* <span data-ttu-id="04ad9-541">Hinzufügung neuer Parameter („Expand“, „ResourceGroup“, „InstanceName“, „InstanceId“, „Tags“ und „Top“) für das Cmdlet „Get-AzureRmConsumptionUsageDetail“</span><span class="sxs-lookup"><span data-stu-id="04ad9-541">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="04ad9-542">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="04ad9-542">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="04ad9-543">Korrektur des Beispiels für „Export AzureRmDataLakeStoreChildItemProperties“</span><span class="sxs-lookup"><span data-stu-id="04ad9-543">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="04ad9-544">Korrektur der NULL-Parameterausnahme für rekursiven Fall in „Set-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="04ad9-544">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="04ad9-545">Korrektur der Hilfedateien für „Set-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ und „Remove-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="04ad9-545">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="04ad9-546">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="04ad9-546">AzureRM.Network</span></span>
* <span data-ttu-id="04ad9-547">Erhöhung der Network SDK-Version von 18.0.0-preview auf 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="04ad9-547">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="04ad9-548">Cmdlet zum Erstellen der Protokollkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-548">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="04ad9-549">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="04ad9-549">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="04ad9-550">Cmdlet zum Hinzufügen einer neuen Leitungsverbindung zu einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-550">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="04ad9-551">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="04ad9-551">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="04ad9-552">Cmdlet zum Entfernen einer Leitungsverbindung aus einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-552">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="04ad9-553">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="04ad9-553">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="04ad9-554">Cmdlet zum Abrufen einer Leitungsverbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="04ad9-554">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="04ad9-555">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="04ad9-555">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="04ad9-556">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="04ad9-556">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="04ad9-557">Verwendung der Serverauthentifizierung mit generierten Zertifikaten korrigiert (Problemnr. 5998)</span><span class="sxs-lookup"><span data-stu-id="04ad9-557">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="04ad9-558">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="04ad9-558">AzureRM.Sql</span></span>
* <span data-ttu-id="04ad9-559">Überwachungscmdlets korrigiert, um das Entfernen von „AuditActions“ oder „AuditActionGroups“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="04ad9-559">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="04ad9-560">Problem mit „Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy“ behoben, das beim Festlegen einer neuen flexiblen Aufbewahrungsrichtlinie zu folgendem Fehler führte: „Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span><span class="sxs-lookup"><span data-stu-id="04ad9-560">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="04ad9-561">Please submit request with the new flexible retention policy“ (Das Konfigurieren einer langfristigen Aufbewahrungsrichtlinie mit Azure Recovery Service-Tresor und -Richtlinie wird nicht mehr unterstützt. Übermitteln Sie eine Anforderung mit der neuen flexiblen Aufbewahrungsrichtlinie.)</span><span class="sxs-lookup"><span data-stu-id="04ad9-561">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="04ad9-562">Aktualisierung aller Cmdlets für Azure SQL-Datenbank, für die Erstellung von Pools für elastische Datenbanken und für die Aktualisierung, sodass sie die neue Datenbank-API verwenden. Diese unterstützt die Sku-Eigenschaft für skalierungs- und tarifbezogene Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="04ad9-562">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="04ad9-563">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="04ad9-563">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="04ad9-564">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="04ad9-564">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="04ad9-565">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="04ad9-565">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="04ad9-566">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="04ad9-566">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="04ad9-567">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="04ad9-567">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="04ad9-568">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="04ad9-568">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="04ad9-569">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="04ad9-569">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="04ad9-570">Aktualisierung der Parameter für „Get-AzureRmTrafficManagerProfile“, sodass bei Verwendung des Parameters „-Name“ der Parameter „-ResourceGroupName“ erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="04ad9-570">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
