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
ms.sourcegitcommit: f6f5e256143aa6c097de3e57e930d8badea49f30
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/18/2018
ms.locfileid: "49399058"
---
# <a name="release-notes"></a><span data-ttu-id="d453b-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="d453b-103">Release notes</span></span>

<span data-ttu-id="d453b-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="d453b-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="6100---october-2018"></a><span data-ttu-id="d453b-105">6.10.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="d453b-105">6.10.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="d453b-106">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="d453b-106">Azure.Storage</span></span>
* <span data-ttu-id="d453b-107">Fehler beim Kopieren von Blobs/Dateien behoben, aufgrund dessen bei einem Metadatenproblem des Ziels keine Metadaten kopiert wurden</span><span class="sxs-lookup"><span data-stu-id="d453b-107">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="d453b-108">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="d453b-108">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="d453b-109">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="d453b-109">Start-AzureStorageFileCopy</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="d453b-110">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="d453b-110">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="d453b-111">„Get-AzureRmCognitiveServicesAccountSkus“ wird ohne vorhandenes Konto unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d453b-111">Support Get-AzureRmCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="d453b-112">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="d453b-112">AzureRM.Compute</span></span>
* <span data-ttu-id="d453b-113">Korrektur von „Get-AzureRmVM -ResourceGroupName <rg>“ sodass ggf. mehr als 50 Ergebnisse zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="d453b-113">Fix Get-AzureRmVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="d453b-114">Der Cmdlet-Hilfe zu „New-AzureRmVmss“ wurde ein Beispiel für „SimpleParameterSet“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d453b-114">Added an example of the 'SimpleParameterSet' to New-AzureRmVmss cmdlet help.</span></span>
* <span data-ttu-id="d453b-115">Tippfehler in der Azure Disk Encryption-Statusmeldung behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-115">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="d453b-116">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="d453b-116">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="d453b-117">Die Version des ADF .Net-SDK wurde auf 2.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="d453b-117">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="d453b-118">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="d453b-118">AzureRM.Network</span></span>
* <span data-ttu-id="d453b-119">NetworkProfile-Funktionalität wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d453b-119">Added NetworkProfile functionality.</span></span> <span data-ttu-id="d453b-120">Neue Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-120">new cmdlets added</span></span>
    - <span data-ttu-id="d453b-121">Get-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d453b-121">Get-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="d453b-122">New-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d453b-122">New-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="d453b-123">Remove-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d453b-123">Remove-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="d453b-124">Set-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d453b-124">Set-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="d453b-125">New-AzureRMContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-125">New-AzureRMContainerNicConfig</span></span>
    - <span data-ttu-id="d453b-126">New-AzureRmContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-126">New-AzureRmContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="d453b-127">Dienstzuordnungslink in Subnetzmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-127">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="d453b-128">Cmdlets „New-AzureRmVirtualNetworkTap“, „Get-AzureRmVirtualNetworkTap“, „Set-AzureRmVirtualNetworkTap“, „Remove-AzureRmVirtualNetworkTap“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-128">Added cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span></span>
