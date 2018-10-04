---
title: Übersicht über Azure Stack PowerShell mit Administratorrechten | Microsoft-Dokumentation
description: Enthält eine Übersicht über Azure Stack PowerShell mit Administratorrechten und eine Anleitung zur Installation und Konfiguration.
author: bganapa
ms.author: bganapa
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 09/21/2018
ms.openlocfilehash: 72d147f5bc9c882083dda6b33b1c89663fd2eb34
ms.sourcegitcommit: 6c38e86e16da99f65cd183c63e34f7176b121ab8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/04/2018
ms.locfileid: "47424852"
---
# <a name="azure-stack-module-140"></a><span data-ttu-id="83d03-103">Azure Stack-Modul 1.4.0</span><span class="sxs-lookup"><span data-stu-id="83d03-103">Azure Stack Module 1.4.0</span></span>

## <a name="requirements"></a><span data-ttu-id="83d03-104">Anforderungen:</span><span class="sxs-lookup"><span data-stu-id="83d03-104">Requirements:</span></span>
<span data-ttu-id="83d03-105">Die niedrigste unterstützte Azure Stack-Version ist 1804.</span><span class="sxs-lookup"><span data-stu-id="83d03-105">Minimum supported Azure Stack version is 1804.</span></span>

<span data-ttu-id="83d03-106">Hinweis: Falls Sie eine niedrigere Version verwenden, installieren Sie die Version 1.2.11.</span><span class="sxs-lookup"><span data-stu-id="83d03-106">Note: If you are using an earlier version install version 1.2.11</span></span>

## <a name="known-issues"></a><span data-ttu-id="83d03-107">Bekannte Probleme:</span><span class="sxs-lookup"><span data-stu-id="83d03-107">Known issues:</span></span>

- <span data-ttu-id="83d03-108">Zum Schließen einer Warnung wird die Azure Stack-Version 1803 benötigt.</span><span class="sxs-lookup"><span data-stu-id="83d03-108">Close Alert requires Azure Stack version 1803</span></span>
- <span data-ttu-id="83d03-109">Mit „New-AzsOffer“ können keine öffentlichen Angebote erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="83d03-109">New-AzsOffer does not allow to create an offer with state public.</span></span> <span data-ttu-id="83d03-110">Das Cmdlet „Set-AzsOffer“ muss hinterher aufgerufen werden, um den Zustand zu ändern.</span><span class="sxs-lookup"><span data-stu-id="83d03-110">The Set-AzsOffer cmdlet needs to be called afterwards to change the state.</span></span>
- <span data-ttu-id="83d03-111">Ein IP-Pool kann nicht ohne erneute Bereitstellung entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="83d03-111">An IP Pool cannot be removed without a redeployment</span></span>

## <a name="breaking-changes"></a><span data-ttu-id="83d03-112">Wichtige Änderungen</span><span class="sxs-lookup"><span data-stu-id="83d03-112">Breaking Changes</span></span>
<span data-ttu-id="83d03-113">Für die Folgeversion von Version 1.3.0 wurden keine Breaking Changes vorgenommen.</span><span class="sxs-lookup"><span data-stu-id="83d03-113">There are no breaking changes from the version 1.3.0.</span></span> <span data-ttu-id="83d03-114">Alle Breaking Changes, die aus der Version 1.2.11 migriert werden, sind hier dokumentiert: https://aka.ms/azspowershellmigration</span><span class="sxs-lookup"><span data-stu-id="83d03-114">All breaking changes migrating from 1.2.11 are documented here https://aka.ms/azspowershellmigration</span></span>

