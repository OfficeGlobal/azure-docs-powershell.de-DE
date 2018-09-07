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
ms.openlocfilehash: f4f3141998be14f0b5b223aed1af283534bf061d
ms.sourcegitcommit: 971f19181b2cd68b7845bbebdb22858c06541c8c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/06/2018
ms.locfileid: "43383837"
---
# <a name="release-notes"></a><span data-ttu-id="c0720-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="c0720-103">Release notes</span></span>

<span data-ttu-id="c0720-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="c0720-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="681---august-2018"></a><span data-ttu-id="c0720-105">6.8.1: August 2018</span><span class="sxs-lookup"><span data-stu-id="c0720-105">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="c0720-106">Allgemein</span><span class="sxs-lookup"><span data-stu-id="c0720-106">General</span></span>
* <span data-ttu-id="c0720-107">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="c0720-107">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="c0720-108">Allgemeine Laufzeitassemblys aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-108">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="c0720-109">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0720-109">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="c0720-110">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="c0720-110">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="c0720-111">Problem https://github.com/Azure/azure-powershell/issues/6603 behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-111">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="c0720-112">Die Cmdlets „Import-AzureRmApiManagementApi“ und „\*-AzureRmApiManagementCertificate“ können jetzt relative Pfade verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="c0720-112">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="c0720-113">Problem https://github.com/Azure/azure-powershell/issues/6879 behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-113">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="c0720-114">„CertificateInformation“ ist eine festlegbare Eigenschaft, die die ordnungsgemäße Funktionsweise des Cmdlets „Set-AzureRmApiManagement“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="c0720-114">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="c0720-115">Behoben durch Upgrade auf NuGet-Paket „4.0.4-preview“</span><span class="sxs-lookup"><span data-stu-id="c0720-115">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="c0720-116">Problem https://github.com/Azure/azure-powershell/issues/6853 behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-116">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="c0720-117">OData-Filter für die Suche anhand des Namens korrigiert (Produkt)</span><span class="sxs-lookup"><span data-stu-id="c0720-117">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="c0720-118">Problem https://github.com/Azure/azure-powershell/issues/6814 behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-118">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="c0720-119">OData-Filter für die Suche anhand des Namens korrigiert (API)</span><span class="sxs-lookup"><span data-stu-id="c0720-119">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="c0720-120">Unterstützung für AzureMonitor-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-120">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="c0720-121">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c0720-121">AzureRM.Compute</span></span>
* <span data-ttu-id="c0720-122">Problem des fehlenden Ziels in der Fehlerausgabe behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-122">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="c0720-123">Problem mit dem Speicherkontotyp für den virtuellen Computer mit verwaltetem Datenträgern behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-123">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="c0720-124">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="c0720-124">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="c0720-125">AEM-Erweiterungs-Cmdlets für andere Umgebungen (etwa Azure China) korrigiert</span><span class="sxs-lookup"><span data-stu-id="c0720-125">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="c0720-126">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c0720-126">AzureRM.Network</span></span>
* <span data-ttu-id="c0720-127">Standarddarstellung der Cmdlet-Ausgabe in Tabellenansicht geändert</span><span class="sxs-lookup"><span data-stu-id="c0720-127">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="c0720-128">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="c0720-128">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="c0720-129">Fehler in „Update-AzureRmPowerBIEmbeddedCapacity“ beim Skalieren der angehaltenen Kapazität behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-129">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="c0720-130">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="c0720-130">AzureRM.Resources</span></span>
* <span data-ttu-id="c0720-131">Problem beim Erstellen verwalteter Anwendungen über Marketplace behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-131">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="c0720-132">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c0720-132">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="c0720-133">Behobene Probleme</span><span class="sxs-lookup"><span data-stu-id="c0720-133">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="c0720-134">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c0720-134">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="c0720-135">Unterstützung für Routingmethode „MultiValue“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-135">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="c0720-136">Neuer Parameter „MaxReturn“ für Routingtyp „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="c0720-136">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="c0720-137">Unterstützung für Subnetzroutingmethode hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-137">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="c0720-138">Unterstützung für IP-Adressbereiche (Subnetze) in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="c0720-138">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="c0720-139">Unterstützung für benutzerdefinierte Header in Profilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-139">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="c0720-140">Unterstützung für erwartete Statuscodebereiche in Profilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-140">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="c0720-141">Unterstützung für benutzerdefinierte Header in Endpunkten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-141">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="c0720-142">6.8.0: August 2018</span><span class="sxs-lookup"><span data-stu-id="c0720-142">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="c0720-143">Allgemein</span><span class="sxs-lookup"><span data-stu-id="c0720-143">General</span></span>
* <span data-ttu-id="c0720-144">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="c0720-144">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="c0720-145">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c0720-145">AzureRM.Profile</span></span>
* <span data-ttu-id="c0720-146">Ablaufeigenschaft zu Token hinzugefügt, die während „Connect-AzureRmAccount“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="c0720-146">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="c0720-147">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c0720-147">AzureRM.Compute</span></span>
* <span data-ttu-id="c0720-148">Problem des fehlenden Ziels in der Fehlerausgabe behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-148">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="c0720-149">Problem mit dem Speicherkontotyp für den virtuellen Computer mit verwaltetem Datenträgern behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-149">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="c0720-150">AEM-Erweiterungs-Cmdlets für andere Umgebungen (etwa Azure China) korrigiert</span><span class="sxs-lookup"><span data-stu-id="c0720-150">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="c0720-151">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="c0720-151">AzureRM.IotHub</span></span>
* <span data-ttu-id="c0720-152">Beispiele für „New-AzureRmIotHubExportDevices“ und „New-AzureRmIotHubImportDevices“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="c0720-152">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="c0720-153">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c0720-153">AzureRM.Network</span></span>
* <span data-ttu-id="c0720-154">Standarddarstellung von Modellen in Tabellenansicht geändert</span><span class="sxs-lookup"><span data-stu-id="c0720-154">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="c0720-155">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="c0720-155">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="c0720-156">Fehler in „Update-AzureRmPowerBIEmbeddedCapacity“ beim Skalieren der angehaltenen Kapazität behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-156">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="c0720-157">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="c0720-157">AzureRM.Resources</span></span>
* <span data-ttu-id="c0720-158">Problem beim Erstellen der verwalteten Anwendung über Marketplace behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-158">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="c0720-159">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c0720-159">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="c0720-160">Fehlerbehebung</span><span class="sxs-lookup"><span data-stu-id="c0720-160">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="c0720-161">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c0720-161">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="c0720-162">Unterstützung für Routingmethode „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="c0720-162">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="c0720-163">Neuer Parameter „MaxReturn“ für Routingtyp „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="c0720-163">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="c0720-164">Unterstützung für Subnetzroutingmethode</span><span class="sxs-lookup"><span data-stu-id="c0720-164">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="c0720-165">Unterstützung für IP-Adressbereiche (Subnetze) in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="c0720-165">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="c0720-166">Unterstützung für benutzerdefinierte Header in Profilen</span><span class="sxs-lookup"><span data-stu-id="c0720-166">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="c0720-167">Unterstützung für erwartete Statuscodebereiche in Profilen</span><span class="sxs-lookup"><span data-stu-id="c0720-167">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="c0720-168">Unterstützung für benutzerdefinierte Header in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="c0720-168">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="c0720-169">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="c0720-169">AzureRM.Websites</span></span>
* <span data-ttu-id="c0720-170">Das Problem, dass die Standardressourcengruppe falsch festgelegt wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="c0720-170">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="c0720-171">6.7.0: August 2018</span><span class="sxs-lookup"><span data-stu-id="c0720-171">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="c0720-172">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c0720-172">AzureRM.Profile</span></span>
* <span data-ttu-id="c0720-173">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-173">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="c0720-174">Benutzer-ID zum Standardkontextnamen hinzugefügt, um Kontextkonflikte zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="c0720-174">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="c0720-175">Probleme mit „Clear-AzureRmContext“ behoben, die Fehler beim Auswählen eines Kontexts verursacht haben (6398)</span><span class="sxs-lookup"><span data-stu-id="c0720-175">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="c0720-176">Ermöglicht, dass für „Connect-AzureRmAccount“ die Mandantendomäne an den Parameter „-TenantId“ übergeben wird</span><span class="sxs-lookup"><span data-stu-id="c0720-176">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="c0720-177">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="c0720-177">Azure.Storage</span></span>
* <span data-ttu-id="c0720-178">Begrenzung von 5 TB für das Kontingent der Azure-Dateifreigabe entfernt</span><span class="sxs-lookup"><span data-stu-id="c0720-178">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="c0720-179">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="c0720-179">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="c0720-180">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c0720-180">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="c0720-181">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-181">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="c0720-182">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c0720-182">Azure.AnalysisServices</span></span>
* <span data-ttu-id="c0720-183">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-183">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="c0720-184">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0720-184">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="c0720-185">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-185">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="c0720-186">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="c0720-186">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="c0720-187">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-187">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="c0720-188">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="c0720-188">AzureRM.Automation</span></span>
* <span data-ttu-id="c0720-189">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-189">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="c0720-190">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="c0720-190">AzureRM.Backup</span></span>
* <span data-ttu-id="c0720-191">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-191">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="c0720-192">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="c0720-192">AzureRM.Batch</span></span>
* <span data-ttu-id="c0720-193">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-193">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="c0720-194">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="c0720-194">AzureRM.Billing</span></span>
* <span data-ttu-id="c0720-195">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-195">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="c0720-196">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="c0720-196">AzureRM.Cdn</span></span>
* <span data-ttu-id="c0720-197">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-197">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="c0720-198">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c0720-198">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="c0720-199">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-199">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="c0720-200">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c0720-200">AzureRM.Compute</span></span>
* <span data-ttu-id="c0720-201">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-201">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="c0720-202">EvictionPolicy-Parameter zu „New-AzureRmVmssConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-202">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="c0720-203">Standort in „DiskFileParameterSet“ von „New-AzureRmVm“ angeben, wenn kein Ort angegeben ist</span><span class="sxs-lookup"><span data-stu-id="c0720-203">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="c0720-204">Parameterbeschreibung in „Save-AzureRmVMImage“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="c0720-204">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="c0720-205">Cmdlet „Get-AzureRmVMDiskEncryptionStatus“ für bestimmte Szenarien im Zusammenhang mit einem Durchlauf korrigiert</span><span class="sxs-lookup"><span data-stu-id="c0720-205">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="c0720-206">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="c0720-206">AzureRM.Consumption</span></span>
* <span data-ttu-id="c0720-207">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-207">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="c0720-208">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="c0720-208">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="c0720-209">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-209">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="c0720-210">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="c0720-210">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="c0720-211">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-211">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="c0720-212">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="c0720-212">AzureRM.DataFactories</span></span>
* <span data-ttu-id="c0720-213">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-213">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="c0720-214">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="c0720-214">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="c0720-215">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-215">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="c0720-216">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="c0720-216">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="c0720-217">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-217">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="c0720-218">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0720-218">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="c0720-219">Debuggen korrigiert, wenn „DebugPreference“ über die PowerShell-Befehlszeile festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="c0720-219">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="c0720-220">Beispiel für „Set-AzureRmDataLakeStoreItemAcl“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-220">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="c0720-221">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="c0720-221">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="c0720-222">Beispiel für „Set-AzureRmDataLakeStoreItemAclEntry“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-222">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="c0720-223">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="c0720-223">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="c0720-224">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-224">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="c0720-225">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="c0720-225">AzureRM.Dns</span></span>
* <span data-ttu-id="c0720-226">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-226">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="c0720-227">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c0720-227">AzureRM.EventGrid</span></span>
* <span data-ttu-id="c0720-228">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-228">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="c0720-229">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="c0720-229">AzureRM.EventHub</span></span>
* <span data-ttu-id="c0720-230">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-230">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="c0720-231">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c0720-231">AzureRM.HDInsight</span></span>
* <span data-ttu-id="c0720-232">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-232">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="c0720-233">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="c0720-233">AzureRM.Insights</span></span>
* <span data-ttu-id="c0720-234">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-234">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="c0720-235">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="c0720-235">AzureRM.IotHub</span></span>
* <span data-ttu-id="c0720-236">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-236">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="c0720-237">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0720-237">AzureRM.KeyVault</span></span>
* <span data-ttu-id="c0720-238">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-238">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="c0720-239">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c0720-239">AzureRM.LogicApp</span></span>
* <span data-ttu-id="c0720-240">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-240">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="c0720-241">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="c0720-241">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="c0720-242">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-242">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="c0720-243">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="c0720-243">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="c0720-244">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-244">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="c0720-245">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="c0720-245">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="c0720-246">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-246">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="c0720-247">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="c0720-247">AzureRM.Media</span></span>
* <span data-ttu-id="c0720-248">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-248">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="c0720-249">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c0720-249">AzureRM.Network</span></span>
* <span data-ttu-id="c0720-250">Beispiel für „Set-AzureRmLocalNetworkGateway“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-250">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="c0720-251">Beispiele und Beschreibungen für „Add-AzureRmVirtualNetworkGatewayIpConfig“, „Get-AzureRmVirtualNetworkGatewayConnectionSharedKey“ und „New-AzureRmVirtualNetworkGatewayConnection“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-251">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="c0720-252">Beispiele für „Remove-AzureRmVirtualNetworkGatewayIpConfig“ und „Reset-AzureRmVirtualNetworkGateway“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-252">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="c0720-253">Beispiel für „Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-253">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="c0720-254">Beispiel für „Set-AzureRmVirtualNetworkGatewayConnectionSharedKey“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-254">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="c0720-255">Beispiel für „Set-AzureRmVirtualNetworkGatewayConnection“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-255">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="c0720-256">Cmdlets für „ApplicationSecurityGroup“, „RouteTable“ und „Usage“ mithilfe des aktuellen Code-Generators erneut erstellt</span><span class="sxs-lookup"><span data-stu-id="c0720-256">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="c0720-257">Deutlichere Formulierung der Fehlermeldung für „Get-AzureRmVirtualNetworkSubnetConfig“, wenn ein nicht vorhandenes Subnetz abgerufen wird</span><span class="sxs-lookup"><span data-stu-id="c0720-257">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="c0720-258">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="c0720-258">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="c0720-259">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-259">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="c0720-260">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c0720-260">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="c0720-261">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-261">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="c0720-262">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c0720-262">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="c0720-263">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-263">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="c0720-264">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="c0720-264">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="c0720-265">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-265">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="c0720-266">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0720-266">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="c0720-267">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-267">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="c0720-268">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="c0720-268">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="c0720-269">Richtlinienfilter zum Cmdlet „Get-AzureRmRecoveryServicesBackItem“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c0720-269">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="c0720-270">Der Befehl gibt die Liste der Sicherungselemente zurück, die durch die angegebene Richtlinien-ID geschützt sind.</span><span class="sxs-lookup"><span data-stu-id="c0720-270">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="c0720-271">„Microsoft.Azure.Management.RecoveryServices.Backup“ auf Version 3.0.0-preview aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-271">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="c0720-272">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-272">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="c0720-273">TargetResourceGroupName-Parameter zu „Restore-AzureRmRecoveryServicesBackupItem“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c0720-273">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="c0720-274">Die Ressourcengruppe, in der die verwalteten Datenträger wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="c0720-274">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="c0720-275">Gilt für die Sicherung des virtuellen Computers mit verwalteten Datenträgern.</span><span class="sxs-lookup"><span data-stu-id="c0720-275">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="c0720-276">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="c0720-276">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="c0720-277">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-277">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="c0720-278">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="c0720-278">AzureRM.RedisCache</span></span>
* <span data-ttu-id="c0720-279">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-279">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="c0720-280">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="c0720-280">AzureRM.Relay</span></span>
* <span data-ttu-id="c0720-281">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-281">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="c0720-282">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="c0720-282">AzureRM.Resources</span></span>
* <span data-ttu-id="c0720-283">Unterstützung der Vorlagenbereitstellung im Abonnementbereich.</span><span class="sxs-lookup"><span data-stu-id="c0720-283">Support template deployment at subscription scope.</span></span> <span data-ttu-id="c0720-284">Neue Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="c0720-284">Add new Cmdlets:</span></span>
    - <span data-ttu-id="c0720-285">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="c0720-285">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="c0720-286">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="c0720-286">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="c0720-287">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="c0720-287">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="c0720-288">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="c0720-288">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="c0720-289">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="c0720-289">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="c0720-290">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="c0720-290">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="c0720-291">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="c0720-291">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="c0720-292">Problem behoben, aufgrund dessen beim Übergeben eines Kontexts an „Set-AzureRmResource“ ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="c0720-292">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="c0720-293">Beispiel in „New-AzureRmResourceGroupDeployment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="c0720-293">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="c0720-294">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-294">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="c0720-295">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="c0720-295">AzureRM.Scheduler</span></span>
