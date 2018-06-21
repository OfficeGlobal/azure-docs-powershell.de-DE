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
ms.date: 5/1/2018
ms.openlocfilehash: 8515a267e80e5d1f7bb97557efa72b9e86b7b45d
ms.sourcegitcommit: 37bfbf11fd0967a8e7977c692ab829d286baf88a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/08/2018
ms.locfileid: "33912002"
---
# <a name="release-notes"></a><span data-ttu-id="8d69d-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="8d69d-103">Release notes</span></span>

<span data-ttu-id="8d69d-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="8d69d-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---

## <a name="600---may-2018"></a><span data-ttu-id="8d69d-105">6.0.0 – Mai 2018</span><span class="sxs-lookup"><span data-stu-id="8d69d-105">6.0.0 - May 2018</span></span>

### <a name="general"></a><span data-ttu-id="8d69d-106">Allgemein</span><span class="sxs-lookup"><span data-stu-id="8d69d-106">General</span></span>
* <span data-ttu-id="8d69d-107">Festlegung der Mindestabhängigkeit von Modulen auf PowerShell 5.0</span><span class="sxs-lookup"><span data-stu-id="8d69d-107">Set minimum dependency of modules to PowerShell 5.0</span></span>

### <a name="azurestorage"></a><span data-ttu-id="8d69d-108">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="8d69d-108">Azure.Storage</span></span>
* <span data-ttu-id="8d69d-109">Unterstützung als Storage-Blobcontainername</span><span class="sxs-lookup"><span data-stu-id="8d69d-109">Support  as Storage blob container name</span></span>
    - <span data-ttu-id="8d69d-110">New-AzureStorageBlobContainer</span><span class="sxs-lookup"><span data-stu-id="8d69d-110">New-AzureStorageBlobContainer</span></span>
    - <span data-ttu-id="8d69d-111">Remove-AzureStorageBlobContainer</span><span class="sxs-lookup"><span data-stu-id="8d69d-111">Remove-AzureStorageBlobContainer</span></span>
    - <span data-ttu-id="8d69d-112">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8d69d-112">Set-AzureStorageBlobContent</span></span>
    - <span data-ttu-id="8d69d-113">Get-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8d69d-113">Get-AzureStorageBlobContent</span></span>
* <span data-ttu-id="8d69d-114">Behebung des Problems, bei dem einige Fehlerausgaben von Storage-Cmdlets keine ausführlichen Informationen zum Fehler enthalten</span><span class="sxs-lookup"><span data-stu-id="8d69d-114">Fix the issue that some Storage cmdlets failure output not contain detail failure information</span></span>

### <a name="azurermapimanagement"></a><span data-ttu-id="8d69d-115">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d69d-115">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="8d69d-116">Einführung mehrerer grundlegender Änderungen</span><span class="sxs-lookup"><span data-stu-id="8d69d-116">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="8d69d-117">Weitere Informationen im Migrationsleitfaden</span><span class="sxs-lookup"><span data-stu-id="8d69d-117">Please refer to the migration guide for more information</span></span>

### <a name="azurermautomation"></a><span data-ttu-id="8d69d-118">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="8d69d-118">AzureRM.Automation</span></span>
* <span data-ttu-id="8d69d-119">Entfernung des veralteten „Tags“-Alias aus Cmdlets</span><span class="sxs-lookup"><span data-stu-id="8d69d-119">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="8d69d-120">„Set-AzureRmAutomationRunbook“</span><span class="sxs-lookup"><span data-stu-id="8d69d-120">'Set-AzureRmAutomationRunbook'</span></span>

### <a name="azurermbatch"></a><span data-ttu-id="8d69d-121">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="8d69d-121">AzureRM.Batch</span></span>
* <span data-ttu-id="8d69d-122">Aktualisierung der Dokumentation zu „New-AzureBatchPool“ mit Entfernung des veralteten Beispiels</span><span class="sxs-lookup"><span data-stu-id="8d69d-122">Updated New-AzureBatchPool documentation to remove deprecated example</span></span>

### <a name="azurermcdn"></a><span data-ttu-id="8d69d-123">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="8d69d-123">AzureRM.Cdn</span></span>
* <span data-ttu-id="8d69d-124">Einführung mehrerer grundlegender Änderungen</span><span class="sxs-lookup"><span data-stu-id="8d69d-124">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="8d69d-125">Weitere Informationen im Migrationsleitfaden</span><span class="sxs-lookup"><span data-stu-id="8d69d-125">Please refer to the migration guide for more information</span></span>

