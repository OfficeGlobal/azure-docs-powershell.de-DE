# <a name="azure-stack-module-140"></a><span data-ttu-id="3eefd-101">Azure Stack-Modul 1.4.0</span><span class="sxs-lookup"><span data-stu-id="3eefd-101">Azure Stack Module 1.4.0</span></span>

## <a name="requirements"></a><span data-ttu-id="3eefd-102">Anforderungen:</span><span class="sxs-lookup"><span data-stu-id="3eefd-102">Requirements:</span></span>
<span data-ttu-id="3eefd-103">Die niedrigste unterstützte Azure Stack-Version ist 1804.</span><span class="sxs-lookup"><span data-stu-id="3eefd-103">Minimum supported Azure Stack version is 1804.</span></span>

<span data-ttu-id="3eefd-104">Hinweis: Falls Sie eine niedrigere Version verwenden, installieren Sie die Version 1.2.11.</span><span class="sxs-lookup"><span data-stu-id="3eefd-104">Note: If you are using an earlier version install version 1.2.11</span></span>

## <a name="known-issues"></a><span data-ttu-id="3eefd-105">Bekannte Probleme:</span><span class="sxs-lookup"><span data-stu-id="3eefd-105">Known issues:</span></span>

- <span data-ttu-id="3eefd-106">Zum Schließen einer Warnung wird die Azure Stack-Version 1803 benötigt.</span><span class="sxs-lookup"><span data-stu-id="3eefd-106">Close Alert requires Azure Stack version 1803</span></span>
- <span data-ttu-id="3eefd-107">Mit „New-AzsOffer“ können keine öffentlichen Angebote erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="3eefd-107">New-AzsOffer does not allow to create an offer with state public.</span></span> <span data-ttu-id="3eefd-108">Das Cmdlet „Set-AzsOffer“ muss hinterher aufgerufen werden, um den Zustand zu ändern.</span><span class="sxs-lookup"><span data-stu-id="3eefd-108">The Set-AzsOffer cmdlet needs to be called afterwards to change the state.</span></span>
- <span data-ttu-id="3eefd-109">Ein IP-Pool kann nicht ohne erneute Bereitstellung entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="3eefd-109">An IP Pool cannot be removed without a redeployment</span></span>

## <a name="breaking-changes"></a><span data-ttu-id="3eefd-110">Wichtige Änderungen</span><span class="sxs-lookup"><span data-stu-id="3eefd-110">Breaking Changes</span></span>
<span data-ttu-id="3eefd-111">Für die Folgeversion von Version 1.3.0 wurden keine Breaking Changes vorgenommen.</span><span class="sxs-lookup"><span data-stu-id="3eefd-111">There are no breaking changes from the version 1.3.0.</span></span> <span data-ttu-id="3eefd-112">Alle Breaking Changes, die aus der Version 1.2.11 migriert werden, sind hier dokumentiert: https://aka.ms/azspowershellmigration</span><span class="sxs-lookup"><span data-stu-id="3eefd-112">All breaking changes migrating from 1.2.11 are documented here https://aka.ms/azspowershellmigration</span></span>

