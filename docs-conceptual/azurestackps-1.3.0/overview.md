# <a name="azure-stack-module-130"></a><span data-ttu-id="8c0da-101">Azure Stack-Modul 1.3.0</span><span class="sxs-lookup"><span data-stu-id="8c0da-101">Azure Stack Module 1.3.0</span></span>

## <a name="requirements"></a><span data-ttu-id="8c0da-102">Anforderungen:</span><span class="sxs-lookup"><span data-stu-id="8c0da-102">Requirements:</span></span>
<span data-ttu-id="8c0da-103">Die niedrigste unterstützte Azure Stack-Version ist 1804.</span><span class="sxs-lookup"><span data-stu-id="8c0da-103">Minimum supported Azure Stack version is 1804.</span></span>

<span data-ttu-id="8c0da-104">Hinweis: Falls Sie eine niedrigere Version verwenden, installieren Sie die Version 1.2.11.</span><span class="sxs-lookup"><span data-stu-id="8c0da-104">Note: If you are using an earlier version install version 1.2.11</span></span>

## <a name="known-issues"></a><span data-ttu-id="8c0da-105">Bekannte Probleme:</span><span class="sxs-lookup"><span data-stu-id="8c0da-105">Known issues:</span></span>

- <span data-ttu-id="8c0da-106">Zum Schließen einer Warnung wird die Azure Stack-Version 1803 benötigt.</span><span class="sxs-lookup"><span data-stu-id="8c0da-106">Close Alert requires Azure Stack version 1803</span></span>
- <span data-ttu-id="8c0da-107">Bei einigen Storage-Cmdlets wird die Azure Stack-Version 1804 vorausgesetzt.</span><span class="sxs-lookup"><span data-stu-id="8c0da-107">Some Storage cmdlets do require Azure Stack version 1804</span></span>
- <span data-ttu-id="8c0da-108">Mit „New-AzsOffer“ können keine öffentlichen Angebote erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="8c0da-108">New-AzsOffer does not allow to create an offer with state public.</span></span> <span data-ttu-id="8c0da-109">Das Cmdlet „Set-AzsOffer“ muss hinterher aufgerufen werden, um den Zustand zu ändern.</span><span class="sxs-lookup"><span data-stu-id="8c0da-109">The Set-AzsOffer cmdlet needs to be called afterwards to change the state.</span></span>
- <span data-ttu-id="8c0da-110">Ein IP-Pool kann nicht ohne erneute Bereitstellung entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="8c0da-110">An IP Pool cannot be removed without a redeployment</span></span>

## <a name="breaking-changes"></a><span data-ttu-id="8c0da-111">Wichtige Änderungen</span><span class="sxs-lookup"><span data-stu-id="8c0da-111">Breaking Changes</span></span>
<span data-ttu-id="8c0da-112">Alle Breaking Changes, die aus der Version 1.2.11 migriert werden, sind hier dokumentiert: https://aka.ms/azspowershellmigration</span><span class="sxs-lookup"><span data-stu-id="8c0da-112">All breaking changes migrating from 1.2.11 are documented here https://aka.ms/azspowershellmigration</span></span>