### <a name="azurermcompute"></a><span data-ttu-id="8d69d-126">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="8d69d-126">AzureRM.Compute</span></span>
* <span data-ttu-id="8d69d-127">Unterstützung der ausführlichen Ausgabe von Parametern durch „New-AzureRmVm“ und „New-AzureRmVmss“</span><span class="sxs-lookup"><span data-stu-id="8d69d-127">'New-AzureRmVm' and 'New-AzureRmVmss' support verbose output of parameters</span></span>
* <span data-ttu-id="8d69d-128">Unterstützung der Zuweisung von benutzer- bzw. systemdefinierten Identitäten zu VMs durch „New-AzureRmVm“ und „New-AzureRmVmss“</span><span class="sxs-lookup"><span data-stu-id="8d69d-128">'New-AzureRmVm' and 'New-AzureRmVmss' (simple parameter set) support assigning user defined and(or) system defined identities to the VM(s).</span></span>
* <span data-ttu-id="8d69d-129">Erneute VMSS-Bereitstellung (Redeploy) und PerformMaintenance-Feature</span><span class="sxs-lookup"><span data-stu-id="8d69d-129">VMSS Redeploy and PerformMaintenance feature</span></span>
    -  <span data-ttu-id="8d69d-130">Hinzufügung der neuen Switchparameter „-Redeploy“ und „-PerformMaintenance“ zu „Set-AzureRmVmss“ und „Set-AzureRmVmssVM“</span><span class="sxs-lookup"><span data-stu-id="8d69d-130">Add new switch parameter -Redeploy and -PerformMaintenance to 'Set-AzureRmVmss' and 'Set-AzureRmVmssVM'</span></span>
* <span data-ttu-id="8d69d-131">Hinzufügung des Switchparameters „Add DisableVMAgent“ zum Set-AzureRmVMOperatingSystem-Cmdlet</span><span class="sxs-lookup"><span data-stu-id="8d69d-131">Add DisableVMAgent switch parameter to 'Set-AzureRmVMOperatingSystem' cmdlet</span></span>
* <span data-ttu-id="8d69d-132">Unterstützung eines „Win10“-Images durch „New-AzureRmVm“ und „New-AzureRmVmss“ (einfacher Parametersatz)</span><span class="sxs-lookup"><span data-stu-id="8d69d-132">'New-AzureRmVm' and 'New-AzureRmVmss' (simple parameter set) support a 'Win10' image.</span></span>
* <span data-ttu-id="8d69d-133">Hinzufügung des Repair-AzureRmVmssServiceFabricUpdateDomain-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="8d69d-133">'Repair-AzureRmVmssServiceFabricUpdateDomain' cmdlet is added.</span></span>
* <span data-ttu-id="8d69d-134">Einführung mehrerer grundlegender Änderungen</span><span class="sxs-lookup"><span data-stu-id="8d69d-134">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="8d69d-135">Ausführlichere Informationen im Migrationsleitfaden</span><span class="sxs-lookup"><span data-stu-id="8d69d-135">Please refer to the migration guide for more details</span></span>
* <span data-ttu-id="8d69d-136">AAD-Parameter werden durch „Set-AzureRmVmDiskEncryptionExtension“ optional</span><span class="sxs-lookup"><span data-stu-id="8d69d-136">'Set-AzureRmVmDiskEncryptionExtension' makes AAD parameters optional</span></span>

### <a name="azurermdatafactories"></a><span data-ttu-id="8d69d-137">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="8d69d-137">AzureRM.DataFactories</span></span>
* <span data-ttu-id="8d69d-138">Entfernung des veralteten „Tags“-Alias aus Cmdlets</span><span class="sxs-lookup"><span data-stu-id="8d69d-138">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="8d69d-139">New-AzureRmDataFactory</span><span class="sxs-lookup"><span data-stu-id="8d69d-139">New-AzureRmDataFactory</span></span>