## <a name="install"></a><span data-ttu-id="3eefd-113">Installieren</span><span class="sxs-lookup"><span data-stu-id="3eefd-113">Install</span></span>
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
## <a name="release-notes"></a><span data-ttu-id="3eefd-114">Versionsinformationen</span><span class="sxs-lookup"><span data-stu-id="3eefd-114">Release Notes</span></span>
    * <span data-ttu-id="3eefd-115">Zwischen der Vorgängerversion 1.3.0 und der Azure Stack-Version 1.4.0 wurden keine Breaking Changes eingeführt.</span><span class="sxs-lookup"><span data-stu-id="3eefd-115">Azurestack 1.4.0 version has no breaking changes from the previous release 1.3.0</span></span>
    * <span data-ttu-id="3eefd-116">Azs.AzureBridge.Admin</span><span class="sxs-lookup"><span data-stu-id="3eefd-116">Azs.AzureBridge.Admin</span></span>
        - <span data-ttu-id="3eefd-117">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="3eefd-117">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="3eefd-118">Azs.Backup.Admin</span><span class="sxs-lookup"><span data-stu-id="3eefd-118">Azs.Backup.Admin</span></span>
        - <span data-ttu-id="3eefd-119">Die neuen Parameter „BackupFrequencyInHours“, „IsBackupSchedulerEnabled“ und „BackupRetentionPeriodInDays“ wurden im Cmdlet „Set-AzsBackupShare“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="3eefd-119">Added new parameters BackupFrequencyInHours, IsBackupSchedulerEnabled, BackupRetentionPeriodInDays in cmdlet Set-AzsBackupShare</span></span>
        - <span data-ttu-id="3eefd-120">Cmdlet „New-EncyptionKeyBase64“ hinzugefügt, um die Erstellung eines Verschlüsselungsschlüssels zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="3eefd-120">Added a cmdlet New-EncyptionKeyBase64 to facilitate creating encryption key</span></span>
        - <span data-ttu-id="3eefd-121">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="3eefd-121">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="3eefd-122">Azs.Commerce.Admin</span><span class="sxs-lookup"><span data-stu-id="3eefd-122">Azs.Commerce.Admin</span></span>
        - <span data-ttu-id="3eefd-123">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="3eefd-123">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="3eefd-124">Azs.Fabric.Admin</span><span class="sxs-lookup"><span data-stu-id="3eefd-124">Azs.Fabric.Admin</span></span>
        - <span data-ttu-id="3eefd-125">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="3eefd-125">Fix for the bug that returned only a single page in paginated results</span></span>
        - <span data-ttu-id="3eefd-126">Cmdlet „Add-AzsScaleUnitNode“ hinzugefügt, um dem Administrator das Hinzufügen neuer Skalierungseinheitknoten azurestack-Stempel zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="3eefd-126">Added a cmdlet Add-AzsScaleUnitNode to enable admin to add new scale unit nodes to the azurestack stamp</span></span>
        - <span data-ttu-id="3eefd-127">Cmdlet „New-AzsScaleUnitNodeObject“ hinzugefügt, um die Erstellung von Skalierungseinheit-Parameterobjekten zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="3eefd-127">Added cmdlet and New-AzsScaleUnitNodeObject to facilitate the creation scale unit parameter objects</span></span>
    * <span data-ttu-id="3eefd-128">Azs.Gallery.Admin</span><span class="sxs-lookup"><span data-stu-id="3eefd-128">Azs.Gallery.Admin</span></span>
        - <span data-ttu-id="3eefd-129">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="3eefd-129">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="3eefd-130">Azs.InfrastructureInsights.Admin</span><span class="sxs-lookup"><span data-stu-id="3eefd-130">Azs.InfrastructureInsights.Admin</span></span>
        - <span data-ttu-id="3eefd-131">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="3eefd-131">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="3eefd-132">Azs.Network.Admin</span><span class="sxs-lookup"><span data-stu-id="3eefd-132">Azs.Network.Admin</span></span>
        - <span data-ttu-id="3eefd-133">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="3eefd-133">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="3eefd-134">Azs.Update.Admin</span><span class="sxs-lookup"><span data-stu-id="3eefd-134">Azs.Update.Admin</span></span>
        - <span data-ttu-id="3eefd-135">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="3eefd-135">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="3eefd-136">Azs.Subscriptions</span><span class="sxs-lookup"><span data-stu-id="3eefd-136">Azs.Subscriptions</span></span>
        - <span data-ttu-id="3eefd-137">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="3eefd-137">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="3eefd-138">Azs.Subscriptions.Admin</span><span class="sxs-lookup"><span data-stu-id="3eefd-138">Azs.Subscriptions.Admin</span></span>
        - <span data-ttu-id="3eefd-139">Cmdlet „Move-AzsSubscription“ hinzugefügt, um Abonnements zwischen Angeboten delegierter Anbieter zu verschieben</span><span class="sxs-lookup"><span data-stu-id="3eefd-139">Added a cmdlet Move-AzsSubscription to move subscriptions between delegated provider offers</span></span>
        - <span data-ttu-id="3eefd-140">Cmdlet „Test-AzsMoveSubscription“ hinzugefügt, um zu überprüfen, ob Benutzerabonnements zwischen Angeboten delegierter Anbieter verschoben werden können</span><span class="sxs-lookup"><span data-stu-id="3eefd-140">Added a cmdlet Test-AzsMoveSubscription to validate that user subscriptions can be moved between delegated provider offers</span></span>
        - <span data-ttu-id="3eefd-141">Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="3eefd-141">Fix for the bug that returned only a single page in paginated results'</span></span>

