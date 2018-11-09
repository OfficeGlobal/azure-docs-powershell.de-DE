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
ms.openlocfilehash: fb892daeafb1365ea62324392ac806cf9f3d39cf
ms.sourcegitcommit: 06f9206e025afa7207d4657c8f57c94ddb74817a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/07/2018
ms.locfileid: "51211977"
---
# <a name="azure-stack-module-130"></a><span data-ttu-id="72603-103">Azure Stack-Modul 1.3.0</span><span class="sxs-lookup"><span data-stu-id="72603-103">Azure Stack Module 1.3.0</span></span>

## <a name="requirements"></a><span data-ttu-id="72603-104">Anforderungen:</span><span class="sxs-lookup"><span data-stu-id="72603-104">Requirements:</span></span>
<span data-ttu-id="72603-105">Die niedrigste unterstützte Azure Stack-Version ist 1804.</span><span class="sxs-lookup"><span data-stu-id="72603-105">Minimum supported Azure Stack version is 1804.</span></span>

<span data-ttu-id="72603-106">Hinweis: Falls Sie eine niedrigere Version verwenden, installieren Sie die Version 1.2.11.</span><span class="sxs-lookup"><span data-stu-id="72603-106">Note: If you are using an earlier version install version 1.2.11</span></span>

## <a name="known-issues"></a><span data-ttu-id="72603-107">Bekannte Probleme:</span><span class="sxs-lookup"><span data-stu-id="72603-107">Known issues:</span></span>

- <span data-ttu-id="72603-108">Zum Schließen einer Warnung wird die Azure Stack-Version 1803 benötigt.</span><span class="sxs-lookup"><span data-stu-id="72603-108">Close Alert requires Azure Stack version 1803</span></span>
- <span data-ttu-id="72603-109">Bei einigen Storage-Cmdlets wird die Azure Stack-Version 1804 vorausgesetzt.</span><span class="sxs-lookup"><span data-stu-id="72603-109">Some Storage cmdlets do require Azure Stack version 1804</span></span>
- <span data-ttu-id="72603-110">Mit „New-AzsOffer“ können keine öffentlichen Angebote erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="72603-110">New-AzsOffer does not allow to create an offer with state public.</span></span> <span data-ttu-id="72603-111">Das Cmdlet „Set-AzsOffer“ muss hinterher aufgerufen werden, um den Zustand zu ändern.</span><span class="sxs-lookup"><span data-stu-id="72603-111">The Set-AzsOffer cmdlet needs to be called afterwards to change the state.</span></span>
- <span data-ttu-id="72603-112">Ein IP-Pool kann nicht ohne erneute Bereitstellung entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="72603-112">An IP Pool cannot be removed without a redeployment</span></span>

## <a name="breaking-changes"></a><span data-ttu-id="72603-113">Wichtige Änderungen</span><span class="sxs-lookup"><span data-stu-id="72603-113">Breaking Changes</span></span>
<span data-ttu-id="72603-114">Alle Breaking Changes, die aus der Version 1.2.11 migriert werden, sind hier dokumentiert: https://aka.ms/azspowershellmigration</span><span class="sxs-lookup"><span data-stu-id="72603-114">All breaking changes migrating from 1.2.11 are documented here https://aka.ms/azspowershellmigration</span></span>