## <a name="install"></a><span data-ttu-id="83d03-115">Installieren</span><span class="sxs-lookup"><span data-stu-id="83d03-115">Install</span></span>
```
# Remove previous versions of AzureStack modules
Uninstall-Module -Name AzureStack -Force 
Uninstall-Module AzureRM.AzureStackAdmin -Force
Uninstall-Module AzureRM.AzureStackStorage -Force
Get-Module Azs.* -ListAvailable | Uninstall-Module -Force


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2017-03-09-profile -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.4.0
```
## <a name="release-notes"></a><span data-ttu-id="83d03-116">Versionsinformationen</span><span class="sxs-lookup"><span data-stu-id="83d03-116">Release Notes</span></span>
    * <span data-ttu-id="83d03-117">Zwischen der Vorgängerversion 1.3.0 und der Azure Stack-Version 1.4.0 wurden keine Breaking Changes eingeführt.</span><span class="sxs-lookup"><span data-stu-id="83d03-117">Azurestack 1.4.0 version has no breaking changes from the previous release 1.3.0</span></span>
    * <span data-ttu-id="83d03-118">Azs.AzureBridge.Admin</span><span class="sxs-lookup"><span data-stu-id="83d03-118">Azs.AzureBridge.Admin</span></span>
        - <span data-ttu-id="83d03-119">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="83d03-119">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="83d03-120">Azs.Backup.Admin</span><span class="sxs-lookup"><span data-stu-id="83d03-120">Azs.Backup.Admin</span></span>
        - <span data-ttu-id="83d03-121">Die neuen Parameter „BackupFrequencyInHours“, „IsBackupSchedulerEnabled“ und „BackupRetentionPeriodInDays“ wurden im Cmdlet „Set-AzsBackupShare“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="83d03-121">Added new parameters BackupFrequencyInHours, IsBackupSchedulerEnabled, BackupRetentionPeriodInDays in cmdlet Set-AzsBackupShare</span></span>
        - <span data-ttu-id="83d03-122">Cmdlet „New-EncyptionKeyBase64“ hinzugefügt, um die Erstellung eines Verschlüsselungsschlüssels zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="83d03-122">Added a cmdlet New-EncyptionKeyBase64 to facilitate creating encryption key</span></span>
        - <span data-ttu-id="83d03-123">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="83d03-123">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="83d03-124">Azs.Commerce.Admin</span><span class="sxs-lookup"><span data-stu-id="83d03-124">Azs.Commerce.Admin</span></span>
        - <span data-ttu-id="83d03-125">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="83d03-125">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="83d03-126">Azs.Fabric.Admin</span><span class="sxs-lookup"><span data-stu-id="83d03-126">Azs.Fabric.Admin</span></span>
        - <span data-ttu-id="83d03-127">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="83d03-127">Fix for the bug that returned only a single page in paginated results</span></span>
        - <span data-ttu-id="83d03-128">Cmdlet „Add-AzsScaleUnitNode“ hinzugefügt, um dem Administrator das Hinzufügen neuer Skalierungseinheitknoten azurestack-Stempel zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="83d03-128">Added a cmdlet Add-AzsScaleUnitNode to enable admin to add new scale unit nodes to the azurestack stamp</span></span>
        - <span data-ttu-id="83d03-129">Cmdlet „New-AzsScaleUnitNodeObject“ hinzugefügt, um die Erstellung von Skalierungseinheit-Parameterobjekten zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="83d03-129">Added cmdlet and New-AzsScaleUnitNodeObject to facilitate the creation scale unit parameter objects</span></span>
    * <span data-ttu-id="83d03-130">Azs.Gallery.Admin</span><span class="sxs-lookup"><span data-stu-id="83d03-130">Azs.Gallery.Admin</span></span>
        - <span data-ttu-id="83d03-131">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="83d03-131">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="83d03-132">Azs.InfrastructureInsights.Admin</span><span class="sxs-lookup"><span data-stu-id="83d03-132">Azs.InfrastructureInsights.Admin</span></span>
        - <span data-ttu-id="83d03-133">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="83d03-133">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="83d03-134">Azs.Network.Admin</span><span class="sxs-lookup"><span data-stu-id="83d03-134">Azs.Network.Admin</span></span>
        - <span data-ttu-id="83d03-135">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="83d03-135">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="83d03-136">Azs.Update.Admin</span><span class="sxs-lookup"><span data-stu-id="83d03-136">Azs.Update.Admin</span></span>
        - <span data-ttu-id="83d03-137">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="83d03-137">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="83d03-138">Azs.Subscriptions</span><span class="sxs-lookup"><span data-stu-id="83d03-138">Azs.Subscriptions</span></span>
        - <span data-ttu-id="83d03-139">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="83d03-139">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="83d03-140">Azs.Subscriptions.Admin</span><span class="sxs-lookup"><span data-stu-id="83d03-140">Azs.Subscriptions.Admin</span></span>
        - <span data-ttu-id="83d03-141">Cmdlet „Move-AzsSubscription“ hinzugefügt, um Abonnements zwischen Angeboten delegierter Anbieter zu verschieben</span><span class="sxs-lookup"><span data-stu-id="83d03-141">Added a cmdlet Move-AzsSubscription to move subscriptions between delegated provider offers</span></span>
        - <span data-ttu-id="83d03-142">Cmdlet „Test-AzsMoveSubscription“ hinzugefügt, um zu überprüfen, ob Benutzerabonnements zwischen Angeboten delegierter Anbieter verschoben werden können</span><span class="sxs-lookup"><span data-stu-id="83d03-142">Added a cmdlet Test-AzsMoveSubscription to validate that user subscriptions can be moved between delegated provider offers</span></span>
        - <span data-ttu-id="83d03-143">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="83d03-143">Fix for the bug that returned only a single page in paginated results'</span></span>