## <a name="content"></a><span data-ttu-id="3eefd-142">Inhalt:</span><span class="sxs-lookup"><span data-stu-id="3eefd-142">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="3eefd-143">Azure-Bridge</span><span class="sxs-lookup"><span data-stu-id="3eefd-143">Azure Bridge</span></span>
<span data-ttu-id="3eefd-144">Vorschauversion des AzureBridge-Administratormoduls von Azure Stack, mit dem Sie Images aus Azure syndizieren können.</span><span class="sxs-lookup"><span data-stu-id="3eefd-144">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="3eefd-145">Backup</span><span class="sxs-lookup"><span data-stu-id="3eefd-145">Backup</span></span>
<span data-ttu-id="3eefd-146">Vorschauversion des Backup-Administratormoduls, das Administratoren Folgendes ermöglicht:</span><span class="sxs-lookup"><span data-stu-id="3eefd-146">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="3eefd-147">Konfigurieren des Speicherorts von Sicherungen</span><span class="sxs-lookup"><span data-stu-id="3eefd-147">Configure where backups are stored</span></span>
- <span data-ttu-id="3eefd-148">Durchführen von Sicherungen</span><span class="sxs-lookup"><span data-stu-id="3eefd-148">Perform backups</span></span>
- <span data-ttu-id="3eefd-149">Auflisten und Wiederherstellen abgeschlossener Sicherungen</span><span class="sxs-lookup"><span data-stu-id="3eefd-149">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="3eefd-150">Commerce</span><span class="sxs-lookup"><span data-stu-id="3eefd-150">Commerce</span></span>
<span data-ttu-id="3eefd-151">Vorschauversion des Commerce-Administratormoduls von Azure Stack, mit dem die aggregierte Datennutzung für das gesamte Azure Stack-System angezeigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="3eefd-151">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="3eefd-152">Compute</span><span class="sxs-lookup"><span data-stu-id="3eefd-152">Compute</span></span>
<span data-ttu-id="3eefd-153">Vorschauversion des Compute-Administratormoduls von Azure Stack mit Funktionen zur Verwaltung von Computekontingenten, Plattformimages und VM-Erweiterungen.</span><span class="sxs-lookup"><span data-stu-id="3eefd-153">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="3eefd-154">Fabric</span><span class="sxs-lookup"><span data-stu-id="3eefd-154">Fabric</span></span>
<span data-ttu-id="3eefd-155">Vorschauversion des Fabric-Administratormoduls von Azure Stack, mit dem Administratoren Infrastrukturkomponenten anzeigen und verwalten können:</span><span class="sxs-lookup"><span data-stu-id="3eefd-155">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="3eefd-156">Beenden, Starten und Herunterfahren von Skalierungseinheitknoten</span><span class="sxs-lookup"><span data-stu-id="3eefd-156">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="3eefd-157">Entladen und Fortsetzen von Skalierungseinheitknoten für FRU-bezogene Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="3eefd-157">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="3eefd-158">Reparieren von Skalierungseinheitknoten</span><span class="sxs-lookup"><span data-stu-id="3eefd-158">Repair of scale unit nodes</span></span>
- <span data-ttu-id="3eefd-159">Neustarten der Infrastrukturrolle</span><span class="sxs-lookup"><span data-stu-id="3eefd-159">Restart of Infrastructure role</span></span>
- <span data-ttu-id="3eefd-160">Beenden, Starten und Herunterfahren von Instanzen der Infrastrukturrolle</span><span class="sxs-lookup"><span data-stu-id="3eefd-160">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="3eefd-161">Erstellen neuer IP-Pools</span><span class="sxs-lookup"><span data-stu-id="3eefd-161">Create new IP Pools</span></span>