## <a name="install"></a><span data-ttu-id="72603-115">Installieren</span><span class="sxs-lookup"><span data-stu-id="72603-115">Install</span></span>
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
## <a name="content"></a><span data-ttu-id="72603-116">Inhalt:</span><span class="sxs-lookup"><span data-stu-id="72603-116">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="72603-117">Azure-Bridge</span><span class="sxs-lookup"><span data-stu-id="72603-117">Azure Bridge</span></span>
<span data-ttu-id="72603-118">Vorschauversion des AzureBridge-Administratormoduls von Azure Stack, mit dem Sie Images aus Azure syndizieren können.</span><span class="sxs-lookup"><span data-stu-id="72603-118">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="72603-119">Backup</span><span class="sxs-lookup"><span data-stu-id="72603-119">Backup</span></span>
<span data-ttu-id="72603-120">Vorschauversion des Backup-Administratormoduls, das Administratoren Folgendes ermöglicht:</span><span class="sxs-lookup"><span data-stu-id="72603-120">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="72603-121">Konfigurieren des Speicherorts von Sicherungen</span><span class="sxs-lookup"><span data-stu-id="72603-121">Configure where backups are stored</span></span>
- <span data-ttu-id="72603-122">Durchführen von Sicherungen</span><span class="sxs-lookup"><span data-stu-id="72603-122">Perform backups</span></span>
- <span data-ttu-id="72603-123">Auflisten und Wiederherstellen abgeschlossener Sicherungen</span><span class="sxs-lookup"><span data-stu-id="72603-123">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="72603-124">Commerce</span><span class="sxs-lookup"><span data-stu-id="72603-124">Commerce</span></span>
<span data-ttu-id="72603-125">Vorschauversion des Commerce-Administratormoduls von Azure Stack, mit dem die aggregierte Datennutzung für das gesamte Azure Stack-System angezeigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="72603-125">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="72603-126">Compute</span><span class="sxs-lookup"><span data-stu-id="72603-126">Compute</span></span>
<span data-ttu-id="72603-127">Vorschauversion des Compute-Administratormoduls von Azure Stack mit Funktionen zur Verwaltung von Computekontingenten, Plattformimages und VM-Erweiterungen.</span><span class="sxs-lookup"><span data-stu-id="72603-127">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="72603-128">Fabric</span><span class="sxs-lookup"><span data-stu-id="72603-128">Fabric</span></span>
<span data-ttu-id="72603-129">Vorschauversion des Fabric-Administratormoduls von Azure Stack, mit dem Administratoren Infrastrukturkomponenten anzeigen und verwalten können:</span><span class="sxs-lookup"><span data-stu-id="72603-129">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="72603-130">Beenden, Starten und Herunterfahren von Skalierungseinheitknoten</span><span class="sxs-lookup"><span data-stu-id="72603-130">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="72603-131">Entladen und Fortsetzen von Skalierungseinheitknoten für FRU-bezogene Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="72603-131">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="72603-132">Reparieren von Skalierungseinheitknoten</span><span class="sxs-lookup"><span data-stu-id="72603-132">Repair of scale unit nodes</span></span>
- <span data-ttu-id="72603-133">Neustarten der Infrastrukturrolle</span><span class="sxs-lookup"><span data-stu-id="72603-133">Restart of Infrastructure role</span></span>
- <span data-ttu-id="72603-134">Beenden, Starten und Herunterfahren von Instanzen der Infrastrukturrolle</span><span class="sxs-lookup"><span data-stu-id="72603-134">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="72603-135">Erstellen neuer IP-Pools</span><span class="sxs-lookup"><span data-stu-id="72603-135">Create new IP Pools</span></span>