## <a name="install"></a><span data-ttu-id="8c0da-113">Installieren</span><span class="sxs-lookup"><span data-stu-id="8c0da-113">Install</span></span>
```
# Remove previous Versions
Uninstall-Module AzureRM.AzureStackAdmin -Force
Uninstall-Module AzureRM.AzureStackStorage -Force
Uninstall-Module -Name AzureStack -Force 


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2017-03-09-profile -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.3.0
```
## <a name="content"></a><span data-ttu-id="8c0da-114">Inhalt:</span><span class="sxs-lookup"><span data-stu-id="8c0da-114">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="8c0da-115">Azure-Bridge</span><span class="sxs-lookup"><span data-stu-id="8c0da-115">Azure Bridge</span></span>
<span data-ttu-id="8c0da-116">Vorschauversion des AzureBridge-Administratormoduls von Azure Stack, mit dem Sie Images aus Azure syndizieren können.</span><span class="sxs-lookup"><span data-stu-id="8c0da-116">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="8c0da-117">Backup</span><span class="sxs-lookup"><span data-stu-id="8c0da-117">Backup</span></span>
<span data-ttu-id="8c0da-118">Vorschauversion des Backup-Administratormoduls, das Administratoren Folgendes ermöglicht:</span><span class="sxs-lookup"><span data-stu-id="8c0da-118">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="8c0da-119">Konfigurieren des Speicherorts von Sicherungen</span><span class="sxs-lookup"><span data-stu-id="8c0da-119">Configure where backups are stored</span></span>
- <span data-ttu-id="8c0da-120">Durchführen von Sicherungen</span><span class="sxs-lookup"><span data-stu-id="8c0da-120">Perform backups</span></span>
- <span data-ttu-id="8c0da-121">Auflisten und Wiederherstellen abgeschlossener Sicherungen</span><span class="sxs-lookup"><span data-stu-id="8c0da-121">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="8c0da-122">Commerce</span><span class="sxs-lookup"><span data-stu-id="8c0da-122">Commerce</span></span>
<span data-ttu-id="8c0da-123">Vorschauversion des Commerce-Administratormoduls von Azure Stack, mit dem die aggregierte Datennutzung für das gesamte Azure Stack-System angezeigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="8c0da-123">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="8c0da-124">Compute</span><span class="sxs-lookup"><span data-stu-id="8c0da-124">Compute</span></span>
<span data-ttu-id="8c0da-125">Vorschauversion des Compute-Administratormoduls von Azure Stack mit Funktionen zur Verwaltung von Computekontingenten, Plattformimages und VM-Erweiterungen.</span><span class="sxs-lookup"><span data-stu-id="8c0da-125">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="8c0da-126">Fabric</span><span class="sxs-lookup"><span data-stu-id="8c0da-126">Fabric</span></span>
<span data-ttu-id="8c0da-127">Vorschauversion des Fabric-Administratormoduls von Azure Stack, mit dem Administratoren Infrastrukturkomponenten anzeigen und verwalten können:</span><span class="sxs-lookup"><span data-stu-id="8c0da-127">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="8c0da-128">Beenden, Starten und Herunterfahren von Skalierungseinheitknoten</span><span class="sxs-lookup"><span data-stu-id="8c0da-128">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="8c0da-129">Entladen und Fortsetzen von Skalierungseinheitknoten für FRU-bezogene Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="8c0da-129">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="8c0da-130">Reparieren von Skalierungseinheitknoten</span><span class="sxs-lookup"><span data-stu-id="8c0da-130">Repair of scale unit nodes</span></span>
- <span data-ttu-id="8c0da-131">Neustarten der Infrastrukturrolle</span><span class="sxs-lookup"><span data-stu-id="8c0da-131">Restart of Infrastructure role</span></span>
- <span data-ttu-id="8c0da-132">Beenden, Starten und Herunterfahren von Instanzen der Infrastrukturrolle</span><span class="sxs-lookup"><span data-stu-id="8c0da-132">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="8c0da-133">Erstellen neuer IP-Pools</span><span class="sxs-lookup"><span data-stu-id="8c0da-133">Create new IP Pools</span></span>