## <a name="content"></a><span data-ttu-id="83d03-144">Inhalt:</span><span class="sxs-lookup"><span data-stu-id="83d03-144">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="83d03-145">Azure-Bridge</span><span class="sxs-lookup"><span data-stu-id="83d03-145">Azure Bridge</span></span>
<span data-ttu-id="83d03-146">Vorschauversion des AzureBridge-Administratormoduls von Azure Stack, mit dem Sie Images aus Azure syndizieren können.</span><span class="sxs-lookup"><span data-stu-id="83d03-146">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="83d03-147">Backup</span><span class="sxs-lookup"><span data-stu-id="83d03-147">Backup</span></span>
<span data-ttu-id="83d03-148">Vorschauversion des Backup-Administratormoduls, das Administratoren Folgendes ermöglicht:</span><span class="sxs-lookup"><span data-stu-id="83d03-148">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="83d03-149">Konfigurieren des Speicherorts von Sicherungen</span><span class="sxs-lookup"><span data-stu-id="83d03-149">Configure where backups are stored</span></span>
- <span data-ttu-id="83d03-150">Durchführen von Sicherungen</span><span class="sxs-lookup"><span data-stu-id="83d03-150">Perform backups</span></span>
- <span data-ttu-id="83d03-151">Auflisten und Wiederherstellen abgeschlossener Sicherungen</span><span class="sxs-lookup"><span data-stu-id="83d03-151">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="83d03-152">Commerce</span><span class="sxs-lookup"><span data-stu-id="83d03-152">Commerce</span></span>
<span data-ttu-id="83d03-153">Vorschauversion des Commerce-Administratormoduls von Azure Stack, mit dem die aggregierte Datennutzung für das gesamte Azure Stack-System angezeigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="83d03-153">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="83d03-154">Compute</span><span class="sxs-lookup"><span data-stu-id="83d03-154">Compute</span></span>
<span data-ttu-id="83d03-155">Vorschauversion des Compute-Administratormoduls von Azure Stack mit Funktionen zur Verwaltung von Computekontingenten, Plattformimages und VM-Erweiterungen.</span><span class="sxs-lookup"><span data-stu-id="83d03-155">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="83d03-156">Fabric</span><span class="sxs-lookup"><span data-stu-id="83d03-156">Fabric</span></span>
<span data-ttu-id="83d03-157">Vorschauversion des Fabric-Administratormoduls von Azure Stack, mit dem Administratoren Infrastrukturkomponenten anzeigen und verwalten können:</span><span class="sxs-lookup"><span data-stu-id="83d03-157">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="83d03-158">Beenden, Starten und Herunterfahren von Skalierungseinheitknoten</span><span class="sxs-lookup"><span data-stu-id="83d03-158">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="83d03-159">Entladen und Fortsetzen von Skalierungseinheitknoten für FRU-bezogene Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="83d03-159">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="83d03-160">Reparieren von Skalierungseinheitknoten</span><span class="sxs-lookup"><span data-stu-id="83d03-160">Repair of scale unit nodes</span></span>
- <span data-ttu-id="83d03-161">Neustarten der Infrastrukturrolle</span><span class="sxs-lookup"><span data-stu-id="83d03-161">Restart of Infrastructure role</span></span>
- <span data-ttu-id="83d03-162">Beenden, Starten und Herunterfahren von Instanzen der Infrastrukturrolle</span><span class="sxs-lookup"><span data-stu-id="83d03-162">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="83d03-163">Erstellen neuer IP-Pools</span><span class="sxs-lookup"><span data-stu-id="83d03-163">Create new IP Pools</span></span>

