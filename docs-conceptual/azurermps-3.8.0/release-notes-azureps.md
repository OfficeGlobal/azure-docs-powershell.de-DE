---
title: Azure PowerShell-Änderungsprotokoll | Microsoft-Dokumentation
description: Hierbei handelt es sich um einen Verlauf der Änderungen, die in der neuesten Version an Azure PowerShell vorgenommen wurden.
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: 04f89e8d47d0825d46cb1b8817efbcc0cafa0acd
ms.sourcegitcommit: 37bfbf11fd0967a8e7977c692ab829d286baf88a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/08/2018
---
# <a name="release-notes"></a><span data-ttu-id="b2bb4-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="b2bb4-103">Release notes</span></span>

<span data-ttu-id="b2bb4-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-380"></a><span data-ttu-id="b2bb4-105">Version 3.8.0</span><span class="sxs-lookup"><span data-stu-id="b2bb4-105">Version 3.8.0</span></span>
* <span data-ttu-id="b2bb4-106">Compute</span><span class="sxs-lookup"><span data-stu-id="b2bb4-106">Compute</span></span>
  - <span data-ttu-id="b2bb4-107">Korrektur eines Fehlers in Get-\*-Cmdlets, um das Abrufen mehrerer Seiten mit Daten (mehr als 120 Elemente) zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b2bb4-107">Fix bug in Get-\* cmdlets, to allow retrieving multiple pages of data (more than 120 items)</span></span>
* <span data-ttu-id="b2bb4-108">DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="b2bb4-108">DataLakeAnalytics</span></span>
  - <span data-ttu-id="b2bb4-109">Korrektur der Hilfe für einige Befehle, sodass sie die richtige Sprache und die richtigen Beispiele enthalten.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-109">Fix help for some commands to have the proper verbage and examples.</span></span>
* <span data-ttu-id="b2bb4-110">DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="b2bb4-110">DataLakeStore</span></span>
  - <span data-ttu-id="b2bb4-111">Zum `Get-AzureRMDataLakeStoreItemContent`-Cmdlet wurde Unterstützung für den Anfangs- und Endbereich hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-111">Add support for head and tail to the `Get-AzureRMDataLakeStoreItemContent` cmdlet.</span></span> <span data-ttu-id="b2bb4-112">Dies ermöglicht die Rückgabe der ersten n oder letzten n durch Zeilenumbrüche getrennten Zeilen für die Anzeige.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-112">This enables returning the top N or last N new line delimited rows to be displayed.</span></span>
* <span data-ttu-id="b2bb4-113">HDInsight</span><span class="sxs-lookup"><span data-stu-id="b2bb4-113">HDInsight</span></span>
  - <span data-ttu-id="b2bb4-114">Unterstützung für den RServer-Clustertyp wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-114">Added support for RServer cluster type</span></span>
    + <span data-ttu-id="b2bb4-115">Die Größe virtueller Edgeknotencomputer kann für RServer-Cluster in „New-AzureRmHDInsightCluster“ oder „New-AzureRmHDInsightClusterConfig“ angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-115">Edgenode VM size can be specified for RServer cluster in New-AzureRmHDInsightCluster or New-AzureRmHDInsightClusterConfig</span></span>
    + <span data-ttu-id="b2bb4-116">„RServer“ ist jetzt eine Konfigurationsoption in „Add-AzureRmHDInsightConfigValues“.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-116">RServer is now a configuration option in Add-AzureRmHDInsightConfigValues.</span></span> <span data-ttu-id="b2bb4-117">Sie ermöglicht das Festlegen des RStudio-Flags, um anzugeben, dass die R Studio-Installation ausgeführt werden sollte.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-117">It allows for RStudio flag to be set to indicate that R Studio installation should be done.</span></span>
* <span data-ttu-id="b2bb4-118">LogicApp</span><span class="sxs-lookup"><span data-stu-id="b2bb4-118">LogicApp</span></span>
  - <span data-ttu-id="b2bb4-119">Die Cmdlets „Set-AzureRmIntegrationAccountSchema“ und „Set-AzureRmIntegrationAccountMap“ wurden zur Behebung des contentlink-Problems korrigiert. („content“ und „contentlink“ führten zu einem Updatefehler.)</span><span class="sxs-lookup"><span data-stu-id="b2bb4-119">Set-AzureRmIntegrationAccountSchema and Set-AzureRmIntegrationAccountMap cmdlets are fixed for the contentlink issue(Both content and contentlink were set resulting in update failure).</span></span>