* <span data-ttu-id="c0720-296">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-296">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="c0720-297">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c0720-297">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="c0720-298">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-298">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="c0720-299">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c0720-299">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="c0720-300">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-300">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="c0720-301">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="c0720-301">AzureRM.Sql</span></span>
* <span data-ttu-id="c0720-302">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-302">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="c0720-303">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="c0720-303">AzureRM.Storage</span></span>
* <span data-ttu-id="c0720-304">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-304">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="c0720-305">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="c0720-305">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="c0720-306">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-306">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="c0720-307">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="c0720-307">AzureRM.Tags</span></span>
* <span data-ttu-id="c0720-308">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-308">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="c0720-309">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c0720-309">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="c0720-310">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-310">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="c0720-311">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="c0720-311">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="c0720-312">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-312">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="c0720-313">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="c0720-313">AzureRM.Websites</span></span>
* <span data-ttu-id="c0720-314">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-314">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="c0720-315">6.6.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="c0720-315">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="c0720-316">Allgemein</span><span class="sxs-lookup"><span data-stu-id="c0720-316">General</span></span>
* <span data-ttu-id="c0720-317">Alle Hilfedateien aktualisiert, um vollständige Parametertypen und die richtigen Eingabe/Ausgabe-Typen einzuschließen.</span><span class="sxs-lookup"><span data-stu-id="c0720-317">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="c0720-318">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c0720-318">AzureRM.Profile</span></span>
* <span data-ttu-id="c0720-319">Bibliothek „Common.Strategy“ aktualisiert, um überprüfen zu können, ob die aktuelle Konfiguration für eine Ressource mit der Zielressource kompatibel ist.</span><span class="sxs-lookup"><span data-stu-id="c0720-319">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="c0720-320">ps1xml-Typen zu „Common.Storage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-320">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="c0720-321">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="c0720-321">Azure.Storage</span></span>
* <span data-ttu-id="c0720-322">Unterstützung zum Abrufen von Speicherkontext aus „DefaultProfile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-322">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="c0720-323">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-323">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="c0720-324">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0720-324">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="c0720-325">Problem https://github.com/Azure/azure-powershell/issues/6370 behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-325">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="c0720-326">Fehler in Automapper behoben, um „PsApiManagementApi“ in „ApiContract“ zu verschieben</span><span class="sxs-lookup"><span data-stu-id="c0720-326">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="c0720-327">Problem https://github.com/Azure/azure-powershell/issues/6515 behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-327">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="c0720-328">Fehler in „File.Save“ behoben, um Überladung mit Codierungstyp zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="c0720-328">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="c0720-329">Problem https://github.com/Azure/azure-powershell/issues/6560 behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-329">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="c0720-330">Upgrade auf Nuget-Version 4.0.3 durchgeführt, in der Musterausnahme in „apiId“ behoben wurde</span><span class="sxs-lookup"><span data-stu-id="c0720-330">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="c0720-331">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c0720-331">AzureRM.Compute</span></span>
* <span data-ttu-id="c0720-332">Das Problem, aufgrund dessen beim Erstellen eines virtuellen Computers mithilfe von „DiskFileParameterSet“ in „New-AzureRmVm“ wegen einer Umbenennung des Speicherkontotyps „PremiumLRS“ ein Fehler auftrat, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="c0720-332">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="c0720-333">Cmdlet „Invoke-AzureRmVMRunCommand“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="c0720-333">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="c0720-334">„Get-AzureRmAvailabilitySet“ aktualisiert, um die Auflistung aller Verfügbarkeitsgruppen in einem Abonnement zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="c0720-334">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="c0720-335">(ResouceGroupName-Parameter ist jetzt optional.)</span><span class="sxs-lookup"><span data-stu-id="c0720-335">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="c0720-336">„SimpleParameterSet“ von „New-AzureRmVm“ aktualisiert, um Accelerated Networking auf kompatiblen virtuellen Computern zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="c0720-336">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="c0720-337">Einfacher Parametersatz „New-AzureRmVmss“ aktualisiert, sodass das Erstellen der VMSS fehlschlägt, wenn bereits ein benutzerdefinierter LB vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="c0720-337">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="c0720-338">Beispiel für „New-AzureRmDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-338">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="c0720-339">Beispiel für „New-AzureRmVM“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-339">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="c0720-340">Beschreibung für „Set-AzureRmVMOSDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-340">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="c0720-341">Beispiel 1 für „Set-AzureRmVMBginfoExtension“ aktualisiert, um Rechtschreibung und Präfix zu korrigieren.</span><span class="sxs-lookup"><span data-stu-id="c0720-341">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="c0720-342">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="c0720-342">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="c0720-343">ADF .Net SDK-Version auf 1.1.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="c0720-343">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="c0720-344">Unterstützung der Freigabe der selbstgehosteten Integration Runtime über Data Factorys hinweg.</span><span class="sxs-lookup"><span data-stu-id="c0720-344">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="c0720-345">Neuer Parameter „-SharedIntegrationRuntimeResourceId“ zu Cmdlet „Set-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c0720-345">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="c0720-346">Neuer optionaler Parameter „-LinkedDataFactoryName“ zu Cmdlet „Remove-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c0720-346">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="c0720-347">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0720-347">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="c0720-348">DataPlane SDK-Version (Microsoft.Azure.DataLake.Store) auf 1.1.9 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-348">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="c0720-349">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="c0720-349">AzureRM.EventHub</span></span>
* <span data-ttu-id="c0720-350">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-350">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="c0720-351">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="c0720-351">AzureRM.Insights</span></span>
* <span data-ttu-id="c0720-352">Formatierung von „OutputType“ in Hilfedateien korrigiert</span><span class="sxs-lookup"><span data-stu-id="c0720-352">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="c0720-353">Verwendung von Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span><span class="sxs-lookup"><span data-stu-id="c0720-353">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="c0720-354">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0720-354">AzureRM.KeyVault</span></span>
* <span data-ttu-id="c0720-355">Piping-Problem in „Set-AzureRmKeyVaultAccessPolicy“ behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-355">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="c0720-356">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c0720-356">AzureRM.Network</span></span>
* <span data-ttu-id="c0720-357">Beispiele für LoadBalancerInboundNatPoolConfig-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c0720-357">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="c0720-358">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="c0720-358">AzureRM.Resources</span></span>
* <span data-ttu-id="c0720-359">Problem beim Angeben sowohl des Tag-Namens als auch des Werts für „Get-AzureRmResource“ behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-359">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="c0720-360">Piping-Szenario mit „Set-AzureRmResource“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="c0720-360">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="c0720-361">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c0720-361">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="c0720-362">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-362">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="c0720-363">Einige Probleme behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-363">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="c0720-364">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="c0720-364">AzureRM.Sql</span></span>
* <span data-ttu-id="c0720-365">Unterstützung für Advanced Threat Protection für Server bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="c0720-365">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="c0720-366">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c0720-366">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="c0720-367">Unterstützung für Sicherheitsrisikobewertung bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="c0720-367">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="c0720-368">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="c0720-368">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="c0720-369">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="c0720-369">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="c0720-370">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="c0720-370">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="c0720-371">Beispiel in „Remove-AzureRmSqlServerFirewallRule“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="c0720-371">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="c0720-372">Falsche Verarbeitung von „datetime“ für nicht US-basierte Kultur in „Get-AzureSqlSyncGroupLog“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="c0720-372">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="c0720-373">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="c0720-373">AzureRM.Storage</span></span>
* <span data-ttu-id="c0720-374">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-374">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="c0720-375">Cmdlet-Ausgabe von „StorageAccount“ in Tabellenansicht anzeigen</span><span class="sxs-lookup"><span data-stu-id="c0720-375">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="c0720-376">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c0720-376">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="c0720-377">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c0720-377">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="c0720-378">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c0720-378">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="c0720-379">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="c0720-379">AzureRM.Tags</span></span>
* <span data-ttu-id="c0720-380">Falsche Anweisung aus Tag-Cmdlet-Hilfe entfernt</span><span class="sxs-lookup"><span data-stu-id="c0720-380">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="c0720-381">6.5.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="c0720-381">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="c0720-382">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c0720-382">AzureRM.Profile</span></span>
* <span data-ttu-id="c0720-383">Hilfe für „Get-AzureRmContextAutosaveSetting“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-383">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="c0720-384">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="c0720-384">Azure.Storage</span></span>
* <span data-ttu-id="c0720-385">Unterstützung des Blob- oder Dateiuploads mit lesegeschütztem SAS-Token</span><span class="sxs-lookup"><span data-stu-id="c0720-385">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="c0720-386">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="c0720-386">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="c0720-387">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="c0720-387">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="c0720-388">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c0720-388">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="c0720-389">Erforderliche Eigenschaft „ResourceGroupName“ zu AS hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c0720-389">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="c0720-390">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="c0720-390">AzureRM.Automation</span></span>
* <span data-ttu-id="c0720-391">Hilfe aktualisiert und Beispiel für „New-AzureRMAutomationSchedule“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-391">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="c0720-392">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c0720-392">AzureRM.Compute</span></span>
* <span data-ttu-id="c0720-393">Parameter „-Tag“ zu „Update/New-AzureRmAvailabilitySet“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-393">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="c0720-394">Beispiel für „Add-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-394">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="c0720-395">Beispiele für „Remove-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-395">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="c0720-396">Hilfe für „Set-AzureRmVMAccessExtension“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-396">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="c0720-397">„SimpleParameterSet“ für „New-AzureRmVmss“ so aktualisiert, dass „SinglePlacementGroup“ standardmäßig auf „false“ festgelegt ist, und Switch-Parameter „SinglePlacementGroup“ hinzugefügt, der dem Benutzer das Erstellen der VMSS in einer einzelnen Platzierungsgruppe ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="c0720-397">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="c0720-398">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="c0720-398">AzureRM.EventHub</span></span>
* <span data-ttu-id="c0720-399">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSEventHubDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="c0720-399">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="c0720-400">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0720-400">AzureRM.KeyVault</span></span>
* <span data-ttu-id="c0720-401">Fehlermeldung für „Set-AzureRmKeyVaultAccessPolicy“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-401">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="c0720-402">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c0720-402">AzureRM.LogicApp</span></span>
* <span data-ttu-id="c0720-403">Fehler „Parametersatz konnte nicht aufgelöst werden“ in „New-AzureRmLogicApp“behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-403">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="c0720-404">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c0720-404">AzureRM.Network</span></span>
* <span data-ttu-id="c0720-405">Peering über mehrere virtuelle Netzwerke in mehreren Mandanten für „Set/Add-AzureRmVirtualNetworkPeering“ aktiviert</span><span class="sxs-lookup"><span data-stu-id="c0720-405">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="c0720-406">Folgende Cmdlets für Application Gateway aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-406">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="c0720-407">New-AzureRmApplicationGateway: EnableFIPS-Flag und Zonenunterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-407">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="c0720-408">New-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-408">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="c0720-409">Set-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-409">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="c0720-410">RouteTable-Cmdlets mit aktueller Generatorversion erneut generiert</span><span class="sxs-lookup"><span data-stu-id="c0720-410">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="c0720-411">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="c0720-411">AzureRM.Relay</span></span>
* <span data-ttu-id="c0720-412">Markdowndateien aktualisiert, Problem mit Parametername in Beispiel behoben</span><span class="sxs-lookup"><span data-stu-id="c0720-412">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="c0720-413">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="c0720-413">AzureRM.Resources</span></span>
* <span data-ttu-id="c0720-414">Roleassignment- und roledefinition-Cmdlets aktualisiert:</span><span class="sxs-lookup"><span data-stu-id="c0720-414">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="c0720-415">Zusätzliche roledefinition-Aufrufe entfernt, die als Teil des Pagings durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="c0720-415">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="c0720-416">Get-AzureRmRoleAssignment-Cmdlet korrigiert</span><span class="sxs-lookup"><span data-stu-id="c0720-416">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="c0720-417">Befehlsparameterfunktion von „-ExpandPrincipalGroups“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="c0720-417">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="c0720-418">Problem mit „Get-AzureRmResource“ behoben, aufgrund dessen die Groß-/Kleinschreibung des Parameters „-ResourceType“ beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="c0720-418">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="c0720-419">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c0720-419">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="c0720-420">top- und skip-Parameter zu Listen-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-420">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="c0720-421">Cmdlets für die Migration von Standard- zu Premium-Namespace hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="c0720-421">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="c0720-422">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="c0720-422">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="c0720-423">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="c0720-423">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="c0720-424">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="c0720-424">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="c0720-425">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="c0720-425">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="c0720-426">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="c0720-426">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="c0720-427">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSServiceBusDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="c0720-427">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="c0720-428">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c0720-428">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="c0720-429">Beispiel für „New-AzureRmServiceFabricCluster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-429">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="c0720-430">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="c0720-430">AzureRM.Sql</span></span>
* <span data-ttu-id="c0720-431">Neue Cmdlets für „Management.Sql“ hinzugefügt, um Kunden das Hinzufügen des TDE-Zertifikats zu einer SQL Server-Instanz oder einer verwalteten Instanz zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="c0720-431">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="c0720-432">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="c0720-432">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="c0720-433">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="c0720-433">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="c0720-434">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="c0720-434">AzureRM.Websites</span></span>
* <span data-ttu-id="c0720-435">Wenn `Set-AzureRmWebApp -AssignIdentity` und `Set-AzureRmWebAppSlot -AssignIdentity` auf „false“ festgelegt sind, wird jetzt die Identity-Eigenschaft aus dem Websiteobjekt entfernt. Auch das Vorschau-Tag wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="c0720-435">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="c0720-436">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics`-Beispiel aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-436">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="c0720-437">Unterstützung von `Set-AzureRmWebApp -PhpVersion` als gültige PHP-Version eingestellt</span><span class="sxs-lookup"><span data-stu-id="c0720-437">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="c0720-438">6.4.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="c0720-438">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="c0720-439">Allgemein</span><span class="sxs-lookup"><span data-stu-id="c0720-439">General</span></span>
* <span data-ttu-id="c0720-440">Formatierung von OutputType in Hilfedateien für die meisten Module korrigiert</span><span class="sxs-lookup"><span data-stu-id="c0720-440">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="c0720-441">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c0720-441">AzureRM.Profile</span></span>
* <span data-ttu-id="c0720-442">Attribut „Ps1Xml“ wurde den Standardausgabetypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-442">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="c0720-443">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c0720-443">AzureRM.Compute</span></span>
* <span data-ttu-id="c0720-444">IP-Tag-Funktion für VMSS</span><span class="sxs-lookup"><span data-stu-id="c0720-444">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="c0720-445">Cmdlet „New-AzureRmVmssIpTagConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-445">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="c0720-446">IpTag-Parameter zu „New-AzureRmVmssIpConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-446">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="c0720-447">Funktion für automatisches Betriebssystemrollback für VMSS</span><span class="sxs-lookup"><span data-stu-id="c0720-447">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="c0720-448">DisableAutoRollback-Parameter zu „New-AzureRmVmssConfig“ und „Update-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-448">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="c0720-449">Funktion für Upgradeverlauf des Betriebssystems für VMSS</span><span class="sxs-lookup"><span data-stu-id="c0720-449">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="c0720-450">Switch-Parameter „OSUpgradeHistory“ zu „Get-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-450">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="c0720-451">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="c0720-451">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="c0720-452">Unterstützung für Katalog-ACLs über die folgenden Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="c0720-452">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="c0720-453">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="c0720-453">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="c0720-454">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="c0720-454">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="c0720-455">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="c0720-455">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="c0720-456">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0720-456">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="c0720-457">Abbruchunterstützung und Nachverfolgung des Fortschritts für „Set-AzureRmDataLakeStoreItemAclEntry“, „Remove-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-457">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="c0720-458">Abbruchunterstützung „Export-AzureRmDataLakeStoreChildItemProperties“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-458">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="c0720-459">Leerung von Debugmeldungen für Cmdlets korrigiert, die rekursive Vorgänge durchführt</span><span class="sxs-lookup"><span data-stu-id="c0720-459">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="c0720-460">Speicherort des Test von DataLake-Cmdlets korrigiert</span><span class="sxs-lookup"><span data-stu-id="c0720-460">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="c0720-461">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="c0720-461">AzureRM.EventHub</span></span>
* <span data-ttu-id="c0720-462">Optionaler Parameter „MaxCount“ zu Listenvorgangs-Cmdlets „Get-AzureRmEventHub“ und „Get-AzureRmEventHubConsumerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-462">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="c0720-463">Problem in Cmdlet „New-AzureRmEventHub“ behoben, aufgrund dessen beim Erstellen einer neuen EventHub-Instanz mindestens ein Parameter benötigt wurde.</span><span class="sxs-lookup"><span data-stu-id="c0720-463">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="c0720-464">Standardparametersatz wurde bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="c0720-464">Provided Default Parameter set.</span></span>
* <span data-ttu-id="c0720-465">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmEventHubKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="c0720-465">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="c0720-466">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0720-466">AzureRM.KeyVault</span></span>
* <span data-ttu-id="c0720-467">Problem behoben, aufgrund dessen von „Get-AzureRmKeyVault -Tag“ alle Ressourcen zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="c0720-467">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="c0720-468">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c0720-468">AzureRM.Network</span></span>
* <span data-ttu-id="c0720-469">Neue SKUs für zonenredundante VirtualNetworkGateways-Instanzen verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="c0720-469">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="c0720-470">Neue Befehle für Funktion hinzugefügt: ExpressRoute-Partner-APIs über ARM</span><span class="sxs-lookup"><span data-stu-id="c0720-470">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="c0720-471">Get-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-471">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="c0720-472">Set-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-472">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="c0720-473">Add-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-473">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="c0720-474">Get-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-474">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="c0720-475">Remove-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-475">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="c0720-476">Get-AzureRMExpressRouteCrossConnectionArpTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-476">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="c0720-477">Get-AzureRMExpressRouteCrossConnectionRouteTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-477">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="c0720-478">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-478">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="c0720-479">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="c0720-479">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="c0720-480">Cmdlet „Get-AzureRmRecoveryServicesBackupStatus“ wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c0720-480">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="c0720-481">Dieses Cmdlet überprüft anhand der ID eines virtuellen Computers, ob dieser durch einen Tresor im Abonnement geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="c0720-481">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="c0720-482">Wenn ein solcher Tresor vorhanden ist, gibt das Cmdlet die Tresordetails aus.</span><span class="sxs-lookup"><span data-stu-id="c0720-482">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="c0720-483">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="c0720-483">AzureRM.Resources</span></span>
* <span data-ttu-id="c0720-484">Cmdlets vom Typ „Get-AzureRmPolicyAssignment“ aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="c0720-484">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="c0720-485">Unterstützung für das Auflisten von „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-485">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="c0720-486">Unterstützung für das Abrufen einzelner Arbeitsaufträge mit „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-486">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="c0720-487">Switches „-Effective“ und „-All“ zu Steuerparameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-487">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="c0720-488">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicyDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-488">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="c0720-489">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="c0720-489">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="c0720-490">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="c0720-490">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="c0720-491">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicySetDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-491">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="c0720-492">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="c0720-492">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="c0720-493">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="c0720-493">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="c0720-494">Unterstützung für KeyVault-Geheimnisverweis in Parametern hinzugefügt, wenn „TemplateParameterObject“ in „New-AzureRmResourceGroupDeployment“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="c0720-494">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="c0720-495">Problem behoben, aufgrund dessen, der Parameter „-EndDate“ für „New-AzureRmADAppCredential“ ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="c0720-495">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="c0720-496">Problem behoben, aufgrund dessen „Add-AzureRmADGroupMember“ eine falsche URL für Anforderungen verwendete</span><span class="sxs-lookup"><span data-stu-id="c0720-496">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="c0720-497">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c0720-497">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="c0720-498">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmServiceBusKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="c0720-498">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="c0720-499">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="c0720-499">AzureRM.Sql</span></span>
* <span data-ttu-id="c0720-500">Benutzerdefinierte Wiederherstellungspunkte für SQLDW in Hilfe zu „New-AzureRmSqlDatabaseRestorePoint“ erläutert</span><span class="sxs-lookup"><span data-stu-id="c0720-500">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="c0720-501">Dokumentation von Parameter „-ComputeGeneration“ in mehreren Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-501">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="c0720-502">6.3.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="c0720-502">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="c0720-503">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c0720-503">AzureRM.Profile</span></span>
* <span data-ttu-id="c0720-504">Aktualisierte Fehlermeldungen für „Enable-AzureRmContextAutoSave“</span><span class="sxs-lookup"><span data-stu-id="c0720-504">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="c0720-505">Erstellen eines Kontexts für jedes Abonnement beim Ausführen von „Connect-AzureRmAccount“ ohne vorherigen Kontext</span><span class="sxs-lookup"><span data-stu-id="c0720-505">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="c0720-506">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="c0720-506">Azure.Storage</span></span>
* <span data-ttu-id="c0720-507">Zusätzliche Informationen zum Parameter „-Permissions“ in Hilfedateien</span><span class="sxs-lookup"><span data-stu-id="c0720-507">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="c0720-508">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c0720-508">AzureRM.Compute</span></span>
* <span data-ttu-id="c0720-509">„Get-AzureRmVmDiskEncryptionStatus“ behebt ein Problem, das bei virtuellen Computern ohne Datenträger festgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="c0720-509">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="c0720-510">Version der Computeclientbibliothek aktualisiert, um folgende Cmdlets zu korrigieren:</span><span class="sxs-lookup"><span data-stu-id="c0720-510">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="c0720-511">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="c0720-511">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="c0720-512">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="c0720-512">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="c0720-513">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="c0720-513">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="c0720-514">Die folgenden Cmdlets wurden korrigiert, um die Vorgangs-ID und den Vorgangsstatus korrekt anzuzeigen:</span><span class="sxs-lookup"><span data-stu-id="c0720-514">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="c0720-515">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="c0720-515">Start-AzureRmVM</span></span>
    - <span data-ttu-id="c0720-516">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="c0720-516">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="c0720-517">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="c0720-517">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="c0720-518">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="c0720-518">Set-AzureRmVM</span></span>
    - <span data-ttu-id="c0720-519">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="c0720-519">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="c0720-520">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="c0720-520">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="c0720-521">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="c0720-521">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="c0720-522">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="c0720-522">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="c0720-523">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="c0720-523">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="c0720-524">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="c0720-524">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="c0720-525">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="c0720-525">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="c0720-526">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="c0720-526">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="c0720-527">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="c0720-527">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="c0720-528">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="c0720-528">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="c0720-529">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="c0720-529">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="c0720-530">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="c0720-530">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="c0720-531">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="c0720-531">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="c0720-532">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="c0720-532">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="c0720-533">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="c0720-533">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="c0720-534">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c0720-534">AzureRM.EventGrid</span></span>
* <span data-ttu-id="c0720-535">ValidateNotNullOrEmpty-Überprüfungskonditionen für „SubjectBeginsWith“/„SubjectEndsWith“ im Cmdlet „Update-AzureRmEventGridSubscription“ wurden entfernt, um bei Bedarf die Änderung dieser Parameter in eine leere Zeichenfolge zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="c0720-535">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="c0720-536">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0720-536">AzureRM.KeyVault</span></span>
* <span data-ttu-id="c0720-537">Ein Problem wurde behoben, aufgrund dessen bei Ausführung von „Get-AzureRmKeyVault -Tag“ keine Tags zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="c0720-537">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="c0720-538">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c0720-538">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="c0720-539">Offizielle Veröffentlichung von Policy Insights-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="c0720-539">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="c0720-540">Verwendung der API-Version 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="c0720-540">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="c0720-541">„PolicyDefinitionReferenceId“ zu den Ergebnissen von „Get-AzureRmPolicyStateSummary“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-541">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="c0720-542">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="c0720-542">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="c0720-543">Parameter „-Vault“ zu den RecoveryServices.Backup-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c0720-543">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="c0720-544">Bei der Übergabe wird dadurch das Cmdlet „Set-AzureRmRecoveryServicesContext“ außer Kraft gesetzt.</span><span class="sxs-lookup"><span data-stu-id="c0720-544">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="c0720-545">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="c0720-545">AzureRM.Sql</span></span>
* <span data-ttu-id="c0720-546">Aktualisiertes Beispiel in der Hilfedatei für „Get-AzureRmSqlDatabaseExpanded“</span><span class="sxs-lookup"><span data-stu-id="c0720-546">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="c0720-547">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c0720-547">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="c0720-548">Hilfedatei für „Add-AzureRmTrafficManagerEndpointConfig“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="c0720-548">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="c0720-549">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="c0720-549">AzureRM.Websites</span></span>
* <span data-ttu-id="c0720-550">„Set-AzureRmWebApp“ wurde aktualisiert, damit „AppSettings“ bei der Verwendung von „-AssignIdentity“ nicht außer Kraft gesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="c0720-550">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="c0720-551">„New-AzureRmWebAppSlot“ wurde aktualisiert, um „AppServicePlan“ als optionalen Parameter anzuerkennen</span><span class="sxs-lookup"><span data-stu-id="c0720-551">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="c0720-552">6.2.1: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="c0720-552">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="c0720-553">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c0720-553">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="c0720-554">PSWorkspace-Modell aktualisiert, damit das Netzwerk „type“ als Parameter verwenden kann</span><span class="sxs-lookup"><span data-stu-id="c0720-554">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="c0720-555">6.2.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="c0720-555">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="c0720-556">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c0720-556">AzureRM.Profile</span></span>
* <span data-ttu-id="c0720-557">Beheben des Problems, aufgrund dessen Version 10.0.3 von Newtonsoft.Json beim Modulimport nicht geladen wurde</span><span class="sxs-lookup"><span data-stu-id="c0720-557">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="c0720-558">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c0720-558">AzureRM.Compute</span></span>
* <span data-ttu-id="c0720-559">Feature zum Aktualisieren von virtuellen VMSS-Computern</span><span class="sxs-lookup"><span data-stu-id="c0720-559">VMSS VM Update feature</span></span>
    - <span data-ttu-id="c0720-560">Cmdlets „Update-AzureRmVmssVM“ und „New-AzureRmVMDataDisk“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-560">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="c0720-561">Fügen Sie den Parameter „VirtualMachineScaleSetVM“ zum Cmdlet „Add-AzureRmVMDataDisk“ hinzu, um das Hinzufügen eines Datenträgers zum virtuellen VMSS-Computer zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="c0720-561">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="c0720-562">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="c0720-562">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="c0720-563">Aktualisierung der ADF .Net SDK-Version auf 0.8.0-preview mit den folgenden Änderungen:</span><span class="sxs-lookup"><span data-stu-id="c0720-563">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="c0720-564">Vorgang zum Konfigurieren des Factoryrepositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-564">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="c0720-565">Der verknüpfte QuickBooks-Dienst wurde aktualisiert, um die Eigenschaften „consumerKey“ und „consumerSecret“ verfügbar zu machen.</span><span class="sxs-lookup"><span data-stu-id="c0720-565">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="c0720-566">Aktualisierung verschiedener Modelltypen von „SecretBase“ auf „Object“</span><span class="sxs-lookup"><span data-stu-id="c0720-566">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="c0720-567">Blobereignisauslöser hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-567">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="c0720-568">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0720-568">AzureRM.KeyVault</span></span>
* <span data-ttu-id="c0720-569">Aktualisierung der Dokumentation mit Beispielausgabe</span><span class="sxs-lookup"><span data-stu-id="c0720-569">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="c0720-570">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c0720-570">AzureRM.Network</span></span>
* <span data-ttu-id="c0720-571">Aktivierung der Traffic Analytics-Parameter für Network Watcher-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="c0720-571">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="c0720-572">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="c0720-572">AzureRM.Resources</span></span>
* <span data-ttu-id="c0720-573">Behebung des Problems mit der Eigenschaft „Properties“ von PSResource-Objekten, die von „Get-AzureRmResource“ zurückgegeben wurden</span><span class="sxs-lookup"><span data-stu-id="c0720-573">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="c0720-574">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="c0720-574">AzureRM.Scheduler</span></span>
* <span data-ttu-id="c0720-575">Behebung des Problems, dass beim Aktualisieren von „ServiceBusQueueJob“ keine neuen Authentifizierungswerte festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="c0720-575">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="c0720-576">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="c0720-576">AzureRM.Sql</span></span>
* <span data-ttu-id="c0720-577">Aktualisierung der folgenden Cmdlets mit dem optionalen LicenseType-Parameter</span><span class="sxs-lookup"><span data-stu-id="c0720-577">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="c0720-578">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="c0720-578">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="c0720-579">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="c0720-579">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="c0720-580">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="c0720-580">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="c0720-581">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="c0720-581">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="c0720-582">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="c0720-582">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="c0720-583">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="c0720-583">AzureRM.Websites</span></span>
* <span data-ttu-id="c0720-584">„New-AzureRMWebApp“ aktualisiert, um allgemeine Algorithmen aus der Strategiebibliothek zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="c0720-584">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="c0720-585">6.1.0 – Mai 2018</span><span class="sxs-lookup"><span data-stu-id="c0720-585">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="c0720-586">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c0720-586">AzureRM.Profile</span></span>
* <span data-ttu-id="c0720-587">Behebung eines Problems, durch das beim Ausführen von „Clear-AzureRmContext“ ein leerer Kontext mit dem Namen des vorherigen Standardkontexts beibehalten wurde und der Benutzer dadurch keinen neuen Kontext mit dem alten Namen erstellen konnte</span><span class="sxs-lookup"><span data-stu-id="c0720-587">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="c0720-588">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c0720-588">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="c0720-589">Ermöglichung der Zuordnung von Gateways/Aufhebung der Gatewayzuordnung in AS</span><span class="sxs-lookup"><span data-stu-id="c0720-589">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="c0720-590">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0720-590">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="c0720-591">Unterstützung für „ApiVersions“, „ApiReleases“ und „ApiRevisions“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-591">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="c0720-592">Unterstützung für ServiceFabric-Back-End hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-592">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="c0720-593">Unterstützung für Application Insights-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-593">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="c0720-594">Unterstützung für die Erkennung von SKUs vom Typ „Basic“ als gültige SKU des API Management-Diensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-594">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="c0720-595">Unterstützung hinzugefügt, damit Zertifikate, die von der privaten Zertifizierungsstelle ausgestellt wurden, als Stamm- oder ZS-Zertifikate installiert werden können</span><span class="sxs-lookup"><span data-stu-id="c0720-595">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="c0720-596">Unterstützung für die Akzeptierung benutzerdefinierter SSL-Zertifikate über KeyVault und mehrere Proxyhostnamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-596">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="c0720-597">Unterstützung für die verwaltete Dienstidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-597">Added support for MSI identity</span></span>
* <span data-ttu-id="c0720-598">Unterstützung für die Annahme von Richtlinien über URL hinzugefügt; HINWEIS: Folgende Cmdlets werden in einem zukünftigen Release als veraltet gekennzeichnet:</span><span class="sxs-lookup"><span data-stu-id="c0720-598">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="c0720-599">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="c0720-599">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="c0720-600">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0720-600">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="c0720-601">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="c0720-601">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="c0720-602">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="c0720-602">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="c0720-603">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="c0720-603">AzureRM.Batch</span></span>
* <span data-ttu-id="c0720-604">Veröffentlichung des neuen Cmdlets „Get-AzureBatchPoolNodeCounts“</span><span class="sxs-lookup"><span data-stu-id="c0720-604">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="c0720-605">Veröffentlichung des neuen Cmdlets „Start-AzureBatchComputeNodeServiceLogUpload“</span><span class="sxs-lookup"><span data-stu-id="c0720-605">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="c0720-606">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="c0720-606">AzureRM.Consumption</span></span>
* <span data-ttu-id="c0720-607">Hinzufügung neuer Parameter („Expand“, „ResourceGroup“, „InstanceName“, „InstanceId“, „Tags“ und „Top“) für das Cmdlet „Get-AzureRmConsumptionUsageDetail“</span><span class="sxs-lookup"><span data-stu-id="c0720-607">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="c0720-608">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0720-608">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="c0720-609">Korrektur des Beispiels für „Export AzureRmDataLakeStoreChildItemProperties“</span><span class="sxs-lookup"><span data-stu-id="c0720-609">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="c0720-610">Korrektur der NULL-Parameterausnahme für rekursiven Fall in „Set-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="c0720-610">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="c0720-611">Korrektur der Hilfedateien für „Set-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ und „Remove-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="c0720-611">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="c0720-612">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c0720-612">AzureRM.Network</span></span>
* <span data-ttu-id="c0720-613">Erhöhung der Network SDK-Version von 18.0.0-preview auf 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="c0720-613">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="c0720-614">Cmdlet zum Erstellen der Protokollkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-614">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="c0720-615">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0720-615">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="c0720-616">Cmdlet zum Hinzufügen einer neuen Leitungsverbindung zu einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-616">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="c0720-617">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="c0720-617">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="c0720-618">Cmdlet zum Entfernen einer Leitungsverbindung aus einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-618">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="c0720-619">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="c0720-619">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="c0720-620">Cmdlet zum Abrufen einer Leitungsverbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="c0720-620">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="c0720-621">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="c0720-621">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="c0720-622">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c0720-622">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="c0720-623">Verwendung der Serverauthentifizierung mit generierten Zertifikaten korrigiert (Problemnr. 5998)</span><span class="sxs-lookup"><span data-stu-id="c0720-623">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="c0720-624">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="c0720-624">AzureRM.Sql</span></span>
* <span data-ttu-id="c0720-625">Überwachungscmdlets korrigiert, um das Entfernen von „AuditActions“ oder „AuditActionGroups“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="c0720-625">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="c0720-626">Problem mit „Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy“ behoben, das beim Festlegen einer neuen flexiblen Aufbewahrungsrichtlinie zu folgendem Fehler führte: „Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span><span class="sxs-lookup"><span data-stu-id="c0720-626">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="c0720-627">Please submit request with the new flexible retention policy“ (Das Konfigurieren einer langfristigen Aufbewahrungsrichtlinie mit Azure Recovery Service-Tresor und -Richtlinie wird nicht mehr unterstützt. Übermitteln Sie eine Anforderung mit der neuen flexiblen Aufbewahrungsrichtlinie.)</span><span class="sxs-lookup"><span data-stu-id="c0720-627">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="c0720-628">Aktualisierung aller Cmdlets für Azure SQL-Datenbank, für die Erstellung von Pools für elastische Datenbanken und für die Aktualisierung, sodass sie die neue Datenbank-API verwenden. Diese unterstützt die Sku-Eigenschaft für skalierungs- und tarifbezogene Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="c0720-628">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="c0720-629">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c0720-629">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="c0720-630">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="c0720-630">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="c0720-631">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="c0720-631">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="c0720-632">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="c0720-632">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="c0720-633">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="c0720-633">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="c0720-634">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="c0720-634">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="c0720-635">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c0720-635">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="c0720-636">Aktualisierung der Parameter für „Get-AzureRmTrafficManagerProfile“, sodass bei Verwendung des Parameters „-Name“ der Parameter „-ResourceGroupName“ erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="c0720-636">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