* <span data-ttu-id="d453b-129">Cmdlets „Set-AzureRmNEtworkInterfaceTapConfig“, „Get-AzureRmNEtworkInterfaceTapConfig“, „Remove-AzureRmNEtworkInterfaceTapConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-129">Added cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="d453b-130">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="d453b-130">AzureRM.RedisCache</span></span>
* <span data-ttu-id="d453b-131">Künftig sind beliebige Zeichenfolgen als Größenparameter zulässig.</span><span class="sxs-lookup"><span data-stu-id="d453b-131">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="d453b-132">P5 in Popup „PSArgumentCompleter“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-132">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="d453b-133">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="d453b-133">AzureRM.Resources</span></span>
* <span data-ttu-id="d453b-134">Fehlender Parameter „-Mode“ zu „Set-AzureRmPolicyDefinition“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-134">Add missing -Mode parameter to Set-AzureRmPolicyDefinition</span></span>
* <span data-ttu-id="d453b-135">Cmdlet-Fehler bei „Fix Get-AzureRmProviderOperation“ für Vorgänge mit Ursprung behoben, der den Benutzer enthält</span><span class="sxs-lookup"><span data-stu-id="d453b-135">Fix Get-AzureRmProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="d453b-136">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="d453b-136">AzureRM.Sql</span></span>
* <span data-ttu-id="d453b-137">Problem behoben, aufgrund dessen einige Sicherungs-Cmdlets das aktuelle Azure-Abonnements nicht erkannt haben</span><span class="sxs-lookup"><span data-stu-id="d453b-137">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="d453b-138">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="d453b-138">AzureRM.Storage</span></span>
* <span data-ttu-id="d453b-139">Der Abruf der Speicherressourcennutzung eines bestimmten Standorts wird jetzt unterstützt, und das Hinzufügen einer Warnmeldung für den Abruf der globalen Speicherressourcennutzung ist überflüssig.</span><span class="sxs-lookup"><span data-stu-id="d453b-139">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="d453b-140">Get-AzureRmStorageUsage</span><span class="sxs-lookup"><span data-stu-id="d453b-140">Get-AzureRmStorageUsage</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="d453b-141">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="d453b-141">AzureRM.Websites</span></span>
* <span data-ttu-id="d453b-142">Neues Cmdlet „Get-AzureRMWebAppContainerContinuousDeploymentUrl“ zum Abruf der Webhook-URL von Continuous Deployment für Container</span><span class="sxs-lookup"><span data-stu-id="d453b-142">New Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="d453b-143">Neue Cmdlets „New-AzureRMWebAppContainerPSSession“ und „Enter-WebAppContainerPSSession“ zum Initiieren einer PowerShell-Remotesitzung in einer Windows-Container-App</span><span class="sxs-lookup"><span data-stu-id="d453b-143">New Cmdlets New-AzureRMWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="690---september-2018"></a><span data-ttu-id="d453b-144">6.9.0 – September 2018</span><span class="sxs-lookup"><span data-stu-id="d453b-144">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="d453b-145">Allgemein</span><span class="sxs-lookup"><span data-stu-id="d453b-145">General</span></span>
* <span data-ttu-id="d453b-146">AzureRM.SignalR wurde dem Rollupmodul AzureRM hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-146">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="d453b-147">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="d453b-147">AzureRM.Profile</span></span>
* <span data-ttu-id="d453b-148">Kleinere Änderungen am allgemeinen Speichercode</span><span class="sxs-lookup"><span data-stu-id="d453b-148">Minor changes to the storage common code</span></span>
* <span data-ttu-id="d453b-149">Hilfedateien aktualisiert, um vollständige Parametertypen einzubinden.</span><span class="sxs-lookup"><span data-stu-id="d453b-149">Updated help files to include full parameter types.</span></span>
- <span data-ttu-id="d453b-150">„-ServicePrincipal“ im Parametersatz „ServicePrincipalCertificateWithSubscriptionId“ in nicht obligatorisch geändert</span><span class="sxs-lookup"><span data-stu-id="d453b-150">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="d453b-151">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="d453b-151">Azure.Storage</span></span>
* <span data-ttu-id="d453b-152">Unterstützung für die Erstellung des Speicherkontexts mit OAuth.</span><span class="sxs-lookup"><span data-stu-id="d453b-152">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="d453b-153">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="d453b-153">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="d453b-154">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="d453b-154">AzureRM.Cdn</span></span>
* <span data-ttu-id="d453b-155">Standard_Microsoft in SKU für CDN-Preise hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d453b-155">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="d453b-156">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="d453b-156">AzureRM.Compute</span></span>
* <span data-ttu-id="d453b-157">Abhängigkeiten für Key Vault und Storage in allgemeine Abhängigkeiten verschieben</span><span class="sxs-lookup"><span data-stu-id="d453b-157">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="d453b-158">Unterstützung für weitere VM-Größen zu AEM-Cmdlets hinzufügen</span><span class="sxs-lookup"><span data-stu-id="d453b-158">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="d453b-159">Parameter „PublicIPPrefix“ zu „New-AzureRmVmssIpConfig“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="d453b-159">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="d453b-160">Parameter „ResourceId“ zu Cmdlet „Invoke-AzureRmVMRunCommand“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="d453b-160">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="d453b-161">Cmdlet „Invoke-AzureRmVmssVMRunCommand“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="d453b-161">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="d453b-162">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="d453b-162">AzureRM.Dns</span></span>
* <span data-ttu-id="d453b-163">Unterstützung für Aliaseintrag während der Erstellung des DNS-Eintrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-163">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="d453b-164">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="d453b-164">AzureRM.Insights</span></span>
* <span data-ttu-id="d453b-165">Probleme #6833 und #7102 behoben (Bereich „Diagnoseeinstellungen“)</span><span class="sxs-lookup"><span data-stu-id="d453b-165">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="d453b-166">Probleme mit dem Standardnamen, also „service“, beim Erstellen und Auflisten/Abrufen von Diagnoseeinstellungen</span><span class="sxs-lookup"><span data-stu-id="d453b-166">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="d453b-167">Probleme beim Erstellen von Diagnoseeinstellungen mit Kategorien</span><span class="sxs-lookup"><span data-stu-id="d453b-167">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="d453b-168">Meldung zur Einstellung der Unterstützung für Metrikaggregationsintervall-Parameter</span><span class="sxs-lookup"><span data-stu-id="d453b-168">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="d453b-169">Aggregationsintervall-Parameter werden weiterhin akzeptiert (Änderung ohne Funktionsbeeinträchtigung), aber sie werden auf dem Back-End ignoriert, da nur PT1M gültig ist</span><span class="sxs-lookup"><span data-stu-id="d453b-169">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="d453b-170">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="d453b-170">AzureRM.Network</span></span>
* <span data-ttu-id="d453b-171">Änderungen an LoadBalancer-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="d453b-171">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="d453b-172">LoadBalancerInboundNatPoolConfig: Parameter IdleTimeoutInMinutes, EnableFloatingIp und EnableTcpReset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-172">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="d453b-173">LoadBalancerInboundNatRuleConfig: Parameter EnableTcpReset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-173">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="d453b-174">LoadBalancerRuleConfig: Parameter EnableTcpReset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-174">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="d453b-175">LoadBalancerProbeConfig: Unterstützung für Wert „Https“ für Parameter „Protocol“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-175">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="d453b-176">Neue Befehle für neue Unterressource „OutboundRule“ von LoadBalancer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-176">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="d453b-177">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-177">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="d453b-178">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-178">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="d453b-179">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-179">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="d453b-180">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-180">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="d453b-181">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-181">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="d453b-182">Neue HostedWorkloads-Eigenschaft für PSNetworkInterface hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-182">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="d453b-183">Neue Cmdlets für Feature: Azure Firewall über ARM</span><span class="sxs-lookup"><span data-stu-id="d453b-183">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="d453b-184">Get-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-184">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="d453b-185">Set-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-185">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="d453b-186">New-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-186">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="d453b-187">Remove-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-187">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="d453b-188">New-AzureRmFirewallApplicationRuleCollection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-188">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="d453b-189">New-AzureRmFirewallApplicationRule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-189">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="d453b-190">New-AzureRmFirewallNatRuleCollection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-190">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="d453b-191">New-AzureRmFirewallNatRule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-191">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="d453b-192">New-AzureRmFirewallNetworkRuleCollection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-192">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="d453b-193">New-AzureRmFirewallNetworkRule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-193">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="d453b-194">Unterstützung für vertrauenswürdiges Stammzertifikat und Konfiguration der automatischen Skalierung in Application Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-194">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="d453b-195">Neue Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="d453b-195">New Cmdlets added:</span></span>
      - <span data-ttu-id="d453b-196">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d453b-196">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="d453b-197">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d453b-197">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="d453b-198">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d453b-198">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="d453b-199">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d453b-199">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="d453b-200">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d453b-200">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="d453b-201">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="d453b-201">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="d453b-202">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="d453b-202">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="d453b-203">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="d453b-203">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="d453b-204">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="d453b-204">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="d453b-205">Cmdlets mit optionalem Parameter „-TrustedRootCertificate“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-205">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="d453b-206">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="d453b-206">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="d453b-207">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="d453b-207">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="d453b-208">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="d453b-208">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="d453b-209">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="d453b-209">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="d453b-210">Cmdlets mit optionalem Parameter „-AutoscaleConfiguration“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-210">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="d453b-211">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="d453b-211">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="d453b-212">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="d453b-212">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="d453b-213">Cmdlet für Schnittstellenendpunkt Get-AzureInterfaceEndpoint hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-213">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="d453b-214">Unterstützung für mehrere Adresspräfixe in einem Subnetz hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d453b-214">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="d453b-215">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d453b-215">Updated cmdlets:</span></span>
  - <span data-ttu-id="d453b-216">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-216">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="d453b-217">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-217">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="d453b-218">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-218">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="d453b-219">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-219">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="d453b-220">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="d453b-220">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="d453b-221">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-221">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="d453b-222">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-222">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="d453b-223">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-223">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="d453b-224">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="d453b-224">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="d453b-225">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="d453b-225">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="d453b-226">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="d453b-226">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="d453b-227">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-227">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="d453b-228">New-AzureRmNetworkInterfaceIpConfig – Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-228">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="d453b-229">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-229">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="d453b-230">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-230">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="d453b-231">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-231">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="d453b-232">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-232">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="d453b-233">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-233">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="d453b-234">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="d453b-234">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="d453b-235">Cmdlets für die Subnetzdelegierung hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="d453b-235">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="d453b-236">New-AzureRmDelegation: Erstellt eine neue Delegierung, die einem Subnetz hinzugefügt werden kann</span><span class="sxs-lookup"><span data-stu-id="d453b-236">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="d453b-237">Remove-AzureRmDelegation: Nutzt ein Subnetz und entfernt den bereitgestellten Delegierungsnamen aus diesem Subnetz</span><span class="sxs-lookup"><span data-stu-id="d453b-237">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="d453b-238">Add-AzureRmDelegation: Nutzt ein Subnetz und fügt den angegebenen Dienstnamen diesem Subnetz als Delegierung hinzu</span><span class="sxs-lookup"><span data-stu-id="d453b-238">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="d453b-239">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="d453b-239">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="d453b-240">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="d453b-240">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="d453b-241">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="d453b-241">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="d453b-242">Unterstützung für verwalteten Datenträger</span><span class="sxs-lookup"><span data-stu-id="d453b-242">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="d453b-243">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="d453b-243">AzureRM.RedisCache</span></span>