### <a name="azurermdatafactoryv2"></a><span data-ttu-id="8d69d-140">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="8d69d-140">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="8d69d-141">Aktualisierung des ADF-.Net SDK auf Vorschauversion 0.7.0 mit den folgenden Änderungen:</span><span class="sxs-lookup"><span data-stu-id="8d69d-141">Updated the ADF .Net SDK version to 0.7.0-preview containing following changes:</span></span>
    - <span data-ttu-id="8d69d-142">Hinzufügung von Ausführungsparametern und der Verbindungs-Manager-Eigenschaft zur ExecuteSSISPackage-Aktivität</span><span class="sxs-lookup"><span data-stu-id="8d69d-142">Added execution parameters and connection managers property on ExecuteSSISPackage Activity</span></span>
    - <span data-ttu-id="8d69d-143">Aktualisierung des verknüpften PostgreSql-/MySql-Diensts auf die Nutzung der vollständigen Verbindungszeichenfolge anstelle von Server, Datenbank, Schema, Benutzername und Kennwort</span><span class="sxs-lookup"><span data-stu-id="8d69d-143">Updated PostgreSql, MySql llinked service to use full connection string instead of server, database, schema, username and password</span></span>
    - <span data-ttu-id="8d69d-144">Entfernung des Schemas aus dem verknüpften DB2-Dienst</span><span class="sxs-lookup"><span data-stu-id="8d69d-144">Removed the schema from DB2 linked service</span></span>
    - <span data-ttu-id="8d69d-145">Entfernung der Schemaeigenschaft aus dem verknüpften Teradata-Dienst</span><span class="sxs-lookup"><span data-stu-id="8d69d-145">Removed schema property from Teradata linked service</span></span>
    - <span data-ttu-id="8d69d-146">Hinzufügung von LinkedService, Dataset und CopySource für Responsys</span><span class="sxs-lookup"><span data-stu-id="8d69d-146">Added LinkedService, Dataset, CopySource for Responsys</span></span>

### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="8d69d-147">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="8d69d-147">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="8d69d-148">Entfernung des veralteten „Tags“-Alias aus Cmdlets</span><span class="sxs-lookup"><span data-stu-id="8d69d-148">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="8d69d-149">„New-AzureRmDataLakeAnalyticsAccount“</span><span class="sxs-lookup"><span data-stu-id="8d69d-149">'New-AzureRmDataLakeAnalyticsAccount'</span></span>
    - <span data-ttu-id="8d69d-150">„Set-AzureRmDataLakeAnalyticsAccount“</span><span class="sxs-lookup"><span data-stu-id="8d69d-150">'Set-AzureRmDataLakeAnalyticsAccount'</span></span>

### <a name="azurermdatalakestore"></a><span data-ttu-id="8d69d-151">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d69d-151">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="8d69d-152">Hinzufügung des neuen Features für die rekursive ACL-Änderung zu „Remove-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAclEntry“ und „Set-AzureRmDataLakeStoreItemAcl“</span><span class="sxs-lookup"><span data-stu-id="8d69d-152">Add new feature of recursive Acl Change to Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="8d69d-153">Hinzufügung eines neuen Cmdlets zum Abrufen der Inhaltszusammenfassung unter einem Verzeichnis</span><span class="sxs-lookup"><span data-stu-id="8d69d-153">Add new cmdlet for retrieving the content summary under a directory</span></span>
* <span data-ttu-id="8d69d-154">Hinzufügung eines neuen Cmdlets zu Abrufen der Datenträgerauslastung und eines ACL-Abbilds</span><span class="sxs-lookup"><span data-stu-id="8d69d-154">Add new cmdlet for retrieving the disk usage and Acl dump</span></span>
* <span data-ttu-id="8d69d-155">Korrektur des Rückgabetyps von „Set-AzureRmDataLakeStoreItemAcl“ von „Bool“ in „IEnumerable<DataLakeStoreItemAce>“</span><span class="sxs-lookup"><span data-stu-id="8d69d-155">Correct return type of Set-AzureRmDataLakeStoreItemAcl bool to IEnumerable<DataLakeStoreItemAce></span></span>
* <span data-ttu-id="8d69d-156">Korrektur des Rückgabetyps von „Set-AzureRmDataLakeStoreItemAclEntry“ von „Bool“ in „IEnumerable<DataLakeStoreItemAce>“</span><span class="sxs-lookup"><span data-stu-id="8d69d-156">Correct return type of Set-AzureRmDataLakeStoreItemAclEntry bool to IEnumerable<DataLakeStoreItemAce></span></span>
* <span data-ttu-id="8d69d-157">Grundlegende Änderungen in „Export-AzureRmDataLakeStoreItem“, „Import-AzureRmDataLakeStoreItem“ und „Remove-AzureRmDataLakeStoreItem“</span><span class="sxs-lookup"><span data-stu-id="8d69d-157">Breaking changes in Export-AzureRmDataLakeStoreItem, Import-AzureRmDataLakeStoreItem, Remove-AzureRmDataLakeStoreItem</span></span>

