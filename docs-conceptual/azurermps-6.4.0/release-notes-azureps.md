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
ms.openlocfilehash: 255e26aea5ea3cea866faa0d095cdf643c8ef0a8
ms.sourcegitcommit: de0e60800df1add9f3400166faacca202ef567d9
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/03/2018
ms.locfileid: "37406293"
---
# <a name="release-notes"></a><span data-ttu-id="f2a32-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="f2a32-103">Release notes</span></span>

<span data-ttu-id="f2a32-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="f2a32-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="640---july-2018"></a><span data-ttu-id="f2a32-105">6.4.0 – Juli 2018</span><span class="sxs-lookup"><span data-stu-id="f2a32-105">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="f2a32-106">Allgemein</span><span class="sxs-lookup"><span data-stu-id="f2a32-106">General</span></span>
* <span data-ttu-id="f2a32-107">Formatierung von OutputType in Hilfedateien für die meisten Module korrigiert</span><span class="sxs-lookup"><span data-stu-id="f2a32-107">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="f2a32-108">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="f2a32-108">AzureRM.Profile</span></span>
* <span data-ttu-id="f2a32-109">Attribut „Ps1Xml“ wurde den Standardausgabetypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-109">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="f2a32-110">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="f2a32-110">AzureRM.Compute</span></span>
* <span data-ttu-id="f2a32-111">IP-Tag-Funktion für VMSS</span><span class="sxs-lookup"><span data-stu-id="f2a32-111">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="f2a32-112">Cmdlet „New-AzureRmVmssIpTagConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-112">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="f2a32-113">IpTag-Parameter zu „New-AzureRmVmssIpConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-113">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="f2a32-114">Funktion für automatisches Betriebssystemrollback für VMSS</span><span class="sxs-lookup"><span data-stu-id="f2a32-114">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="f2a32-115">DisableAutoRollback-Parameter zu „New-AzureRmVmssConfig“ und „Update-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-115">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="f2a32-116">Funktion für Upgradeverlauf des Betriebssystems für VMSS</span><span class="sxs-lookup"><span data-stu-id="f2a32-116">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="f2a32-117">Switch-Parameter „OSUpgradeHistory“ zu „Get-AzureRmVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-117">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="f2a32-118">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="f2a32-118">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="f2a32-119">Unterstützung für Katalog-ACLs über die folgenden Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f2a32-119">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="f2a32-120">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="f2a32-120">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="f2a32-121">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="f2a32-121">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="f2a32-122">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="f2a32-122">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="f2a32-123">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f2a32-123">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="f2a32-124">Abbruchunterstützung und Nachverfolgung des Fortschritts für „Set-AzureRmDataLakeStoreItemAclEntry“, „Remove-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-124">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="f2a32-125">Abbruchunterstützung „Export-AzureRmDataLakeStoreChildItemProperties“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-125">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="f2a32-126">Leerung von Debugmeldungen für Cmdlets korrigiert, die rekursive Vorgänge durchführt</span><span class="sxs-lookup"><span data-stu-id="f2a32-126">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="f2a32-127">Speicherort des Test von DataLake-Cmdlets korrigiert</span><span class="sxs-lookup"><span data-stu-id="f2a32-127">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="f2a32-128">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="f2a32-128">AzureRM.EventHub</span></span>
* <span data-ttu-id="f2a32-129">Optionaler Parameter „MaxCount“ zu Listenvorgangs-Cmdlets „Get-AzureRmEventHub“ und „Get-AzureRmEventHubConsumerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-129">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="f2a32-130">Problem in Cmdlet „New-AzureRmEventHub“ behoben, aufgrund dessen beim Erstellen einer neuen EventHub-Instanz mindestens ein Parameter benötigt wurde.</span><span class="sxs-lookup"><span data-stu-id="f2a32-130">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="f2a32-131">Standardparametersatz wurde bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="f2a32-131">Provided Default Parameter set.</span></span>
* <span data-ttu-id="f2a32-132">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmEventHubKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="f2a32-132">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="f2a32-133">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="f2a32-133">AzureRM.KeyVault</span></span>
* <span data-ttu-id="f2a32-134">Problem behoben, aufgrund dessen von „Get-AzureRmKeyVault -Tag“ alle Ressourcen zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="f2a32-134">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="f2a32-135">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="f2a32-135">AzureRM.Network</span></span>
* <span data-ttu-id="f2a32-136">Neue SKUs für zonenredundante VirtualNetworkGateways-Instanzen verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f2a32-136">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="f2a32-137">Neue Befehle für Funktion hinzugefügt: ExpressRoute-Partner-APIs über ARM</span><span class="sxs-lookup"><span data-stu-id="f2a32-137">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="f2a32-138">Get-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-138">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="f2a32-139">Set-AzureRmExpressRouteCrossConnection hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-139">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="f2a32-140">Add-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-140">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="f2a32-141">Get-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-141">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="f2a32-142">Remove-AzureRmExpressRouteCrossConnectionPeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-142">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="f2a32-143">Get-AzureRMExpressRouteCrossConnectionArpTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-143">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="f2a32-144">Get-AzureRMExpressRouteCrossConnectionRouteTable hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-144">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="f2a32-145">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-145">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="f2a32-146">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="f2a32-146">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="f2a32-147">Cmdlet „Get-AzureRmRecoveryServicesBackupStatus“ wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f2a32-147">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="f2a32-148">Dieses Cmdlet überprüft anhand der ID eines virtuellen Computers, ob dieser durch einen Tresor im Abonnement geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="f2a32-148">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="f2a32-149">Wenn ein solcher Tresor vorhanden ist, gibt das Cmdlet die Tresordetails aus.</span><span class="sxs-lookup"><span data-stu-id="f2a32-149">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="f2a32-150">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="f2a32-150">AzureRM.Resources</span></span>
* <span data-ttu-id="f2a32-151">Cmdlets vom Typ „Get-AzureRmPolicyAssignment“ aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="f2a32-151">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="f2a32-152">Unterstützung für das Auflisten von „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-152">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="f2a32-153">Unterstützung für das Abrufen einzelner Arbeitsaufträge mit „-Scope“-Werten auf Verwaltungsgruppenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-153">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="f2a32-154">Switches „-Effective“ und „-All“ zu Steuerparameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-154">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="f2a32-155">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicyDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f2a32-155">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="f2a32-156">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="f2a32-156">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="f2a32-157">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="f2a32-157">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="f2a32-158">Cmdlets vom Typ Get/New/Remove/Set-AzureRmPolicySetDefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f2a32-158">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="f2a32-159">Parameter „-ManagementGroupName“ hinzugefügt, um Vorgänge auf eine bestimmte Verwaltungsgruppe anzuwenden</span><span class="sxs-lookup"><span data-stu-id="f2a32-159">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="f2a32-160">Parameter „-SubscriptionId“ hinzugefügt, um Vorgänge auf ein bestimmtes Abonnement anzuwenden</span><span class="sxs-lookup"><span data-stu-id="f2a32-160">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="f2a32-161">Unterstützung für KeyVault-Geheimnisverweis in Parametern hinzugefügt, wenn „TemplateParameterObject“ in „New-AzureRmResourceGroupDeployment“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f2a32-161">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="f2a32-162">Problem behoben, aufgrund dessen, der Parameter „-EndDate“ für „New-AzureRmADAppCredential“ ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="f2a32-162">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="f2a32-163">Problem behoben, aufgrund dessen „Add-AzureRmADGroupMember“ eine falsche URL für Anforderungen verwendete</span><span class="sxs-lookup"><span data-stu-id="f2a32-163">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="f2a32-164">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f2a32-164">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="f2a32-165">Optionaler Parameter“ -KeyValue“ zu Cmdlet „New-AzureRmServiceBusKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="f2a32-165">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="f2a32-166">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="f2a32-166">AzureRM.Sql</span></span>
* <span data-ttu-id="f2a32-167">Benutzerdefinierte Wiederherstellungspunkte für SQLDW in Hilfe zu „New-AzureRmSqlDatabaseRestorePoint“ erläutert</span><span class="sxs-lookup"><span data-stu-id="f2a32-167">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="f2a32-168">Dokumentation von Parameter „-ComputeGeneration“ in mehreren Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f2a32-168">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="f2a32-169">6.3.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f2a32-169">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="f2a32-170">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="f2a32-170">AzureRM.Profile</span></span>
* <span data-ttu-id="f2a32-171">Aktualisierte Fehlermeldungen für „Enable-AzureRmContextAutoSave“</span><span class="sxs-lookup"><span data-stu-id="f2a32-171">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="f2a32-172">Erstellen eines Kontexts für jedes Abonnement beim Ausführen von „Connect-AzureRmAccount“ ohne vorherigen Kontext</span><span class="sxs-lookup"><span data-stu-id="f2a32-172">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="f2a32-173">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="f2a32-173">Azure.Storage</span></span>
* <span data-ttu-id="f2a32-174">Zusätzliche Informationen zum Parameter „-Permissions“ in Hilfedateien</span><span class="sxs-lookup"><span data-stu-id="f2a32-174">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="f2a32-175">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="f2a32-175">AzureRM.Compute</span></span>
* <span data-ttu-id="f2a32-176">„Get-AzureRmVmDiskEncryptionStatus“ behebt ein Problem, das bei virtuellen Computern ohne Datenträger festgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="f2a32-176">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="f2a32-177">Version der Computeclientbibliothek aktualisiert, um folgende Cmdlets zu korrigieren:</span><span class="sxs-lookup"><span data-stu-id="f2a32-177">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="f2a32-178">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="f2a32-178">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="f2a32-179">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="f2a32-179">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="f2a32-180">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="f2a32-180">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="f2a32-181">Die folgenden Cmdlets wurden korrigiert, um die Vorgangs-ID und den Vorgangsstatus korrekt anzuzeigen:</span><span class="sxs-lookup"><span data-stu-id="f2a32-181">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="f2a32-182">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="f2a32-182">Start-AzureRmVM</span></span>
    - <span data-ttu-id="f2a32-183">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="f2a32-183">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="f2a32-184">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="f2a32-184">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="f2a32-185">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="f2a32-185">Set-AzureRmVM</span></span>
    - <span data-ttu-id="f2a32-186">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="f2a32-186">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="f2a32-187">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="f2a32-187">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="f2a32-188">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="f2a32-188">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="f2a32-189">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="f2a32-189">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="f2a32-190">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="f2a32-190">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="f2a32-191">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="f2a32-191">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="f2a32-192">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="f2a32-192">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="f2a32-193">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="f2a32-193">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="f2a32-194">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="f2a32-194">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="f2a32-195">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="f2a32-195">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="f2a32-196">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="f2a32-196">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="f2a32-197">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="f2a32-197">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="f2a32-198">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="f2a32-198">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="f2a32-199">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="f2a32-199">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="f2a32-200">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="f2a32-200">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="f2a32-201">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="f2a32-201">AzureRM.EventGrid</span></span>