* <span data-ttu-id="d453b-244">Insights-Abhängigkeit aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="d453b-244">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="d453b-245">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="d453b-245">AzureRM.Resources</span></span>
* <span data-ttu-id="d453b-246">New-AzureRmResourceGroupDeployment mit neuem Parameter „RollbackAction“ aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d453b-246">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="d453b-247">Unterstützung für OnErrorDeployment mit dem neuen Parameter hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="d453b-247">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="d453b-248">Unterstützung für verwaltete Identität in Richtlinienzuweisungen.</span><span class="sxs-lookup"><span data-stu-id="d453b-248">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="d453b-249">Parameter mit Standardwerten sind nicht mehr erforderlich, wenn eine Richtlinie mit „New-AzureRmPolicyAssignment“ zugewiesen wird</span><span class="sxs-lookup"><span data-stu-id="d453b-249">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="d453b-250">Neues Cmdlet „Get-AzureRmPolicyAlias“ zum Abrufen von Richtlinienaliasen hinzufügen</span><span class="sxs-lookup"><span data-stu-id="d453b-250">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="d453b-251">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d453b-251">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="d453b-252">Problem #7161 behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-252">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="d453b-253">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="d453b-253">AzureRM.SignalR</span></span>
* <span data-ttu-id="d453b-254">SKU-Namen auf Free_F1 und Standard_S1 aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d453b-254">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="d453b-255">Versionsfeld zum PSSignalRResource-Objekt und Verbindungszeichenfolge zum PSSignalRKeys-Objekt hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="d453b-255">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="d453b-256">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="d453b-256">AzureRM.Storage</span></span>
* <span data-ttu-id="d453b-257">Unterstützung für Unveränderlichkeitsrichtlinie in AzureRm.Storage</span><span class="sxs-lookup"><span data-stu-id="d453b-257">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="d453b-258">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="d453b-258">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="d453b-259">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="d453b-259">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="d453b-260">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="d453b-260">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="d453b-261">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="d453b-261">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="d453b-262">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="d453b-262">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="d453b-263">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="d453b-263">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="d453b-264">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="d453b-264">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="d453b-265">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="d453b-265">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="d453b-266">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="d453b-266">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="d453b-267">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="d453b-267">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="d453b-268">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="d453b-268">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="d453b-269">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="d453b-269">AzureRM.Websites</span></span>
* <span data-ttu-id="d453b-270">Zwei neue Cmdlets hinzugefügt: Get-AzureRmDeletedWebApp und Restore-AzureRmDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="d453b-270">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="d453b-271">New-AzureRmAppServicePlan -HyperV-Switch für „App Service-Plan erstellen“ mit Windows-Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-271">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="d453b-272">New-AzureRmWebApp/New-AzureRmWebAppSlot/Set-AzureRmWebApp/Set-AzureRmWebAppSlot: Neue Parameter (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) für die Erstellung und Verwaltung der Windows-Container-App hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-272">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="d453b-273">6.8.1: August 2018</span><span class="sxs-lookup"><span data-stu-id="d453b-273">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="d453b-274">Allgemein</span><span class="sxs-lookup"><span data-stu-id="d453b-274">General</span></span>
* <span data-ttu-id="d453b-275">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="d453b-275">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="d453b-276">Allgemeine Laufzeitassemblys aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-276">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="d453b-277">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d453b-277">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="d453b-278">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="d453b-278">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="d453b-279">Problem https://github.com/Azure/azure-powershell/issues/6603 behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-279">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="d453b-280">Die Cmdlets „Import-AzureRmApiManagementApi“ und „\*-AzureRmApiManagementCertificate“ können jetzt relative Pfade verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="d453b-280">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="d453b-281">Problem https://github.com/Azure/azure-powershell/issues/6879 behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-281">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="d453b-282">„CertificateInformation“ ist eine festlegbare Eigenschaft, die die ordnungsgemäße Funktionsweise des Cmdlets „Set-AzureRmApiManagement“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="d453b-282">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="d453b-283">Behoben durch Upgrade auf NuGet-Paket „4.0.4-preview“</span><span class="sxs-lookup"><span data-stu-id="d453b-283">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="d453b-284">Problem https://github.com/Azure/azure-powershell/issues/6853 behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-284">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="d453b-285">OData-Filter für die Suche anhand des Namens korrigiert (Produkt)</span><span class="sxs-lookup"><span data-stu-id="d453b-285">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="d453b-286">Problem https://github.com/Azure/azure-powershell/issues/6814 behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-286">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="d453b-287">OData-Filter für die Suche anhand des Namens korrigiert (API)</span><span class="sxs-lookup"><span data-stu-id="d453b-287">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="d453b-288">Unterstützung für AzureMonitor-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-288">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="d453b-289">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="d453b-289">AzureRM.Compute</span></span>
* <span data-ttu-id="d453b-290">Problem des fehlenden Ziels in der Fehlerausgabe behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-290">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="d453b-291">Problem mit dem Speicherkontotyp für den virtuellen Computer mit verwaltetem Datenträgern behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-291">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="d453b-292">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="d453b-292">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="d453b-293">AEM-Erweiterungs-Cmdlets für andere Umgebungen (etwa Azure China) korrigiert</span><span class="sxs-lookup"><span data-stu-id="d453b-293">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="d453b-294">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="d453b-294">AzureRM.Network</span></span>
* <span data-ttu-id="d453b-295">Standarddarstellung der Cmdlet-Ausgabe in Tabellenansicht geändert</span><span class="sxs-lookup"><span data-stu-id="d453b-295">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="d453b-296">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="d453b-296">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="d453b-297">Fehler in „Update-AzureRmPowerBIEmbeddedCapacity“ beim Skalieren der angehaltenen Kapazität behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-297">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="d453b-298">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="d453b-298">AzureRM.Resources</span></span>
* <span data-ttu-id="d453b-299">Problem beim Erstellen verwalteter Anwendungen über Marketplace behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-299">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="d453b-300">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d453b-300">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="d453b-301">Behobene Probleme</span><span class="sxs-lookup"><span data-stu-id="d453b-301">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="d453b-302">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="d453b-302">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="d453b-303">Unterstützung für Routingmethode „MultiValue“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-303">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="d453b-304">Neuer Parameter „MaxReturn“ für Routingtyp „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="d453b-304">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="d453b-305">Unterstützung für Subnetzroutingmethode hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-305">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="d453b-306">Unterstützung für IP-Adressbereiche (Subnetze) in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="d453b-306">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="d453b-307">Unterstützung für benutzerdefinierte Header in Profilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-307">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="d453b-308">Unterstützung für erwartete Statuscodebereiche in Profilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-308">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="d453b-309">Unterstützung für benutzerdefinierte Header in Endpunkten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-309">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="d453b-310">6.8.0: August 2018</span><span class="sxs-lookup"><span data-stu-id="d453b-310">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="d453b-311">Allgemein</span><span class="sxs-lookup"><span data-stu-id="d453b-311">General</span></span>
* <span data-ttu-id="d453b-312">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="d453b-312">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="d453b-313">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="d453b-313">AzureRM.Profile</span></span>
* <span data-ttu-id="d453b-314">Ablaufeigenschaft zu Token hinzugefügt, die während „Connect-AzureRmAccount“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="d453b-314">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="d453b-315">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="d453b-315">AzureRM.Compute</span></span>
* <span data-ttu-id="d453b-316">Problem des fehlenden Ziels in der Fehlerausgabe behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-316">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="d453b-317">Problem mit dem Speicherkontotyp für den virtuellen Computer mit verwaltetem Datenträgern behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-317">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="d453b-318">AEM-Erweiterungs-Cmdlets für andere Umgebungen (etwa Azure China) korrigiert</span><span class="sxs-lookup"><span data-stu-id="d453b-318">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="d453b-319">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="d453b-319">AzureRM.IotHub</span></span>
* <span data-ttu-id="d453b-320">Beispiele für „New-AzureRmIotHubExportDevices“ und „New-AzureRmIotHubImportDevices“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="d453b-320">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="d453b-321">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="d453b-321">AzureRM.Network</span></span>
* <span data-ttu-id="d453b-322">Standarddarstellung von Modellen in Tabellenansicht geändert</span><span class="sxs-lookup"><span data-stu-id="d453b-322">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="d453b-323">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="d453b-323">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="d453b-324">Fehler in „Update-AzureRmPowerBIEmbeddedCapacity“ beim Skalieren der angehaltenen Kapazität behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-324">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="d453b-325">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="d453b-325">AzureRM.Resources</span></span>
* <span data-ttu-id="d453b-326">Problem beim Erstellen der verwalteten Anwendung über Marketplace behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-326">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="d453b-327">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d453b-327">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="d453b-328">Fehlerbehebung</span><span class="sxs-lookup"><span data-stu-id="d453b-328">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="d453b-329">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="d453b-329">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="d453b-330">Unterstützung für Routingmethode „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="d453b-330">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="d453b-331">Neuer Parameter „MaxReturn“ für Routingtyp „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="d453b-331">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="d453b-332">Unterstützung für Subnetzroutingmethode</span><span class="sxs-lookup"><span data-stu-id="d453b-332">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="d453b-333">Unterstützung für IP-Adressbereiche (Subnetze) in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="d453b-333">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="d453b-334">Unterstützung für benutzerdefinierte Header in Profilen</span><span class="sxs-lookup"><span data-stu-id="d453b-334">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="d453b-335">Unterstützung für erwartete Statuscodebereiche in Profilen</span><span class="sxs-lookup"><span data-stu-id="d453b-335">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="d453b-336">Unterstützung für benutzerdefinierte Header in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="d453b-336">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="d453b-337">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="d453b-337">AzureRM.Websites</span></span>
* <span data-ttu-id="d453b-338">Das Problem, dass die Standardressourcengruppe falsch festgelegt wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="d453b-338">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="d453b-339">6.7.0: August 2018</span><span class="sxs-lookup"><span data-stu-id="d453b-339">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="d453b-340">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="d453b-340">AzureRM.Profile</span></span>
* <span data-ttu-id="d453b-341">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-341">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="d453b-342">Benutzer-ID zum Standardkontextnamen hinzugefügt, um Kontextkonflikte zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="d453b-342">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="d453b-343">Probleme mit „Clear-AzureRmContext“ behoben, die Fehler beim Auswählen eines Kontexts verursacht haben (6398)</span><span class="sxs-lookup"><span data-stu-id="d453b-343">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="d453b-344">Ermöglicht, dass für „Connect-AzureRmAccount“ die Mandantendomäne an den Parameter „-TenantId“ übergeben wird</span><span class="sxs-lookup"><span data-stu-id="d453b-344">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="d453b-345">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="d453b-345">Azure.Storage</span></span>
* <span data-ttu-id="d453b-346">Begrenzung von 5 TB für das Kontingent der Azure-Dateifreigabe entfernt</span><span class="sxs-lookup"><span data-stu-id="d453b-346">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="d453b-347">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="d453b-347">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="d453b-348">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="d453b-348">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="d453b-349">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-349">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="d453b-350">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="d453b-350">Azure.AnalysisServices</span></span>
* <span data-ttu-id="d453b-351">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-351">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="d453b-352">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d453b-352">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="d453b-353">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-353">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="d453b-354">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="d453b-354">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="d453b-355">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-355">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="d453b-356">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="d453b-356">AzureRM.Automation</span></span>
* <span data-ttu-id="d453b-357">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-357">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="d453b-358">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="d453b-358">AzureRM.Backup</span></span>
* <span data-ttu-id="d453b-359">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-359">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="d453b-360">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="d453b-360">AzureRM.Batch</span></span>
* <span data-ttu-id="d453b-361">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-361">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="d453b-362">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="d453b-362">AzureRM.Billing</span></span>
* <span data-ttu-id="d453b-363">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-363">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="d453b-364">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="d453b-364">AzureRM.Cdn</span></span>
* <span data-ttu-id="d453b-365">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-365">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="d453b-366">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="d453b-366">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="d453b-367">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-367">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="d453b-368">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="d453b-368">AzureRM.Compute</span></span>
* <span data-ttu-id="d453b-369">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-369">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="d453b-370">EvictionPolicy-Parameter zu „New-AzureRmVmssConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-370">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="d453b-371">Standort in „DiskFileParameterSet“ von „New-AzureRmVm“ angeben, wenn kein Ort angegeben ist</span><span class="sxs-lookup"><span data-stu-id="d453b-371">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="d453b-372">Parameterbeschreibung in „Save-AzureRmVMImage“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="d453b-372">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="d453b-373">Cmdlet „Get-AzureRmVMDiskEncryptionStatus“ für bestimmte Szenarien im Zusammenhang mit einem Durchlauf korrigiert</span><span class="sxs-lookup"><span data-stu-id="d453b-373">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="d453b-374">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="d453b-374">AzureRM.Consumption</span></span>
* <span data-ttu-id="d453b-375">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-375">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="d453b-376">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="d453b-376">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="d453b-377">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-377">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="d453b-378">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="d453b-378">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="d453b-379">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-379">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="d453b-380">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="d453b-380">AzureRM.DataFactories</span></span>
* <span data-ttu-id="d453b-381">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-381">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="d453b-382">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="d453b-382">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="d453b-383">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-383">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="d453b-384">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="d453b-384">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="d453b-385">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-385">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="d453b-386">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d453b-386">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="d453b-387">Debuggen korrigiert, wenn „DebugPreference“ über die PowerShell-Befehlszeile festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="d453b-387">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="d453b-388">Beispiel für „Set-AzureRmDataLakeStoreItemAcl“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-388">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="d453b-389">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="d453b-389">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="d453b-390">Beispiel für „Set-AzureRmDataLakeStoreItemAclEntry“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-390">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="d453b-391">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="d453b-391">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="d453b-392">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-392">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="d453b-393">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="d453b-393">AzureRM.Dns</span></span>
* <span data-ttu-id="d453b-394">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-394">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="d453b-395">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="d453b-395">AzureRM.EventGrid</span></span>
* <span data-ttu-id="d453b-396">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-396">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="d453b-397">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="d453b-397">AzureRM.EventHub</span></span>
* <span data-ttu-id="d453b-398">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-398">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="d453b-399">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="d453b-399">AzureRM.HDInsight</span></span>
* <span data-ttu-id="d453b-400">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-400">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="d453b-401">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="d453b-401">AzureRM.Insights</span></span>
* <span data-ttu-id="d453b-402">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-402">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="d453b-403">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="d453b-403">AzureRM.IotHub</span></span>
* <span data-ttu-id="d453b-404">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-404">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="d453b-405">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d453b-405">AzureRM.KeyVault</span></span>
* <span data-ttu-id="d453b-406">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-406">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="d453b-407">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="d453b-407">AzureRM.LogicApp</span></span>
* <span data-ttu-id="d453b-408">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-408">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="d453b-409">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="d453b-409">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="d453b-410">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-410">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="d453b-411">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="d453b-411">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="d453b-412">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-412">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="d453b-413">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="d453b-413">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="d453b-414">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-414">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="d453b-415">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="d453b-415">AzureRM.Media</span></span>
* <span data-ttu-id="d453b-416">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-416">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="d453b-417">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="d453b-417">AzureRM.Network</span></span>
* <span data-ttu-id="d453b-418">Beispiel für „Set-AzureRmLocalNetworkGateway“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-418">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="d453b-419">Beispiele und Beschreibungen für „Add-AzureRmVirtualNetworkGatewayIpConfig“, „Get-AzureRmVirtualNetworkGatewayConnectionSharedKey“ und „New-AzureRmVirtualNetworkGatewayConnection“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-419">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="d453b-420">Beispiele für „Remove-AzureRmVirtualNetworkGatewayIpConfig“ und „Reset-AzureRmVirtualNetworkGateway“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-420">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="d453b-421">Beispiel für „Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-421">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="d453b-422">Beispiel für „Set-AzureRmVirtualNetworkGatewayConnectionSharedKey“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-422">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="d453b-423">Beispiel für „Set-AzureRmVirtualNetworkGatewayConnection“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-423">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="d453b-424">Cmdlets für „ApplicationSecurityGroup“, „RouteTable“ und „Usage“ mithilfe des aktuellen Code-Generators erneut erstellt</span><span class="sxs-lookup"><span data-stu-id="d453b-424">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="d453b-425">Deutlichere Formulierung der Fehlermeldung für „Get-AzureRmVirtualNetworkSubnetConfig“, wenn ein nicht vorhandenes Subnetz abgerufen wird</span><span class="sxs-lookup"><span data-stu-id="d453b-425">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="d453b-426">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="d453b-426">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="d453b-427">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-427">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="d453b-428">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="d453b-428">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="d453b-429">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-429">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="d453b-430">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="d453b-430">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="d453b-431">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-431">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="d453b-432">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="d453b-432">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="d453b-433">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-433">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="d453b-434">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d453b-434">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="d453b-435">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-435">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="d453b-436">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="d453b-436">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="d453b-437">Richtlinienfilter zum Cmdlet „Get-AzureRmRecoveryServicesBackItem“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d453b-437">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="d453b-438">Der Befehl gibt die Liste der Sicherungselemente zurück, die durch die angegebene Richtlinien-ID geschützt sind.</span><span class="sxs-lookup"><span data-stu-id="d453b-438">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="d453b-439">„Microsoft.Azure.Management.RecoveryServices.Backup“ auf Version 3.0.0-preview aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-439">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="d453b-440">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-440">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="d453b-441">TargetResourceGroupName-Parameter zu „Restore-AzureRmRecoveryServicesBackupItem“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d453b-441">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="d453b-442">Die Ressourcengruppe, in der die verwalteten Datenträger wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="d453b-442">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="d453b-443">Gilt für die Sicherung des virtuellen Computers mit verwalteten Datenträgern.</span><span class="sxs-lookup"><span data-stu-id="d453b-443">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="d453b-444">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="d453b-444">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="d453b-445">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-445">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="d453b-446">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="d453b-446">AzureRM.RedisCache</span></span>
* <span data-ttu-id="d453b-447">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-447">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="d453b-448">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="d453b-448">AzureRM.Relay</span></span>
* <span data-ttu-id="d453b-449">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-449">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="d453b-450">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="d453b-450">AzureRM.Resources</span></span>
* <span data-ttu-id="d453b-451">Unterstützung der Vorlagenbereitstellung im Abonnementbereich.</span><span class="sxs-lookup"><span data-stu-id="d453b-451">Support template deployment at subscription scope.</span></span> <span data-ttu-id="d453b-452">Neue Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="d453b-452">Add new Cmdlets:</span></span>
    - <span data-ttu-id="d453b-453">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="d453b-453">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="d453b-454">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="d453b-454">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="d453b-455">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="d453b-455">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="d453b-456">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="d453b-456">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="d453b-457">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="d453b-457">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="d453b-458">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="d453b-458">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="d453b-459">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="d453b-459">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="d453b-460">Problem behoben, aufgrund dessen beim Übergeben eines Kontexts an „Set-AzureRmResource“ ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="d453b-460">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="d453b-461">Beispiel in „New-AzureRmResourceGroupDeployment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="d453b-461">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="d453b-462">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-462">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="d453b-463">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="d453b-463">AzureRM.Scheduler</span></span>
