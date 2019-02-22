---
title: Übersicht über Azure Stack PowerShell | Microsoft-Dokumentation
description: Enthält eine Übersicht über Azure Stack PowerShell und eine Anleitung zur Installation und Konfiguration.
author: bganapa
ms.author: bganapa
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 09/21/2018
ms.openlocfilehash: cd415e862bfaa2b767cce108689ebaf34ef74305
ms.sourcegitcommit: 2054a8f74cd9bf5a50ea7fdfddccaa632c842934
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "56144750"
---
# <a name="azurerm-module-230"></a><span data-ttu-id="b2b00-103">AzureRM-Modul 2.3.0</span><span class="sxs-lookup"><span data-stu-id="b2b00-103">AzureRM Module 2.3.0</span></span>

## <a name="requirements"></a><span data-ttu-id="b2b00-104">Anforderungen:</span><span class="sxs-lookup"><span data-stu-id="b2b00-104">Requirements:</span></span>
<span data-ttu-id="b2b00-105">Die niedrigste unterstützte Azure Stack-Version ist 1808.</span><span class="sxs-lookup"><span data-stu-id="b2b00-105">Minimum supported Azure Stack version is 1808.</span></span>

<span data-ttu-id="b2b00-106">Hinweis: Falls Sie eine niedrigere Version verwenden, sollten Sie Version 1.2.11 installieren.</span><span class="sxs-lookup"><span data-stu-id="b2b00-106">Note: If you are using an earlier version install version 1.2.11</span></span>


## <a name="install"></a><span data-ttu-id="b2b00-107">Installieren</span><span class="sxs-lookup"><span data-stu-id="b2b00-107">Install</span></span>
```powershell-interactive
# Remove previous versions of AzureStack modules
Uninstall-Module -Name AzureStack -Force 
Uninstall-Module -Name AzureRM -Force 
Uninstall-Module AzureRM.AzureStackAdmin -Force -ErrorAction Continue
Uninstall-Module AzureRM.AzureStackStorage -Force -ErrorAction Continue
Get-Module Azs.* -ListAvailable | Uninstall-Module -Force
Get-Module Azure.* -ListAvailable | Uninstall-Module -Force


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2018-03-01-hybrid -Force

```

## <a name="release-notes"></a><span data-ttu-id="b2b00-108">Versionsinformationen</span><span class="sxs-lookup"><span data-stu-id="b2b00-108">Release Notes</span></span>
* <span data-ttu-id="b2b00-109">Das Release 2.3.0 verfügt über eine Liste mit Breaking Changes.</span><span class="sxs-lookup"><span data-stu-id="b2b00-109">The release 2.3.0 comes with a list of breaking changes.</span></span> <span data-ttu-id="b2b00-110">Für das Upgrade von Version 1.2.11 haben wir unter https://aka.ms/azspowershellmigration einen Migrationsleitfaden erstellt.</span><span class="sxs-lookup"><span data-stu-id="b2b00-110">To upgrade from the 1.2.11 version, we have created a migration guide at https://aka.ms/azspowershellmigration</span></span>
* <span data-ttu-id="b2b00-111">Dieses Release entspricht dem Azure Stack-spezifischen API-Profil 2018-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="b2b00-111">This release corresponds to the azurestack specific api profile 2018-03-01-hybrid</span></span>
* <span data-ttu-id="b2b00-112">Alle Module sind mindestens vom AzureRm.Profile-Modul abhängig.</span><span class="sxs-lookup"><span data-stu-id="b2b00-112">All the modules are taking greater than or equal to dependency on the AzureRm.Profile module.</span></span>
* <span data-ttu-id="b2b00-113">Die von den einzelnen Modulen unterstützten API-Versionen werden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="b2b00-113">Api version suppoerted by  each of the modules are updated.</span></span> 
    * <span data-ttu-id="b2b00-114">Compute – 2017-03-30</span><span class="sxs-lookup"><span data-stu-id="b2b00-114">Compute - 2017-03-30</span></span>
    * <span data-ttu-id="b2b00-115">Netzwerk – 2017-10-01</span><span class="sxs-lookup"><span data-stu-id="b2b00-115">Network - 2017-10-01</span></span>
    * <span data-ttu-id="b2b00-116">Storage – 2016-01-01</span><span class="sxs-lookup"><span data-stu-id="b2b00-116">Storage - 2016-01-01</span></span>
    * <span data-ttu-id="b2b00-117">Ressourcen – 2018-02-01</span><span class="sxs-lookup"><span data-stu-id="b2b00-117">Resources - 2018-02-01</span></span>
    * <span data-ttu-id="b2b00-118">Key Vault – 2016-10-01</span><span class="sxs-lookup"><span data-stu-id="b2b00-118">Keyvault - 2016-10-01</span></span>
    * <span data-ttu-id="b2b00-119">DNS – 2016-04-01</span><span class="sxs-lookup"><span data-stu-id="b2b00-119">Dns - 2016-04-01</span></span>