* <span data-ttu-id="f2a32-202">ValidateNotNullOrEmpty-Überprüfungskonditionen für „SubjectBeginsWith“/„SubjectEndsWith“ im Cmdlet „Update-AzureRmEventGridSubscription“ wurden entfernt, um bei Bedarf die Änderung dieser Parameter in eine leere Zeichenfolge zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f2a32-202">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="f2a32-203">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="f2a32-203">AzureRM.KeyVault</span></span>
* <span data-ttu-id="f2a32-204">Ein Problem wurde behoben, aufgrund dessen bei Ausführung von „Get-AzureRmKeyVault -Tag“ keine Tags zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="f2a32-204">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="f2a32-205">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="f2a32-205">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="f2a32-206">Offizielle Veröffentlichung von Policy Insights-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="f2a32-206">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="f2a32-207">Verwendung der API-Version 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="f2a32-207">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="f2a32-208">„PolicyDefinitionReferenceId“ zu den Ergebnissen von „Get-AzureRmPolicyStateSummary“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-208">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="f2a32-209">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="f2a32-209">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="f2a32-210">Parameter „-Vault“ zu den RecoveryServices.Backup-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f2a32-210">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="f2a32-211">Bei der Übergabe wird dadurch das Cmdlet „Set-AzureRmRecoveryServicesContext“ außer Kraft gesetzt.</span><span class="sxs-lookup"><span data-stu-id="f2a32-211">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="f2a32-212">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="f2a32-212">AzureRM.Sql</span></span>
* <span data-ttu-id="f2a32-213">Aktualisiertes Beispiel in der Hilfedatei für „Get-AzureRmSqlDatabaseExpanded“</span><span class="sxs-lookup"><span data-stu-id="f2a32-213">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="f2a32-214">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="f2a32-214">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="f2a32-215">Hilfedatei für „Add-AzureRmTrafficManagerEndpointConfig“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f2a32-215">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="f2a32-216">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="f2a32-216">AzureRM.Websites</span></span>
* <span data-ttu-id="f2a32-217">„Set-AzureRmWebApp“ wurde aktualisiert, damit „AppSettings“ bei der Verwendung von „-AssignIdentity“ nicht außer Kraft gesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="f2a32-217">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="f2a32-218">„New-AzureRmWebAppSlot“ wurde aktualisiert, um „AppServicePlan“ als optionalen Parameter anzuerkennen</span><span class="sxs-lookup"><span data-stu-id="f2a32-218">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="f2a32-219">6.2.1: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f2a32-219">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="f2a32-220">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="f2a32-220">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="f2a32-221">PSWorkspace-Modell aktualisiert, damit das Netzwerk „type“ als Parameter verwenden kann</span><span class="sxs-lookup"><span data-stu-id="f2a32-221">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="f2a32-222">6.2.0: Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f2a32-222">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="f2a32-223">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="f2a32-223">AzureRM.Profile</span></span>
* <span data-ttu-id="f2a32-224">Beheben des Problems, aufgrund dessen Version 10.0.3 von Newtonsoft.Json beim Modulimport nicht geladen wurde</span><span class="sxs-lookup"><span data-stu-id="f2a32-224">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="f2a32-225">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="f2a32-225">AzureRM.Compute</span></span>
* <span data-ttu-id="f2a32-226">Feature zum Aktualisieren von virtuellen VMSS-Computern</span><span class="sxs-lookup"><span data-stu-id="f2a32-226">VMSS VM Update feature</span></span>
    - <span data-ttu-id="f2a32-227">Cmdlets „Update-AzureRmVmssVM“ und „New-AzureRmVMDataDisk“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-227">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="f2a32-228">Fügen Sie den Parameter „VirtualMachineScaleSetVM“ zum Cmdlet „Add-AzureRmVMDataDisk“ hinzu, um das Hinzufügen eines Datenträgers zum virtuellen VMSS-Computer zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f2a32-228">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="f2a32-229">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="f2a32-229">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="f2a32-230">Aktualisierung der ADF .Net SDK-Version auf 0.8.0-preview mit den folgenden Änderungen:</span><span class="sxs-lookup"><span data-stu-id="f2a32-230">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="f2a32-231">Vorgang zum Konfigurieren des Factoryrepositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-231">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="f2a32-232">Der verknüpfte QuickBooks-Dienst wurde aktualisiert, um die Eigenschaften „consumerKey“ und „consumerSecret“ verfügbar zu machen.</span><span class="sxs-lookup"><span data-stu-id="f2a32-232">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="f2a32-233">Aktualisierung verschiedener Modelltypen von „SecretBase“ auf „Object“</span><span class="sxs-lookup"><span data-stu-id="f2a32-233">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="f2a32-234">Blobereignisauslöser hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-234">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="f2a32-235">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="f2a32-235">AzureRM.KeyVault</span></span>