* <span data-ttu-id="d453b-464">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-464">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="d453b-465">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d453b-465">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="d453b-466">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-466">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="d453b-467">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d453b-467">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="d453b-468">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-468">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="d453b-469">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="d453b-469">AzureRM.Sql</span></span>
* <span data-ttu-id="d453b-470">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-470">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="d453b-471">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="d453b-471">AzureRM.Storage</span></span>
* <span data-ttu-id="d453b-472">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-472">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="d453b-473">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="d453b-473">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="d453b-474">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-474">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="d453b-475">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="d453b-475">AzureRM.Tags</span></span>
* <span data-ttu-id="d453b-476">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-476">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="d453b-477">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="d453b-477">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="d453b-478">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-478">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="d453b-479">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="d453b-479">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="d453b-480">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-480">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="d453b-481">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="d453b-481">AzureRM.Websites</span></span>
* <span data-ttu-id="d453b-482">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-482">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="d453b-483">6.6.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="d453b-483">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="d453b-484">Allgemein</span><span class="sxs-lookup"><span data-stu-id="d453b-484">General</span></span>
* <span data-ttu-id="d453b-485">Alle Hilfedateien aktualisiert, um vollständige Parametertypen und die richtigen Eingabe/Ausgabe-Typen einzuschließen.</span><span class="sxs-lookup"><span data-stu-id="d453b-485">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="d453b-486">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="d453b-486">AzureRM.Profile</span></span>
* <span data-ttu-id="d453b-487">Bibliothek „Common.Strategy“ aktualisiert, um überprüfen zu können, ob die aktuelle Konfiguration für eine Ressource mit der Zielressource kompatibel ist.</span><span class="sxs-lookup"><span data-stu-id="d453b-487">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="d453b-488">ps1xml-Typen zu „Common.Storage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-488">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="d453b-489">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="d453b-489">Azure.Storage</span></span>
* <span data-ttu-id="d453b-490">Unterstützung zum Abrufen von Speicherkontext aus „DefaultProfile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-490">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="d453b-491">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-491">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="d453b-492">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d453b-492">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="d453b-493">Problem https://github.com/Azure/azure-powershell/issues/6370 behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-493">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="d453b-494">Fehler in Automapper behoben, um „PsApiManagementApi“ in „ApiContract“ zu verschieben</span><span class="sxs-lookup"><span data-stu-id="d453b-494">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="d453b-495">Problem https://github.com/Azure/azure-powershell/issues/6515 behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-495">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="d453b-496">Fehler in „File.Save“ behoben, um Überladung mit Codierungstyp zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="d453b-496">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="d453b-497">Problem https://github.com/Azure/azure-powershell/issues/6560 behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-497">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="d453b-498">Upgrade auf Nuget-Version 4.0.3 durchgeführt, in der Musterausnahme in „apiId“ behoben wurde</span><span class="sxs-lookup"><span data-stu-id="d453b-498">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="d453b-499">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="d453b-499">AzureRM.Compute</span></span>
* <span data-ttu-id="d453b-500">Das Problem, aufgrund dessen beim Erstellen eines virtuellen Computers mithilfe von „DiskFileParameterSet“ in „New-AzureRmVm“ wegen einer Umbenennung des Speicherkontotyps „PremiumLRS“ ein Fehler auftrat, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="d453b-500">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="d453b-501">Cmdlet „Invoke-AzureRmVMRunCommand“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="d453b-501">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="d453b-502">„Get-AzureRmAvailabilitySet“ aktualisiert, um die Auflistung aller Verfügbarkeitsgruppen in einem Abonnement zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="d453b-502">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="d453b-503">(ResouceGroupName-Parameter ist jetzt optional.)</span><span class="sxs-lookup"><span data-stu-id="d453b-503">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="d453b-504">„SimpleParameterSet“ von „New-AzureRmVm“ aktualisiert, um Accelerated Networking auf kompatiblen virtuellen Computern zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="d453b-504">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="d453b-505">Einfacher Parametersatz „New-AzureRmVmss“ aktualisiert, sodass das Erstellen der VMSS fehlschlägt, wenn bereits ein benutzerdefinierter LB vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="d453b-505">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="d453b-506">Beispiel für „New-AzureRmDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-506">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="d453b-507">Beispiel für „New-AzureRmVM“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-507">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="d453b-508">Beschreibung für „Set-AzureRmVMOSDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-508">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="d453b-509">Beispiel 1 für „Set-AzureRmVMBginfoExtension“ aktualisiert, um Rechtschreibung und Präfix zu korrigieren.</span><span class="sxs-lookup"><span data-stu-id="d453b-509">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="d453b-510">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="d453b-510">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="d453b-511">ADF .Net SDK-Version auf 1.1.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="d453b-511">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="d453b-512">Unterstützung der Freigabe der selbstgehosteten Integration Runtime über Data Factorys hinweg.</span><span class="sxs-lookup"><span data-stu-id="d453b-512">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="d453b-513">Neuer Parameter „-SharedIntegrationRuntimeResourceId“ zu Cmdlet „Set-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d453b-513">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="d453b-514">Neuer optionaler Parameter „-LinkedDataFactoryName“ zu Cmdlet „Remove-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d453b-514">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="d453b-515">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d453b-515">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="d453b-516">DataPlane SDK-Version (Microsoft.Azure.DataLake.Store) auf 1.1.9 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-516">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="d453b-517">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="d453b-517">AzureRM.EventHub</span></span>
* <span data-ttu-id="d453b-518">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-518">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="d453b-519">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="d453b-519">AzureRM.Insights</span></span>
* <span data-ttu-id="d453b-520">Formatierung von „OutputType“ in Hilfedateien korrigiert</span><span class="sxs-lookup"><span data-stu-id="d453b-520">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="d453b-521">Verwendung von Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span><span class="sxs-lookup"><span data-stu-id="d453b-521">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="d453b-522">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d453b-522">AzureRM.KeyVault</span></span>
* <span data-ttu-id="d453b-523">Piping-Problem in „Set-AzureRmKeyVaultAccessPolicy“ behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-523">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="d453b-524">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="d453b-524">AzureRM.Network</span></span>
* <span data-ttu-id="d453b-525">Beispiele für LoadBalancerInboundNatPoolConfig-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d453b-525">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="d453b-526">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="d453b-526">AzureRM.Resources</span></span>
* <span data-ttu-id="d453b-527">Problem beim Angeben sowohl des Tag-Namens als auch des Werts für „Get-AzureRmResource“ behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-527">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="d453b-528">Piping-Szenario mit „Set-AzureRmResource“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="d453b-528">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="d453b-529">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d453b-529">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="d453b-530">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-530">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="d453b-531">Einige Probleme behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-531">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="d453b-532">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="d453b-532">AzureRM.Sql</span></span>
* <span data-ttu-id="d453b-533">Unterstützung für Advanced Threat Protection für Server bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="d453b-533">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="d453b-534">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="d453b-534">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="d453b-535">Unterstützung für Sicherheitsrisikobewertung bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="d453b-535">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="d453b-536">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="d453b-536">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="d453b-537">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="d453b-537">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="d453b-538">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="d453b-538">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="d453b-539">Beispiel in „Remove-AzureRmSqlServerFirewallRule“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="d453b-539">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="d453b-540">Falsche Verarbeitung von „datetime“ für nicht US-basierte Kultur in „Get-AzureSqlSyncGroupLog“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="d453b-540">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="d453b-541">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="d453b-541">AzureRM.Storage</span></span>
* <span data-ttu-id="d453b-542">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-542">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="d453b-543">Cmdlet-Ausgabe von „StorageAccount“ in Tabellenansicht anzeigen</span><span class="sxs-lookup"><span data-stu-id="d453b-543">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="d453b-544">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d453b-544">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="d453b-545">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d453b-545">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="d453b-546">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d453b-546">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="d453b-547">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="d453b-547">AzureRM.Tags</span></span>
* <span data-ttu-id="d453b-548">Falsche Anweisung aus Tag-Cmdlet-Hilfe entfernt</span><span class="sxs-lookup"><span data-stu-id="d453b-548">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="d453b-549">6.5.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="d453b-549">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="d453b-550">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="d453b-550">AzureRM.Profile</span></span>
* <span data-ttu-id="d453b-551">Hilfe für „Get-AzureRmContextAutosaveSetting“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-551">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="d453b-552">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="d453b-552">Azure.Storage</span></span>
* <span data-ttu-id="d453b-553">Unterstützung des Blob- oder Dateiuploads mit lesegeschütztem SAS-Token</span><span class="sxs-lookup"><span data-stu-id="d453b-553">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="d453b-554">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="d453b-554">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="d453b-555">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="d453b-555">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="d453b-556">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="d453b-556">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="d453b-557">Erforderliche Eigenschaft „ResourceGroupName“ zu AS hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d453b-557">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="d453b-558">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="d453b-558">AzureRM.Automation</span></span>
* <span data-ttu-id="d453b-559">Hilfe aktualisiert und Beispiel für „New-AzureRMAutomationSchedule“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-559">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="d453b-560">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="d453b-560">AzureRM.Compute</span></span>
* <span data-ttu-id="d453b-561">Parameter „-Tag“ zu „Update/New-AzureRmAvailabilitySet“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-561">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="d453b-562">Beispiel für „Add-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-562">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="d453b-563">Beispiele für „Remove-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-563">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="d453b-564">Hilfe für „Set-AzureRmVMAccessExtension“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-564">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="d453b-565">„SimpleParameterSet“ für „New-AzureRmVmss“ so aktualisiert, dass „SinglePlacementGroup“ standardmäßig auf „false“ festgelegt ist, und Switch-Parameter „SinglePlacementGroup“ hinzugefügt, der dem Benutzer das Erstellen der VMSS in einer einzelnen Platzierungsgruppe ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="d453b-565">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="d453b-566">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="d453b-566">AzureRM.EventHub</span></span>
* <span data-ttu-id="d453b-567">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSEventHubDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="d453b-567">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="d453b-568">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d453b-568">AzureRM.KeyVault</span></span>
* <span data-ttu-id="d453b-569">Fehlermeldung für „Set-AzureRmKeyVaultAccessPolicy“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-569">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="d453b-570">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="d453b-570">AzureRM.LogicApp</span></span>
* <span data-ttu-id="d453b-571">Fehler „Parametersatz konnte nicht aufgelöst werden“ in „New-AzureRmLogicApp“behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-571">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="d453b-572">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="d453b-572">AzureRM.Network</span></span>
* <span data-ttu-id="d453b-573">Peering über mehrere virtuelle Netzwerke in mehreren Mandanten für „Set/Add-AzureRmVirtualNetworkPeering“ aktiviert</span><span class="sxs-lookup"><span data-stu-id="d453b-573">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="d453b-574">Folgende Cmdlets für Application Gateway aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-574">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="d453b-575">New-AzureRmApplicationGateway: EnableFIPS-Flag und Zonenunterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-575">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="d453b-576">New-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-576">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="d453b-577">Set-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-577">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="d453b-578">RouteTable-Cmdlets mit aktueller Generatorversion erneut generiert</span><span class="sxs-lookup"><span data-stu-id="d453b-578">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="d453b-579">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="d453b-579">AzureRM.Relay</span></span>
* <span data-ttu-id="d453b-580">Markdowndateien aktualisiert, Problem mit Parametername in Beispiel behoben</span><span class="sxs-lookup"><span data-stu-id="d453b-580">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="d453b-581">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="d453b-581">AzureRM.Resources</span></span>
* <span data-ttu-id="d453b-582">Roleassignment- und roledefinition-Cmdlets aktualisiert:</span><span class="sxs-lookup"><span data-stu-id="d453b-582">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="d453b-583">Zusätzliche roledefinition-Aufrufe entfernt, die als Teil des Pagings durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="d453b-583">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="d453b-584">Get-AzureRmRoleAssignment-Cmdlet korrigiert</span><span class="sxs-lookup"><span data-stu-id="d453b-584">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="d453b-585">Befehlsparameterfunktion von „-ExpandPrincipalGroups“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="d453b-585">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="d453b-586">Problem mit „Get-AzureRmResource“ behoben, aufgrund dessen die Groß-/Kleinschreibung des Parameters „-ResourceType“ beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="d453b-586">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="d453b-587">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d453b-587">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="d453b-588">top- und skip-Parameter zu Listen-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-588">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="d453b-589">Cmdlets für die Migration von Standard- zu Premium-Namespace hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="d453b-589">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="d453b-590">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="d453b-590">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="d453b-591">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="d453b-591">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="d453b-592">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="d453b-592">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="d453b-593">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="d453b-593">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="d453b-594">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="d453b-594">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="d453b-595">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSServiceBusDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="d453b-595">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="d453b-596">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d453b-596">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="d453b-597">Beispiel für „New-AzureRmServiceFabricCluster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-597">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="d453b-598">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="d453b-598">AzureRM.Sql</span></span>
* <span data-ttu-id="d453b-599">Neue Cmdlets für „Management.Sql“ hinzugefügt, um Kunden das Hinzufügen des TDE-Zertifikats zu einer SQL Server-Instanz oder einer verwalteten Instanz zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="d453b-599">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="d453b-600">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="d453b-600">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="d453b-601">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="d453b-601">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="d453b-602">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="d453b-602">AzureRM.Websites</span></span>
* <span data-ttu-id="d453b-603">Wenn `Set-AzureRmWebApp -AssignIdentity` und `Set-AzureRmWebAppSlot -AssignIdentity` auf „false“ festgelegt sind, wird jetzt die Identity-Eigenschaft aus dem Websiteobjekt entfernt. Auch das Vorschau-Tag wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="d453b-603">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="d453b-604">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics`-Beispiel aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-604">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="d453b-605">Unterstützung von `Set-AzureRmWebApp -PhpVersion` als gültige PHP-Version eingestellt</span><span class="sxs-lookup"><span data-stu-id="d453b-605">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="d453b-606">6.4.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="d453b-606">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="d453b-607">Allgemein</span><span class="sxs-lookup"><span data-stu-id="d453b-607">General</span></span>
* <span data-ttu-id="d453b-608">Formatierung von OutputType in Hilfedateien für die meisten Module korrigiert</span><span class="sxs-lookup"><span data-stu-id="d453b-608">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="d453b-609">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="d453b-609">AzureRM.Profile</span></span>
* <span data-ttu-id="d453b-610">Attribut „Ps1Xml“ wurde den Standardausgabetypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-610">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="d453b-611">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="d453b-611">AzureRM.Compute</span></span>
* <span data-ttu-id="d453b-612">IP-Tag-Funktion für VMSS</span><span class="sxs-lookup"><span data-stu-id="d453b-612">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="d453b-613">Cmdlet „New-AzureRmVmssIpTagConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-613">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="d453b-614">IpTag-Parameter zu „New-AzureRmVmssIpConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-614">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="d453b-615">Funktion für automatisches Betriebssystemrollback für VMSS</span><span class="sxs-lookup"><span data-stu-id="d453b-615">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="d453b-616">DisableAutoRollback-Parameter zu „New-AzureRmVmssConfig“ und „Update-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-616">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="d453b-617">Funktion für Upgradeverlauf des Betriebssystems für VMSS</span><span class="sxs-lookup"><span data-stu-id="d453b-617">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="d453b-618">Switch-Parameter „OSUpgradeHistory“ zu „Get-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-618">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="d453b-619">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="d453b-619">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="d453b-620">Unterstützung für Katalog-ACLs über die folgenden Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="d453b-620">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="d453b-621">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="d453b-621">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="d453b-622">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="d453b-622">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="d453b-623">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="d453b-623">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="d453b-624">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d453b-624">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="d453b-625">Abbruchunterstützung und Nachverfolgung des Fortschritts für „Set-AzureRmDataLakeStoreItemAclEntry“, „Remove-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-625">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="d453b-626">Abbruchunterstützung „Export-AzureRmDataLakeStoreChildItemProperties“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-626">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="d453b-627">Leerung von Debugmeldungen für Cmdlets korrigiert, die rekursive Vorgänge durchführt</span><span class="sxs-lookup"><span data-stu-id="d453b-627">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="d453b-628">Speicherort des Test von DataLake-Cmdlets korrigiert</span><span class="sxs-lookup"><span data-stu-id="d453b-628">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="d453b-629">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="d453b-629">AzureRM.EventHub</span></span>
* <span data-ttu-id="d453b-630">Optionaler Parameter „MaxCount“ zu Listenvorgangs-Cmdlets „Get-AzureRmEventHub“ und „Get-AzureRmEventHubConsumerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-630">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="d453b-631">Problem in Cmdlet „New-AzureRmEventHub“ behoben, aufgrund dessen beim Erstellen einer neuen EventHub-Instanz mindestens ein Parameter benötigt wurde.</span><span class="sxs-lookup"><span data-stu-id="d453b-631">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="d453b-632">Standardparametersatz wurde bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="d453b-632">Provided Default Parameter set.</span></span>
* <span data-ttu-id="d453b-633">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmEventHubKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="d453b-633">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="d453b-634">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d453b-634">AzureRM.KeyVault</span></span>
* <span data-ttu-id="d453b-635">Problem behoben, aufgrund dessen von „Get-AzureRmKeyVault -Tag“ alle Ressourcen zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="d453b-635">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="d453b-636">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="d453b-636">AzureRM.Network</span></span>
* <span data-ttu-id="d453b-637">Neue SKUs für zonenredundante VirtualNetworkGateways-Instanzen verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="d453b-637">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="d453b-638">Neue Befehle für Funktion hinzugefügt: ExpressRoute-Partner-APIs über ARM</span><span class="sxs-lookup"><span data-stu-id="d453b-638">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="d453b-639">Get-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-639">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="d453b-640">Set-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-640">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="d453b-641">Add-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-641">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="d453b-642">Get-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-642">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="d453b-643">Remove-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-643">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="d453b-644">Get-AzureRMExpressRouteCrossConnectionArpTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-644">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="d453b-645">Get-AzureRMExpressRouteCrossConnectionRouteTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-645">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="d453b-646">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-646">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="d453b-647">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="d453b-647">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="d453b-648">Cmdlet „Get-AzureRmRecoveryServicesBackupStatus“ wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d453b-648">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="d453b-649">Dieses Cmdlet überprüft anhand der ID eines virtuellen Computers, ob dieser durch einen Tresor im Abonnement geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="d453b-649">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="d453b-650">Wenn ein solcher Tresor vorhanden ist, gibt das Cmdlet die Tresordetails aus.</span><span class="sxs-lookup"><span data-stu-id="d453b-650">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="d453b-651">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="d453b-651">AzureRM.Resources</span></span>
* <span data-ttu-id="d453b-652">Cmdlets vom Typ „Get-AzureRmPolicyAssignment“ aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="d453b-652">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="d453b-653">Unterstützung für das Auflisten von „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-653">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="d453b-654">Unterstützung für das Abrufen einzelner Arbeitsaufträge mit „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-654">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="d453b-655">Switches „-Effective“ und „-All“ zu Steuerparameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-655">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="d453b-656">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicyDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-656">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="d453b-657">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="d453b-657">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="d453b-658">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="d453b-658">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="d453b-659">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicySetDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-659">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="d453b-660">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="d453b-660">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="d453b-661">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="d453b-661">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="d453b-662">Unterstützung für KeyVault-Geheimnisverweis in Parametern hinzugefügt, wenn „TemplateParameterObject“ in „New-AzureRmResourceGroupDeployment“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="d453b-662">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="d453b-663">Problem behoben, aufgrund dessen, der Parameter „-EndDate“ für „New-AzureRmADAppCredential“ ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="d453b-663">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="d453b-664">Problem behoben, aufgrund dessen „Add-AzureRmADGroupMember“ eine falsche URL für Anforderungen verwendete</span><span class="sxs-lookup"><span data-stu-id="d453b-664">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="d453b-665">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d453b-665">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="d453b-666">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmServiceBusKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="d453b-666">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="d453b-667">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="d453b-667">AzureRM.Sql</span></span>
* <span data-ttu-id="d453b-668">Benutzerdefinierte Wiederherstellungspunkte für SQLDW in Hilfe zu „New-AzureRmSqlDatabaseRestorePoint“ erläutert</span><span class="sxs-lookup"><span data-stu-id="d453b-668">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="d453b-669">Dokumentation von Parameter „-ComputeGeneration“ in mehreren Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-669">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="d453b-670">6.3.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="d453b-670">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="d453b-671">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="d453b-671">AzureRM.Profile</span></span>
* <span data-ttu-id="d453b-672">Aktualisierte Fehlermeldungen für „Enable-AzureRmContextAutoSave“</span><span class="sxs-lookup"><span data-stu-id="d453b-672">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="d453b-673">Erstellen eines Kontexts für jedes Abonnement beim Ausführen von „Connect-AzureRmAccount“ ohne vorherigen Kontext</span><span class="sxs-lookup"><span data-stu-id="d453b-673">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="d453b-674">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="d453b-674">Azure.Storage</span></span>
* <span data-ttu-id="d453b-675">Zusätzliche Informationen zum Parameter „-Permissions“ in Hilfedateien</span><span class="sxs-lookup"><span data-stu-id="d453b-675">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="d453b-676">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="d453b-676">AzureRM.Compute</span></span>
* <span data-ttu-id="d453b-677">„Get-AzureRmVmDiskEncryptionStatus“ behebt ein Problem, das bei virtuellen Computern ohne Datenträger festgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="d453b-677">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="d453b-678">Version der Computeclientbibliothek aktualisiert, um folgende Cmdlets zu korrigieren:</span><span class="sxs-lookup"><span data-stu-id="d453b-678">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="d453b-679">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="d453b-679">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="d453b-680">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="d453b-680">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="d453b-681">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="d453b-681">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="d453b-682">Die folgenden Cmdlets wurden korrigiert, um die Vorgangs-ID und den Vorgangsstatus korrekt anzuzeigen:</span><span class="sxs-lookup"><span data-stu-id="d453b-682">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="d453b-683">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="d453b-683">Start-AzureRmVM</span></span>
    - <span data-ttu-id="d453b-684">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="d453b-684">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="d453b-685">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="d453b-685">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="d453b-686">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="d453b-686">Set-AzureRmVM</span></span>
    - <span data-ttu-id="d453b-687">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="d453b-687">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="d453b-688">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="d453b-688">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="d453b-689">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="d453b-689">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="d453b-690">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="d453b-690">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="d453b-691">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="d453b-691">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="d453b-692">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="d453b-692">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="d453b-693">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="d453b-693">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="d453b-694">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="d453b-694">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="d453b-695">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="d453b-695">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="d453b-696">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="d453b-696">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="d453b-697">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="d453b-697">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="d453b-698">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="d453b-698">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="d453b-699">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="d453b-699">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="d453b-700">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="d453b-700">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="d453b-701">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="d453b-701">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="d453b-702">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="d453b-702">AzureRM.EventGrid</span></span>
* <span data-ttu-id="d453b-703">ValidateNotNullOrEmpty-Überprüfungskonditionen für „SubjectBeginsWith“/„SubjectEndsWith“ im Cmdlet „Update-AzureRmEventGridSubscription“ wurden entfernt, um bei Bedarf die Änderung dieser Parameter in eine leere Zeichenfolge zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="d453b-703">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="d453b-704">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d453b-704">AzureRM.KeyVault</span></span>
* <span data-ttu-id="d453b-705">Ein Problem wurde behoben, aufgrund dessen bei Ausführung von „Get-AzureRmKeyVault -Tag“ keine Tags zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="d453b-705">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="d453b-706">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="d453b-706">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="d453b-707">Offizielle Veröffentlichung von Policy Insights-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="d453b-707">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="d453b-708">Verwendung der API-Version 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="d453b-708">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="d453b-709">„PolicyDefinitionReferenceId“ zu den Ergebnissen von „Get-AzureRmPolicyStateSummary“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-709">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="d453b-710">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="d453b-710">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="d453b-711">Parameter „-Vault“ zu den RecoveryServices.Backup-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d453b-711">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="d453b-712">Bei der Übergabe wird dadurch das Cmdlet „Set-AzureRmRecoveryServicesContext“ außer Kraft gesetzt.</span><span class="sxs-lookup"><span data-stu-id="d453b-712">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="d453b-713">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="d453b-713">AzureRM.Sql</span></span>
* <span data-ttu-id="d453b-714">Aktualisiertes Beispiel in der Hilfedatei für „Get-AzureRmSqlDatabaseExpanded“</span><span class="sxs-lookup"><span data-stu-id="d453b-714">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="d453b-715">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="d453b-715">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="d453b-716">Hilfedatei für „Add-AzureRmTrafficManagerEndpointConfig“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d453b-716">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="d453b-717">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="d453b-717">AzureRM.Websites</span></span>
* <span data-ttu-id="d453b-718">„Set-AzureRmWebApp“ wurde aktualisiert, damit „AppSettings“ bei der Verwendung von „-AssignIdentity“ nicht außer Kraft gesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="d453b-718">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="d453b-719">„New-AzureRmWebAppSlot“ wurde aktualisiert, um „AppServicePlan“ als optionalen Parameter anzuerkennen</span><span class="sxs-lookup"><span data-stu-id="d453b-719">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="d453b-720">6.2.1: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="d453b-720">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="d453b-721">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="d453b-721">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="d453b-722">PSWorkspace-Modell aktualisiert, damit das Netzwerk „type“ als Parameter verwenden kann</span><span class="sxs-lookup"><span data-stu-id="d453b-722">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="d453b-723">6.2.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="d453b-723">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="d453b-724">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="d453b-724">AzureRM.Profile</span></span>
* <span data-ttu-id="d453b-725">Beheben des Problems, aufgrund dessen Version 10.0.3 von Newtonsoft.Json beim Modulimport nicht geladen wurde</span><span class="sxs-lookup"><span data-stu-id="d453b-725">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="d453b-726">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="d453b-726">AzureRM.Compute</span></span>
* <span data-ttu-id="d453b-727">Feature zum Aktualisieren von virtuellen VMSS-Computern</span><span class="sxs-lookup"><span data-stu-id="d453b-727">VMSS VM Update feature</span></span>
    - <span data-ttu-id="d453b-728">Cmdlets „Update-AzureRmVmssVM“ und „New-AzureRmVMDataDisk“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-728">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="d453b-729">Fügen Sie den Parameter „VirtualMachineScaleSetVM“ zum Cmdlet „Add-AzureRmVMDataDisk“ hinzu, um das Hinzufügen eines Datenträgers zum virtuellen VMSS-Computer zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="d453b-729">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="d453b-730">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="d453b-730">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="d453b-731">Aktualisierung der ADF .Net SDK-Version auf 0.8.0-preview mit den folgenden Änderungen:</span><span class="sxs-lookup"><span data-stu-id="d453b-731">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="d453b-732">Vorgang zum Konfigurieren des Factoryrepositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-732">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="d453b-733">Der verknüpfte QuickBooks-Dienst wurde aktualisiert, um die Eigenschaften „consumerKey“ und „consumerSecret“ verfügbar zu machen.</span><span class="sxs-lookup"><span data-stu-id="d453b-733">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="d453b-734">Aktualisierung verschiedener Modelltypen von „SecretBase“ auf „Object“</span><span class="sxs-lookup"><span data-stu-id="d453b-734">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="d453b-735">Blobereignisauslöser hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-735">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="d453b-736">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d453b-736">AzureRM.KeyVault</span></span>
* <span data-ttu-id="d453b-737">Aktualisierung der Dokumentation mit Beispielausgabe</span><span class="sxs-lookup"><span data-stu-id="d453b-737">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="d453b-738">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="d453b-738">AzureRM.Network</span></span>
* <span data-ttu-id="d453b-739">Aktivierung der Traffic Analytics-Parameter für Network Watcher-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="d453b-739">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="d453b-740">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="d453b-740">AzureRM.Resources</span></span>
* <span data-ttu-id="d453b-741">Behebung des Problems mit der Eigenschaft „Properties“ von PSResource-Objekten, die von „Get-AzureRmResource“ zurückgegeben wurden</span><span class="sxs-lookup"><span data-stu-id="d453b-741">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="d453b-742">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="d453b-742">AzureRM.Scheduler</span></span>
* <span data-ttu-id="d453b-743">Behebung des Problems, dass beim Aktualisieren von „ServiceBusQueueJob“ keine neuen Authentifizierungswerte festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="d453b-743">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="d453b-744">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="d453b-744">AzureRM.Sql</span></span>
* <span data-ttu-id="d453b-745">Aktualisierung der folgenden Cmdlets mit dem optionalen LicenseType-Parameter</span><span class="sxs-lookup"><span data-stu-id="d453b-745">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="d453b-746">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="d453b-746">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="d453b-747">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="d453b-747">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="d453b-748">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="d453b-748">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="d453b-749">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="d453b-749">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="d453b-750">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="d453b-750">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="d453b-751">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="d453b-751">AzureRM.Websites</span></span>
* <span data-ttu-id="d453b-752">„New-AzureRMWebApp“ aktualisiert, um allgemeine Algorithmen aus der Strategiebibliothek zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="d453b-752">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="d453b-753">6.1.0 – Mai 2018</span><span class="sxs-lookup"><span data-stu-id="d453b-753">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="d453b-754">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="d453b-754">AzureRM.Profile</span></span>
* <span data-ttu-id="d453b-755">Behebung eines Problems, durch das beim Ausführen von „Clear-AzureRmContext“ ein leerer Kontext mit dem Namen des vorherigen Standardkontexts beibehalten wurde und der Benutzer dadurch keinen neuen Kontext mit dem alten Namen erstellen konnte</span><span class="sxs-lookup"><span data-stu-id="d453b-755">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="d453b-756">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="d453b-756">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="d453b-757">Ermöglichung der Zuordnung von Gateways/Aufhebung der Gatewayzuordnung in AS</span><span class="sxs-lookup"><span data-stu-id="d453b-757">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="d453b-758">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d453b-758">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="d453b-759">Unterstützung für „ApiVersions“, „ApiReleases“ und „ApiRevisions“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-759">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="d453b-760">Unterstützung für ServiceFabric-Back-End hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-760">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="d453b-761">Unterstützung für Application Insights-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-761">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="d453b-762">Unterstützung für die Erkennung von SKUs vom Typ „Basic“ als gültige SKU des API Management-Diensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-762">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="d453b-763">Unterstützung hinzugefügt, damit Zertifikate, die von der privaten Zertifizierungsstelle ausgestellt wurden, als Stamm- oder ZS-Zertifikate installiert werden können</span><span class="sxs-lookup"><span data-stu-id="d453b-763">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="d453b-764">Unterstützung für die Akzeptierung benutzerdefinierter SSL-Zertifikate über KeyVault und mehrere Proxyhostnamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-764">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="d453b-765">Unterstützung für die verwaltete Dienstidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-765">Added support for MSI identity</span></span>
* <span data-ttu-id="d453b-766">Unterstützung für die Annahme von Richtlinien über URL hinzugefügt; HINWEIS: Folgende Cmdlets werden in einem zukünftigen Release als veraltet gekennzeichnet:</span><span class="sxs-lookup"><span data-stu-id="d453b-766">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="d453b-767">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="d453b-767">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="d453b-768">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="d453b-768">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="d453b-769">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="d453b-769">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="d453b-770">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="d453b-770">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="d453b-771">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="d453b-771">AzureRM.Batch</span></span>
* <span data-ttu-id="d453b-772">Veröffentlichung des neuen Cmdlets „Get-AzureBatchPoolNodeCounts“</span><span class="sxs-lookup"><span data-stu-id="d453b-772">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="d453b-773">Veröffentlichung des neuen Cmdlets „Start-AzureBatchComputeNodeServiceLogUpload“</span><span class="sxs-lookup"><span data-stu-id="d453b-773">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="d453b-774">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="d453b-774">AzureRM.Consumption</span></span>
* <span data-ttu-id="d453b-775">Hinzufügung neuer Parameter („Expand“, „ResourceGroup“, „InstanceName“, „InstanceId“, „Tags“ und „Top“) für das Cmdlet „Get-AzureRmConsumptionUsageDetail“</span><span class="sxs-lookup"><span data-stu-id="d453b-775">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="d453b-776">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d453b-776">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="d453b-777">Korrektur des Beispiels für „Export AzureRmDataLakeStoreChildItemProperties“</span><span class="sxs-lookup"><span data-stu-id="d453b-777">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="d453b-778">Korrektur der NULL-Parameterausnahme für rekursiven Fall in „Set-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="d453b-778">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="d453b-779">Korrektur der Hilfedateien für „Set-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ und „Remove-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="d453b-779">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="d453b-780">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="d453b-780">AzureRM.Network</span></span>
* <span data-ttu-id="d453b-781">Erhöhung der Network SDK-Version von 18.0.0-preview auf 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="d453b-781">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="d453b-782">Cmdlet zum Erstellen der Protokollkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-782">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="d453b-783">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="d453b-783">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="d453b-784">Cmdlet zum Hinzufügen einer neuen Leitungsverbindung zu einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-784">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="d453b-785">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-785">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="d453b-786">Cmdlet zum Entfernen einer Leitungsverbindung aus einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-786">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="d453b-787">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-787">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="d453b-788">Cmdlet zum Abrufen einer Leitungsverbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d453b-788">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="d453b-789">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="d453b-789">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="d453b-790">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d453b-790">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="d453b-791">Verwendung der Serverauthentifizierung mit generierten Zertifikaten korrigiert (Problemnr. 5998)</span><span class="sxs-lookup"><span data-stu-id="d453b-791">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="d453b-792">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="d453b-792">AzureRM.Sql</span></span>
* <span data-ttu-id="d453b-793">Überwachungscmdlets korrigiert, um das Entfernen von „AuditActions“ oder „AuditActionGroups“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="d453b-793">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="d453b-794">Problem mit „Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy“ behoben, das beim Festlegen einer neuen flexiblen Aufbewahrungsrichtlinie zu folgendem Fehler führte: „Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span><span class="sxs-lookup"><span data-stu-id="d453b-794">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="d453b-795">Please submit request with the new flexible retention policy“ (Das Konfigurieren einer langfristigen Aufbewahrungsrichtlinie mit Azure Recovery Service-Tresor und -Richtlinie wird nicht mehr unterstützt. Übermitteln Sie eine Anforderung mit der neuen flexiblen Aufbewahrungsrichtlinie.)</span><span class="sxs-lookup"><span data-stu-id="d453b-795">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="d453b-796">Aktualisierung aller Cmdlets für Azure SQL-Datenbank, für die Erstellung von Pools für elastische Datenbanken und für die Aktualisierung, sodass sie die neue Datenbank-API verwenden. Diese unterstützt die Sku-Eigenschaft für skalierungs- und tarifbezogene Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="d453b-796">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="d453b-797">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d453b-797">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="d453b-798">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="d453b-798">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="d453b-799">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="d453b-799">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="d453b-800">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="d453b-800">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="d453b-801">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="d453b-801">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="d453b-802">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="d453b-802">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="d453b-803">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="d453b-803">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="d453b-804">Aktualisierung der Parameter für „Get-AzureRmTrafficManagerProfile“, sodass bei Verwendung des Parameters „-Name“ der Parameter „-ResourceGroupName“ erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="d453b-804">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
