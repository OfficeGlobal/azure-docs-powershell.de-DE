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
ms.openlocfilehash: 6a33d1a85fc61d0281bf1183163185b0dc4d3a12
ms.sourcegitcommit: a749eb729f583c9d0dd86141bbd04984d77ae9ab
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/11/2018
ms.locfileid: "48882145"
---
# <a name="release-notes"></a><span data-ttu-id="111e4-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="111e4-103">Release notes</span></span>

<span data-ttu-id="111e4-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="111e4-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="6100---october-2018"></a><span data-ttu-id="111e4-105">6.10.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="111e4-105">6.10.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="111e4-106">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="111e4-106">Azure.Storage</span></span>
* <span data-ttu-id="111e4-107">Fehler beim Kopieren von Blobs/Dateien behoben, aufgrund dessen bei einem Metadatenproblem des Ziels keine Metadaten kopiert wurden</span><span class="sxs-lookup"><span data-stu-id="111e4-107">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="111e4-108">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="111e4-108">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="111e4-109">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="111e4-109">Start-AzureStorageFileCopy</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="111e4-110">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="111e4-110">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="111e4-111">„Get-AzureRmCognitiveServicesAccountSkus“ wird ohne vorhandenes Konto unterstützt.</span><span class="sxs-lookup"><span data-stu-id="111e4-111">Support Get-AzureRmCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="111e4-112">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="111e4-112">AzureRM.Compute</span></span>
* <span data-ttu-id="111e4-113">Korrektur von „Get-AzureRmVM -ResourceGroupName <rg>“ sodass ggf. mehr als 50 Ergebnisse zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="111e4-113">Fix Get-AzureRmVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="111e4-114">Der Cmdlet-Hilfe zu „New-AzureRmVmss“ wurde ein Beispiel für „SimpleParameterSet“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="111e4-114">Added an example of the 'SimpleParameterSet' to New-AzureRmVmss cmdlet help.</span></span>
* <span data-ttu-id="111e4-115">Tippfehler in der Azure Disk Encryption-Statusmeldung behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-115">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="111e4-116">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="111e4-116">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="111e4-117">Die Version des ADF .Net-SDK wurde auf 2.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="111e4-117">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="111e4-118">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="111e4-118">AzureRM.Network</span></span>
* <span data-ttu-id="111e4-119">NetworkProfile-Funktionalität wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="111e4-119">Added NetworkProfile functionality.</span></span> <span data-ttu-id="111e4-120">Neue Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-120">new cmdlets added</span></span>
    - <span data-ttu-id="111e4-121">Get-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="111e4-121">Get-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="111e4-122">New-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="111e4-122">New-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="111e4-123">Remove-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="111e4-123">Remove-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="111e4-124">Set-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="111e4-124">Set-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="111e4-125">New-AzureRMContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-125">New-AzureRMContainerNicConfig</span></span>
    - <span data-ttu-id="111e4-126">New-AzureRmContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-126">New-AzureRmContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="111e4-127">Dienstzuordnungslink in Subnetzmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-127">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="111e4-128">Cmdlets „New-AzureRmVirtualNetworkTap“, „Get-AzureRmVirtualNetworkTap“, „Set-AzureRmVirtualNetworkTap“, „Remove-AzureRmVirtualNetworkTap“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-128">Added cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span></span>
