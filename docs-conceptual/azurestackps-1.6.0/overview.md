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
ms.openlocfilehash: b0e85bec82b9b7c876b2bbf337b603c8d68cf6a3
ms.sourcegitcommit: 2054a8f74cd9bf5a50ea7fdfddccaa632c842934
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "56153148"
---
# <a name="azure-stack-module-160"></a><span data-ttu-id="0affd-103">Azure Stack-Modul 1.6.0</span><span class="sxs-lookup"><span data-stu-id="0affd-103">Azure Stack Module 1.6.0</span></span>

## <a name="requirements"></a><span data-ttu-id="0affd-104">Anforderungen:</span><span class="sxs-lookup"><span data-stu-id="0affd-104">Requirements:</span></span>
<span data-ttu-id="0affd-105">Die niedrigste unterstützte Azure Stack-Version ist 1811.</span><span class="sxs-lookup"><span data-stu-id="0affd-105">Minimum supported Azure Stack version is 1811.</span></span>

<span data-ttu-id="0affd-106">Hinweis: Falls Sie eine niedrigere Version verwenden, sollten Sie Version 1.6.0 installieren.</span><span class="sxs-lookup"><span data-stu-id="0affd-106">Note: If you are using an earlier version install version 1.6.0</span></span>

## <a name="install"></a><span data-ttu-id="0affd-107">Installieren</span><span class="sxs-lookup"><span data-stu-id="0affd-107">Install</span></span>
```
# Remove previous versions of AzureStack and AzureRM modules
Uninstall-Module -Name AzureRM -Force
Uninstall-Module -Name Azure.Storage -Force
Uninstall-Module -Name AzureStack -Force
Get-Module -Name "Azs*" -ListAvailable | Uninstall-Module  -Force 
Get-Module -Name "AzureRm*" -ListAvailable | Uninstall-Module  -Force

# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2018-03-01-hybrid -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.6.0
```

## <a name="release-notes"></a><span data-ttu-id="0affd-108">Versionsinformationen</span><span class="sxs-lookup"><span data-stu-id="0affd-108">Release Notes</span></span>
* <span data-ttu-id="0affd-109">Wird mit dem 1811-Update unterstützt</span><span class="sxs-lookup"><span data-stu-id="0affd-109">Supported with 1811 update</span></span>
* <span data-ttu-id="0affd-110">Azs.Compute.Admin-Modul</span><span class="sxs-lookup"><span data-stu-id="0affd-110">Azs.Compute.Admin Module</span></span>
    * <span data-ttu-id="0affd-111">Fehlen des Azs-Präfix für „New-DataDiskObject“ korrigiert und Alias mit Warnung zur bevorstehenden Einstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0affd-111">Fixed missing Azs prefix for New-DataDiskObject and added alias with warning of future deprecation.</span></span>
* <span data-ttu-id="0affd-112">Azs.Update.Admin-Modul</span><span class="sxs-lookup"><span data-stu-id="0affd-112">Azs.Update.Admin Module</span></span>
    * <span data-ttu-id="0affd-113">Warnung hinzugefügt, um die Ausführung von „Test-AzureStack“ vor „Install-AzsUpdate“ zu empfehlen</span><span class="sxs-lookup"><span data-stu-id="0affd-113">Added a warning to recommend running Test-AzureStack before Install-AzsUpdate</span></span>
* <span data-ttu-id="0affd-114">Azs.Fabric.Admin</span><span class="sxs-lookup"><span data-stu-id="0affd-114">Azs.Fabric.Admin</span></span>
    * <span data-ttu-id="0affd-115">Neues Cmdlet (die Funktionen werden von Azure Stack 1811 und höher unterstützt)</span><span class="sxs-lookup"><span data-stu-id="0affd-115">New cmdlet (The features are supported by Azure Stack 1811+)</span></span>
        * <span data-ttu-id="0affd-116">Get-AzsDrive</span><span class="sxs-lookup"><span data-stu-id="0affd-116">Get-AzsDrive</span></span>
        * <span data-ttu-id="0affd-117">Get-AzsVolume</span><span class="sxs-lookup"><span data-stu-id="0affd-117">Get-AzsVolume</span></span>
        * <span data-ttu-id="0affd-118">Get-AzsStorageSubSystem</span><span class="sxs-lookup"><span data-stu-id="0affd-118">Get-AzsStorageSubSystem</span></span>
    * <span data-ttu-id="0affd-119">Eingestellte Unterstützung</span><span class="sxs-lookup"><span data-stu-id="0affd-119">Deprecation</span></span>
        * <span data-ttu-id="0affd-120">„Get-AzsInfrastructureVolume“ ist jetzt ein Alias für das Cmdlet „Get-AzsVolume“</span><span class="sxs-lookup"><span data-stu-id="0affd-120">Get-AzsInfrastructureVolume is an alias now to the cmdlet Get-AzsVolume</span></span>
* <span data-ttu-id="0affd-121">Azs.InfrastructureInsights.Admin</span><span class="sxs-lookup"><span data-stu-id="0affd-121">Azs.InfrastructureInsights.Admin</span></span>
    *  <span data-ttu-id="0affd-122">Neues Cmdlet „Repair-AzsAlert“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0affd-122">Added a new cmdlet Repair-AzsAlert</span></span>
* <span data-ttu-id="0affd-123">Azs.Storage.Admin</span><span class="sxs-lookup"><span data-stu-id="0affd-123">Azs.Storage.Admin</span></span>
    * <span data-ttu-id="0affd-124">Fehler behoben, aufgrund dessen Standardkontingentwerte nicht verwendet wurden</span><span class="sxs-lookup"><span data-stu-id="0affd-124">Bug fix where default quota values are not being used</span></span>
* <span data-ttu-id="0affd-125">Azs.Subscriptions.Admin-Modul</span><span class="sxs-lookup"><span data-stu-id="0affd-125">Azs.Subscriptions.Admin Module</span></span>
    * <span data-ttu-id="0affd-126">Fehlen des Azs-Präfix für „New-AddonPlanDefinitionObject“ korrigiert und Alias mit Warnung zur bevorstehenden Einstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0affd-126">Fixed missing Azs prefix for New-AddonPlanDefinitionObject and added alias with warning of future deprecation.</span></span>