* <span data-ttu-id="b2bb4-120">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b2bb4-120">Network</span></span>
  - <span data-ttu-id="b2bb4-121">Anwendungsgateways wurde Unterstützung für neue Web Application Firewall-Features hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-121">Added support for new web application firewall features to Application Gateways</span></span>
    + <span data-ttu-id="b2bb4-122">„New-AzureRmApplicationGatewayFirewallDisabledRuleGroupConfig“ wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-122">Added New-AzureRmApplicationGatewayFirewallDisabledRuleGroupConfig</span></span>
    + <span data-ttu-id="b2bb4-123">„Get-AzureRmApplicationGatewayAvailableWafRuleSets“ wurde hinzugefügt (Alias: List-AzureRmApplicationGatewayAvailableWafRuleSets).</span><span class="sxs-lookup"><span data-stu-id="b2bb4-123">Added Get-AzureRmApplicationGatewayAvailableWafRuleSets (Alias: List-AzureRmApplicationGatewayAvailableWafRuleSets)</span></span>
    + <span data-ttu-id="b2bb4-124">„New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration“ wurde aktualisiert: Die Parameter „-RuleSetType -RuleSetVersion“ und „-DisabledRuleGroups“ wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-124">Updated New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration: Added parameter -RuleSetType -RuleSetVersion and -DisabledRuleGroups</span></span>
    + <span data-ttu-id="b2bb4-125">„Set-AzureRmApplicationGatewayWebApplicationFirewallConfiguration“ wurde aktualisiert: Die Parameter „-RuleSetType -RuleSetVersion“ und „-DisabledRuleGroups“ wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-125">Updated Set-AzureRmApplicationGatewayWebApplicationFirewallConfiguration: Added parameter -RuleSetType -RuleSetVersion and -DisabledRuleGroups</span></span>
  - <span data-ttu-id="b2bb4-126">Für Verbindungen für das virtuelle Netzwerkgateway wurde Unterstützung für IPSec-Richtlinien hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-126">Added support for IPSec policies to Virtual Network Gateway Connections</span></span>
  - <span data-ttu-id="b2bb4-127">„New-AzureRmIpsecPolicy“ wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-127">Added New-AzureRmIpsecPolicy</span></span>
  - <span data-ttu-id="b2bb4-128">„New-AzureRmVirtualNetworkGatewayConnection“ wurde aktualisiert: Die Parameter „-IpsecPolicies“ und „-UsePolicyBasedTrafficSelectors“ wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-128">Updated New-AzureRmVirtualNetworkGatewayConnection: Added parameter -IpsecPolicies and -UsePolicyBasedTrafficSelectors</span></span>
* <span data-ttu-id="b2bb4-129">Profil</span><span class="sxs-lookup"><span data-stu-id="b2bb4-129">Profile</span></span>
  - <span data-ttu-id="b2bb4-130">*Veraltet*: „Save-AzureRmProfile“ wurde in „Save-AzureRmContext“ umbenannt. Es gibt einen Alias für den alten Cmdlet-Namen. Der Alias wird in der nächsten Version entfernt.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-130">*Obsolete*: Save-AzureRmProfile is renamed to Save-AzureRmContext, there is an alias to the old cmdlet name, the alias will be removed in the next release.</span></span>
  - <span data-ttu-id="b2bb4-131">*Veraltet*: „Select-AzureRmProfile“ wurde in „Import-AzureRmContext“ umbenannt. Es gibt einen Alias für den alten Cmdlet-Namen. Der Alias wird in der nächsten Version entfernt.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-131">*Obsolete*: Select-AzureRmProfile is renamed to Import-AzureRmContext, there is an alias to the old cmdlet name, the alias will be removed in the next release.</span></span>
  - <span data-ttu-id="b2bb4-132">Die Ausgabetypen „PSAzureContext“ und „PSAzureProfile“ der Profil-Cmdlets werden in der nächsten Version geändert.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-132">The PSAzureContext and PSAzureProfile output types of profile cmdlets will be changed in the next release.</span></span>
  - <span data-ttu-id="b2bb4-133">Das Cmdlet „Save-AzureRmContext“ enthält in der nächsten Version kein OutputType-Element.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-133">The Save-AzureRmContext cmdlet will have no OutputType in the next release.</span></span>
  - <span data-ttu-id="b2bb4-134">Fehlerbehebung im allgemeinen Cmdlet-Code in Bezug auf die Verwendung eines FIPS-konformen Algorithmus für Datenhashes: https://github.com/Azure/azure-powershell/issues/3651</span><span class="sxs-lookup"><span data-stu-id="b2bb4-134">Fix bug in cmdlet common code to use FIPS-compliant algorithm for data hashes: https://github.com/Azure/azure-powershell/issues/3651</span></span>