### <a name="azurermdns"></a><span data-ttu-id="8d69d-158">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="8d69d-158">AzureRM.Dns</span></span>
* <span data-ttu-id="8d69d-159">Einführung mehrerer grundlegender Änderungen</span><span class="sxs-lookup"><span data-stu-id="8d69d-159">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="8d69d-160">Weitere Informationen im Migrationsleitfaden</span><span class="sxs-lookup"><span data-stu-id="8d69d-160">Please refer to the migration guide for more information</span></span>

### <a name="azurermeventhub"></a><span data-ttu-id="8d69d-161">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="8d69d-161">AzureRM.EventHub</span></span>
* <span data-ttu-id="8d69d-162">Aktualisierung der Hilfe für Cmdlets mit fehlenden Beispielen</span><span class="sxs-lookup"><span data-stu-id="8d69d-162">Updated Help for cmdlets with missing examples</span></span>

### <a name="azurerminsights"></a><span data-ttu-id="8d69d-163">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="8d69d-163">AzureRM.Insights</span></span>
* <span data-ttu-id="8d69d-164">Einführung mehrerer grundlegender Änderungen</span><span class="sxs-lookup"><span data-stu-id="8d69d-164">Introduced multiple breaking changes</span></span>
    - <span data-ttu-id="8d69d-165">Weitere Informationen im Migrationsleitfaden</span><span class="sxs-lookup"><span data-stu-id="8d69d-165">Please refer to the migration guide for more information</span></span>

### <a name="azurermiothub"></a><span data-ttu-id="8d69d-166">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d69d-166">AzureRM.IotHub</span></span>
* <span data-ttu-id="8d69d-167">Aktivierung von Tags und Basic-SKU für IotHub</span><span class="sxs-lookup"><span data-stu-id="8d69d-167">Enable tags and Basic Sku to the IotHub</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="8d69d-168">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d69d-168">AzureRM.KeyVault</span></span>
* <span data-ttu-id="8d69d-169">Grundlegende Änderungen zur Unterstützung von Pipingszenarien</span><span class="sxs-lookup"><span data-stu-id="8d69d-169">Breaking changes to support piping scenarios</span></span>
* <span data-ttu-id="8d69d-170">Neu hinzugefügte Cmdlets: „Backup/Restore-AzureKeyVaultManagedStorageAccount“, „Backup/Restore-AzureKeyVaultCertificate“, „Undo-AzureKeyVaultManagedStorageSasDefinitionRemoval“ und „Undo-AzureKeyVaultManagedStorageAccountRemoval“</span><span class="sxs-lookup"><span data-stu-id="8d69d-170">Added new cmdlets: Backup/Restore-AzureKeyVaultManagedStorageAccount, Backup/Restore-AzureKeyVaultCertificate, Undo-AzureKeyVaultManagedStorageSasDefinitionRemoval, and Undo-AzureKeyVaultManagedStorageAccountRemoval</span></span>

### <a name="azurermmachinelearning"></a><span data-ttu-id="8d69d-171">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="8d69d-171">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="8d69d-172">Entfernung des veralteten „Tags“-Alias aus Cmdlets</span><span class="sxs-lookup"><span data-stu-id="8d69d-172">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="8d69d-173">Update-AzureRmMlCommitmentPlan</span><span class="sxs-lookup"><span data-stu-id="8d69d-173">Update-AzureRmMlCommitmentPlan</span></span>

### <a name="azurermmedia"></a><span data-ttu-id="8d69d-174">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="8d69d-174">AzureRM.Media</span></span>
* <span data-ttu-id="8d69d-175">Entfernung des veralteten „Tags“-Alias aus Cmdlets</span><span class="sxs-lookup"><span data-stu-id="8d69d-175">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="8d69d-176">„Set-AzureRmMediaService“</span><span class="sxs-lookup"><span data-stu-id="8d69d-176">'Set-AzureRmMediaService'</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="8d69d-177">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="8d69d-177">AzureRM.Network</span></span>
* <span data-ttu-id="8d69d-178">Hinzufügung von Unterstützung für DDoS-Schutzplanressource</span><span class="sxs-lookup"><span data-stu-id="8d69d-178">Add support for DDoS protection plan resource</span></span>
* <span data-ttu-id="8d69d-179">Einführung mehrerer grundlegender Änderungen</span><span class="sxs-lookup"><span data-stu-id="8d69d-179">Introduced multiple breaking changes</span></span>
    - <span data-ttu-id="8d69d-180">Weitere Informationen im Migrationsleitfaden</span><span class="sxs-lookup"><span data-stu-id="8d69d-180">Please refer to the migration guide for more information</span></span>