### <a name="gallery"></a><span data-ttu-id="8c0da-134">Gallery</span><span class="sxs-lookup"><span data-stu-id="8c0da-134">Gallery</span></span>
<span data-ttu-id="8c0da-135">Vorschauversion des Gallery-Administratormoduls von Azure Stack mit Funktionen zum Verwalten von Katalogelementen im Azure Stack-Marketplace.</span><span class="sxs-lookup"><span data-stu-id="8c0da-135">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="8c0da-136">Infrastructure Insights</span><span class="sxs-lookup"><span data-stu-id="8c0da-136">Infrastructure Insights</span></span>
<span data-ttu-id="8c0da-137">Vorschauversion des Infrastructure Insights-Administratormoduls, das Administratoren Folgendes ermöglicht:</span><span class="sxs-lookup"><span data-stu-id="8c0da-137">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="8c0da-138">Anzeigen der Integrität ihrer Azure Stack-Stempelressourcen</span><span class="sxs-lookup"><span data-stu-id="8c0da-138">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="8c0da-139">Anzeigen und Verwalten von Warnungen</span><span class="sxs-lookup"><span data-stu-id="8c0da-139">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="8c0da-140">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8c0da-140">KeyVault</span></span>
<span data-ttu-id="8c0da-141">Vorschauversion des KeyVault-Administratormoduls von Azure Stack, mit dem Administratoren KeyVault-Kontingente anzeigen können.</span><span class="sxs-lookup"><span data-stu-id="8c0da-141">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="8c0da-142">Network</span><span class="sxs-lookup"><span data-stu-id="8c0da-142">Network</span></span>
<span data-ttu-id="8c0da-143">Vorschauversion des Network-Administratormoduls, das Folgendes ermöglicht:</span><span class="sxs-lookup"><span data-stu-id="8c0da-143">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="8c0da-144">Verwalten von Netzwerkkontingenten</span><span class="sxs-lookup"><span data-stu-id="8c0da-144">Management of network quotas</span></span>
- <span data-ttu-id="8c0da-145">Anzeigen zugeordneter Netzwerkressourcen (beispielsweise öffentliche IP-Adressen, virtuelle Netzwerke oder Lastenausgleichsmodule)</span><span class="sxs-lookup"><span data-stu-id="8c0da-145">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="8c0da-146">Stellt ein Cmdlet zum Anzeigen einer Administratorübersicht bereit.</span><span class="sxs-lookup"><span data-stu-id="8c0da-146">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="8c0da-147">Storage</span><span class="sxs-lookup"><span data-stu-id="8c0da-147">Storage</span></span>
<span data-ttu-id="8c0da-148">Vorschauversion des Storage-Administratormoduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8c0da-148">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="8c0da-149">Dieses Release bietet Funktionen für Folgendes:</span><span class="sxs-lookup"><span data-stu-id="8c0da-149">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="8c0da-150">Verwalten von Speicherkontingenten</span><span class="sxs-lookup"><span data-stu-id="8c0da-150">Manage storage quotas</span></span>
- <span data-ttu-id="8c0da-151">Durchführen der Garbage Collection für gelöschte Speicherressourcen</span><span class="sxs-lookup"><span data-stu-id="8c0da-151">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="8c0da-152">Wiederherstellen gelöschter Speicherkonten</span><span class="sxs-lookup"><span data-stu-id="8c0da-152">Restore deleted storage accounts</span></span>
- <span data-ttu-id="8c0da-153">Migrieren von Containern zwischen Freigaben</span><span class="sxs-lookup"><span data-stu-id="8c0da-153">Migrate containers from one share to another</span></span>
- <span data-ttu-id="8c0da-154">Anzeigen von Informationen zu den einzelnen Speicherkomponenten</span><span class="sxs-lookup"><span data-stu-id="8c0da-154">View information about the individual storage components</span></span>
- <span data-ttu-id="8c0da-155">Anzeigen von Nutzungs- und Leistungsinformationen</span><span class="sxs-lookup"><span data-stu-id="8c0da-155">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="8c0da-156">Abonnementadministrator</span><span class="sxs-lookup"><span data-stu-id="8c0da-156">Subscription Admin</span></span>
<span data-ttu-id="8c0da-157">Vorschauversion des Subscription-Administratormoduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8c0da-157">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="8c0da-158">Dieses Modul bietet Administratorfunktionen für Folgendes:</span><span class="sxs-lookup"><span data-stu-id="8c0da-158">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="8c0da-159">Verwalten von Plänen und Angeboten</span><span class="sxs-lookup"><span data-stu-id="8c0da-159">Manage plans and offers</span></span>
- <span data-ttu-id="8c0da-160">Anzeigen von Nutzungs- und Leistungsinformationen</span><span class="sxs-lookup"><span data-stu-id="8c0da-160">View usage and performance information</span></span>
- <span data-ttu-id="8c0da-161">Verwalten der RBAC</span><span class="sxs-lookup"><span data-stu-id="8c0da-161">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="8c0da-162">Subscription</span><span class="sxs-lookup"><span data-stu-id="8c0da-162">Subscription</span></span>
<span data-ttu-id="8c0da-163">Vorschauversion des Subscription-Moduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8c0da-163">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="8c0da-164">Dieses Modul bietet Benutzerfunktionen für Folgendes:</span><span class="sxs-lookup"><span data-stu-id="8c0da-164">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="8c0da-165">Erstellen, Löschen und Aktualisieren von Abonnements</span><span class="sxs-lookup"><span data-stu-id="8c0da-165">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="8c0da-166">Update</span><span class="sxs-lookup"><span data-stu-id="8c0da-166">Update</span></span>
<span data-ttu-id="8c0da-167">Vorschauversion des Update-Administratormoduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8c0da-167">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="8c0da-168">Dieses Modul ermöglicht Administratoren Folgendes:</span><span class="sxs-lookup"><span data-stu-id="8c0da-168">In this module administrators can:</span></span>
- <span data-ttu-id="8c0da-169">Auflisten und Installieren verfügbarer Updates</span><span class="sxs-lookup"><span data-stu-id="8c0da-169">List and install available updates</span></span>
- <span data-ttu-id="8c0da-170">Fortsetzen unterbrochener Updates</span><span class="sxs-lookup"><span data-stu-id="8c0da-170">Resume interrupted updates</span></span>
- <span data-ttu-id="8c0da-171">Anzeigen installierter Updates</span><span class="sxs-lookup"><span data-stu-id="8c0da-171">View installed updates</span></span>