* <span data-ttu-id="111e4-129">Cmdlets „Set-AzureRmNEtworkInterfaceTapConfig“, „Get-AzureRmNEtworkInterfaceTapConfig“, „Remove-AzureRmNEtworkInterfaceTapConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-129">Added cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="111e4-130">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="111e4-130">AzureRM.RedisCache</span></span>
* <span data-ttu-id="111e4-131">Künftig sind beliebige Zeichenfolgen als Größenparameter zulässig.</span><span class="sxs-lookup"><span data-stu-id="111e4-131">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="111e4-132">P5 in Popup „PSArgumentCompleter“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-132">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="111e4-133">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="111e4-133">AzureRM.Resources</span></span>
* <span data-ttu-id="111e4-134">Fehlender Parameter „-Mode“ zu „Set-AzureRmPolicyDefinition“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-134">Add missing -Mode parameter to Set-AzureRmPolicyDefinition</span></span>
* <span data-ttu-id="111e4-135">Cmdlet-Fehler bei „Fix Get-AzureRmProviderOperation“ für Vorgänge mit Ursprung behoben, der den Benutzer enthält</span><span class="sxs-lookup"><span data-stu-id="111e4-135">Fix Get-AzureRmProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="111e4-136">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="111e4-136">AzureRM.Sql</span></span>
* <span data-ttu-id="111e4-137">Problem behoben, aufgrund dessen einige Sicherungs-Cmdlets das aktuelle Azure-Abonnements nicht erkannt haben</span><span class="sxs-lookup"><span data-stu-id="111e4-137">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="111e4-138">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="111e4-138">AzureRM.Storage</span></span>
* <span data-ttu-id="111e4-139">Der Abruf der Speicherressourcennutzung eines bestimmten Standorts wird jetzt unterstützt, und das Hinzufügen einer Warnmeldung für den Abruf der globalen Speicherressourcennutzung ist überflüssig.</span><span class="sxs-lookup"><span data-stu-id="111e4-139">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="111e4-140">Get-AzureRmStorageUsage</span><span class="sxs-lookup"><span data-stu-id="111e4-140">Get-AzureRmStorageUsage</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="111e4-141">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="111e4-141">AzureRM.Websites</span></span>
* <span data-ttu-id="111e4-142">Neues Cmdlet „Get-AzureRMWebAppContainerContinuousDeploymentUrl“ zum Abruf der Webhook-URL von Continuous Deployment für Container</span><span class="sxs-lookup"><span data-stu-id="111e4-142">New Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="111e4-143">Neue Cmdlets „New-AzureRMWebAppContainerPSSession“ und „Enter-WebAppContainerPSSession“ zum Initiieren einer PowerShell-Remotesitzung in einer Windows-Container-App</span><span class="sxs-lookup"><span data-stu-id="111e4-143">New Cmdlets New-AzureRMWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="690---september-2018"></a><span data-ttu-id="111e4-144">6.9.0 – September 2018</span><span class="sxs-lookup"><span data-stu-id="111e4-144">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="111e4-145">Allgemein</span><span class="sxs-lookup"><span data-stu-id="111e4-145">General</span></span>
* <span data-ttu-id="111e4-146">AzureRM.SignalR wurde dem Rollupmodul AzureRM hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-146">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="111e4-147">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="111e4-147">AzureRM.Profile</span></span>
* <span data-ttu-id="111e4-148">Kleinere Änderungen am allgemeinen Speichercode</span><span class="sxs-lookup"><span data-stu-id="111e4-148">Minor changes to the storage common code</span></span>
* <span data-ttu-id="111e4-149">Hilfedateien aktualisiert, um vollständige Parametertypen einzubinden.</span><span class="sxs-lookup"><span data-stu-id="111e4-149">Updated help files to include full parameter types.</span></span>
- <span data-ttu-id="111e4-150">„-ServicePrincipal“ im Parametersatz „ServicePrincipalCertificateWithSubscriptionId“ in nicht obligatorisch geändert</span><span class="sxs-lookup"><span data-stu-id="111e4-150">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="111e4-151">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="111e4-151">Azure.Storage</span></span>
* <span data-ttu-id="111e4-152">Unterstützung für die Erstellung des Speicherkontexts mit OAuth.</span><span class="sxs-lookup"><span data-stu-id="111e4-152">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="111e4-153">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="111e4-153">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="111e4-154">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="111e4-154">AzureRM.Cdn</span></span>
* <span data-ttu-id="111e4-155">Standard_Microsoft in SKU für CDN-Preise hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="111e4-155">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="111e4-156">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="111e4-156">AzureRM.Compute</span></span>
* <span data-ttu-id="111e4-157">Abhängigkeiten für Key Vault und Storage in allgemeine Abhängigkeiten verschieben</span><span class="sxs-lookup"><span data-stu-id="111e4-157">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="111e4-158">Unterstützung für weitere VM-Größen zu AEM-Cmdlets hinzufügen</span><span class="sxs-lookup"><span data-stu-id="111e4-158">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="111e4-159">Parameter „PublicIPPrefix“ zu „New-AzureRmVmssIpConfig“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="111e4-159">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="111e4-160">Parameter „ResourceId“ zu Cmdlet „Invoke-AzureRmVMRunCommand“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="111e4-160">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="111e4-161">Cmdlet „Invoke-AzureRmVmssVMRunCommand“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="111e4-161">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="111e4-162">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="111e4-162">AzureRM.Dns</span></span>
* <span data-ttu-id="111e4-163">Unterstützung für Aliaseintrag während der Erstellung des DNS-Eintrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-163">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="111e4-164">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="111e4-164">AzureRM.Insights</span></span>
* <span data-ttu-id="111e4-165">Probleme #6833 und #7102 behoben (Bereich „Diagnoseeinstellungen“)</span><span class="sxs-lookup"><span data-stu-id="111e4-165">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="111e4-166">Probleme mit dem Standardnamen, also „service“, beim Erstellen und Auflisten/Abrufen von Diagnoseeinstellungen</span><span class="sxs-lookup"><span data-stu-id="111e4-166">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="111e4-167">Probleme beim Erstellen von Diagnoseeinstellungen mit Kategorien</span><span class="sxs-lookup"><span data-stu-id="111e4-167">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="111e4-168">Meldung zur Einstellung der Unterstützung für Metrikaggregationsintervall-Parameter</span><span class="sxs-lookup"><span data-stu-id="111e4-168">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="111e4-169">Aggregationsintervall-Parameter werden weiterhin akzeptiert (Änderung ohne Funktionsbeeinträchtigung), aber sie werden auf dem Back-End ignoriert, da nur PT1M gültig ist</span><span class="sxs-lookup"><span data-stu-id="111e4-169">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="111e4-170">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="111e4-170">AzureRM.Network</span></span>
* <span data-ttu-id="111e4-171">Änderungen an LoadBalancer-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="111e4-171">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="111e4-172">LoadBalancerInboundNatPoolConfig: Parameter IdleTimeoutInMinutes, EnableFloatingIp und EnableTcpReset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-172">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="111e4-173">LoadBalancerInboundNatRuleConfig: Parameter EnableTcpReset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-173">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="111e4-174">LoadBalancerRuleConfig: Parameter EnableTcpReset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-174">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="111e4-175">LoadBalancerProbeConfig: Unterstützung für Wert „Https“ für Parameter „Protocol“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-175">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="111e4-176">Neue Befehle für neue Unterressource „OutboundRule“ von LoadBalancer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-176">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="111e4-177">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-177">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="111e4-178">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-178">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="111e4-179">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-179">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="111e4-180">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-180">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="111e4-181">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-181">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="111e4-182">Neue HostedWorkloads-Eigenschaft für PSNetworkInterface hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-182">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="111e4-183">Neue Cmdlets für Feature: Azure Firewall über ARM</span><span class="sxs-lookup"><span data-stu-id="111e4-183">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="111e4-184">Get-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-184">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="111e4-185">Set-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-185">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="111e4-186">New-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-186">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="111e4-187">Remove-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-187">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="111e4-188">New-AzureRmFirewallApplicationRuleCollection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-188">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="111e4-189">New-AzureRmFirewallApplicationRule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-189">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="111e4-190">New-AzureRmFirewallNatRuleCollection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-190">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="111e4-191">New-AzureRmFirewallNatRule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-191">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="111e4-192">New-AzureRmFirewallNetworkRuleCollection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-192">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="111e4-193">New-AzureRmFirewallNetworkRule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-193">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="111e4-194">Unterstützung für vertrauenswürdiges Stammzertifikat und Konfiguration der automatischen Skalierung in Application Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-194">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="111e4-195">Neue Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="111e4-195">New Cmdlets added:</span></span>
      - <span data-ttu-id="111e4-196">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="111e4-196">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="111e4-197">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="111e4-197">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="111e4-198">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="111e4-198">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="111e4-199">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="111e4-199">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="111e4-200">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="111e4-200">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="111e4-201">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="111e4-201">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="111e4-202">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="111e4-202">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="111e4-203">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="111e4-203">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="111e4-204">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="111e4-204">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="111e4-205">Cmdlets mit optionalem Parameter „-TrustedRootCertificate“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-205">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="111e4-206">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="111e4-206">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="111e4-207">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="111e4-207">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="111e4-208">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="111e4-208">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="111e4-209">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="111e4-209">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="111e4-210">Cmdlets mit optionalem Parameter „-AutoscaleConfiguration“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-210">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="111e4-211">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="111e4-211">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="111e4-212">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="111e4-212">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="111e4-213">Cmdlet für Schnittstellenendpunkt Get-AzureInterfaceEndpoint hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-213">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="111e4-214">Unterstützung für mehrere Adresspräfixe in einem Subnetz hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="111e4-214">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="111e4-215">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="111e4-215">Updated cmdlets:</span></span>
  - <span data-ttu-id="111e4-216">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-216">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="111e4-217">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-217">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="111e4-218">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-218">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="111e4-219">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-219">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="111e4-220">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="111e4-220">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="111e4-221">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-221">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="111e4-222">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-222">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="111e4-223">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-223">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="111e4-224">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="111e4-224">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="111e4-225">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="111e4-225">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="111e4-226">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="111e4-226">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="111e4-227">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-227">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="111e4-228">New-AzureRmNetworkInterfaceIpConfig – Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-228">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="111e4-229">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-229">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="111e4-230">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-230">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="111e4-231">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-231">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="111e4-232">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-232">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="111e4-233">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-233">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="111e4-234">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="111e4-234">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="111e4-235">Cmdlets für die Subnetzdelegierung hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="111e4-235">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="111e4-236">New-AzureRmDelegation: Erstellt eine neue Delegierung, die einem Subnetz hinzugefügt werden kann</span><span class="sxs-lookup"><span data-stu-id="111e4-236">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="111e4-237">Remove-AzureRmDelegation: Nutzt ein Subnetz und entfernt den bereitgestellten Delegierungsnamen aus diesem Subnetz</span><span class="sxs-lookup"><span data-stu-id="111e4-237">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="111e4-238">Add-AzureRmDelegation: Nutzt ein Subnetz und fügt den angegebenen Dienstnamen diesem Subnetz als Delegierung hinzu</span><span class="sxs-lookup"><span data-stu-id="111e4-238">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="111e4-239">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="111e4-239">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="111e4-240">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="111e4-240">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="111e4-241">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="111e4-241">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="111e4-242">Unterstützung für verwalteten Datenträger</span><span class="sxs-lookup"><span data-stu-id="111e4-242">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="111e4-243">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="111e4-243">AzureRM.RedisCache</span></span>