* <span data-ttu-id="b2b00-120">Die vollständige Zuordnung aller API-Versionen für die einzelnen Ressourcentypen finden Sie unter https://github.com/Azure/azure-rest-api-specs/blob/master/profile/2018-03-01-hybrid.json.</span><span class="sxs-lookup"><span data-stu-id="b2b00-120">The complete api version map for each of the resource types can be found at https://github.com/Azure/azure-rest-api-specs/blob/master/profile/2018-03-01-hybrid.json</span></span>

## <a name="content"></a><span data-ttu-id="b2b00-121">Inhalt:</span><span class="sxs-lookup"><span data-stu-id="b2b00-121">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="b2b00-122">Azure-Bridge</span><span class="sxs-lookup"><span data-stu-id="b2b00-122">Azure Bridge</span></span>
<span data-ttu-id="b2b00-123">Vorschauversion des AzureBridge-Administratormoduls von Azure Stack, mit dem Sie Images aus Azure syndizieren können.</span><span class="sxs-lookup"><span data-stu-id="b2b00-123">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="b2b00-124">Backup</span><span class="sxs-lookup"><span data-stu-id="b2b00-124">Backup</span></span>
<span data-ttu-id="b2b00-125">Vorschauversion des Backup-Administratormoduls, das Administratoren Folgendes ermöglicht:</span><span class="sxs-lookup"><span data-stu-id="b2b00-125">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="b2b00-126">Konfigurieren des Speicherorts von Sicherungen</span><span class="sxs-lookup"><span data-stu-id="b2b00-126">Configure where backups are stored</span></span>
- <span data-ttu-id="b2b00-127">Durchführen von Sicherungen</span><span class="sxs-lookup"><span data-stu-id="b2b00-127">Perform backups</span></span>
- <span data-ttu-id="b2b00-128">Auflisten und Wiederherstellen abgeschlossener Sicherungen</span><span class="sxs-lookup"><span data-stu-id="b2b00-128">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="b2b00-129">Commerce</span><span class="sxs-lookup"><span data-stu-id="b2b00-129">Commerce</span></span>
<span data-ttu-id="b2b00-130">Vorschauversion des Commerce-Administratormoduls von Azure Stack, mit dem die aggregierte Datennutzung für das gesamte Azure Stack-System angezeigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="b2b00-130">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="b2b00-131">Compute</span><span class="sxs-lookup"><span data-stu-id="b2b00-131">Compute</span></span>
<span data-ttu-id="b2b00-132">Vorschauversion des Compute-Administratormoduls von Azure Stack mit Funktionen zur Verwaltung von Computekontingenten, Plattformimages, verwalteten Datenträgern und VM-Erweiterungen.</span><span class="sxs-lookup"><span data-stu-id="b2b00-132">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, managed disks and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="b2b00-133">Fabric</span><span class="sxs-lookup"><span data-stu-id="b2b00-133">Fabric</span></span>
<span data-ttu-id="b2b00-134">Vorschauversion des Fabric-Administratormoduls von Azure Stack, mit dem Administratoren Infrastrukturkomponenten anzeigen und verwalten können:</span><span class="sxs-lookup"><span data-stu-id="b2b00-134">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="b2b00-135">Beenden, Starten und Herunterfahren von Skalierungseinheitknoten</span><span class="sxs-lookup"><span data-stu-id="b2b00-135">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="b2b00-136">Entladen und Fortsetzen von Skalierungseinheitknoten für FRU-bezogene Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="b2b00-136">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="b2b00-137">Reparieren von Skalierungseinheitknoten</span><span class="sxs-lookup"><span data-stu-id="b2b00-137">Repair of scale unit nodes</span></span>
- <span data-ttu-id="b2b00-138">Neustarten der Infrastrukturrolle</span><span class="sxs-lookup"><span data-stu-id="b2b00-138">Restart of Infrastructure role</span></span>
- <span data-ttu-id="b2b00-139">Beenden, Starten und Herunterfahren von Instanzen der Infrastrukturrolle</span><span class="sxs-lookup"><span data-stu-id="b2b00-139">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="b2b00-140">Erstellen neuer IP-Pools</span><span class="sxs-lookup"><span data-stu-id="b2b00-140">Create new IP Pools</span></span>