### <a name="gallery"></a><span data-ttu-id="72603-136">Gallery</span><span class="sxs-lookup"><span data-stu-id="72603-136">Gallery</span></span>
<span data-ttu-id="72603-137">Vorschauversion des Gallery-Administratormoduls von Azure Stack mit Funktionen zum Verwalten von Katalogelementen im Azure Stack-Marketplace.</span><span class="sxs-lookup"><span data-stu-id="72603-137">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="72603-138">Infrastructure Insights</span><span class="sxs-lookup"><span data-stu-id="72603-138">Infrastructure Insights</span></span>
<span data-ttu-id="72603-139">Vorschauversion des Infrastructure Insights-Administratormoduls, das Administratoren Folgendes ermöglicht:</span><span class="sxs-lookup"><span data-stu-id="72603-139">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="72603-140">Anzeigen der Integrität ihrer Azure Stack-Stempelressourcen</span><span class="sxs-lookup"><span data-stu-id="72603-140">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="72603-141">Anzeigen und Verwalten von Warnungen</span><span class="sxs-lookup"><span data-stu-id="72603-141">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="72603-142">KeyVault</span><span class="sxs-lookup"><span data-stu-id="72603-142">KeyVault</span></span>
<span data-ttu-id="72603-143">Vorschauversion des KeyVault-Administratormoduls von Azure Stack, mit dem Administratoren KeyVault-Kontingente anzeigen können.</span><span class="sxs-lookup"><span data-stu-id="72603-143">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="72603-144">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="72603-144">Network</span></span>
<span data-ttu-id="72603-145">Vorschauversion des Network-Administratormoduls, das Folgendes ermöglicht:</span><span class="sxs-lookup"><span data-stu-id="72603-145">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="72603-146">Verwalten von Netzwerkkontingenten</span><span class="sxs-lookup"><span data-stu-id="72603-146">Management of network quotas</span></span>
- <span data-ttu-id="72603-147">Anzeigen zugeordneter Netzwerkressourcen (beispielsweise öffentliche IP-Adressen, virtuelle Netzwerke oder Lastenausgleichsmodule)</span><span class="sxs-lookup"><span data-stu-id="72603-147">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="72603-148">Stellt ein Cmdlet zum Anzeigen einer Administratorübersicht bereit.</span><span class="sxs-lookup"><span data-stu-id="72603-148">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="72603-149">Speicher</span><span class="sxs-lookup"><span data-stu-id="72603-149">Storage</span></span>
<span data-ttu-id="72603-150">Vorschauversion des Storage-Administratormoduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="72603-150">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="72603-151">Dieses Release bietet Funktionen für Folgendes:</span><span class="sxs-lookup"><span data-stu-id="72603-151">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="72603-152">Verwalten von Speicherkontingenten</span><span class="sxs-lookup"><span data-stu-id="72603-152">Manage storage quotas</span></span>
- <span data-ttu-id="72603-153">Durchführen der Garbage Collection für gelöschte Speicherressourcen</span><span class="sxs-lookup"><span data-stu-id="72603-153">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="72603-154">Wiederherstellen gelöschter Speicherkonten</span><span class="sxs-lookup"><span data-stu-id="72603-154">Restore deleted storage accounts</span></span>
- <span data-ttu-id="72603-155">Migrieren von Containern zwischen Freigaben</span><span class="sxs-lookup"><span data-stu-id="72603-155">Migrate containers from one share to another</span></span>
- <span data-ttu-id="72603-156">Anzeigen von Informationen zu den einzelnen Speicherkomponenten</span><span class="sxs-lookup"><span data-stu-id="72603-156">View information about the individual storage components</span></span>
- <span data-ttu-id="72603-157">Anzeigen von Nutzungs- und Leistungsinformationen</span><span class="sxs-lookup"><span data-stu-id="72603-157">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="72603-158">Abonnementadministrator</span><span class="sxs-lookup"><span data-stu-id="72603-158">Subscription Admin</span></span>
<span data-ttu-id="72603-159">Vorschauversion des Subscription-Administratormoduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="72603-159">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="72603-160">Dieses Modul bietet Administratorfunktionen für Folgendes:</span><span class="sxs-lookup"><span data-stu-id="72603-160">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="72603-161">Verwalten von Plänen und Angeboten</span><span class="sxs-lookup"><span data-stu-id="72603-161">Manage plans and offers</span></span>
- <span data-ttu-id="72603-162">Anzeigen von Nutzungs- und Leistungsinformationen</span><span class="sxs-lookup"><span data-stu-id="72603-162">View usage and performance information</span></span>
- <span data-ttu-id="72603-163">Verwalten der RBAC</span><span class="sxs-lookup"><span data-stu-id="72603-163">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="72603-164">Abonnement</span><span class="sxs-lookup"><span data-stu-id="72603-164">Subscription</span></span>
<span data-ttu-id="72603-165">Vorschauversion des Subscription-Moduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="72603-165">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="72603-166">Dieses Modul bietet Benutzerfunktionen für Folgendes:</span><span class="sxs-lookup"><span data-stu-id="72603-166">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="72603-167">Erstellen, Löschen und Aktualisieren von Abonnements</span><span class="sxs-lookup"><span data-stu-id="72603-167">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="72603-168">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="72603-168">Update</span></span>
<span data-ttu-id="72603-169">Vorschauversion des Update-Administratormoduls von Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="72603-169">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="72603-170">Dieses Modul ermöglicht Administratoren Folgendes:</span><span class="sxs-lookup"><span data-stu-id="72603-170">In this module administrators can:</span></span>
- <span data-ttu-id="72603-171">Auflisten und Installieren verfügbarer Updates</span><span class="sxs-lookup"><span data-stu-id="72603-171">List and install available updates</span></span>
- <span data-ttu-id="72603-172">Fortsetzen unterbrochener Updates</span><span class="sxs-lookup"><span data-stu-id="72603-172">Resume interrupted updates</span></span>
- <span data-ttu-id="72603-173">Anzeigen installierter Updates</span><span class="sxs-lookup"><span data-stu-id="72603-173">View installed updates</span></span>
