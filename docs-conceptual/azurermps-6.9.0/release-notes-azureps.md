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
ms.openlocfilehash: 3cb71087a61a0fcd06c014394e8f9e5654d4c1a8
ms.sourcegitcommit: 6c38e86e16da99f65cd183c63e34f7176b121ab8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/04/2018
ms.locfileid: "47425022"
---
# <a name="release-notes"></a><span data-ttu-id="90406-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="90406-103">Release notes</span></span>

<span data-ttu-id="90406-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="90406-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="690---september-2018"></a><span data-ttu-id="90406-105">6.9.0 – September 2018</span><span class="sxs-lookup"><span data-stu-id="90406-105">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="90406-106">Allgemein</span><span class="sxs-lookup"><span data-stu-id="90406-106">General</span></span>
* <span data-ttu-id="90406-107">AzureRM.SignalR wurde dem Rollupmodul AzureRM hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-107">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="90406-108">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="90406-108">AzureRM.Profile</span></span>
* <span data-ttu-id="90406-109">Kleinere Änderungen am allgemeinen Speichercode</span><span class="sxs-lookup"><span data-stu-id="90406-109">Minor changes to the storage common code</span></span>
* <span data-ttu-id="90406-110">Hilfedateien aktualisiert, um vollständige Parametertypen einzubinden.</span><span class="sxs-lookup"><span data-stu-id="90406-110">Updated help files to include full parameter types.</span></span>
- <span data-ttu-id="90406-111">„-ServicePrincipal“ im Parametersatz „ServicePrincipalCertificateWithSubscriptionId“ in nicht obligatorisch geändert</span><span class="sxs-lookup"><span data-stu-id="90406-111">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="90406-112">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="90406-112">Azure.Storage</span></span>
* <span data-ttu-id="90406-113">Unterstützung für die Erstellung des Speicherkontexts mit OAuth.</span><span class="sxs-lookup"><span data-stu-id="90406-113">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="90406-114">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="90406-114">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="90406-115">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="90406-115">AzureRM.Cdn</span></span>
* <span data-ttu-id="90406-116">Standard_Microsoft in SKU für CDN-Preise hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="90406-116">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="90406-117">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="90406-117">AzureRM.Compute</span></span>
* <span data-ttu-id="90406-118">Abhängigkeiten für Key Vault und Storage in allgemeine Abhängigkeiten verschieben</span><span class="sxs-lookup"><span data-stu-id="90406-118">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="90406-119">Unterstützung für weitere VM-Größen zu AEM-Cmdlets hinzufügen</span><span class="sxs-lookup"><span data-stu-id="90406-119">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="90406-120">Parameter „PublicIPPrefix“ zu „New-AzureRmVmssIpConfig“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="90406-120">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="90406-121">Parameter „ResourceId“ zu Cmdlet „Invoke-AzureRmVMRunCommand“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="90406-121">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="90406-122">Cmdlet „Invoke-AzureRmVmssVMRunCommand“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="90406-122">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="90406-123">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="90406-123">AzureRM.Dns</span></span>
* <span data-ttu-id="90406-124">Unterstützung für Aliaseintrag während der Erstellung des DNS-Eintrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-124">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="90406-125">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="90406-125">AzureRM.Insights</span></span>
* <span data-ttu-id="90406-126">Probleme #6833 und #7102 behoben (Bereich „Diagnoseeinstellungen“)</span><span class="sxs-lookup"><span data-stu-id="90406-126">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="90406-127">Probleme mit dem Standardnamen, also „service“, beim Erstellen und Auflisten/Abrufen von Diagnoseeinstellungen</span><span class="sxs-lookup"><span data-stu-id="90406-127">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="90406-128">Probleme beim Erstellen von Diagnoseeinstellungen mit Kategorien</span><span class="sxs-lookup"><span data-stu-id="90406-128">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="90406-129">Meldung zur Einstellung der Unterstützung für Metrikaggregationsintervall-Parameter</span><span class="sxs-lookup"><span data-stu-id="90406-129">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="90406-130">Aggregationsintervall-Parameter werden weiterhin akzeptiert (Änderung ohne Funktionsbeeinträchtigung), aber sie werden auf dem Back-End ignoriert, da nur PT1M gültig ist</span><span class="sxs-lookup"><span data-stu-id="90406-130">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="90406-131">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="90406-131">AzureRM.Network</span></span>
* <span data-ttu-id="90406-132">Änderungen an LoadBalancer-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="90406-132">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="90406-133">LoadBalancerInboundNatPoolConfig: Parameter IdleTimeoutInMinutes, EnableFloatingIp und EnableTcpReset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-133">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="90406-134">LoadBalancerInboundNatRuleConfig: Parameter EnableTcpReset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-134">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="90406-135">LoadBalancerRuleConfig: Parameter EnableTcpReset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-135">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="90406-136">LoadBalancerProbeConfig: Unterstützung für Wert „Https“ für Parameter „Protocol“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-136">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="90406-137">Neue Befehle für neue Unterressource „OutboundRule“ von LoadBalancer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-137">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="90406-138">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="90406-138">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="90406-139">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="90406-139">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="90406-140">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="90406-140">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="90406-141">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="90406-141">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="90406-142">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="90406-142">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="90406-143">Neue HostedWorkloads-Eigenschaft für PSNetworkInterface hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-143">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="90406-144">Neue Cmdlets für Feature: Azure Firewall über ARM</span><span class="sxs-lookup"><span data-stu-id="90406-144">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="90406-145">Get-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-145">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="90406-146">Set-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-146">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="90406-147">New-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-147">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="90406-148">Remove-AzureRmFirewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-148">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="90406-149">New-AzureRmFirewallApplicationRuleCollection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-149">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="90406-150">New-AzureRmFirewallApplicationRule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-150">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="90406-151">New-AzureRmFirewallNatRuleCollection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-151">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="90406-152">New-AzureRmFirewallNatRule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-152">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="90406-153">New-AzureRmFirewallNetworkRuleCollection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-153">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="90406-154">New-AzureRmFirewallNetworkRule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-154">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="90406-155">Unterstützung für vertrauenswürdiges Stammzertifikat und Konfiguration der automatischen Skalierung in Application Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-155">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="90406-156">Neue Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="90406-156">New Cmdlets added:</span></span>
      - <span data-ttu-id="90406-157">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="90406-157">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="90406-158">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="90406-158">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="90406-159">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="90406-159">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="90406-160">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="90406-160">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="90406-161">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="90406-161">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="90406-162">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="90406-162">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="90406-163">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="90406-163">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="90406-164">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="90406-164">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="90406-165">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="90406-165">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="90406-166">Cmdlets mit optionalem Parameter „-TrustedRootCertificate“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-166">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="90406-167">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="90406-167">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="90406-168">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="90406-168">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="90406-169">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="90406-169">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="90406-170">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="90406-170">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="90406-171">Cmdlets mit optionalem Parameter „-AutoscaleConfiguration“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-171">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="90406-172">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="90406-172">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="90406-173">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="90406-173">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="90406-174">Cmdlet für Schnittstellenendpunkt Get-AzureInterfaceEndpoint hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-174">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="90406-175">Unterstützung für mehrere Adresspräfixe in einem Subnetz hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="90406-175">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="90406-176">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="90406-176">Updated cmdlets:</span></span>
  - <span data-ttu-id="90406-177">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="90406-177">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="90406-178">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="90406-178">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="90406-179">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="90406-179">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="90406-180">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="90406-180">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="90406-181">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="90406-181">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="90406-182">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="90406-182">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="90406-183">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="90406-183">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="90406-184">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="90406-184">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="90406-185">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="90406-185">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="90406-186">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="90406-186">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="90406-187">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="90406-187">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="90406-188">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="90406-188">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="90406-189">New-AzureRmNetworkInterfaceIpConfig – Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="90406-189">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="90406-190">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="90406-190">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="90406-191">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="90406-191">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="90406-192">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="90406-192">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="90406-193">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="90406-193">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="90406-194">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="90406-194">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="90406-195">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="90406-195">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="90406-196">Cmdlets für die Subnetzdelegierung hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="90406-196">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="90406-197">New-AzureRmDelegation: Erstellt eine neue Delegierung, die einem Subnetz hinzugefügt werden kann</span><span class="sxs-lookup"><span data-stu-id="90406-197">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="90406-198">Remove-AzureRmDelegation: Nutzt ein Subnetz und entfernt den bereitgestellten Delegierungsnamen aus diesem Subnetz</span><span class="sxs-lookup"><span data-stu-id="90406-198">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="90406-199">Add-AzureRmDelegation: Nutzt ein Subnetz und fügt den angegebenen Dienstnamen diesem Subnetz als Delegierung hinzu</span><span class="sxs-lookup"><span data-stu-id="90406-199">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="90406-200">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="90406-200">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="90406-201">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="90406-201">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="90406-202">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="90406-202">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="90406-203">Unterstützung für verwalteten Datenträger</span><span class="sxs-lookup"><span data-stu-id="90406-203">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="90406-204">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="90406-204">AzureRM.RedisCache</span></span>