### <a name="gallery"></a><span data-ttu-id="b2b00-141">Gallery</span><span class="sxs-lookup"><span data-stu-id="b2b00-141">Gallery</span></span>
<span data-ttu-id="b2b00-142">Vorschauversion des Gallery-Administratormoduls von Azure Stack mit Funktionen zum Verwalten von Katalogelementen im Azure Stack-Marketplace.</span><span class="sxs-lookup"><span data-stu-id="b2b00-142">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="b2b00-143">Infrastructure Insights</span><span class="sxs-lookup"><span data-stu-id="b2b00-143">Infrastructure Insights</span></span>
<span data-ttu-id="b2b00-144">Vorschauversion des Infrastructure Insights-Administratormoduls, das Administratoren Folgendes ermöglicht:</span><span class="sxs-lookup"><span data-stu-id="b2b00-144">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="b2b00-145">Anzeigen der Integrität ihrer Azure Stack-Stempelressourcen</span><span class="sxs-lookup"><span data-stu-id="b2b00-145">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="b2b00-146">Anzeigen und Verwalten von Warnungen</span><span class="sxs-lookup"><span data-stu-id="b2b00-146">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="b2b00-147">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b2b00-147">KeyVault</span></span>
<span data-ttu-id="b2b00-148">Vorschauversion des KeyVault-Administratormoduls von Azure Stack, mit dem Administratoren KeyVault-Kontingente anzeigen können.</span><span class="sxs-lookup"><span data-stu-id="b2b00-148">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="b2b00-149">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b2b00-149">Network</span></span>
<span data-ttu-id="b2b00-150">Vorschauversion des Network-Administratormoduls, das Folgendes ermöglicht:</span><span class="sxs-lookup"><span data-stu-id="b2b00-150">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="b2b00-151">Verwalten von Netzwerkkontingenten</span><span class="sxs-lookup"><span data-stu-id="b2b00-151">Management of network quotas</span></span>
- <span data-ttu-id="b2b00-152">Anzeigen zugeordneter Netzwerkressourcen (beispielsweise öffentliche IP-Adressen, virtuelle Netzwerke oder Lastenausgleichsmodule)</span><span class="sxs-lookup"><span data-stu-id="b2b00-152">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="b2b00-153">Stellt ein Cmdlet zum Anzeigen einer Administratorübersicht bereit.</span><span class="sxs-lookup"><span data-stu-id="b2b00-153">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="b2b00-154">Storage</span><span class="sxs-lookup"><span data-stu-id="b2b00-154">Storage</span></span>
<span data-ttu-id="b2b00-155">Vorschauversion des Storage-Administratormoduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="b2b00-155">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="b2b00-156">Dieses Release bietet Funktionen für Folgendes:</span><span class="sxs-lookup"><span data-stu-id="b2b00-156">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="b2b00-157">Verwalten von Speicherkontingenten</span><span class="sxs-lookup"><span data-stu-id="b2b00-157">Manage storage quotas</span></span>
- <span data-ttu-id="b2b00-158">Durchführen der Garbage Collection für gelöschte Speicherressourcen</span><span class="sxs-lookup"><span data-stu-id="b2b00-158">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="b2b00-159">Wiederherstellen gelöschter Speicherkonten</span><span class="sxs-lookup"><span data-stu-id="b2b00-159">Restore deleted storage accounts</span></span>
- <span data-ttu-id="b2b00-160">Migrieren von Containern zwischen Freigaben</span><span class="sxs-lookup"><span data-stu-id="b2b00-160">Migrate containers from one share to another</span></span>
- <span data-ttu-id="b2b00-161">Anzeigen von Informationen zu den einzelnen Speicherkomponenten</span><span class="sxs-lookup"><span data-stu-id="b2b00-161">View information about the individual storage components</span></span>
- <span data-ttu-id="b2b00-162">Anzeigen von Nutzungs- und Leistungsinformationen</span><span class="sxs-lookup"><span data-stu-id="b2b00-162">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="b2b00-163">Abonnementadministrator</span><span class="sxs-lookup"><span data-stu-id="b2b00-163">Subscription Admin</span></span>
<span data-ttu-id="b2b00-164">Vorschauversion des Subscription-Administratormoduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="b2b00-164">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="b2b00-165">Dieses Modul bietet Administratorfunktionen für Folgendes:</span><span class="sxs-lookup"><span data-stu-id="b2b00-165">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="b2b00-166">Verwalten von Plänen und Angeboten</span><span class="sxs-lookup"><span data-stu-id="b2b00-166">Manage plans and offers</span></span>
- <span data-ttu-id="b2b00-167">Anzeigen von Nutzungs- und Leistungsinformationen</span><span class="sxs-lookup"><span data-stu-id="b2b00-167">View usage and performance information</span></span>
- <span data-ttu-id="b2b00-168">Verwalten der RBAC</span><span class="sxs-lookup"><span data-stu-id="b2b00-168">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="b2b00-169">Abonnement</span><span class="sxs-lookup"><span data-stu-id="b2b00-169">Subscription</span></span>
<span data-ttu-id="b2b00-170">Vorschauversion des Subscription-Moduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="b2b00-170">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="b2b00-171">Dieses Modul bietet Benutzerfunktionen für Folgendes:</span><span class="sxs-lookup"><span data-stu-id="b2b00-171">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="b2b00-172">Erstellen, Löschen und Aktualisieren von Abonnements</span><span class="sxs-lookup"><span data-stu-id="b2b00-172">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="b2b00-173">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b2b00-173">Update</span></span>
<span data-ttu-id="b2b00-174">Vorschauversion des Update-Administratormoduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="b2b00-174">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="b2b00-175">Dieses Modul ermöglicht Administratoren Folgendes:</span><span class="sxs-lookup"><span data-stu-id="b2b00-175">In this module administrators can:</span></span>
- <span data-ttu-id="b2b00-176">Auflisten und Installieren verfügbarer Updates</span><span class="sxs-lookup"><span data-stu-id="b2b00-176">List and install available updates</span></span>
- <span data-ttu-id="b2b00-177">Fortsetzen unterbrochener Updates</span><span class="sxs-lookup"><span data-stu-id="b2b00-177">Resume interrupted updates</span></span>
- <span data-ttu-id="b2b00-178">Anzeigen installierter Updates</span><span class="sxs-lookup"><span data-stu-id="b2b00-178">View installed updates</span></span>