* <span data-ttu-id="b2bb4-135">Sql</span><span class="sxs-lookup"><span data-stu-id="b2bb4-135">Sql</span></span>
  - <span data-ttu-id="b2bb4-136">Fehlerbehebungen für Azure-Failovergruppen-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="b2bb4-136">Bug fixes on Azure Failover Group Cmdlets</span></span>
  - <span data-ttu-id="b2bb4-137">Korrektur für den Vorgangsabruf</span><span class="sxs-lookup"><span data-stu-id="b2bb4-137">Fix for operation polling</span></span>
  - <span data-ttu-id="b2bb4-138">Korrektur des GracePeriodWithDataLossHour-Werts, wenn für „FailoverPolicy“ die Option „Manuell“ festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="b2bb4-138">Fix GracePeriodWithDataLossHour value when setting FailoverPolicy to Manual</span></span>
* <span data-ttu-id="b2bb4-139">Traffic Manager</span><span class="sxs-lookup"><span data-stu-id="b2bb4-139">TrafficManager</span></span>
  - <span data-ttu-id="b2bb4-140">Unterstützung für die geografische Methode für das Datenverkehrsrouting</span><span class="sxs-lookup"><span data-stu-id="b2bb4-140">Support for the Geographic traffic routing method</span></span>
    + <span data-ttu-id="b2bb4-141">Neuer Wert „Geographic“ für den TrafficRoutingMethod-Parameter von „New-AzureRmTrafficManagerProfile“</span><span class="sxs-lookup"><span data-stu-id="b2bb4-141">New value 'Geographic' for the TrafficRoutingMethod parameter of New-AzureRmTrafficManagerProfile</span></span>
    + <span data-ttu-id="b2bb4-142">Neuer Parameter „GeoMapping“ für „New-AzureRmTrafficManagerEndpoint“ und „Add-AzureRmTrafficManagerEndpointConfig“</span><span class="sxs-lookup"><span data-stu-id="b2bb4-142">New parameter 'GeoMapping' for the New-AzureRmTrafficManagerEndpoint and Add-AzureRmTrafficManagerEndpointConfig</span></span>
    + <span data-ttu-id="b2bb4-143">Behebung eines Fehlers beim Übergeben für „Get-AzureRmTrafficManagerProfile“, wenn eine Sammlung mit Profilen zurückgegeben wird</span><span class="sxs-lookup"><span data-stu-id="b2bb4-143">Fix piping for Get-AzureRmTrafficManagerProfile when it returns a collection of profiles</span></span>
* <span data-ttu-id="b2bb4-144">ServiceManagement</span><span class="sxs-lookup"><span data-stu-id="b2bb4-144">ServiceManagement</span></span>
  - <span data-ttu-id="b2bb4-145">Restart-AzureVM: Der InitiateMaintenance-Parameter für die Ausführung einer Wartung während des VM-Neustarts wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-145">Restart-AzureVM: Added InitiateMaintenance parameter for performing maintenance during VM restart.</span></span>
  - <span data-ttu-id="b2bb4-146">Get-AzureVM: Das Feld für den Wartungsstatus wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-146">Get-AzureVM: Added Maintenance Status field.</span></span>
  - <span data-ttu-id="b2bb4-147">Neue Cmdlets zur Unterstützung des Recovery Services-Tresorupgrades wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b2bb4-147">Added new cmdlets to support Recovery Services vault upgrade</span></span>
    + <span data-ttu-id="b2bb4-148">Test-AzureRecoveryServicesVaultUpgrade</span><span class="sxs-lookup"><span data-stu-id="b2bb4-148">Test-AzureRecoveryServicesVaultUpgrade</span></span>
    + <span data-ttu-id="b2bb4-149">Invoke-AzureRecoveryServicesVaultUpgrade</span><span class="sxs-lookup"><span data-stu-id="b2bb4-149">Invoke-AzureRecoveryServicesVaultUpgrade</span></span>