* <span data-ttu-id="f2a32-236">Aktualisierung der Dokumentation mit Beispielausgabe</span><span class="sxs-lookup"><span data-stu-id="f2a32-236">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="f2a32-237">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="f2a32-237">AzureRM.Network</span></span>
* <span data-ttu-id="f2a32-238">Aktivierung der Traffic Analytics-Parameter für Network Watcher-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="f2a32-238">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="f2a32-239">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="f2a32-239">AzureRM.Resources</span></span>
* <span data-ttu-id="f2a32-240">Behebung des Problems mit der Eigenschaft „Properties“ von PSResource-Objekten, die von „Get-AzureRmResource“ zurückgegeben wurden</span><span class="sxs-lookup"><span data-stu-id="f2a32-240">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="f2a32-241">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="f2a32-241">AzureRM.Scheduler</span></span>
* <span data-ttu-id="f2a32-242">Behebung des Problems, dass beim Aktualisieren von „ServiceBusQueueJob“ keine neuen Authentifizierungswerte festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="f2a32-242">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="f2a32-243">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="f2a32-243">AzureRM.Sql</span></span>
* <span data-ttu-id="f2a32-244">Aktualisierung der folgenden Cmdlets mit dem optionalen LicenseType-Parameter</span><span class="sxs-lookup"><span data-stu-id="f2a32-244">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="f2a32-245">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="f2a32-245">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="f2a32-246">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="f2a32-246">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="f2a32-247">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="f2a32-247">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="f2a32-248">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="f2a32-248">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="f2a32-249">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="f2a32-249">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="f2a32-250">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="f2a32-250">AzureRM.Websites</span></span>
* <span data-ttu-id="f2a32-251">„New-AzureRMWebApp“ aktualisiert, um allgemeine Algorithmen aus der Strategiebibliothek zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="f2a32-251">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="f2a32-252">6.1.0 – Mai 2018</span><span class="sxs-lookup"><span data-stu-id="f2a32-252">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="f2a32-253">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="f2a32-253">AzureRM.Profile</span></span>
* <span data-ttu-id="f2a32-254">Behebung eines Problems, durch das beim Ausführen von „Clear-AzureRmContext“ ein leerer Kontext mit dem Namen des vorherigen Standardkontexts beibehalten wurde und der Benutzer dadurch keinen neuen Kontext mit dem alten Namen erstellen konnte</span><span class="sxs-lookup"><span data-stu-id="f2a32-254">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="f2a32-255">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="f2a32-255">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="f2a32-256">Ermöglichung der Zuordnung von Gateways/Aufhebung der Gatewayzuordnung in AS</span><span class="sxs-lookup"><span data-stu-id="f2a32-256">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="f2a32-257">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="f2a32-257">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="f2a32-258">Unterstützung für „ApiVersions“, „ApiReleases“ und „ApiRevisions“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-258">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="f2a32-259">Unterstützung für ServiceFabric-Back-End hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-259">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="f2a32-260">Unterstützung für Application Insights-Protokollierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-260">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="f2a32-261">Unterstützung für die Erkennung von SKUs vom Typ „Basic“ als gültige SKU des API Management-Diensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-261">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="f2a32-262">Unterstützung hinzugefügt, damit Zertifikate, die von der privaten Zertifizierungsstelle ausgestellt wurden, als Stamm- oder ZS-Zertifikate installiert werden können</span><span class="sxs-lookup"><span data-stu-id="f2a32-262">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="f2a32-263">Unterstützung für die Akzeptierung benutzerdefinierter SSL-Zertifikate über KeyVault und mehrere Proxyhostnamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-263">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="f2a32-264">Unterstützung für die verwaltete Dienstidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-264">Added support for MSI identity</span></span>
* <span data-ttu-id="f2a32-265">Unterstützung für die Annahme von Richtlinien über URL hinzugefügt; HINWEIS: Folgende Cmdlets werden in einem zukünftigen Release als veraltet gekennzeichnet:</span><span class="sxs-lookup"><span data-stu-id="f2a32-265">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="f2a32-266">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="f2a32-266">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="f2a32-267">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2a32-267">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="f2a32-268">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="f2a32-268">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="f2a32-269">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="f2a32-269">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="f2a32-270">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="f2a32-270">AzureRM.Batch</span></span>
* <span data-ttu-id="f2a32-271">Veröffentlichung des neuen Cmdlets „Get-AzureBatchPoolNodeCounts“</span><span class="sxs-lookup"><span data-stu-id="f2a32-271">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="f2a32-272">Veröffentlichung des neuen Cmdlets „Start-AzureBatchComputeNodeServiceLogUpload“</span><span class="sxs-lookup"><span data-stu-id="f2a32-272">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="f2a32-273">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="f2a32-273">AzureRM.Consumption</span></span>
* <span data-ttu-id="f2a32-274">Hinzufügung neuer Parameter („Expand“, „ResourceGroup“, „InstanceName“, „InstanceId“, „Tags“ und „Top“) für das Cmdlet „Get-AzureRmConsumptionUsageDetail“</span><span class="sxs-lookup"><span data-stu-id="f2a32-274">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="f2a32-275">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f2a32-275">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="f2a32-276">Korrektur des Beispiels für „Export AzureRmDataLakeStoreChildItemProperties“</span><span class="sxs-lookup"><span data-stu-id="f2a32-276">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="f2a32-277">Korrektur der NULL-Parameterausnahme für rekursiven Fall in „Set-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="f2a32-277">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="f2a32-278">Korrektur der Hilfedateien für „Set-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ und „Remove-AzureRmDataLakeStoreItemAclEntry“</span><span class="sxs-lookup"><span data-stu-id="f2a32-278">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="f2a32-279">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="f2a32-279">AzureRM.Network</span></span>
* <span data-ttu-id="f2a32-280">Erhöhung der Network SDK-Version von 18.0.0-preview auf 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="f2a32-280">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="f2a32-281">Cmdlet zum Erstellen der Protokollkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-281">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="f2a32-282">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2a32-282">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="f2a32-283">Cmdlet zum Hinzufügen einer neuen Leitungsverbindung zu einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-283">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="f2a32-284">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="f2a32-284">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="f2a32-285">Cmdlet zum Entfernen einer Leitungsverbindung aus einer vorhandenen ExpressRoute-Leitung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-285">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="f2a32-286">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="f2a32-286">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="f2a32-287">Cmdlet zum Abrufen einer Leitungsverbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f2a32-287">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="f2a32-288">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="f2a32-288">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="f2a32-289">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f2a32-289">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="f2a32-290">Verwendung der Serverauthentifizierung mit generierten Zertifikaten korrigiert (Problemnr. 5998)</span><span class="sxs-lookup"><span data-stu-id="f2a32-290">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="f2a32-291">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="f2a32-291">AzureRM.Sql</span></span>
* <span data-ttu-id="f2a32-292">Überwachungscmdlets korrigiert, um das Entfernen von „AuditActions“ oder „AuditActionGroups“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f2a32-292">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="f2a32-293">Problem mit „Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy“ behoben, das beim Festlegen einer neuen flexiblen Aufbewahrungsrichtlinie zu folgendem Fehler führte: „Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span><span class="sxs-lookup"><span data-stu-id="f2a32-293">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="f2a32-294">Please submit request with the new flexible retention policy“ (Das Konfigurieren einer langfristigen Aufbewahrungsrichtlinie mit Azure Recovery Service-Tresor und -Richtlinie wird nicht mehr unterstützt. Übermitteln Sie eine Anforderung mit der neuen flexiblen Aufbewahrungsrichtlinie.)</span><span class="sxs-lookup"><span data-stu-id="f2a32-294">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="f2a32-295">Aktualisierung aller Cmdlets für Azure SQL-Datenbank, für die Erstellung von Pools für elastische Datenbanken und für die Aktualisierung, sodass sie die neue Datenbank-API verwenden. Diese unterstützt die Sku-Eigenschaft für skalierungs- und tarifbezogene Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="f2a32-295">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="f2a32-296">Aktualisierte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="f2a32-296">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="f2a32-297">New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="f2a32-297">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="f2a32-298">New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="f2a32-298">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="f2a32-299">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="f2a32-299">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="f2a32-300">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="f2a32-300">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="f2a32-301">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="f2a32-301">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="f2a32-302">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="f2a32-302">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="f2a32-303">Aktualisierung der Parameter für „Get-AzureRmTrafficManagerProfile“, sodass bei Verwendung des Parameters „-Name“ der Parameter „-ResourceGroupName“ erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="f2a32-303">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>