* <span data-ttu-id="90406-205">Insights-Abhängigkeit aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="90406-205">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="90406-206">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="90406-206">AzureRM.Resources</span></span>
* <span data-ttu-id="90406-207">New-AzureRmResourceGroupDeployment mit neuem Parameter „RollbackAction“ aktualisieren</span><span class="sxs-lookup"><span data-stu-id="90406-207">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="90406-208">Unterstützung für OnErrorDeployment mit dem neuen Parameter hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="90406-208">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="90406-209">Unterstützung für verwaltete Identität in Richtlinienzuweisungen.</span><span class="sxs-lookup"><span data-stu-id="90406-209">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="90406-210">Parameter mit Standardwerten sind nicht mehr erforderlich, wenn eine Richtlinie mit „New-AzureRmPolicyAssignment“ zugewiesen wird</span><span class="sxs-lookup"><span data-stu-id="90406-210">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="90406-211">Neues Cmdlet „Get-AzureRmPolicyAlias“ zum Abrufen von Richtlinienaliasen hinzufügen</span><span class="sxs-lookup"><span data-stu-id="90406-211">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="90406-212">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="90406-212">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="90406-213">Problem #7161 behoben</span><span class="sxs-lookup"><span data-stu-id="90406-213">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="90406-214">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="90406-214">AzureRM.SignalR</span></span>
* <span data-ttu-id="90406-215">SKU-Namen auf Free_F1 und Standard_S1 aktualisieren</span><span class="sxs-lookup"><span data-stu-id="90406-215">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="90406-216">Versionsfeld zum PSSignalRResource-Objekt und Verbindungszeichenfolge zum PSSignalRKeys-Objekt hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="90406-216">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="90406-217">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="90406-217">AzureRM.Storage</span></span>
* <span data-ttu-id="90406-218">Unterstützung für Unveränderlichkeitsrichtlinie in AzureRm.Storage</span><span class="sxs-lookup"><span data-stu-id="90406-218">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="90406-219">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="90406-219">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="90406-220">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="90406-220">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="90406-221">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="90406-221">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="90406-222">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="90406-222">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="90406-223">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="90406-223">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="90406-224">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="90406-224">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="90406-225">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="90406-225">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="90406-226">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="90406-226">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="90406-227">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="90406-227">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="90406-228">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="90406-228">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="90406-229">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="90406-229">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="90406-230">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="90406-230">AzureRM.Websites</span></span>
* <span data-ttu-id="90406-231">Zwei neue Cmdlets hinzugefügt: Get-AzureRmDeletedWebApp und Restore-AzureRmDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="90406-231">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="90406-232">New-AzureRmAppServicePlan -HyperV-Switch für „App Service-Plan erstellen“ mit Windows-Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-232">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="90406-233">New-AzureRmWebApp/New-AzureRmWebAppSlot/Set-AzureRmWebApp/Set-AzureRmWebAppSlot: Neue Parameter (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) für die Erstellung und Verwaltung der Windows-Container-App hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-233">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="90406-234">6.8.1: August 2018</span><span class="sxs-lookup"><span data-stu-id="90406-234">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="90406-235">Allgemein</span><span class="sxs-lookup"><span data-stu-id="90406-235">General</span></span>
* <span data-ttu-id="90406-236">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="90406-236">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="90406-237">Allgemeine Laufzeitassemblys aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-237">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="90406-238">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="90406-238">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="90406-239">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="90406-239">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="90406-240">Problem https://github.com/Azure/azure-powershell/issues/6603 behoben</span><span class="sxs-lookup"><span data-stu-id="90406-240">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="90406-241">Die Cmdlets „Import-AzureRmApiManagementApi“ und „\*-AzureRmApiManagementCertificate“ können jetzt relative Pfade verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="90406-241">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="90406-242">Problem https://github.com/Azure/azure-powershell/issues/6879 behoben</span><span class="sxs-lookup"><span data-stu-id="90406-242">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="90406-243">„CertificateInformation“ ist eine festlegbare Eigenschaft, die die ordnungsgemäße Funktionsweise des Cmdlets „Set-AzureRmApiManagement“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="90406-243">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="90406-244">Behoben durch Upgrade auf NuGet-Paket „4.0.4-preview“</span><span class="sxs-lookup"><span data-stu-id="90406-244">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="90406-245">Problem https://github.com/Azure/azure-powershell/issues/6853 behoben</span><span class="sxs-lookup"><span data-stu-id="90406-245">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="90406-246">OData-Filter für die Suche anhand des Namens korrigiert (Produkt)</span><span class="sxs-lookup"><span data-stu-id="90406-246">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="90406-247">Problem https://github.com/Azure/azure-powershell/issues/6814 behoben</span><span class="sxs-lookup"><span data-stu-id="90406-247">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="90406-248">OData-Filter für die Suche anhand des Namens korrigiert (API)</span><span class="sxs-lookup"><span data-stu-id="90406-248">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="90406-249">Unterstützung für AzureMonitor-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-249">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="90406-250">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="90406-250">AzureRM.Compute</span></span>
* <span data-ttu-id="90406-251">Problem des fehlenden Ziels in der Fehlerausgabe behoben</span><span class="sxs-lookup"><span data-stu-id="90406-251">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="90406-252">Problem mit dem Speicherkontotyp für den virtuellen Computer mit verwaltetem Datenträgern behoben</span><span class="sxs-lookup"><span data-stu-id="90406-252">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="90406-253">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="90406-253">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="90406-254">AEM-Erweiterungs-Cmdlets für andere Umgebungen (etwa Azure China) korrigiert</span><span class="sxs-lookup"><span data-stu-id="90406-254">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="90406-255">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="90406-255">AzureRM.Network</span></span>
* <span data-ttu-id="90406-256">Standarddarstellung der Cmdlet-Ausgabe in Tabellenansicht geändert</span><span class="sxs-lookup"><span data-stu-id="90406-256">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="90406-257">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="90406-257">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="90406-258">Fehler in „Update-AzureRmPowerBIEmbeddedCapacity“ beim Skalieren der angehaltenen Kapazität behoben</span><span class="sxs-lookup"><span data-stu-id="90406-258">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="90406-259">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="90406-259">AzureRM.Resources</span></span>
* <span data-ttu-id="90406-260">Problem beim Erstellen verwalteter Anwendungen über Marketplace behoben</span><span class="sxs-lookup"><span data-stu-id="90406-260">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="90406-261">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="90406-261">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="90406-262">Behobene Probleme</span><span class="sxs-lookup"><span data-stu-id="90406-262">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="90406-263">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="90406-263">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="90406-264">Unterstützung für Routingmethode „MultiValue“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-264">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="90406-265">Neuer Parameter „MaxReturn“ für Routingtyp „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="90406-265">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="90406-266">Unterstützung für Subnetzroutingmethode hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-266">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="90406-267">Unterstützung für IP-Adressbereiche (Subnetze) in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="90406-267">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="90406-268">Unterstützung für benutzerdefinierte Header in Profilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-268">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="90406-269">Unterstützung für erwartete Statuscodebereiche in Profilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-269">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="90406-270">Unterstützung für benutzerdefinierte Header in Endpunkten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-270">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="90406-271">6.8.0: August 2018</span><span class="sxs-lookup"><span data-stu-id="90406-271">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="90406-272">Allgemein</span><span class="sxs-lookup"><span data-stu-id="90406-272">General</span></span>
* <span data-ttu-id="90406-273">Das Problem, dass Standardressourcengruppen nicht festgelegt wurden, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="90406-273">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="90406-274">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="90406-274">AzureRM.Profile</span></span>
* <span data-ttu-id="90406-275">Ablaufeigenschaft zu Token hinzugefügt, die während „Connect-AzureRmAccount“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="90406-275">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="90406-276">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="90406-276">AzureRM.Compute</span></span>
* <span data-ttu-id="90406-277">Problem des fehlenden Ziels in der Fehlerausgabe behoben</span><span class="sxs-lookup"><span data-stu-id="90406-277">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="90406-278">Problem mit dem Speicherkontotyp für den virtuellen Computer mit verwaltetem Datenträgern behoben</span><span class="sxs-lookup"><span data-stu-id="90406-278">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="90406-279">AEM-Erweiterungs-Cmdlets für andere Umgebungen (etwa Azure China) korrigiert</span><span class="sxs-lookup"><span data-stu-id="90406-279">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="90406-280">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="90406-280">AzureRM.IotHub</span></span>
* <span data-ttu-id="90406-281">Beispiele für „New-AzureRmIotHubExportDevices“ und „New-AzureRmIotHubImportDevices“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="90406-281">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="90406-282">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="90406-282">AzureRM.Network</span></span>
* <span data-ttu-id="90406-283">Standarddarstellung von Modellen in Tabellenansicht geändert</span><span class="sxs-lookup"><span data-stu-id="90406-283">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="90406-284">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="90406-284">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="90406-285">Fehler in „Update-AzureRmPowerBIEmbeddedCapacity“ beim Skalieren der angehaltenen Kapazität behoben</span><span class="sxs-lookup"><span data-stu-id="90406-285">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="90406-286">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="90406-286">AzureRM.Resources</span></span>
* <span data-ttu-id="90406-287">Problem beim Erstellen der verwalteten Anwendung über Marketplace behoben</span><span class="sxs-lookup"><span data-stu-id="90406-287">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="90406-288">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="90406-288">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="90406-289">Fehlerbehebung</span><span class="sxs-lookup"><span data-stu-id="90406-289">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="90406-290">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="90406-290">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="90406-291">Unterstützung für Routingmethode „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="90406-291">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="90406-292">Neuer Parameter „MaxReturn“ für Routingtyp „MultiValue“</span><span class="sxs-lookup"><span data-stu-id="90406-292">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="90406-293">Unterstützung für Subnetzroutingmethode</span><span class="sxs-lookup"><span data-stu-id="90406-293">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="90406-294">Unterstützung für IP-Adressbereiche (Subnetze) in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="90406-294">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="90406-295">Unterstützung für benutzerdefinierte Header in Profilen</span><span class="sxs-lookup"><span data-stu-id="90406-295">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="90406-296">Unterstützung für erwartete Statuscodebereiche in Profilen</span><span class="sxs-lookup"><span data-stu-id="90406-296">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="90406-297">Unterstützung für benutzerdefinierte Header in Endpunkten</span><span class="sxs-lookup"><span data-stu-id="90406-297">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="90406-298">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="90406-298">AzureRM.Websites</span></span>
* <span data-ttu-id="90406-299">Das Problem, dass die Standardressourcengruppe falsch festgelegt wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="90406-299">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="90406-300">6.7.0: August 2018</span><span class="sxs-lookup"><span data-stu-id="90406-300">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="90406-301">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="90406-301">AzureRM.Profile</span></span>
* <span data-ttu-id="90406-302">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-302">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="90406-303">Benutzer-ID zum Standardkontextnamen hinzugefügt, um Kontextkonflikte zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="90406-303">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="90406-304">Probleme mit „Clear-AzureRmContext“ behoben, die Fehler beim Auswählen eines Kontexts verursacht haben (6398)</span><span class="sxs-lookup"><span data-stu-id="90406-304">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="90406-305">Ermöglicht, dass für „Connect-AzureRmAccount“ die Mandantendomäne an den Parameter „-TenantId“ übergeben wird</span><span class="sxs-lookup"><span data-stu-id="90406-305">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="90406-306">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="90406-306">Azure.Storage</span></span>
* <span data-ttu-id="90406-307">Begrenzung von 5 TB für das Kontingent der Azure-Dateifreigabe entfernt</span><span class="sxs-lookup"><span data-stu-id="90406-307">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="90406-308">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="90406-308">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="90406-309">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="90406-309">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="90406-310">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-310">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="90406-311">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="90406-311">Azure.AnalysisServices</span></span>
* <span data-ttu-id="90406-312">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-312">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="90406-313">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="90406-313">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="90406-314">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-314">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="90406-315">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="90406-315">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="90406-316">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-316">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="90406-317">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="90406-317">AzureRM.Automation</span></span>
* <span data-ttu-id="90406-318">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-318">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="90406-319">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="90406-319">AzureRM.Backup</span></span>
* <span data-ttu-id="90406-320">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-320">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="90406-321">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="90406-321">AzureRM.Batch</span></span>
* <span data-ttu-id="90406-322">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-322">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="90406-323">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="90406-323">AzureRM.Billing</span></span>
* <span data-ttu-id="90406-324">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-324">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="90406-325">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="90406-325">AzureRM.Cdn</span></span>
* <span data-ttu-id="90406-326">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-326">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="90406-327">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="90406-327">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="90406-328">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-328">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="90406-329">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="90406-329">AzureRM.Compute</span></span>
* <span data-ttu-id="90406-330">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-330">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="90406-331">EvictionPolicy-Parameter zu „New-AzureRmVmssConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-331">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="90406-332">Standort in „DiskFileParameterSet“ von „New-AzureRmVm“ angeben, wenn kein Ort angegeben ist</span><span class="sxs-lookup"><span data-stu-id="90406-332">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="90406-333">Parameterbeschreibung in „Save-AzureRmVMImage“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="90406-333">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="90406-334">Cmdlet „Get-AzureRmVMDiskEncryptionStatus“ für bestimmte Szenarien im Zusammenhang mit einem Durchlauf korrigiert</span><span class="sxs-lookup"><span data-stu-id="90406-334">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="90406-335">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="90406-335">AzureRM.Consumption</span></span>
* <span data-ttu-id="90406-336">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-336">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="90406-337">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="90406-337">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="90406-338">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-338">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="90406-339">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="90406-339">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="90406-340">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-340">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="90406-341">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="90406-341">AzureRM.DataFactories</span></span>
* <span data-ttu-id="90406-342">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-342">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="90406-343">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="90406-343">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="90406-344">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-344">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="90406-345">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="90406-345">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="90406-346">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-346">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="90406-347">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="90406-347">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="90406-348">Debuggen korrigiert, wenn „DebugPreference“ über die PowerShell-Befehlszeile festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="90406-348">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="90406-349">Beispiel für „Set-AzureRmDataLakeStoreItemAcl“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-349">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="90406-350">Aktualisiert auf die aktuelle Version von Azure ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="90406-350">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="90406-351">Beispiel für „Set-AzureRmDataLakeStoreItemAclEntry“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-351">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="90406-352">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="90406-352">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="90406-353">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-353">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="90406-354">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="90406-354">AzureRM.Dns</span></span>
* <span data-ttu-id="90406-355">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-355">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="90406-356">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="90406-356">AzureRM.EventGrid</span></span>
* <span data-ttu-id="90406-357">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-357">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="90406-358">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="90406-358">AzureRM.EventHub</span></span>
* <span data-ttu-id="90406-359">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-359">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="90406-360">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="90406-360">AzureRM.HDInsight</span></span>
* <span data-ttu-id="90406-361">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-361">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="90406-362">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="90406-362">AzureRM.Insights</span></span>
* <span data-ttu-id="90406-363">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-363">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="90406-364">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="90406-364">AzureRM.IotHub</span></span>
* <span data-ttu-id="90406-365">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-365">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="90406-366">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="90406-366">AzureRM.KeyVault</span></span>
* <span data-ttu-id="90406-367">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-367">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="90406-368">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="90406-368">AzureRM.LogicApp</span></span>
* <span data-ttu-id="90406-369">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-369">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="90406-370">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="90406-370">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="90406-371">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-371">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="90406-372">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="90406-372">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="90406-373">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-373">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="90406-374">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="90406-374">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="90406-375">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-375">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="90406-376">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="90406-376">AzureRM.Media</span></span>
* <span data-ttu-id="90406-377">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-377">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="90406-378">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="90406-378">AzureRM.Network</span></span>
* <span data-ttu-id="90406-379">Beispiel für „Set-AzureRmLocalNetworkGateway“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-379">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="90406-380">Beispiele und Beschreibungen für „Add-AzureRmVirtualNetworkGatewayIpConfig“, „Get-AzureRmVirtualNetworkGatewayConnectionSharedKey“ und „New-AzureRmVirtualNetworkGatewayConnection“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-380">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="90406-381">Beispiele für „Remove-AzureRmVirtualNetworkGatewayIpConfig“ und „Reset-AzureRmVirtualNetworkGateway“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-381">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="90406-382">Beispiel für „Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-382">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="90406-383">Beispiel für „Set-AzureRmVirtualNetworkGatewayConnectionSharedKey“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-383">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="90406-384">Beispiel für „Set-AzureRmVirtualNetworkGatewayConnection“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-384">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="90406-385">Cmdlets für „ApplicationSecurityGroup“, „RouteTable“ und „Usage“ mithilfe des aktuellen Code-Generators erneut erstellt</span><span class="sxs-lookup"><span data-stu-id="90406-385">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="90406-386">Deutlichere Formulierung der Fehlermeldung für „Get-AzureRmVirtualNetworkSubnetConfig“, wenn ein nicht vorhandenes Subnetz abgerufen wird</span><span class="sxs-lookup"><span data-stu-id="90406-386">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="90406-387">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="90406-387">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="90406-388">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-388">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="90406-389">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="90406-389">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="90406-390">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-390">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="90406-391">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="90406-391">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="90406-392">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-392">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="90406-393">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="90406-393">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="90406-394">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-394">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="90406-395">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="90406-395">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="90406-396">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-396">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="90406-397">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="90406-397">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="90406-398">Richtlinienfilter zum Cmdlet „Get-AzureRmRecoveryServicesBackItem“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="90406-398">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="90406-399">Der Befehl gibt die Liste der Sicherungselemente zurück, die durch die angegebene Richtlinien-ID geschützt sind.</span><span class="sxs-lookup"><span data-stu-id="90406-399">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="90406-400">„Microsoft.Azure.Management.RecoveryServices.Backup“ auf Version 3.0.0-preview aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-400">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="90406-401">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-401">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="90406-402">TargetResourceGroupName-Parameter zu „Restore-AzureRmRecoveryServicesBackupItem“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="90406-402">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="90406-403">Die Ressourcengruppe, in der die verwalteten Datenträger wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="90406-403">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="90406-404">Gilt für die Sicherung des virtuellen Computers mit verwalteten Datenträgern.</span><span class="sxs-lookup"><span data-stu-id="90406-404">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="90406-405">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="90406-405">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="90406-406">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-406">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="90406-407">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="90406-407">AzureRM.RedisCache</span></span>
* <span data-ttu-id="90406-408">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-408">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="90406-409">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="90406-409">AzureRM.Relay</span></span>
* <span data-ttu-id="90406-410">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-410">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="90406-411">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="90406-411">AzureRM.Resources</span></span>
* <span data-ttu-id="90406-412">Unterstützung der Vorlagenbereitstellung im Abonnementbereich.</span><span class="sxs-lookup"><span data-stu-id="90406-412">Support template deployment at subscription scope.</span></span> <span data-ttu-id="90406-413">Neue Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="90406-413">Add new Cmdlets:</span></span>
    - <span data-ttu-id="90406-414">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="90406-414">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="90406-415">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="90406-415">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="90406-416">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="90406-416">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="90406-417">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="90406-417">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="90406-418">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="90406-418">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="90406-419">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="90406-419">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="90406-420">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="90406-420">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="90406-421">Problem behoben, aufgrund dessen beim Übergeben eines Kontexts an „Set-AzureRmResource“ ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="90406-421">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="90406-422">Beispiel in „New-AzureRmResourceGroupDeployment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="90406-422">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="90406-423">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-423">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="90406-424">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="90406-424">AzureRM.Scheduler</span></span>