### <a name="azurermnotificationhubs"></a><span data-ttu-id="8d69d-181">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="8d69d-181">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="8d69d-182">Einführung mehrerer grundlegender Änderungen</span><span class="sxs-lookup"><span data-stu-id="8d69d-182">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="8d69d-183">Weitere Informationen im Migrationsleitfaden</span><span class="sxs-lookup"><span data-stu-id="8d69d-183">Please refer to the migration guide for more information</span></span>

### <a name="azurermoperationalinsights"></a><span data-ttu-id="8d69d-184">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d69d-184">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="8d69d-185">Einführung mehrerer grundlegender Änderungen</span><span class="sxs-lookup"><span data-stu-id="8d69d-185">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="8d69d-186">Weitere Informationen im Migrationsleitfaden</span><span class="sxs-lookup"><span data-stu-id="8d69d-186">Please refer to the migration guide for more information</span></span>

### <a name="azurermprofile"></a><span data-ttu-id="8d69d-187">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="8d69d-187">AzureRM.Profile</span></span>
* <span data-ttu-id="8d69d-188">Standardmäßige Aktivierung der automatischen Kontextspeicherung</span><span class="sxs-lookup"><span data-stu-id="8d69d-188">Enable context autosave by default</span></span>
* <span data-ttu-id="8d69d-189">Hinzufügung der Eigenschaften „USGovernmentOperationalInsightsEndpoint“ und „USGovernmentOperationalInsightsEndpointResourceId“ zur Azure-Umgebung für US Gov</span><span class="sxs-lookup"><span data-stu-id="8d69d-189">Add USGovernmentOperationalInsightsEndpoint and USGovernmentOperationalInsightsEndpointResourceId properties to Azure environment for US Gov.</span></span>

### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="8d69d-190">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="8d69d-190">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="8d69d-191">Feste Authentifizierungsheader in SiteRecovery-Szenarien</span><span class="sxs-lookup"><span data-stu-id="8d69d-191">Fixed Authentication Header in SiteRecovery scenarios</span></span>

### <a name="azurermrediscache"></a><span data-ttu-id="8d69d-192">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8d69d-192">AzureRM.RedisCache</span></span>
* <span data-ttu-id="8d69d-193">Einführung mehrerer grundlegender Änderungen</span><span class="sxs-lookup"><span data-stu-id="8d69d-193">Introduced multiple breaking changes</span></span>
    - <span data-ttu-id="8d69d-194">Weitere Informationen im Migrationsleitfaden</span><span class="sxs-lookup"><span data-stu-id="8d69d-194">Please refer to the migration guide for more information</span></span>