### <a name="gallery"></a><span data-ttu-id="83d03-164">Gallery</span><span class="sxs-lookup"><span data-stu-id="83d03-164">Gallery</span></span>
<span data-ttu-id="83d03-165">Vorschauversion des Gallery-Administratormoduls von Azure Stack mit Funktionen zum Verwalten von Katalogelementen im Azure Stack-Marketplace.</span><span class="sxs-lookup"><span data-stu-id="83d03-165">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="83d03-166">Infrastructure Insights</span><span class="sxs-lookup"><span data-stu-id="83d03-166">Infrastructure Insights</span></span>
<span data-ttu-id="83d03-167">Vorschauversion des Infrastructure Insights-Administratormoduls, das Administratoren Folgendes ermöglicht:</span><span class="sxs-lookup"><span data-stu-id="83d03-167">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="83d03-168">Anzeigen der Integrität ihrer Azure Stack-Stempelressourcen</span><span class="sxs-lookup"><span data-stu-id="83d03-168">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="83d03-169">Anzeigen und Verwalten von Warnungen</span><span class="sxs-lookup"><span data-stu-id="83d03-169">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="83d03-170">KeyVault</span><span class="sxs-lookup"><span data-stu-id="83d03-170">KeyVault</span></span>
<span data-ttu-id="83d03-171">Vorschauversion des KeyVault-Administratormoduls von Azure Stack, mit dem Administratoren KeyVault-Kontingente anzeigen können.</span><span class="sxs-lookup"><span data-stu-id="83d03-171">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="83d03-172">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="83d03-172">Network</span></span>
<span data-ttu-id="83d03-173">Vorschauversion des Network-Administratormoduls, das Folgendes ermöglicht:</span><span class="sxs-lookup"><span data-stu-id="83d03-173">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="83d03-174">Verwalten von Netzwerkkontingenten</span><span class="sxs-lookup"><span data-stu-id="83d03-174">Management of network quotas</span></span>
- <span data-ttu-id="83d03-175">Anzeigen zugeordneter Netzwerkressourcen (beispielsweise öffentliche IP-Adressen, virtuelle Netzwerke oder Lastenausgleichsmodule)</span><span class="sxs-lookup"><span data-stu-id="83d03-175">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="83d03-176">Stellt ein Cmdlet zum Anzeigen einer Administratorübersicht bereit.</span><span class="sxs-lookup"><span data-stu-id="83d03-176">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="83d03-177">Speicher</span><span class="sxs-lookup"><span data-stu-id="83d03-177">Storage</span></span>
<span data-ttu-id="83d03-178">Vorschauversion des Storage-Administratormoduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="83d03-178">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="83d03-179">Dieses Release bietet Funktionen für Folgendes:</span><span class="sxs-lookup"><span data-stu-id="83d03-179">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="83d03-180">Verwalten von Speicherkontingenten</span><span class="sxs-lookup"><span data-stu-id="83d03-180">Manage storage quotas</span></span>
- <span data-ttu-id="83d03-181">Durchführen der Garbage Collection für gelöschte Speicherressourcen</span><span class="sxs-lookup"><span data-stu-id="83d03-181">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="83d03-182">Wiederherstellen gelöschter Speicherkonten</span><span class="sxs-lookup"><span data-stu-id="83d03-182">Restore deleted storage accounts</span></span>
- <span data-ttu-id="83d03-183">Migrieren von Containern zwischen Freigaben</span><span class="sxs-lookup"><span data-stu-id="83d03-183">Migrate containers from one share to another</span></span>
- <span data-ttu-id="83d03-184">Anzeigen von Informationen zu den einzelnen Speicherkomponenten</span><span class="sxs-lookup"><span data-stu-id="83d03-184">View information about the individual storage components</span></span>
- <span data-ttu-id="83d03-185">Anzeigen von Nutzungs- und Leistungsinformationen</span><span class="sxs-lookup"><span data-stu-id="83d03-185">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="83d03-186">Abonnementadministrator</span><span class="sxs-lookup"><span data-stu-id="83d03-186">Subscription Admin</span></span>
<span data-ttu-id="83d03-187">Vorschauversion des Subscription-Administratormoduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="83d03-187">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="83d03-188">Dieses Modul bietet Administratorfunktionen für Folgendes:</span><span class="sxs-lookup"><span data-stu-id="83d03-188">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="83d03-189">Verwalten von Plänen und Angeboten</span><span class="sxs-lookup"><span data-stu-id="83d03-189">Manage plans and offers</span></span>
- <span data-ttu-id="83d03-190">Anzeigen von Nutzungs- und Leistungsinformationen</span><span class="sxs-lookup"><span data-stu-id="83d03-190">View usage and performance information</span></span>
- <span data-ttu-id="83d03-191">Verwalten der RBAC</span><span class="sxs-lookup"><span data-stu-id="83d03-191">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="83d03-192">Abonnement</span><span class="sxs-lookup"><span data-stu-id="83d03-192">Subscription</span></span>
<span data-ttu-id="83d03-193">Vorschauversion des Subscription-Moduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="83d03-193">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="83d03-194">Dieses Modul bietet Benutzerfunktionen für Folgendes:</span><span class="sxs-lookup"><span data-stu-id="83d03-194">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="83d03-195">Erstellen, Löschen und Aktualisieren von Abonnements</span><span class="sxs-lookup"><span data-stu-id="83d03-195">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="83d03-196">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="83d03-196">Update</span></span>
<span data-ttu-id="83d03-197">Vorschauversion des Update-Administratormoduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="83d03-197">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="83d03-198">Dieses Modul ermöglicht Administratoren Folgendes:</span><span class="sxs-lookup"><span data-stu-id="83d03-198">In this module administrators can:</span></span>
- <span data-ttu-id="83d03-199">Auflisten und Installieren verfügbarer Updates</span><span class="sxs-lookup"><span data-stu-id="83d03-199">List and install available updates</span></span>
- <span data-ttu-id="83d03-200">Fortsetzen unterbrochener Updates</span><span class="sxs-lookup"><span data-stu-id="83d03-200">Resume interrupted updates</span></span>
- <span data-ttu-id="83d03-201">Anzeigen installierter Updates</span><span class="sxs-lookup"><span data-stu-id="83d03-201">View installed updates</span></span>