* <span data-ttu-id="90406-425">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-425">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="90406-426">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="90406-426">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="90406-427">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-427">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="90406-428">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="90406-428">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="90406-429">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-429">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="90406-430">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="90406-430">AzureRM.Sql</span></span>
* <span data-ttu-id="90406-431">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-431">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="90406-432">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="90406-432">AzureRM.Storage</span></span>
* <span data-ttu-id="90406-433">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-433">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="90406-434">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="90406-434">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="90406-435">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-435">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="90406-436">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="90406-436">AzureRM.Tags</span></span>
* <span data-ttu-id="90406-437">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-437">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="90406-438">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="90406-438">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="90406-439">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-439">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="90406-440">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="90406-440">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="90406-441">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-441">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="90406-442">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="90406-442">AzureRM.Websites</span></span>
* <span data-ttu-id="90406-443">Auf die aktuelle Version von Azure ClientRuntime aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-443">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="90406-444">6.6.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="90406-444">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="90406-445">Allgemein</span><span class="sxs-lookup"><span data-stu-id="90406-445">General</span></span>
* <span data-ttu-id="90406-446">Alle Hilfedateien aktualisiert, um vollständige Parametertypen und die richtigen Eingabe/Ausgabe-Typen einzuschließen.</span><span class="sxs-lookup"><span data-stu-id="90406-446">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="90406-447">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="90406-447">AzureRM.Profile</span></span>
* <span data-ttu-id="90406-448">Bibliothek „Common.Strategy“ aktualisiert, um überprüfen zu können, ob die aktuelle Konfiguration für eine Ressource mit der Zielressource kompatibel ist.</span><span class="sxs-lookup"><span data-stu-id="90406-448">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="90406-449">ps1xml-Typen zu „Common.Storage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-449">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="90406-450">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="90406-450">Azure.Storage</span></span>
* <span data-ttu-id="90406-451">Unterstützung zum Abrufen von Speicherkontext aus „DefaultProfile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-451">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="90406-452">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-452">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="90406-453">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="90406-453">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="90406-454">Problem https://github.com/Azure/azure-powershell/issues/6370 behoben</span><span class="sxs-lookup"><span data-stu-id="90406-454">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="90406-455">Fehler in Automapper behoben, um „PsApiManagementApi“ in „ApiContract“ zu verschieben</span><span class="sxs-lookup"><span data-stu-id="90406-455">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="90406-456">Problem https://github.com/Azure/azure-powershell/issues/6515 behoben</span><span class="sxs-lookup"><span data-stu-id="90406-456">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="90406-457">Fehler in „File.Save“ behoben, um Überladung mit Codierungstyp zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="90406-457">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="90406-458">Problem https://github.com/Azure/azure-powershell/issues/6560 behoben</span><span class="sxs-lookup"><span data-stu-id="90406-458">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="90406-459">Upgrade auf Nuget-Version 4.0.3 durchgeführt, in der Musterausnahme in „apiId“ behoben wurde</span><span class="sxs-lookup"><span data-stu-id="90406-459">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="90406-460">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="90406-460">AzureRM.Compute</span></span>
* <span data-ttu-id="90406-461">Das Problem, aufgrund dessen beim Erstellen eines virtuellen Computers mithilfe von „DiskFileParameterSet“ in „New-AzureRmVm“ wegen einer Umbenennung des Speicherkontotyps „PremiumLRS“ ein Fehler auftrat, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="90406-461">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="90406-462">Cmdlet „Invoke-AzureRmVMRunCommand“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="90406-462">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="90406-463">„Get-AzureRmAvailabilitySet“ aktualisiert, um die Auflistung aller Verfügbarkeitsgruppen in einem Abonnement zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="90406-463">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="90406-464">(ResouceGroupName-Parameter ist jetzt optional.)</span><span class="sxs-lookup"><span data-stu-id="90406-464">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="90406-465">„SimpleParameterSet“ von „New-AzureRmVm“ aktualisiert, um Accelerated Networking auf kompatiblen virtuellen Computern zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="90406-465">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="90406-466">Einfacher Parametersatz „New-AzureRmVmss“ aktualisiert, sodass das Erstellen der VMSS fehlschlägt, wenn bereits ein benutzerdefinierter LB vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="90406-466">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="90406-467">Beispiel für „New-AzureRmDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-467">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="90406-468">Beispiel für „New-AzureRmVM“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-468">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="90406-469">Beschreibung für „Set-AzureRmVMOSDisk“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-469">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="90406-470">Beispiel 1 für „Set-AzureRmVMBginfoExtension“ aktualisiert, um Rechtschreibung und Präfix zu korrigieren.</span><span class="sxs-lookup"><span data-stu-id="90406-470">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="90406-471">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="90406-471">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="90406-472">ADF .Net SDK-Version auf 1.1.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="90406-472">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="90406-473">Unterstützung der Freigabe der selbstgehosteten Integration Runtime über Data Factorys hinweg.</span><span class="sxs-lookup"><span data-stu-id="90406-473">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="90406-474">Neuer Parameter „-SharedIntegrationRuntimeResourceId“ zu Cmdlet „Set-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="90406-474">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="90406-475">Neuer optionaler Parameter „-LinkedDataFactoryName“ zu Cmdlet „Remove-AzureRmDataFactoryV2IntegrationRuntime“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="90406-475">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="90406-476">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="90406-476">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="90406-477">DataPlane SDK-Version (Microsoft.Azure.DataLake.Store) auf 1.1.9 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-477">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="90406-478">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="90406-478">AzureRM.EventHub</span></span>
* <span data-ttu-id="90406-479">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-479">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="90406-480">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="90406-480">AzureRM.Insights</span></span>
* <span data-ttu-id="90406-481">Formatierung von „OutputType“ in Hilfedateien korrigiert</span><span class="sxs-lookup"><span data-stu-id="90406-481">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="90406-482">Verwendung von Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span><span class="sxs-lookup"><span data-stu-id="90406-482">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="90406-483">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="90406-483">AzureRM.KeyVault</span></span>
* <span data-ttu-id="90406-484">Piping-Problem in „Set-AzureRmKeyVaultAccessPolicy“ behoben</span><span class="sxs-lookup"><span data-stu-id="90406-484">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="90406-485">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="90406-485">AzureRM.Network</span></span>
* <span data-ttu-id="90406-486">Beispiele für LoadBalancerInboundNatPoolConfig-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="90406-486">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="90406-487">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="90406-487">AzureRM.Resources</span></span>
* <span data-ttu-id="90406-488">Problem beim Angeben sowohl des Tag-Namens als auch des Werts für „Get-AzureRmResource“ behoben</span><span class="sxs-lookup"><span data-stu-id="90406-488">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="90406-489">Piping-Szenario mit „Set-AzureRmResource“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="90406-489">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="90406-490">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="90406-490">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="90406-491">Piping für „InputObject“ und „ResourceId“ in Entfernungs-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-491">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="90406-492">Einige Probleme behoben</span><span class="sxs-lookup"><span data-stu-id="90406-492">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="90406-493">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="90406-493">AzureRM.Sql</span></span>
* <span data-ttu-id="90406-494">Unterstützung für Advanced Threat Protection für Server bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="90406-494">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="90406-495">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="90406-495">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="90406-496">Unterstützung für Sicherheitsrisikobewertung bei folgenden Cmdlets hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="90406-496">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="90406-497">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="90406-497">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="90406-498">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="90406-498">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="90406-499">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="90406-499">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="90406-500">Beispiel in „Remove-AzureRmSqlServerFirewallRule“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="90406-500">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="90406-501">Falsche Verarbeitung von „datetime“ für nicht US-basierte Kultur in „Get-AzureSqlSyncGroupLog“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="90406-501">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="90406-502">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="90406-502">AzureRM.Storage</span></span>
* <span data-ttu-id="90406-503">„Ps1XmlAttribute“ zu Typeneigenschaften von Cmdlet-Ausgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-503">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="90406-504">Cmdlet-Ausgabe von „StorageAccount“ in Tabellenansicht anzeigen</span><span class="sxs-lookup"><span data-stu-id="90406-504">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="90406-505">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="90406-505">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="90406-506">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="90406-506">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="90406-507">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="90406-507">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="90406-508">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="90406-508">AzureRM.Tags</span></span>
* <span data-ttu-id="90406-509">Falsche Anweisung aus Tag-Cmdlet-Hilfe entfernt</span><span class="sxs-lookup"><span data-stu-id="90406-509">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="90406-510">6.5.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="90406-510">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="90406-511">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="90406-511">AzureRM.Profile</span></span>
* <span data-ttu-id="90406-512">Hilfe für „Get-AzureRmContextAutosaveSetting“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-512">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="90406-513">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="90406-513">Azure.Storage</span></span>
* <span data-ttu-id="90406-514">Unterstützung des Blob- oder Dateiuploads mit lesegeschütztem SAS-Token</span><span class="sxs-lookup"><span data-stu-id="90406-514">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="90406-515">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="90406-515">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="90406-516">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="90406-516">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="90406-517">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="90406-517">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="90406-518">Erforderliche Eigenschaft „ResourceGroupName“ zu AS hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="90406-518">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="90406-519">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="90406-519">AzureRM.Automation</span></span>
* <span data-ttu-id="90406-520">Hilfe aktualisiert und Beispiel für „New-AzureRMAutomationSchedule“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-520">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="90406-521">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="90406-521">AzureRM.Compute</span></span>
* <span data-ttu-id="90406-522">Parameter „-Tag“ zu „Update/New-AzureRmAvailabilitySet“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-522">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="90406-523">Beispiel für „Add-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-523">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="90406-524">Beispiele für „Remove-AzureRmVmssExtension“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-524">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="90406-525">Hilfe für „Set-AzureRmVMAccessExtension“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-525">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="90406-526">„SimpleParameterSet“ für „New-AzureRmVmss“ so aktualisiert, dass „SinglePlacementGroup“ standardmäßig auf „false“ festgelegt ist, und Switch-Parameter „SinglePlacementGroup“ hinzugefügt, der dem Benutzer das Erstellen der VMSS in einer einzelnen Platzierungsgruppe ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="90406-526">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="90406-527">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="90406-527">AzureRM.EventHub</span></span>
* <span data-ttu-id="90406-528">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSEventHubDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="90406-528">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="90406-529">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="90406-529">AzureRM.KeyVault</span></span>
* <span data-ttu-id="90406-530">Fehlermeldung für „Set-AzureRmKeyVaultAccessPolicy“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-530">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="90406-531">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="90406-531">AzureRM.LogicApp</span></span>
* <span data-ttu-id="90406-532">Fehler „Parametersatz konnte nicht aufgelöst werden“ in „New-AzureRmLogicApp“behoben</span><span class="sxs-lookup"><span data-stu-id="90406-532">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="90406-533">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="90406-533">AzureRM.Network</span></span>
* <span data-ttu-id="90406-534">Peering über mehrere virtuelle Netzwerke in mehreren Mandanten für „Set/Add-AzureRmVirtualNetworkPeering“ aktiviert</span><span class="sxs-lookup"><span data-stu-id="90406-534">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="90406-535">Folgende Cmdlets für Application Gateway aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-535">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="90406-536">New-AzureRmApplicationGateway: EnableFIPS-Flag und Zonenunterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-536">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="90406-537">New-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-537">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="90406-538">Set-AzureRmApplicationGatewaySku: Neue SKUs „Standard_v2“ und „WAF_v2“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-538">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="90406-539">RouteTable-Cmdlets mit aktueller Generatorversion erneut generiert</span><span class="sxs-lookup"><span data-stu-id="90406-539">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="90406-540">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="90406-540">AzureRM.Relay</span></span>
* <span data-ttu-id="90406-541">Markdowndateien aktualisiert, Problem mit Parametername in Beispiel behoben</span><span class="sxs-lookup"><span data-stu-id="90406-541">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="90406-542">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="90406-542">AzureRM.Resources</span></span>
* <span data-ttu-id="90406-543">Roleassignment- und roledefinition-Cmdlets aktualisiert:</span><span class="sxs-lookup"><span data-stu-id="90406-543">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="90406-544">Zusätzliche roledefinition-Aufrufe entfernt, die als Teil des Pagings durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="90406-544">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="90406-545">Get-AzureRmRoleAssignment-Cmdlet korrigiert</span><span class="sxs-lookup"><span data-stu-id="90406-545">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="90406-546">Befehlsparameterfunktion von „-ExpandPrincipalGroups“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="90406-546">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="90406-547">Problem mit „Get-AzureRmResource“ behoben, aufgrund dessen die Groß-/Kleinschreibung des Parameters „-ResourceType“ beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="90406-547">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="90406-548">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="90406-548">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="90406-549">top- und skip-Parameter zu Listen-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-549">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="90406-550">Cmdlets für die Migration von Standard- zu Premium-Namespace hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="90406-550">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="90406-551">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="90406-551">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="90406-552">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="90406-552">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="90406-553">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="90406-553">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="90406-554">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="90406-554">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="90406-555">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="90406-555">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="90406-556">Schreibgeschützte Eigenschaft „PendingReplicationOperationsCount“ zur Klasse „PSServiceBusDRConfigurationAttributes“ hinzugefügt, welche die Anzahl der ausstehenden Replikationsvorgänge während der Replikation angibt</span><span class="sxs-lookup"><span data-stu-id="90406-556">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="90406-557">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="90406-557">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="90406-558">Beispiel für „New-AzureRmServiceFabricCluster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-558">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="90406-559">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="90406-559">AzureRM.Sql</span></span>
* <span data-ttu-id="90406-560">Neue Cmdlets für „Management.Sql“ hinzugefügt, um Kunden das Hinzufügen des TDE-Zertifikats zu einer SQL Server-Instanz oder einer verwalteten Instanz zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="90406-560">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="90406-561">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="90406-561">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="90406-562">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="90406-562">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="90406-563">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="90406-563">AzureRM.Websites</span></span>
* <span data-ttu-id="90406-564">Wenn `Set-AzureRmWebApp -AssignIdentity` und `Set-AzureRmWebAppSlot -AssignIdentity` auf „false“ festgelegt sind, wird jetzt die Identity-Eigenschaft aus dem Websiteobjekt entfernt. Auch das Vorschau-Tag wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="90406-564">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="90406-565">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics`-Beispiel aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-565">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="90406-566">Unterstützung von `Set-AzureRmWebApp -PhpVersion` als gültige PHP-Version eingestellt</span><span class="sxs-lookup"><span data-stu-id="90406-566">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="90406-567">6.4.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="90406-567">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="90406-568">Allgemein</span><span class="sxs-lookup"><span data-stu-id="90406-568">General</span></span>
* <span data-ttu-id="90406-569">Formatierung von OutputType in Hilfedateien für die meisten Module korrigiert</span><span class="sxs-lookup"><span data-stu-id="90406-569">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="90406-570">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="90406-570">AzureRM.Profile</span></span>
* <span data-ttu-id="90406-571">Attribut „Ps1Xml“ wurde den Standardausgabetypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-571">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="90406-572">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="90406-572">AzureRM.Compute</span></span>
* <span data-ttu-id="90406-573">IP-Tag-Funktion für VMSS</span><span class="sxs-lookup"><span data-stu-id="90406-573">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="90406-574">Cmdlet „New-AzureRmVmssIpTagConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-574">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="90406-575">IpTag-Parameter zu „New-AzureRmVmssIpConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-575">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="90406-576">Funktion für automatisches Betriebssystemrollback für VMSS</span><span class="sxs-lookup"><span data-stu-id="90406-576">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="90406-577">DisableAutoRollback-Parameter zu „New-AzureRmVmssConfig“ und „Update-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-577">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="90406-578">Funktion für Upgradeverlauf des Betriebssystems für VMSS</span><span class="sxs-lookup"><span data-stu-id="90406-578">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="90406-579">Switch-Parameter „OSUpgradeHistory“ zu „Get-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-579">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="90406-580">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="90406-580">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="90406-581">Unterstützung für Katalog-ACLs über die folgenden Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="90406-581">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="90406-582">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="90406-582">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="90406-583">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="90406-583">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="90406-584">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="90406-584">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="90406-585">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="90406-585">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="90406-586">Abbruchunterstützung und Nachverfolgung des Fortschritts für „Set-AzureRmDataLakeStoreItemAclEntry“, „Remove-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-586">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="90406-587">Abbruchunterstützung „Export-AzureRmDataLakeStoreChildItemProperties“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-587">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="90406-588">Leerung von Debugmeldungen für Cmdlets korrigiert, die rekursive Vorgänge durchführt</span><span class="sxs-lookup"><span data-stu-id="90406-588">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="90406-589">Speicherort des Test von DataLake-Cmdlets korrigiert</span><span class="sxs-lookup"><span data-stu-id="90406-589">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="90406-590">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="90406-590">AzureRM.EventHub</span></span>
* <span data-ttu-id="90406-591">Optionaler Parameter „MaxCount“ zu Listenvorgangs-Cmdlets „Get-AzureRmEventHub“ und „Get-AzureRmEventHubConsumerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-591">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="90406-592">Problem in Cmdlet „New-AzureRmEventHub“ behoben, aufgrund dessen beim Erstellen einer neuen EventHub-Instanz mindestens ein Parameter benötigt wurde.</span><span class="sxs-lookup"><span data-stu-id="90406-592">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="90406-593">Standardparametersatz wurde bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="90406-593">Provided Default Parameter set.</span></span>
* <span data-ttu-id="90406-594">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmEventHubKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="90406-594">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="90406-595">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="90406-595">AzureRM.KeyVault</span></span>
* <span data-ttu-id="90406-596">Problem behoben, aufgrund dessen von „Get-AzureRmKeyVault -Tag“ alle Ressourcen zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="90406-596">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="90406-597">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="90406-597">AzureRM.Network</span></span>
* <span data-ttu-id="90406-598">Neue SKUs für zonenredundante VirtualNetworkGateways-Instanzen verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="90406-598">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="90406-599">Neue Befehle für Funktion hinzugefügt: ExpressRoute-Partner-APIs über ARM</span><span class="sxs-lookup"><span data-stu-id="90406-599">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="90406-600">Get-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-600">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="90406-601">Set-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-601">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="90406-602">Add-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-602">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="90406-603">Get-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-603">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="90406-604">Remove-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-604">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="90406-605">Get-AzureRMExpressRouteCrossConnectionArpTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-605">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="90406-606">Get-AzureRMExpressRouteCrossConnectionRouteTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-606">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="90406-607">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-607">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="90406-608">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="90406-608">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="90406-609">Cmdlet „Get-AzureRmRecoveryServicesBackupStatus“ wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="90406-609">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="90406-610">Dieses Cmdlet überprüft anhand der ID eines virtuellen Computers, ob dieser durch einen Tresor im Abonnement geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="90406-610">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="90406-611">Wenn ein solcher Tresor vorhanden ist, gibt das Cmdlet die Tresordetails aus.</span><span class="sxs-lookup"><span data-stu-id="90406-611">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="90406-612">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="90406-612">AzureRM.Resources</span></span>
* <span data-ttu-id="90406-613">Cmdlets vom Typ „Get-AzureRmPolicyAssignment“ aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="90406-613">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="90406-614">Unterstützung für das Auflisten von „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-614">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="90406-615">Unterstützung für das Abrufen einzelner Arbeitsaufträge mit „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-615">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="90406-616">Switches „-Effective“ und „-All“ zu Steuerparameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-616">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="90406-617">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicyDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-617">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="90406-618">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="90406-618">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="90406-619">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="90406-619">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="90406-620">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicySetDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-620">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="90406-621">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="90406-621">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="90406-622">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="90406-622">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="90406-623">Unterstützung für KeyVault-Geheimnisverweis in Parametern hinzugefügt, wenn „TemplateParameterObject“ in „New-AzureRmResourceGroupDeployment“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="90406-623">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="90406-624">Problem behoben, aufgrund dessen, der Parameter „-EndDate“ für „New-AzureRmADAppCredential“ ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="90406-624">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="90406-625">Problem behoben, aufgrund dessen „Add-AzureRmADGroupMember“ eine falsche URL für Anforderungen verwendete</span><span class="sxs-lookup"><span data-stu-id="90406-625">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="90406-626">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="90406-626">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="90406-627">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmServiceBusKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="90406-627">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="90406-628">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="90406-628">AzureRM.Sql</span></span>
* <span data-ttu-id="90406-629">Benutzerdefinierte Wiederherstellungspunkte für SQLDW in Hilfe zu „New-AzureRmSqlDatabaseRestorePoint“ erläutert</span><span class="sxs-lookup"><span data-stu-id="90406-629">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="90406-630">Dokumentation von Parameter „-ComputeGeneration“ in mehreren Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-630">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="90406-631">6.3.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="90406-631">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="90406-632">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="90406-632">AzureRM.Profile</span></span>
* <span data-ttu-id="90406-633">Aktualisierte Fehlermeldungen für „Enable-AzureRmContextAutoSave“</span><span class="sxs-lookup"><span data-stu-id="90406-633">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="90406-634">Erstellen eines Kontexts für jedes Abonnement beim Ausführen von „Connect-AzureRmAccount“ ohne vorherigen Kontext</span><span class="sxs-lookup"><span data-stu-id="90406-634">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="90406-635">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="90406-635">Azure.Storage</span></span>
* <span data-ttu-id="90406-636">Zusätzliche Informationen zum Parameter „-Permissions“ in Hilfedateien</span><span class="sxs-lookup"><span data-stu-id="90406-636">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="90406-637">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="90406-637">AzureRM.Compute</span></span>
* <span data-ttu-id="90406-638">„Get-AzureRmVmDiskEncryptionStatus“ behebt ein Problem, das bei virtuellen Computern ohne Datenträger festgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="90406-638">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="90406-639">Version der Computeclientbibliothek aktualisiert, um folgende Cmdlets zu korrigieren:</span><span class="sxs-lookup"><span data-stu-id="90406-639">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="90406-640">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="90406-640">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="90406-641">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="90406-641">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="90406-642">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="90406-642">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="90406-643">Die folgenden Cmdlets wurden korrigiert, um die Vorgangs-ID und den Vorgangsstatus korrekt anzuzeigen:</span><span class="sxs-lookup"><span data-stu-id="90406-643">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="90406-644">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="90406-644">Start-AzureRmVM</span></span>
    - <span data-ttu-id="90406-645">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="90406-645">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="90406-646">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="90406-646">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="90406-647">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="90406-647">Set-AzureRmVM</span></span>
    - <span data-ttu-id="90406-648">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="90406-648">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="90406-649">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="90406-649">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="90406-650">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="90406-650">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="90406-651">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="90406-651">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="90406-652">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="90406-652">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="90406-653">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="90406-653">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="90406-654">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="90406-654">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="90406-655">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="90406-655">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="90406-656">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="90406-656">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="90406-657">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="90406-657">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="90406-658">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="90406-658">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="90406-659">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="90406-659">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="90406-660">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="90406-660">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="90406-661">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="90406-661">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="90406-662">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="90406-662">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="90406-663">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="90406-663">AzureRM.EventGrid</span></span>
* <span data-ttu-id="90406-664">ValidateNotNullOrEmpty-Überprüfungskonditionen für „SubjectBeginsWith“/„SubjectEndsWith“ im Cmdlet „Update-AzureRmEventGridSubscription“ wurden entfernt, um bei Bedarf die Änderung dieser Parameter in eine leere Zeichenfolge zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="90406-664">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="90406-665">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="90406-665">AzureRM.KeyVault</span></span>
* <span data-ttu-id="90406-666">Ein Problem wurde behoben, aufgrund dessen bei Ausführung von „Get-AzureRmKeyVault -Tag“ keine Tags zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="90406-666">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="90406-667">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="90406-667">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="90406-668">Offizielle Veröffentlichung von Policy Insights-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="90406-668">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="90406-669">Verwendung der API-Version 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="90406-669">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="90406-670">„PolicyDefinitionReferenceId“ zu den Ergebnissen von „Get-AzureRmPolicyStateSummary“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-670">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="90406-671">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="90406-671">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="90406-672">Parameter „-Vault“ zu den RecoveryServices.Backup-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="90406-672">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="90406-673">Bei der Übergabe wird dadurch das Cmdlet „Set-AzureRmRecoveryServicesContext“ außer Kraft gesetzt.</span><span class="sxs-lookup"><span data-stu-id="90406-673">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="90406-674">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="90406-674">AzureRM.Sql</span></span>
* <span data-ttu-id="90406-675">Aktualisiertes Beispiel in der Hilfedatei für „Get-AzureRmSqlDatabaseExpanded“</span><span class="sxs-lookup"><span data-stu-id="90406-675">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="90406-676">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="90406-676">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="90406-677">Hilfedatei für „Add-AzureRmTrafficManagerEndpointConfig“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="90406-677">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="90406-678">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="90406-678">AzureRM.Websites</span></span>
* <span data-ttu-id="90406-679">„Set-AzureRmWebApp“ wurde aktualisiert, damit „AppSettings“ bei der Verwendung von „-AssignIdentity“ nicht außer Kraft gesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="90406-679">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="90406-680">„New-AzureRmWebAppSlot“ wurde aktualisiert, um „AppServicePlan“ als optionalen Parameter anzuerkennen</span><span class="sxs-lookup"><span data-stu-id="90406-680">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="90406-681">6.2.1: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="90406-681">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="90406-682">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="90406-682">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="90406-683">PSWorkspace-Modell aktualisiert, damit das Netzwerk „type“ als Parameter verwenden kann</span><span class="sxs-lookup"><span data-stu-id="90406-683">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="90406-684">6.2.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="90406-684">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="90406-685">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="90406-685">AzureRM.Profile</span></span>
* <span data-ttu-id="90406-686">Beheben des Problems, aufgrund dessen Version 10.0.3 von Newtonsoft.Json beim Modulimport nicht geladen wurde</span><span class="sxs-lookup"><span data-stu-id="90406-686">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="90406-687">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="90406-687">AzureRM.Compute</span></span>
* <span data-ttu-id="90406-688">Feature zum Aktualisieren von virtuellen VMSS-Computern</span><span class="sxs-lookup"><span data-stu-id="90406-688">VMSS VM Update feature</span></span>
    - <span data-ttu-id="90406-689">Cmdlets „Update-AzureRmVmssVM“ und „New-AzureRmVMDataDisk“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-689">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="90406-690">Fügen Sie den Parameter „VirtualMachineScaleSetVM“ zum Cmdlet „Add-AzureRmVMDataDisk“ hinzu, um das Hinzufügen eines Datenträgers zum virtuellen VMSS-Computer zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="90406-690">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="90406-691">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="90406-691">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="90406-692">Aktualisierung der ADF .Net SDK-Version auf 0.8.0-preview mit den folgenden Änderungen:</span><span class="sxs-lookup"><span data-stu-id="90406-692">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="90406-693">Vorgang zum Konfigurieren des Factoryrepositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-693">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="90406-694">Der verknüpfte QuickBooks-Dienst wurde aktualisiert, um die Eigenschaften „consumerKey“ und „consumerSecret“ verfügbar zu machen.</span><span class="sxs-lookup"><span data-stu-id="90406-694">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="90406-695">Aktualisierung verschiedener Modelltypen von „SecretBase“ auf „Object“</span><span class="sxs-lookup"><span data-stu-id="90406-695">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="90406-696">Blobereignisauslöser hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-696">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="90406-697">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="90406-697">AzureRM.KeyVault</span></span>
* <span data-ttu-id="90406-698">Aktualisierung der Dokumentation mit Beispielausgabe</span><span class="sxs-lookup"><span data-stu-id="90406-698">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="90406-699">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="90406-699">AzureRM.Network</span></span>
* <span data-ttu-id="90406-700">Aktivierung der Traffic Analytics-Parameter für Network Watcher-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="90406-700">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="90406-701">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="90406-701">AzureRM.Resources</span></span>
* <span data-ttu-id="90406-702">Behebung des Problems mit der Eigenschaft „Properties“ von PSResource-Objekten, die von „Get-AzureRmResource“ zurückgegeben wurden</span><span class="sxs-lookup"><span data-stu-id="90406-702">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="90406-703">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="90406-703">AzureRM.Scheduler</span></span>
* <span data-ttu-id="90406-704">Behebung des Problems, dass beim Aktualisieren von „ServiceBusQueueJob“ keine neuen Authentifizierungswerte festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="90406-704">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="90406-705">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="90406-705">AzureRM.Sql</span></span>
* <span data-ttu-id="90406-706">Aktualisierung der folgenden Cmdlets mit dem optionalen LicenseType-Parameter</span><span class="sxs-lookup"><span data-stu-id="90406-706">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="90406-707">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="90406-707">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="90406-708">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="90406-708">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="90406-709">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="90406-709">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="90406-710">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="90406-710">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="90406-711">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="90406-711">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="90406-712">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="90406-712">AzureRM.Websites</span></span>
* <span data-ttu-id="90406-713">„New-AzureRMWebApp“ aktualisiert, um allgemeine Algorithmen aus der Strategiebibliothek zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="90406-713">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="90406-714">6.1.0 – Mai 2018</span><span class="sxs-lookup"><span data-stu-id="90406-714">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="90406-715">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="90406-715">AzureRM.Profile</span></span>
* <span data-ttu-id="90406-716">Behebung eines Problems, durch das beim Ausführen von „Clear-AzureRmContext“ ein leerer Kontext mit dem Namen des vorherigen Standardkontexts beibehalten wurde und der Benutzer dadurch keinen neuen Kontext mit dem alten Namen erstellen konnte</span><span class="sxs-lookup"><span data-stu-id="90406-716">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="90406-717">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="90406-717">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="90406-718">Ermöglichung der Zuordnung von Gateways/Aufhebung der Gatewayzuordnung in AS</span><span class="sxs-lookup"><span data-stu-id="90406-718">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="90406-719">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="90406-719">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="90406-720">Unterstützung für „ApiVersions“, „ApiReleases“ und „ApiRevisions“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-720">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="90406-721">Unterstützung für ServiceFabric-Back-End hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-721">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="90406-722">Unterstützung für Application Insights-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-722">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="90406-723">Unterstützung für die Erkennung von SKUs vom Typ „Basic“ als gültige SKU des API Management-Diensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-723">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="90406-724">Unterstützung hinzugefügt, damit Zertifikate, die von der privaten Zertifizierungsstelle ausgestellt wurden, als Stamm- oder ZS-Zertifikate installiert werden können</span><span class="sxs-lookup"><span data-stu-id="90406-724">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="90406-725">Unterstützung für die Akzeptierung benutzerdefinierter SSL-Zertifikate über KeyVault und mehrere Proxyhostnamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-725">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="90406-726">Unterstützung für die verwaltete Dienstidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-726">Added support for MSI identity</span></span>
* <span data-ttu-id="90406-727">Unterstützung für die Annahme von Richtlinien über URL hinzugefügt; HINWEIS: Folgende Cmdlets werden in einem zukünftigen Release als veraltet gekennzeichnet:</span><span class="sxs-lookup"><span data-stu-id="90406-727">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="90406-728">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="90406-728">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="90406-729">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="90406-729">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="90406-730">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="90406-730">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="90406-731">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="90406-731">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="90406-732">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="90406-732">AzureRM.Batch</span></span>
* <span data-ttu-id="90406-733">Veröffentlichung des neuen Cmdlets „Get-AzureBatchPoolNodeCounts“</span><span class="sxs-lookup"><span data-stu-id="90406-733">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="90406-734">Veröffentlichung des neuen Cmdlets „Start-AzureBatchComputeNodeServiceLogUpload“</span><span class="sxs-lookup"><span data-stu-id="90406-734">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="90406-735">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="90406-735">AzureRM.Consumption</span></span>
* <span data-ttu-id="90406-736">Hinzufügung neuer Parameter („Expand“, „ResourceGroup“, „InstanceName“, „InstanceId“, „Tags“ und „Top“) für das Cmdlet „Get-AzureRmConsumptionUsageDetail“</span><span class="sxs-lookup"><span data-stu-id="90406-736">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="90406-737">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="90406-737">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="90406-738">Korrektur des Beispiels für „Export AzureRmDataLakeStoreChildItemProperties“</span><span class="sxs-lookup"><span data-stu-id="90406-738">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="90406-739">Korrektur der NULL-Parameterausnahme für rekursiven Fall in „Set-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="90406-739">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="90406-740">Korrektur der Hilfedateien für „Set-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ und „Remove-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="90406-740">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="90406-741">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="90406-741">AzureRM.Network</span></span>
* <span data-ttu-id="90406-742">Erhöhung der Network SDK-Version von 18.0.0-preview auf 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="90406-742">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="90406-743">Cmdlet zum Erstellen der Protokollkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-743">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="90406-744">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="90406-744">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="90406-745">Cmdlet zum Hinzufügen einer neuen Leitungsverbindung zu einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-745">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="90406-746">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="90406-746">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="90406-747">Cmdlet zum Entfernen einer Leitungsverbindung aus einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-747">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="90406-748">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="90406-748">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="90406-749">Cmdlet zum Abrufen einer Leitungsverbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="90406-749">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="90406-750">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="90406-750">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="90406-751">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="90406-751">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="90406-752">Verwendung der Serverauthentifizierung mit generierten Zertifikaten korrigiert (Problemnr. 5998)</span><span class="sxs-lookup"><span data-stu-id="90406-752">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="90406-753">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="90406-753">AzureRM.Sql</span></span>
* <span data-ttu-id="90406-754">Überwachungscmdlets korrigiert, um das Entfernen von „AuditActions“ oder „AuditActionGroups“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="90406-754">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="90406-755">Problem mit „Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy“ behoben, das beim Festlegen einer neuen flexiblen Aufbewahrungsrichtlinie zu folgendem Fehler führte: „Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span><span class="sxs-lookup"><span data-stu-id="90406-755">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="90406-756">Please submit request with the new flexible retention policy“ (Das Konfigurieren einer langfristigen Aufbewahrungsrichtlinie mit Azure Recovery Service-Tresor und -Richtlinie wird nicht mehr unterstützt. Übermitteln Sie eine Anforderung mit der neuen flexiblen Aufbewahrungsrichtlinie.)</span><span class="sxs-lookup"><span data-stu-id="90406-756">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="90406-757">Aktualisierung aller Cmdlets für Azure SQL-Datenbank, für die Erstellung von Pools für elastische Datenbanken und für die Aktualisierung, sodass sie die neue Datenbank-API verwenden. Diese unterstützt die Sku-Eigenschaft für skalierungs- und tarifbezogene Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="90406-757">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="90406-758">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="90406-758">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="90406-759">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="90406-759">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="90406-760">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="90406-760">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="90406-761">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="90406-761">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="90406-762">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="90406-762">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="90406-763">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="90406-763">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="90406-764">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="90406-764">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="90406-765">Aktualisierung der Parameter für „Get-AzureRmTrafficManagerProfile“, sodass bei Verwendung des Parameters „-Name“ der Parameter „-ResourceGroupName“ erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="90406-765">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