* <span data-ttu-id="111e4-244">Insights-Abhängigkeit aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="111e4-244">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="111e4-245">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="111e4-245">AzureRM.Resources</span></span>
* <span data-ttu-id="111e4-246">New-AzureRmResourceGroupDeployment mit neuem Parameter „RollbackAction“ aktualisieren</span><span class="sxs-lookup"><span data-stu-id="111e4-246">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="111e4-247">Unterstützung für OnErrorDeployment mit dem neuen Parameter hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="111e4-247">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="111e4-248">Unterstützung für verwaltete Identität in Richtlinienzuweisungen.</span><span class="sxs-lookup"><span data-stu-id="111e4-248">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="111e4-249">Parameter mit Standardwerten sind nicht mehr erforderlich, wenn eine Richtlinie mit „New-AzureRmPolicyAssignment“ zugewiesen wird</span><span class="sxs-lookup"><span data-stu-id="111e4-249">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="111e4-250">Neues Cmdlet „Get-AzureRmPolicyAlias“ zum Abrufen von Richtlinienaliasen hinzufügen</span><span class="sxs-lookup"><span data-stu-id="111e4-250">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="111e4-251">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="111e4-251">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="111e4-252">Problem #7161 behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-252">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="111e4-253">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="111e4-253">AzureRM.SignalR</span></span>
* <span data-ttu-id="111e4-254">SKU-Namen auf Free_F1 und Standard_S1 aktualisieren</span><span class="sxs-lookup"><span data-stu-id="111e4-254">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="111e4-255">Versionsfeld zum PSSignalRResource-Objekt und Verbindungszeichenfolge zum PSSignalRKeys-Objekt hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="111e4-255">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="111e4-256">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="111e4-256">AzureRM.Storage</span></span>
* <span data-ttu-id="111e4-257">Unterstützung für Unveränderlichkeitsrichtlinie in AzureRm.Storage</span><span class="sxs-lookup"><span data-stu-id="111e4-257">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="111e4-258">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="111e4-258">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="111e4-259">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="111e4-259">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="111e4-260">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="111e4-260">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="111e4-261">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="111e4-261">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="111e4-262">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="111e4-262">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="111e4-263">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="111e4-263">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="111e4-264">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="111e4-264">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="111e4-265">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="111e4-265">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="111e4-266">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="111e4-266">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="111e4-267">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="111e4-267">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="111e4-268">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="111e4-268">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="111e4-269">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="111e4-269">AzureRM.Websites</span></span>
* <span data-ttu-id="111e4-270">Zwei neue Cmdlets hinzugefügt: Get-AzureRmDeletedWebApp und Restore-AzureRmDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="111e4-270">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="111e4-271">New-AzureRmAppServicePlan -HyperV-Switch für „App Service-Plan erstellen“ mit Windows-Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-271">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="111e4-272">New-AzureRmWebApp/New-AzureRmWebAppSlot/Set-AzureRmWebApp/Set-AzureRmWebAppSlot: Neue Parameter (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) für die Erstellung und Verwaltung der Windows-Container-App hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-272">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="111e4-273">6.8.1: August 2018</span><span class="sxs-lookup"><span data-stu-id="111e4-273">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="111e4-274">Allgemein</span><span class="sxs-lookup"><span data-stu-id="111e4-274">General</span></span>
* <span data-ttu-id="111e4-275">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="111e4-275">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="111e4-276">Allgemeine Laufzeitassemblys aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-276">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="111e4-277">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="111e4-277">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="111e4-278">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="111e4-278">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="111e4-279">Problem https://github.com/Azure/azure-powershell/issues/6603 behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-279">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="111e4-280">Die Cmdlets „Import-AzureRmApiManagementApi“ und „\*-AzureRmApiManagementCertificate“ können jetzt relative Pfade verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="111e4-280">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="111e4-281">Problem https://github.com/Azure/azure-powershell/issues/6879 behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-281">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="111e4-282">„CertificateInformation“ ist eine festlegbare Eigenschaft, die die ordnungsgemäße Funktionsweise des Cmdlets „Set-AzureRmApiManagement“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="111e4-282">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="111e4-283">Behoben durch Upgrade auf NuGet-Paket „4.0.4-preview“</span><span class="sxs-lookup"><span data-stu-id="111e4-283">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="111e4-284">Problem https://github.com/Azure/azure-powershell/issues/6853 behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-284">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="111e4-285">OData-Filter für die Suche anhand des Namens korrigiert (Produkt)</span><span class="sxs-lookup"><span data-stu-id="111e4-285">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="111e4-286">Problem https://github.com/Azure/azure-powershell/issues/6814 behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-286">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="111e4-287">OData-Filter für die Suche anhand des Namens korrigiert (API)</span><span class="sxs-lookup"><span data-stu-id="111e4-287">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="111e4-288">Unterstützung für AzureMonitor-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-288">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="111e4-289">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="111e4-289">AzureRM.Compute</span></span>
* <span data-ttu-id="111e4-290">Problem des fehlenden Ziels in der Fehlerausgabe behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-290">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="111e4-291">Problem mit dem Speicherkontotyp für den virtuellen Computer mit verwaltetem Datenträgern behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-291">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="111e4-292">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="111e4-292">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="111e4-293">AEM-Erweiterungs-Cmdlets für andere Umgebungen (etwa Azure China) korrigiert</span><span class="sxs-lookup"><span data-stu-id="111e4-293">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="111e4-294">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="111e4-294">AzureRM.Network</span></span>
* <span data-ttu-id="111e4-295">Standarddarstellung der Cmdlet-Ausgabe in Tabellenansicht geändert</span><span class="sxs-lookup"><span data-stu-id="111e4-295">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="111e4-296">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="111e4-296">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="111e4-297">Fehler in „Update-AzureRmPowerBIEmbeddedCapacity“ beim Skalieren der angehaltenen Kapazität behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-297">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="111e4-298">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="111e4-298">AzureRM.Resources</span></span>
* <span data-ttu-id="111e4-299">Problem beim Erstellen verwalteter Anwendungen über Marketplace behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-299">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="111e4-300">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="111e4-300">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="111e4-301">Behobene Probleme</span><span class="sxs-lookup"><span data-stu-id="111e4-301">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="111e4-302">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="111e4-302">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="111e4-303">Unterstützung für Routingmethode „MultiValue“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-303">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="111e4-304">Neuer Parameter „MaxReturn“ für Routingtyp „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="111e4-304">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="111e4-305">Unterstützung für Subnetzroutingmethode hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-305">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="111e4-306">Unterstützung für IP-Adressbereiche (Subnetze) in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="111e4-306">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="111e4-307">Unterstützung für benutzerdefinierte Header in Profilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-307">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="111e4-308">Unterstützung für erwartete Statuscodebereiche in Profilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-308">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="111e4-309">Unterstützung für benutzerdefinierte Header in Endpunkten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-309">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="111e4-310">6.8.0: August 2018</span><span class="sxs-lookup"><span data-stu-id="111e4-310">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="111e4-311">Allgemein</span><span class="sxs-lookup"><span data-stu-id="111e4-311">General</span></span>
* <span data-ttu-id="111e4-312">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="111e4-312">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="111e4-313">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="111e4-313">AzureRM.Profile</span></span>
* <span data-ttu-id="111e4-314">Ablaufeigenschaft zu Token hinzugefügt, die während „Connect-AzureRmAccount“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="111e4-314">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="111e4-315">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="111e4-315">AzureRM.Compute</span></span>
* <span data-ttu-id="111e4-316">Problem des fehlenden Ziels in der Fehlerausgabe behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-316">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="111e4-317">Problem mit dem Speicherkontotyp für den virtuellen Computer mit verwaltetem Datenträgern behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-317">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="111e4-318">AEM-Erweiterungs-Cmdlets für andere Umgebungen (etwa Azure China) korrigiert</span><span class="sxs-lookup"><span data-stu-id="111e4-318">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="111e4-319">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="111e4-319">AzureRM.IotHub</span></span>
* <span data-ttu-id="111e4-320">Beispiele für „New-AzureRmIotHubExportDevices“ und „New-AzureRmIotHubImportDevices“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="111e4-320">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="111e4-321">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="111e4-321">AzureRM.Network</span></span>
* <span data-ttu-id="111e4-322">Standarddarstellung von Modellen in Tabellenansicht geändert</span><span class="sxs-lookup"><span data-stu-id="111e4-322">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="111e4-323">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="111e4-323">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="111e4-324">Fehler in „Update-AzureRmPowerBIEmbeddedCapacity“ beim Skalieren der angehaltenen Kapazität behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-324">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="111e4-325">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="111e4-325">AzureRM.Resources</span></span>
* <span data-ttu-id="111e4-326">Problem beim Erstellen der verwalteten Anwendung über Marketplace behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-326">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="111e4-327">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="111e4-327">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="111e4-328">Fehlerbehebung</span><span class="sxs-lookup"><span data-stu-id="111e4-328">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="111e4-329">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="111e4-329">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="111e4-330">Unterstützung für Routingmethode „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="111e4-330">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="111e4-331">Neuer Parameter „MaxReturn“ für Routingtyp „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="111e4-331">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="111e4-332">Unterstützung für Subnetzroutingmethode</span><span class="sxs-lookup"><span data-stu-id="111e4-332">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="111e4-333">Unterstützung für IP-Adressbereiche (Subnetze) in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="111e4-333">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="111e4-334">Unterstützung für benutzerdefinierte Header in Profilen</span><span class="sxs-lookup"><span data-stu-id="111e4-334">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="111e4-335">Unterstützung für erwartete Statuscodebereiche in Profilen</span><span class="sxs-lookup"><span data-stu-id="111e4-335">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="111e4-336">Unterstützung für benutzerdefinierte Header in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="111e4-336">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="111e4-337">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="111e4-337">AzureRM.Websites</span></span>
* <span data-ttu-id="111e4-338">Das Problem, dass die Standardressourcengruppe falsch festgelegt wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="111e4-338">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="111e4-339">6.7.0: August 2018</span><span class="sxs-lookup"><span data-stu-id="111e4-339">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="111e4-340">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="111e4-340">AzureRM.Profile</span></span>
* <span data-ttu-id="111e4-341">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-341">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="111e4-342">Benutzer-ID zum Standardkontextnamen hinzugefügt, um Kontextkonflikte zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="111e4-342">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="111e4-343">Probleme mit „Clear-AzureRmContext“ behoben, die Fehler beim Auswählen eines Kontexts verursacht haben (6398)</span><span class="sxs-lookup"><span data-stu-id="111e4-343">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="111e4-344">Ermöglicht, dass für „Connect-AzureRmAccount“ die Mandantendomäne an den Parameter „-TenantId“ übergeben wird</span><span class="sxs-lookup"><span data-stu-id="111e4-344">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="111e4-345">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="111e4-345">Azure.Storage</span></span>
* <span data-ttu-id="111e4-346">Begrenzung von 5 TB für das Kontingent der Azure-Dateifreigabe entfernt</span><span class="sxs-lookup"><span data-stu-id="111e4-346">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="111e4-347">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="111e4-347">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="111e4-348">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="111e4-348">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="111e4-349">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-349">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="111e4-350">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="111e4-350">Azure.AnalysisServices</span></span>
* <span data-ttu-id="111e4-351">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-351">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="111e4-352">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="111e4-352">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="111e4-353">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-353">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="111e4-354">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="111e4-354">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="111e4-355">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-355">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="111e4-356">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="111e4-356">AzureRM.Automation</span></span>
* <span data-ttu-id="111e4-357">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-357">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="111e4-358">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="111e4-358">AzureRM.Backup</span></span>
* <span data-ttu-id="111e4-359">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-359">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="111e4-360">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="111e4-360">AzureRM.Batch</span></span>
* <span data-ttu-id="111e4-361">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-361">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="111e4-362">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="111e4-362">AzureRM.Billing</span></span>
* <span data-ttu-id="111e4-363">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-363">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="111e4-364">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="111e4-364">AzureRM.Cdn</span></span>
* <span data-ttu-id="111e4-365">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-365">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="111e4-366">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="111e4-366">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="111e4-367">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-367">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="111e4-368">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="111e4-368">AzureRM.Compute</span></span>
* <span data-ttu-id="111e4-369">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-369">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="111e4-370">EvictionPolicy-Parameter zu „New-AzureRmVmssConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-370">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="111e4-371">Standort in „DiskFileParameterSet“ von „New-AzureRmVm“ angeben, wenn kein Ort angegeben ist</span><span class="sxs-lookup"><span data-stu-id="111e4-371">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="111e4-372">Parameterbeschreibung in „Save-AzureRmVMImage“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="111e4-372">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="111e4-373">Cmdlet „Get-AzureRmVMDiskEncryptionStatus“ für bestimmte Szenarien im Zusammenhang mit einem Durchlauf korrigiert</span><span class="sxs-lookup"><span data-stu-id="111e4-373">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="111e4-374">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="111e4-374">AzureRM.Consumption</span></span>
* <span data-ttu-id="111e4-375">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-375">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="111e4-376">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="111e4-376">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="111e4-377">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-377">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="111e4-378">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="111e4-378">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="111e4-379">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-379">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="111e4-380">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="111e4-380">AzureRM.DataFactories</span></span>
* <span data-ttu-id="111e4-381">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-381">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="111e4-382">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="111e4-382">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="111e4-383">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-383">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="111e4-384">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="111e4-384">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="111e4-385">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-385">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="111e4-386">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="111e4-386">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="111e4-387">Debuggen korrigiert, wenn „DebugPreference“ über die PowerShell-Befehlszeile festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="111e4-387">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="111e4-388">Beispiel für „Set-AzureRmDataLakeStoreItemAcl“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-388">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="111e4-389">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="111e4-389">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="111e4-390">Beispiel für „Set-AzureRmDataLakeStoreItemAclEntry“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-390">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="111e4-391">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="111e4-391">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="111e4-392">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-392">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="111e4-393">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="111e4-393">AzureRM.Dns</span></span>
* <span data-ttu-id="111e4-394">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-394">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="111e4-395">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="111e4-395">AzureRM.EventGrid</span></span>
* <span data-ttu-id="111e4-396">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-396">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="111e4-397">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="111e4-397">AzureRM.EventHub</span></span>
* <span data-ttu-id="111e4-398">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-398">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="111e4-399">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="111e4-399">AzureRM.HDInsight</span></span>
* <span data-ttu-id="111e4-400">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-400">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="111e4-401">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="111e4-401">AzureRM.Insights</span></span>
* <span data-ttu-id="111e4-402">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-402">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="111e4-403">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="111e4-403">AzureRM.IotHub</span></span>
* <span data-ttu-id="111e4-404">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-404">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="111e4-405">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="111e4-405">AzureRM.KeyVault</span></span>
* <span data-ttu-id="111e4-406">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-406">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="111e4-407">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="111e4-407">AzureRM.LogicApp</span></span>
* <span data-ttu-id="111e4-408">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-408">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="111e4-409">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="111e4-409">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="111e4-410">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-410">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="111e4-411">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="111e4-411">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="111e4-412">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-412">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="111e4-413">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="111e4-413">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="111e4-414">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-414">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="111e4-415">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="111e4-415">AzureRM.Media</span></span>
* <span data-ttu-id="111e4-416">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-416">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="111e4-417">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="111e4-417">AzureRM.Network</span></span>
* <span data-ttu-id="111e4-418">Beispiel für „Set-AzureRmLocalNetworkGateway“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-418">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="111e4-419">Beispiele und Beschreibungen für „Add-AzureRmVirtualNetworkGatewayIpConfig“, „Get-AzureRmVirtualNetworkGatewayConnectionSharedKey“ und „New-AzureRmVirtualNetworkGatewayConnection“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-419">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="111e4-420">Beispiele für „Remove-AzureRmVirtualNetworkGatewayIpConfig“ und „Reset-AzureRmVirtualNetworkGateway“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-420">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="111e4-421">Beispiel für „Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-421">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="111e4-422">Beispiel für „Set-AzureRmVirtualNetworkGatewayConnectionSharedKey“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-422">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="111e4-423">Beispiel für „Set-AzureRmVirtualNetworkGatewayConnection“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-423">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="111e4-424">Cmdlets für „ApplicationSecurityGroup“, „RouteTable“ und „Usage“ mithilfe des aktuellen Code-Generators erneut erstellt</span><span class="sxs-lookup"><span data-stu-id="111e4-424">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="111e4-425">Deutlichere Formulierung der Fehlermeldung für „Get-AzureRmVirtualNetworkSubnetConfig“, wenn ein nicht vorhandenes Subnetz abgerufen wird</span><span class="sxs-lookup"><span data-stu-id="111e4-425">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="111e4-426">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="111e4-426">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="111e4-427">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-427">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="111e4-428">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="111e4-428">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="111e4-429">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-429">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="111e4-430">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="111e4-430">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="111e4-431">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-431">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="111e4-432">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="111e4-432">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="111e4-433">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-433">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="111e4-434">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="111e4-434">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="111e4-435">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-435">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="111e4-436">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="111e4-436">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="111e4-437">Richtlinienfilter zum Cmdlet „Get-AzureRmRecoveryServicesBackItem“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="111e4-437">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="111e4-438">Der Befehl gibt die Liste der Sicherungselemente zurück, die durch die angegebene Richtlinien-ID geschützt sind.</span><span class="sxs-lookup"><span data-stu-id="111e4-438">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="111e4-439">„Microsoft.Azure.Management.RecoveryServices.Backup“ auf Version 3.0.0-preview aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-439">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="111e4-440">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-440">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="111e4-441">TargetResourceGroupName-Parameter zu „Restore-AzureRmRecoveryServicesBackupItem“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="111e4-441">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="111e4-442">Die Ressourcengruppe, in der die verwalteten Datenträger wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="111e4-442">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="111e4-443">Gilt für die Sicherung des virtuellen Computers mit verwalteten Datenträgern.</span><span class="sxs-lookup"><span data-stu-id="111e4-443">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="111e4-444">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="111e4-444">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="111e4-445">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-445">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="111e4-446">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="111e4-446">AzureRM.RedisCache</span></span>
* <span data-ttu-id="111e4-447">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-447">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="111e4-448">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="111e4-448">AzureRM.Relay</span></span>
* <span data-ttu-id="111e4-449">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-449">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="111e4-450">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="111e4-450">AzureRM.Resources</span></span>
* <span data-ttu-id="111e4-451">Unterstützung der Vorlagenbereitstellung im Abonnementbereich.</span><span class="sxs-lookup"><span data-stu-id="111e4-451">Support template deployment at subscription scope.</span></span> <span data-ttu-id="111e4-452">Neue Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="111e4-452">Add new Cmdlets:</span></span>
    - <span data-ttu-id="111e4-453">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="111e4-453">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="111e4-454">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="111e4-454">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="111e4-455">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="111e4-455">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="111e4-456">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="111e4-456">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="111e4-457">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="111e4-457">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="111e4-458">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="111e4-458">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="111e4-459">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="111e4-459">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="111e4-460">Problem behoben, aufgrund dessen beim Übergeben eines Kontexts an „Set-AzureRmResource“ ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="111e4-460">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="111e4-461">Beispiel in „New-AzureRmResourceGroupDeployment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="111e4-461">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="111e4-462">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-462">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="111e4-463">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="111e4-463">AzureRM.Scheduler</span></span>