### <a name="azurermresources"></a><span data-ttu-id="8d69d-195">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="8d69d-195">AzureRM.Resources</span></span>
* <span data-ttu-id="8d69d-196">Entfernung des veralteten Parameters „-AtScopeAndBelow“ aus dem Get-AzureRmRoledefinition-Aufruf</span><span class="sxs-lookup"><span data-stu-id="8d69d-196">Remove obsolete parameter -AtScopeAndBelow from Get-AzureRmRoledefinition call</span></span>
* <span data-ttu-id="8d69d-197">Einbindung von Zuweisungen zu gelöschten Users/Groups/ServicePrincipals in das Get-AzureRmRoleAssignment-Ergebnis</span><span class="sxs-lookup"><span data-stu-id="8d69d-197">Include assignments to deleted USers/Groups/ServicePrincipals in Get-AzureRmRoleAssignment result</span></span>
* <span data-ttu-id="8d69d-198">Hinzufügung von Registerkarten-Completern für Scope und ResourceType</span><span class="sxs-lookup"><span data-stu-id="8d69d-198">Add Tab completers for Scope and ResourceType</span></span>
* <span data-ttu-id="8d69d-199">Hinzufügung des convenience-Cmdlets für die Erstellung von ServicePrincipals</span><span class="sxs-lookup"><span data-stu-id="8d69d-199">Add convenience cmdlet for creating ServicePrincipals</span></span>
* <span data-ttu-id="8d69d-200">Zusammenführung der „Get-“- und „Find-“-Funktionalität in „Get-AzureRmResource“</span><span class="sxs-lookup"><span data-stu-id="8d69d-200">Merge Get- and Find- functionality in Get-AzureRmResource</span></span>
* <span data-ttu-id="8d69d-201">Hinzugefügte AD-Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8d69d-201">Add AD Cmdlets:</span></span>
  - <span data-ttu-id="8d69d-202">Remove-AzureRmADGroupMember</span><span class="sxs-lookup"><span data-stu-id="8d69d-202">Remove-AzureRmADGroupMember</span></span>
  - <span data-ttu-id="8d69d-203">Get-AzureRmADGroup</span><span class="sxs-lookup"><span data-stu-id="8d69d-203">Get-AzureRmADGroup</span></span>
  - <span data-ttu-id="8d69d-204">New-AzureRmADGroup</span><span class="sxs-lookup"><span data-stu-id="8d69d-204">New-AzureRmADGroup</span></span>
  - <span data-ttu-id="8d69d-205">Remove-AzureRmADGroup</span><span class="sxs-lookup"><span data-stu-id="8d69d-205">Remove-AzureRmADGroup</span></span>
  - <span data-ttu-id="8d69d-206">Remove-AzureRmADUser</span><span class="sxs-lookup"><span data-stu-id="8d69d-206">Remove-AzureRmADUser</span></span>
  - <span data-ttu-id="8d69d-207">Update-AzureRmADApplication</span><span class="sxs-lookup"><span data-stu-id="8d69d-207">Update-AzureRmADApplication</span></span>
  - <span data-ttu-id="8d69d-208">Update-AzureRmADServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="8d69d-208">Update-AzureRmADServicePrincipal</span></span>
  - <span data-ttu-id="8d69d-209">Update-AzureRmADUser</span><span class="sxs-lookup"><span data-stu-id="8d69d-209">Update-AzureRmADUser</span></span>

### <a name="azurermservicefabric"></a><span data-ttu-id="8d69d-210">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d69d-210">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="8d69d-211">Aktualisierung der Standard-SKU für die Linux-Imageversion</span><span class="sxs-lookup"><span data-stu-id="8d69d-211">Update default Linux image version sku</span></span>
  - <span data-ttu-id="8d69d-212">„NewAzureServiceFabricCluster.cs“ – UbuntuServer1604-SKU-Standardupdate</span><span class="sxs-lookup"><span data-stu-id="8d69d-212">NewAzureServiceFabricCluster.cs default UbuntuServer1604 Sku update</span></span>

### <a name="azurermstorage"></a><span data-ttu-id="8d69d-213">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="8d69d-213">AzureRM.Storage</span></span>
* <span data-ttu-id="8d69d-214">Einführung mehrerer grundlegender Änderungen</span><span class="sxs-lookup"><span data-stu-id="8d69d-214">Introduced multiple breaking changes</span></span>
    - <span data-ttu-id="8d69d-215">Weitere Informationen im Migrationsleitfaden</span><span class="sxs-lookup"><span data-stu-id="8d69d-215">Please refer to the migration guide for more information</span></span>

### <a name="azurermwebsites"></a><span data-ttu-id="8d69d-216">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="8d69d-216">AzureRM.Websites</span></span>
* <span data-ttu-id="8d69d-217">Upgrade auf die aktuelle Version des Websites-SDK</span><span class="sxs-lookup"><span data-stu-id="8d69d-217">Upgrade to latest version of the Websites SDK</span></span>
* <span data-ttu-id="8d69d-218">Hinzufügung der Eigenschaften „-AssignIdentity“ und „-Httpsonly“ für „Set-AzureRmWebApp“ und „Set-AzureRmWebAppSlot“</span><span class="sxs-lookup"><span data-stu-id="8d69d-218">Added -AssignIdentity & -Httpsonly properties for Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
* <span data-ttu-id="8d69d-219">Hinzufügung von zwei neuen Cmdlets: „Get-AzureRmWebAppSnapshots“ und „Restore-AzureRmWebAppSnapshot“</span><span class="sxs-lookup"><span data-stu-id="8d69d-219">Added two new cmdlets: Get-AzureRmWebAppSnapshots and Restore-AzureRmWebAppSnapshot</span></span>