### <a name="gallery"></a><span data-ttu-id="3eefd-162">Gallery</span><span class="sxs-lookup"><span data-stu-id="3eefd-162">Gallery</span></span>
<span data-ttu-id="3eefd-163">Vorschauversion des Gallery-Administratormoduls von Azure Stack mit Funktionen zum Verwalten von Katalogelementen im Azure Stack-Marketplace.</span><span class="sxs-lookup"><span data-stu-id="3eefd-163">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="3eefd-164">Infrastructure Insights</span><span class="sxs-lookup"><span data-stu-id="3eefd-164">Infrastructure Insights</span></span>
<span data-ttu-id="3eefd-165">Vorschauversion des Infrastructure Insights-Administratormoduls, das Administratoren Folgendes ermöglicht:</span><span class="sxs-lookup"><span data-stu-id="3eefd-165">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="3eefd-166">Anzeigen der Integrität ihrer Azure Stack-Stempelressourcen</span><span class="sxs-lookup"><span data-stu-id="3eefd-166">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="3eefd-167">Anzeigen und Verwalten von Warnungen</span><span class="sxs-lookup"><span data-stu-id="3eefd-167">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="3eefd-168">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3eefd-168">KeyVault</span></span>
<span data-ttu-id="3eefd-169">Vorschauversion des KeyVault-Administratormoduls von Azure Stack, mit dem Administratoren KeyVault-Kontingente anzeigen können.</span><span class="sxs-lookup"><span data-stu-id="3eefd-169">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="3eefd-170">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="3eefd-170">Network</span></span>
<span data-ttu-id="3eefd-171">Vorschauversion des Network-Administratormoduls, das Folgendes ermöglicht:</span><span class="sxs-lookup"><span data-stu-id="3eefd-171">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="3eefd-172">Verwalten von Netzwerkkontingenten</span><span class="sxs-lookup"><span data-stu-id="3eefd-172">Management of network quotas</span></span>
- <span data-ttu-id="3eefd-173">Anzeigen zugeordneter Netzwerkressourcen (beispielsweise öffentliche IP-Adressen, virtuelle Netzwerke oder Lastenausgleichsmodule)</span><span class="sxs-lookup"><span data-stu-id="3eefd-173">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="3eefd-174">Stellt ein Cmdlet zum Anzeigen einer Administratorübersicht bereit.</span><span class="sxs-lookup"><span data-stu-id="3eefd-174">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="3eefd-175">Speicher</span><span class="sxs-lookup"><span data-stu-id="3eefd-175">Storage</span></span>
<span data-ttu-id="3eefd-176">Vorschauversion des Storage-Administratormoduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="3eefd-176">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="3eefd-177">Dieses Release bietet Funktionen für Folgendes:</span><span class="sxs-lookup"><span data-stu-id="3eefd-177">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="3eefd-178">Verwalten von Speicherkontingenten</span><span class="sxs-lookup"><span data-stu-id="3eefd-178">Manage storage quotas</span></span>
- <span data-ttu-id="3eefd-179">Durchführen der Garbage Collection für gelöschte Speicherressourcen</span><span class="sxs-lookup"><span data-stu-id="3eefd-179">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="3eefd-180">Wiederherstellen gelöschter Speicherkonten</span><span class="sxs-lookup"><span data-stu-id="3eefd-180">Restore deleted storage accounts</span></span>
- <span data-ttu-id="3eefd-181">Migrieren von Containern zwischen Freigaben</span><span class="sxs-lookup"><span data-stu-id="3eefd-181">Migrate containers from one share to another</span></span>
- <span data-ttu-id="3eefd-182">Anzeigen von Informationen zu den einzelnen Speicherkomponenten</span><span class="sxs-lookup"><span data-stu-id="3eefd-182">View information about the individual storage components</span></span>
- <span data-ttu-id="3eefd-183">Anzeigen von Nutzungs- und Leistungsinformationen</span><span class="sxs-lookup"><span data-stu-id="3eefd-183">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="3eefd-184">Abonnementadministrator</span><span class="sxs-lookup"><span data-stu-id="3eefd-184">Subscription Admin</span></span>
<span data-ttu-id="3eefd-185">Vorschauversion des Subscription-Administratormoduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="3eefd-185">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="3eefd-186">Dieses Modul bietet Administratorfunktionen für Folgendes:</span><span class="sxs-lookup"><span data-stu-id="3eefd-186">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="3eefd-187">Verwalten von Plänen und Angeboten</span><span class="sxs-lookup"><span data-stu-id="3eefd-187">Manage plans and offers</span></span>
- <span data-ttu-id="3eefd-188">Anzeigen von Nutzungs- und Leistungsinformationen</span><span class="sxs-lookup"><span data-stu-id="3eefd-188">View usage and performance information</span></span>
- <span data-ttu-id="3eefd-189">Verwalten der RBAC</span><span class="sxs-lookup"><span data-stu-id="3eefd-189">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="3eefd-190">Abonnement</span><span class="sxs-lookup"><span data-stu-id="3eefd-190">Subscription</span></span>
<span data-ttu-id="3eefd-191">Vorschauversion des Subscription-Moduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="3eefd-191">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="3eefd-192">Dieses Modul bietet Benutzerfunktionen für Folgendes:</span><span class="sxs-lookup"><span data-stu-id="3eefd-192">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="3eefd-193">Erstellen, Löschen und Aktualisieren von Abonnements</span><span class="sxs-lookup"><span data-stu-id="3eefd-193">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="3eefd-194">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3eefd-194">Update</span></span>
<span data-ttu-id="3eefd-195">Vorschauversion des Update-Administratormoduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="3eefd-195">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="3eefd-196">Dieses Modul ermöglicht Administratoren Folgendes:</span><span class="sxs-lookup"><span data-stu-id="3eefd-196">In this module administrators can:</span></span>
- <span data-ttu-id="3eefd-197">Auflisten und Installieren verfügbarer Updates</span><span class="sxs-lookup"><span data-stu-id="3eefd-197">List and install available updates</span></span>
- <span data-ttu-id="3eefd-198">Fortsetzen unterbrochener Updates</span><span class="sxs-lookup"><span data-stu-id="3eefd-198">Resume interrupted updates</span></span>
- <span data-ttu-id="3eefd-199">Anzeigen installierter Updates</span><span class="sxs-lookup"><span data-stu-id="3eefd-199">View installed updates</span></span>