* <span data-ttu-id="111e4-464">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-464">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="111e4-465">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="111e4-465">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="111e4-466">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-466">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="111e4-467">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="111e4-467">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="111e4-468">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-468">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="111e4-469">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="111e4-469">AzureRM.Sql</span></span>
* <span data-ttu-id="111e4-470">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-470">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="111e4-471">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="111e4-471">AzureRM.Storage</span></span>
* <span data-ttu-id="111e4-472">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-472">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="111e4-473">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="111e4-473">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="111e4-474">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-474">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="111e4-475">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="111e4-475">AzureRM.Tags</span></span>
* <span data-ttu-id="111e4-476">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-476">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="111e4-477">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="111e4-477">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="111e4-478">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-478">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="111e4-479">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="111e4-479">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="111e4-480">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-480">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="111e4-481">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="111e4-481">AzureRM.Websites</span></span>
* <span data-ttu-id="111e4-482">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-482">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="111e4-483">6.6.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="111e4-483">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="111e4-484">Allgemein</span><span class="sxs-lookup"><span data-stu-id="111e4-484">General</span></span>
* <span data-ttu-id="111e4-485">Alle Hilfedateien aktualisiert, um vollständige Parametertypen und die richtigen Eingabe/Ausgabe-Typen einzuschließen.</span><span class="sxs-lookup"><span data-stu-id="111e4-485">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="111e4-486">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="111e4-486">AzureRM.Profile</span></span>
* <span data-ttu-id="111e4-487">Bibliothek „Common.Strategy“ aktualisiert, um überprüfen zu können, ob die aktuelle Konfiguration für eine Ressource mit der Zielressource kompatibel ist.</span><span class="sxs-lookup"><span data-stu-id="111e4-487">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="111e4-488">ps1xml-Typen zu „Common.Storage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-488">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="111e4-489">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="111e4-489">Azure.Storage</span></span>
* <span data-ttu-id="111e4-490">Unterstützung zum Abrufen von Speicherkontext aus „DefaultProfile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-490">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="111e4-491">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-491">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="111e4-492">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="111e4-492">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="111e4-493">Problem https://github.com/Azure/azure-powershell/issues/6370 behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-493">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="111e4-494">Fehler in Automapper behoben, um „PsApiManagementApi“ in „ApiContract“ zu verschieben</span><span class="sxs-lookup"><span data-stu-id="111e4-494">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="111e4-495">Problem https://github.com/Azure/azure-powershell/issues/6515 behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-495">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="111e4-496">Fehler in „File.Save“ behoben, um Überladung mit Codierungstyp zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="111e4-496">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="111e4-497">Problem https://github.com/Azure/azure-powershell/issues/6560 behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-497">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="111e4-498">Upgrade auf Nuget-Version 4.0.3 durchgeführt, in der Musterausnahme in „apiId“ behoben wurde</span><span class="sxs-lookup"><span data-stu-id="111e4-498">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="111e4-499">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="111e4-499">AzureRM.Compute</span></span>
* <span data-ttu-id="111e4-500">Das Problem, aufgrund dessen beim Erstellen eines virtuellen Computers mithilfe von „DiskFileParameterSet“ in „New-AzureRmVm“ wegen einer Umbenennung des Speicherkontotyps „PremiumLRS“ ein Fehler auftrat, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="111e4-500">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="111e4-501">Cmdlet „Invoke-AzureRmVMRunCommand“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="111e4-501">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="111e4-502">„Get-AzureRmAvailabilitySet“ aktualisiert, um die Auflistung aller Verfügbarkeitsgruppen in einem Abonnement zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="111e4-502">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="111e4-503">(ResouceGroupName-Parameter ist jetzt optional.)</span><span class="sxs-lookup"><span data-stu-id="111e4-503">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="111e4-504">„SimpleParameterSet“ von „New-AzureRmVm“ aktualisiert, um Accelerated Networking auf kompatiblen virtuellen Computern zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="111e4-504">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="111e4-505">Einfacher Parametersatz „New-AzureRmVmss“ aktualisiert, sodass das Erstellen der VMSS fehlschlägt, wenn bereits ein benutzerdefinierter LB vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="111e4-505">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="111e4-506">Beispiel für „New-AzureRmDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-506">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="111e4-507">Beispiel für „New-AzureRmVM“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-507">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="111e4-508">Beschreibung für „Set-AzureRmVMOSDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-508">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="111e4-509">Beispiel 1 für „Set-AzureRmVMBginfoExtension“ aktualisiert, um Rechtschreibung und Präfix zu korrigieren.</span><span class="sxs-lookup"><span data-stu-id="111e4-509">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="111e4-510">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="111e4-510">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="111e4-511">ADF .Net SDK-Version auf 1.1.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="111e4-511">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="111e4-512">Unterstützung der Freigabe der selbstgehosteten Integration Runtime über Data Factorys hinweg.</span><span class="sxs-lookup"><span data-stu-id="111e4-512">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="111e4-513">Neuer Parameter „-SharedIntegrationRuntimeResourceId“ zu Cmdlet „Set-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="111e4-513">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="111e4-514">Neuer optionaler Parameter „-LinkedDataFactoryName“ zu Cmdlet „Remove-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="111e4-514">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="111e4-515">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="111e4-515">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="111e4-516">DataPlane SDK-Version (Microsoft.Azure.DataLake.Store) auf 1.1.9 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-516">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="111e4-517">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="111e4-517">AzureRM.EventHub</span></span>
* <span data-ttu-id="111e4-518">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-518">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="111e4-519">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="111e4-519">AzureRM.Insights</span></span>
* <span data-ttu-id="111e4-520">Formatierung von „OutputType“ in Hilfedateien korrigiert</span><span class="sxs-lookup"><span data-stu-id="111e4-520">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="111e4-521">Verwendung von Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span><span class="sxs-lookup"><span data-stu-id="111e4-521">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="111e4-522">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="111e4-522">AzureRM.KeyVault</span></span>
* <span data-ttu-id="111e4-523">Piping-Problem in „Set-AzureRmKeyVaultAccessPolicy“ behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-523">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="111e4-524">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="111e4-524">AzureRM.Network</span></span>
* <span data-ttu-id="111e4-525">Beispiele für LoadBalancerInboundNatPoolConfig-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="111e4-525">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="111e4-526">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="111e4-526">AzureRM.Resources</span></span>
* <span data-ttu-id="111e4-527">Problem beim Angeben sowohl des Tag-Namens als auch des Werts für „Get-AzureRmResource“ behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-527">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="111e4-528">Piping-Szenario mit „Set-AzureRmResource“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="111e4-528">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="111e4-529">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="111e4-529">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="111e4-530">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-530">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="111e4-531">Einige Probleme behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-531">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="111e4-532">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="111e4-532">AzureRM.Sql</span></span>
* <span data-ttu-id="111e4-533">Unterstützung für Advanced Threat Protection für Server bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="111e4-533">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="111e4-534">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="111e4-534">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="111e4-535">Unterstützung für Sicherheitsrisikobewertung bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="111e4-535">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="111e4-536">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="111e4-536">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="111e4-537">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="111e4-537">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="111e4-538">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="111e4-538">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="111e4-539">Beispiel in „Remove-AzureRmSqlServerFirewallRule“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="111e4-539">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="111e4-540">Falsche Verarbeitung von „datetime“ für nicht US-basierte Kultur in „Get-AzureSqlSyncGroupLog“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="111e4-540">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="111e4-541">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="111e4-541">AzureRM.Storage</span></span>
* <span data-ttu-id="111e4-542">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-542">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="111e4-543">Cmdlet-Ausgabe von „StorageAccount“ in Tabellenansicht anzeigen</span><span class="sxs-lookup"><span data-stu-id="111e4-543">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="111e4-544">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="111e4-544">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="111e4-545">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="111e4-545">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="111e4-546">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="111e4-546">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="111e4-547">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="111e4-547">AzureRM.Tags</span></span>
* <span data-ttu-id="111e4-548">Falsche Anweisung aus Tag-Cmdlet-Hilfe entfernt</span><span class="sxs-lookup"><span data-stu-id="111e4-548">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="111e4-549">6.5.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="111e4-549">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="111e4-550">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="111e4-550">AzureRM.Profile</span></span>
* <span data-ttu-id="111e4-551">Hilfe für „Get-AzureRmContextAutosaveSetting“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-551">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="111e4-552">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="111e4-552">Azure.Storage</span></span>
* <span data-ttu-id="111e4-553">Unterstützung des Blob- oder Dateiuploads mit lesegeschütztem SAS-Token</span><span class="sxs-lookup"><span data-stu-id="111e4-553">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="111e4-554">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="111e4-554">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="111e4-555">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="111e4-555">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="111e4-556">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="111e4-556">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="111e4-557">Erforderliche Eigenschaft „ResourceGroupName“ zu AS hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="111e4-557">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="111e4-558">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="111e4-558">AzureRM.Automation</span></span>
* <span data-ttu-id="111e4-559">Hilfe aktualisiert und Beispiel für „New-AzureRMAutomationSchedule“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-559">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="111e4-560">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="111e4-560">AzureRM.Compute</span></span>
* <span data-ttu-id="111e4-561">Parameter „-Tag“ zu „Update/New-AzureRmAvailabilitySet“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-561">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="111e4-562">Beispiel für „Add-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-562">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="111e4-563">Beispiele für „Remove-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-563">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="111e4-564">Hilfe für „Set-AzureRmVMAccessExtension“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-564">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="111e4-565">„SimpleParameterSet“ für „New-AzureRmVmss“ so aktualisiert, dass „SinglePlacementGroup“ standardmäßig auf „false“ festgelegt ist, und Switch-Parameter „SinglePlacementGroup“ hinzugefügt, der dem Benutzer das Erstellen der VMSS in einer einzelnen Platzierungsgruppe ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="111e4-565">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="111e4-566">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="111e4-566">AzureRM.EventHub</span></span>
* <span data-ttu-id="111e4-567">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSEventHubDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="111e4-567">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="111e4-568">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="111e4-568">AzureRM.KeyVault</span></span>
* <span data-ttu-id="111e4-569">Fehlermeldung für „Set-AzureRmKeyVaultAccessPolicy“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-569">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="111e4-570">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="111e4-570">AzureRM.LogicApp</span></span>
* <span data-ttu-id="111e4-571">Fehler „Parametersatz konnte nicht aufgelöst werden“ in „New-AzureRmLogicApp“behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-571">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="111e4-572">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="111e4-572">AzureRM.Network</span></span>
* <span data-ttu-id="111e4-573">Peering über mehrere virtuelle Netzwerke in mehreren Mandanten für „Set/Add-AzureRmVirtualNetworkPeering“ aktiviert</span><span class="sxs-lookup"><span data-stu-id="111e4-573">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="111e4-574">Folgende Cmdlets für Application Gateway aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-574">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="111e4-575">New-AzureRmApplicationGateway: EnableFIPS-Flag und Zonenunterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-575">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="111e4-576">New-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-576">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="111e4-577">Set-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-577">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="111e4-578">RouteTable-Cmdlets mit aktueller Generatorversion erneut generiert</span><span class="sxs-lookup"><span data-stu-id="111e4-578">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="111e4-579">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="111e4-579">AzureRM.Relay</span></span>
* <span data-ttu-id="111e4-580">Markdowndateien aktualisiert, Problem mit Parametername in Beispiel behoben</span><span class="sxs-lookup"><span data-stu-id="111e4-580">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="111e4-581">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="111e4-581">AzureRM.Resources</span></span>
* <span data-ttu-id="111e4-582">Roleassignment- und roledefinition-Cmdlets aktualisiert:</span><span class="sxs-lookup"><span data-stu-id="111e4-582">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="111e4-583">Zusätzliche roledefinition-Aufrufe entfernt, die als Teil des Pagings durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="111e4-583">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="111e4-584">Get-AzureRmRoleAssignment-Cmdlet korrigiert</span><span class="sxs-lookup"><span data-stu-id="111e4-584">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="111e4-585">Befehlsparameterfunktion von „-ExpandPrincipalGroups“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="111e4-585">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="111e4-586">Problem mit „Get-AzureRmResource“ behoben, aufgrund dessen die Groß-/Kleinschreibung des Parameters „-ResourceType“ beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="111e4-586">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="111e4-587">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="111e4-587">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="111e4-588">top- und skip-Parameter zu Listen-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-588">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="111e4-589">Cmdlets für die Migration von Standard- zu Premium-Namespace hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="111e4-589">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="111e4-590">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="111e4-590">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="111e4-591">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="111e4-591">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="111e4-592">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="111e4-592">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="111e4-593">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="111e4-593">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="111e4-594">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="111e4-594">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="111e4-595">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSServiceBusDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="111e4-595">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="111e4-596">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="111e4-596">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="111e4-597">Beispiel für „New-AzureRmServiceFabricCluster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-597">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="111e4-598">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="111e4-598">AzureRM.Sql</span></span>
* <span data-ttu-id="111e4-599">Neue Cmdlets für „Management.Sql“ hinzugefügt, um Kunden das Hinzufügen des TDE-Zertifikats zu einer SQL Server-Instanz oder einer verwalteten Instanz zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="111e4-599">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="111e4-600">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="111e4-600">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="111e4-601">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="111e4-601">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="111e4-602">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="111e4-602">AzureRM.Websites</span></span>
* <span data-ttu-id="111e4-603">Wenn `Set-AzureRmWebApp -AssignIdentity` und `Set-AzureRmWebAppSlot -AssignIdentity` auf „false“ festgelegt sind, wird jetzt die Identity-Eigenschaft aus dem Websiteobjekt entfernt. Auch das Vorschau-Tag wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="111e4-603">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="111e4-604">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics`-Beispiel aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-604">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="111e4-605">Unterstützung von `Set-AzureRmWebApp -PhpVersion` als gültige PHP-Version eingestellt</span><span class="sxs-lookup"><span data-stu-id="111e4-605">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="111e4-606">6.4.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="111e4-606">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="111e4-607">Allgemein</span><span class="sxs-lookup"><span data-stu-id="111e4-607">General</span></span>
* <span data-ttu-id="111e4-608">Formatierung von OutputType in Hilfedateien für die meisten Module korrigiert</span><span class="sxs-lookup"><span data-stu-id="111e4-608">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="111e4-609">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="111e4-609">AzureRM.Profile</span></span>
* <span data-ttu-id="111e4-610">Attribut „Ps1Xml“ wurde den Standardausgabetypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-610">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="111e4-611">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="111e4-611">AzureRM.Compute</span></span>
* <span data-ttu-id="111e4-612">IP-Tag-Funktion für VMSS</span><span class="sxs-lookup"><span data-stu-id="111e4-612">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="111e4-613">Cmdlet „New-AzureRmVmssIpTagConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-613">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="111e4-614">IpTag-Parameter zu „New-AzureRmVmssIpConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-614">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="111e4-615">Funktion für automatisches Betriebssystemrollback für VMSS</span><span class="sxs-lookup"><span data-stu-id="111e4-615">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="111e4-616">DisableAutoRollback-Parameter zu „New-AzureRmVmssConfig“ und „Update-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-616">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="111e4-617">Funktion für Upgradeverlauf des Betriebssystems für VMSS</span><span class="sxs-lookup"><span data-stu-id="111e4-617">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="111e4-618">Switch-Parameter „OSUpgradeHistory“ zu „Get-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-618">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="111e4-619">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="111e4-619">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="111e4-620">Unterstützung für Katalog-ACLs über die folgenden Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="111e4-620">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="111e4-621">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="111e4-621">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="111e4-622">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="111e4-622">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="111e4-623">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="111e4-623">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="111e4-624">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="111e4-624">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="111e4-625">Abbruchunterstützung und Nachverfolgung des Fortschritts für „Set-AzureRmDataLakeStoreItemAclEntry“, „Remove-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-625">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="111e4-626">Abbruchunterstützung „Export-AzureRmDataLakeStoreChildItemProperties“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-626">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="111e4-627">Leerung von Debugmeldungen für Cmdlets korrigiert, die rekursive Vorgänge durchführt</span><span class="sxs-lookup"><span data-stu-id="111e4-627">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="111e4-628">Speicherort des Test von DataLake-Cmdlets korrigiert</span><span class="sxs-lookup"><span data-stu-id="111e4-628">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="111e4-629">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="111e4-629">AzureRM.EventHub</span></span>
* <span data-ttu-id="111e4-630">Optionaler Parameter „MaxCount“ zu Listenvorgangs-Cmdlets „Get-AzureRmEventHub“ und „Get-AzureRmEventHubConsumerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-630">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="111e4-631">Problem in Cmdlet „New-AzureRmEventHub“ behoben, aufgrund dessen beim Erstellen einer neuen EventHub-Instanz mindestens ein Parameter benötigt wurde.</span><span class="sxs-lookup"><span data-stu-id="111e4-631">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="111e4-632">Standardparametersatz wurde bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="111e4-632">Provided Default Parameter set.</span></span>
* <span data-ttu-id="111e4-633">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmEventHubKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="111e4-633">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="111e4-634">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="111e4-634">AzureRM.KeyVault</span></span>
* <span data-ttu-id="111e4-635">Problem behoben, aufgrund dessen von „Get-AzureRmKeyVault -Tag“ alle Ressourcen zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="111e4-635">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="111e4-636">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="111e4-636">AzureRM.Network</span></span>
* <span data-ttu-id="111e4-637">Neue SKUs für zonenredundante VirtualNetworkGateways-Instanzen verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="111e4-637">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="111e4-638">Neue Befehle für Funktion hinzugefügt: ExpressRoute-Partner-APIs über ARM</span><span class="sxs-lookup"><span data-stu-id="111e4-638">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="111e4-639">Get-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-639">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="111e4-640">Set-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-640">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="111e4-641">Add-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-641">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="111e4-642">Get-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-642">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="111e4-643">Remove-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-643">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="111e4-644">Get-AzureRMExpressRouteCrossConnectionArpTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-644">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="111e4-645">Get-AzureRMExpressRouteCrossConnectionRouteTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-645">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="111e4-646">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-646">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="111e4-647">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="111e4-647">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="111e4-648">Cmdlet „Get-AzureRmRecoveryServicesBackupStatus“ wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="111e4-648">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="111e4-649">Dieses Cmdlet überprüft anhand der ID eines virtuellen Computers, ob dieser durch einen Tresor im Abonnement geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="111e4-649">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="111e4-650">Wenn ein solcher Tresor vorhanden ist, gibt das Cmdlet die Tresordetails aus.</span><span class="sxs-lookup"><span data-stu-id="111e4-650">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="111e4-651">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="111e4-651">AzureRM.Resources</span></span>
* <span data-ttu-id="111e4-652">Cmdlets vom Typ „Get-AzureRmPolicyAssignment“ aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="111e4-652">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="111e4-653">Unterstützung für das Auflisten von „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-653">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="111e4-654">Unterstützung für das Abrufen einzelner Arbeitsaufträge mit „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-654">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="111e4-655">Switches „-Effective“ und „-All“ zu Steuerparameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-655">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="111e4-656">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicyDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-656">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="111e4-657">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="111e4-657">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="111e4-658">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="111e4-658">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="111e4-659">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicySetDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-659">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="111e4-660">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="111e4-660">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="111e4-661">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="111e4-661">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="111e4-662">Unterstützung für KeyVault-Geheimnisverweis in Parametern hinzugefügt, wenn „TemplateParameterObject“ in „New-AzureRmResourceGroupDeployment“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="111e4-662">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="111e4-663">Problem behoben, aufgrund dessen, der Parameter „-EndDate“ für „New-AzureRmADAppCredential“ ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="111e4-663">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="111e4-664">Problem behoben, aufgrund dessen „Add-AzureRmADGroupMember“ eine falsche URL für Anforderungen verwendete</span><span class="sxs-lookup"><span data-stu-id="111e4-664">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="111e4-665">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="111e4-665">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="111e4-666">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmServiceBusKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="111e4-666">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="111e4-667">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="111e4-667">AzureRM.Sql</span></span>
* <span data-ttu-id="111e4-668">Benutzerdefinierte Wiederherstellungspunkte für SQLDW in Hilfe zu „New-AzureRmSqlDatabaseRestorePoint“ erläutert</span><span class="sxs-lookup"><span data-stu-id="111e4-668">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="111e4-669">Dokumentation von Parameter „-ComputeGeneration“ in mehreren Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-669">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="111e4-670">6.3.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="111e4-670">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="111e4-671">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="111e4-671">AzureRM.Profile</span></span>
* <span data-ttu-id="111e4-672">Aktualisierte Fehlermeldungen für „Enable-AzureRmContextAutoSave“</span><span class="sxs-lookup"><span data-stu-id="111e4-672">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="111e4-673">Erstellen eines Kontexts für jedes Abonnement beim Ausführen von „Connect-AzureRmAccount“ ohne vorherigen Kontext</span><span class="sxs-lookup"><span data-stu-id="111e4-673">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="111e4-674">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="111e4-674">Azure.Storage</span></span>
* <span data-ttu-id="111e4-675">Zusätzliche Informationen zum Parameter „-Permissions“ in Hilfedateien</span><span class="sxs-lookup"><span data-stu-id="111e4-675">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="111e4-676">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="111e4-676">AzureRM.Compute</span></span>
* <span data-ttu-id="111e4-677">„Get-AzureRmVmDiskEncryptionStatus“ behebt ein Problem, das bei virtuellen Computern ohne Datenträger festgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="111e4-677">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="111e4-678">Version der Computeclientbibliothek aktualisiert, um folgende Cmdlets zu korrigieren:</span><span class="sxs-lookup"><span data-stu-id="111e4-678">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="111e4-679">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="111e4-679">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="111e4-680">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="111e4-680">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="111e4-681">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="111e4-681">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="111e4-682">Die folgenden Cmdlets wurden korrigiert, um die Vorgangs-ID und den Vorgangsstatus korrekt anzuzeigen:</span><span class="sxs-lookup"><span data-stu-id="111e4-682">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="111e4-683">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="111e4-683">Start-AzureRmVM</span></span>
    - <span data-ttu-id="111e4-684">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="111e4-684">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="111e4-685">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="111e4-685">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="111e4-686">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="111e4-686">Set-AzureRmVM</span></span>
    - <span data-ttu-id="111e4-687">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="111e4-687">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="111e4-688">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="111e4-688">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="111e4-689">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="111e4-689">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="111e4-690">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="111e4-690">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="111e4-691">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="111e4-691">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="111e4-692">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="111e4-692">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="111e4-693">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="111e4-693">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="111e4-694">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="111e4-694">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="111e4-695">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="111e4-695">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="111e4-696">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="111e4-696">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="111e4-697">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="111e4-697">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="111e4-698">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="111e4-698">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="111e4-699">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="111e4-699">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="111e4-700">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="111e4-700">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="111e4-701">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="111e4-701">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="111e4-702">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="111e4-702">AzureRM.EventGrid</span></span>
* <span data-ttu-id="111e4-703">ValidateNotNullOrEmpty-Überprüfungskonditionen für „SubjectBeginsWith“/„SubjectEndsWith“ im Cmdlet „Update-AzureRmEventGridSubscription“ wurden entfernt, um bei Bedarf die Änderung dieser Parameter in eine leere Zeichenfolge zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="111e4-703">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="111e4-704">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="111e4-704">AzureRM.KeyVault</span></span>
* <span data-ttu-id="111e4-705">Ein Problem wurde behoben, aufgrund dessen bei Ausführung von „Get-AzureRmKeyVault -Tag“ keine Tags zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="111e4-705">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="111e4-706">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="111e4-706">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="111e4-707">Offizielle Veröffentlichung von Policy Insights-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="111e4-707">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="111e4-708">Verwendung der API-Version 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="111e4-708">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="111e4-709">„PolicyDefinitionReferenceId“ zu den Ergebnissen von „Get-AzureRmPolicyStateSummary“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-709">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="111e4-710">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="111e4-710">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="111e4-711">Parameter „-Vault“ zu den RecoveryServices.Backup-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="111e4-711">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="111e4-712">Bei der Übergabe wird dadurch das Cmdlet „Set-AzureRmRecoveryServicesContext“ außer Kraft gesetzt.</span><span class="sxs-lookup"><span data-stu-id="111e4-712">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="111e4-713">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="111e4-713">AzureRM.Sql</span></span>
* <span data-ttu-id="111e4-714">Aktualisiertes Beispiel in der Hilfedatei für „Get-AzureRmSqlDatabaseExpanded“</span><span class="sxs-lookup"><span data-stu-id="111e4-714">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="111e4-715">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="111e4-715">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="111e4-716">Hilfedatei für „Add-AzureRmTrafficManagerEndpointConfig“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="111e4-716">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="111e4-717">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="111e4-717">AzureRM.Websites</span></span>
* <span data-ttu-id="111e4-718">„Set-AzureRmWebApp“ wurde aktualisiert, damit „AppSettings“ bei der Verwendung von „-AssignIdentity“ nicht außer Kraft gesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="111e4-718">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="111e4-719">„New-AzureRmWebAppSlot“ wurde aktualisiert, um „AppServicePlan“ als optionalen Parameter anzuerkennen</span><span class="sxs-lookup"><span data-stu-id="111e4-719">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="111e4-720">6.2.1: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="111e4-720">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="111e4-721">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="111e4-721">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="111e4-722">PSWorkspace-Modell aktualisiert, damit das Netzwerk „type“ als Parameter verwenden kann</span><span class="sxs-lookup"><span data-stu-id="111e4-722">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="111e4-723">6.2.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="111e4-723">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="111e4-724">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="111e4-724">AzureRM.Profile</span></span>
* <span data-ttu-id="111e4-725">Beheben des Problems, aufgrund dessen Version 10.0.3 von Newtonsoft.Json beim Modulimport nicht geladen wurde</span><span class="sxs-lookup"><span data-stu-id="111e4-725">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="111e4-726">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="111e4-726">AzureRM.Compute</span></span>
* <span data-ttu-id="111e4-727">Feature zum Aktualisieren von virtuellen VMSS-Computern</span><span class="sxs-lookup"><span data-stu-id="111e4-727">VMSS VM Update feature</span></span>
    - <span data-ttu-id="111e4-728">Cmdlets „Update-AzureRmVmssVM“ und „New-AzureRmVMDataDisk“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-728">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="111e4-729">Fügen Sie den Parameter „VirtualMachineScaleSetVM“ zum Cmdlet „Add-AzureRmVMDataDisk“ hinzu, um das Hinzufügen eines Datenträgers zum virtuellen VMSS-Computer zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="111e4-729">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="111e4-730">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="111e4-730">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="111e4-731">Aktualisierung der ADF .Net SDK-Version auf 0.8.0-preview mit den folgenden Änderungen:</span><span class="sxs-lookup"><span data-stu-id="111e4-731">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="111e4-732">Vorgang zum Konfigurieren des Factoryrepositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-732">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="111e4-733">Der verknüpfte QuickBooks-Dienst wurde aktualisiert, um die Eigenschaften „consumerKey“ und „consumerSecret“ verfügbar zu machen.</span><span class="sxs-lookup"><span data-stu-id="111e4-733">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="111e4-734">Aktualisierung verschiedener Modelltypen von „SecretBase“ auf „Object“</span><span class="sxs-lookup"><span data-stu-id="111e4-734">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="111e4-735">Blobereignisauslöser hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-735">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="111e4-736">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="111e4-736">AzureRM.KeyVault</span></span>
* <span data-ttu-id="111e4-737">Aktualisierung der Dokumentation mit Beispielausgabe</span><span class="sxs-lookup"><span data-stu-id="111e4-737">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="111e4-738">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="111e4-738">AzureRM.Network</span></span>
* <span data-ttu-id="111e4-739">Aktivierung der Traffic Analytics-Parameter für Network Watcher-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="111e4-739">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="111e4-740">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="111e4-740">AzureRM.Resources</span></span>
* <span data-ttu-id="111e4-741">Behebung des Problems mit der Eigenschaft „Properties“ von PSResource-Objekten, die von „Get-AzureRmResource“ zurückgegeben wurden</span><span class="sxs-lookup"><span data-stu-id="111e4-741">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="111e4-742">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="111e4-742">AzureRM.Scheduler</span></span>
* <span data-ttu-id="111e4-743">Behebung des Problems, dass beim Aktualisieren von „ServiceBusQueueJob“ keine neuen Authentifizierungswerte festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="111e4-743">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="111e4-744">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="111e4-744">AzureRM.Sql</span></span>
* <span data-ttu-id="111e4-745">Aktualisierung der folgenden Cmdlets mit dem optionalen LicenseType-Parameter</span><span class="sxs-lookup"><span data-stu-id="111e4-745">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="111e4-746">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="111e4-746">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="111e4-747">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="111e4-747">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="111e4-748">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="111e4-748">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="111e4-749">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="111e4-749">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="111e4-750">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="111e4-750">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="111e4-751">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="111e4-751">AzureRM.Websites</span></span>
* <span data-ttu-id="111e4-752">„New-AzureRMWebApp“ aktualisiert, um allgemeine Algorithmen aus der Strategiebibliothek zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="111e4-752">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="111e4-753">6.1.0 – Mai 2018</span><span class="sxs-lookup"><span data-stu-id="111e4-753">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="111e4-754">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="111e4-754">AzureRM.Profile</span></span>
* <span data-ttu-id="111e4-755">Behebung eines Problems, durch das beim Ausführen von „Clear-AzureRmContext“ ein leerer Kontext mit dem Namen des vorherigen Standardkontexts beibehalten wurde und der Benutzer dadurch keinen neuen Kontext mit dem alten Namen erstellen konnte</span><span class="sxs-lookup"><span data-stu-id="111e4-755">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="111e4-756">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="111e4-756">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="111e4-757">Ermöglichung der Zuordnung von Gateways/Aufhebung der Gatewayzuordnung in AS</span><span class="sxs-lookup"><span data-stu-id="111e4-757">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="111e4-758">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="111e4-758">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="111e4-759">Unterstützung für „ApiVersions“, „ApiReleases“ und „ApiRevisions“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-759">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="111e4-760">Unterstützung für ServiceFabric-Back-End hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-760">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="111e4-761">Unterstützung für Application Insights-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-761">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="111e4-762">Unterstützung für die Erkennung von SKUs vom Typ „Basic“ als gültige SKU des API Management-Diensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-762">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="111e4-763">Unterstützung hinzugefügt, damit Zertifikate, die von der privaten Zertifizierungsstelle ausgestellt wurden, als Stamm- oder ZS-Zertifikate installiert werden können</span><span class="sxs-lookup"><span data-stu-id="111e4-763">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="111e4-764">Unterstützung für die Akzeptierung benutzerdefinierter SSL-Zertifikate über KeyVault und mehrere Proxyhostnamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-764">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="111e4-765">Unterstützung für die verwaltete Dienstidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-765">Added support for MSI identity</span></span>
* <span data-ttu-id="111e4-766">Unterstützung für die Annahme von Richtlinien über URL hinzugefügt; HINWEIS: Folgende Cmdlets werden in einem zukünftigen Release als veraltet gekennzeichnet:</span><span class="sxs-lookup"><span data-stu-id="111e4-766">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="111e4-767">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="111e4-767">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="111e4-768">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="111e4-768">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="111e4-769">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="111e4-769">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="111e4-770">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="111e4-770">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="111e4-771">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="111e4-771">AzureRM.Batch</span></span>
* <span data-ttu-id="111e4-772">Veröffentlichung des neuen Cmdlets „Get-AzureBatchPoolNodeCounts“</span><span class="sxs-lookup"><span data-stu-id="111e4-772">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="111e4-773">Veröffentlichung des neuen Cmdlets „Start-AzureBatchComputeNodeServiceLogUpload“</span><span class="sxs-lookup"><span data-stu-id="111e4-773">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="111e4-774">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="111e4-774">AzureRM.Consumption</span></span>
* <span data-ttu-id="111e4-775">Hinzufügung neuer Parameter („Expand“, „ResourceGroup“, „InstanceName“, „InstanceId“, „Tags“ und „Top“) für das Cmdlet „Get-AzureRmConsumptionUsageDetail“</span><span class="sxs-lookup"><span data-stu-id="111e4-775">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="111e4-776">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="111e4-776">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="111e4-777">Korrektur des Beispiels für „Export AzureRmDataLakeStoreChildItemProperties“</span><span class="sxs-lookup"><span data-stu-id="111e4-777">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="111e4-778">Korrektur der NULL-Parameterausnahme für rekursiven Fall in „Set-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="111e4-778">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="111e4-779">Korrektur der Hilfedateien für „Set-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ und „Remove-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="111e4-779">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="111e4-780">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="111e4-780">AzureRM.Network</span></span>
* <span data-ttu-id="111e4-781">Erhöhung der Network SDK-Version von 18.0.0-preview auf 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="111e4-781">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="111e4-782">Cmdlet zum Erstellen der Protokollkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-782">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="111e4-783">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="111e4-783">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="111e4-784">Cmdlet zum Hinzufügen einer neuen Leitungsverbindung zu einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-784">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="111e4-785">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-785">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="111e4-786">Cmdlet zum Entfernen einer Leitungsverbindung aus einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-786">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="111e4-787">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-787">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="111e4-788">Cmdlet zum Abrufen einer Leitungsverbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="111e4-788">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="111e4-789">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="111e4-789">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="111e4-790">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="111e4-790">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="111e4-791">Verwendung der Serverauthentifizierung mit generierten Zertifikaten korrigiert (Problemnr. 5998)</span><span class="sxs-lookup"><span data-stu-id="111e4-791">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="111e4-792">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="111e4-792">AzureRM.Sql</span></span>
* <span data-ttu-id="111e4-793">Überwachungscmdlets korrigiert, um das Entfernen von „AuditActions“ oder „AuditActionGroups“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="111e4-793">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="111e4-794">Problem mit „Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy“ behoben, das beim Festlegen einer neuen flexiblen Aufbewahrungsrichtlinie zu folgendem Fehler führte: „Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span><span class="sxs-lookup"><span data-stu-id="111e4-794">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="111e4-795">Please submit request with the new flexible retention policy“ (Das Konfigurieren einer langfristigen Aufbewahrungsrichtlinie mit Azure Recovery Service-Tresor und -Richtlinie wird nicht mehr unterstützt. Übermitteln Sie eine Anforderung mit der neuen flexiblen Aufbewahrungsrichtlinie.)</span><span class="sxs-lookup"><span data-stu-id="111e4-795">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="111e4-796">Aktualisierung aller Cmdlets für Azure SQL-Datenbank, für die Erstellung von Pools für elastische Datenbanken und für die Aktualisierung, sodass sie die neue Datenbank-API verwenden. Diese unterstützt die Sku-Eigenschaft für skalierungs- und tarifbezogene Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="111e4-796">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="111e4-797">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="111e4-797">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="111e4-798">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="111e4-798">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="111e4-799">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="111e4-799">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="111e4-800">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="111e4-800">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="111e4-801">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="111e4-801">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="111e4-802">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="111e4-802">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="111e4-803">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="111e4-803">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="111e4-804">Aktualisierung der Parameter für „Get-AzureRmTrafficManagerProfile“, sodass bei Verwendung des Parameters „-Name“ der Parameter „-ResourceGroupName“ erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="111e4-804">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
