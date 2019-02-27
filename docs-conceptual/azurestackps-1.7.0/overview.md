---
title: Übersicht über Azure Stack PowerShell mit Administratorrechten | Microsoft-Dokumentation
description: Enthält eine Übersicht über Azure Stack PowerShell mit Administratorrechten und eine Anleitung zur Installation und Konfiguration.
author: sijuman
ms.author: sijuman
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 02/06/2019
ms.openlocfilehash: af34497f243ce8f4f718e88312f6ad54eb6ad848
ms.sourcegitcommit: 993db64e68b222acbcfdeef2e81eb3316b160858
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/14/2019
ms.locfileid: "56240518"
---
# <a name="azure-stack-module-170"></a><span data-ttu-id="ea8ec-103">Azure Stack-Modul 1.7.0</span><span class="sxs-lookup"><span data-stu-id="ea8ec-103">Azure Stack Module 1.7.0</span></span>

## <a name="requirements"></a><span data-ttu-id="ea8ec-104">Anforderungen:</span><span class="sxs-lookup"><span data-stu-id="ea8ec-104">Requirements:</span></span>
<span data-ttu-id="ea8ec-105">Die niedrigste unterstützte Azure Stack-Version ist 1901.</span><span class="sxs-lookup"><span data-stu-id="ea8ec-105">Minimum supported Azure Stack version is 1901.</span></span>

<span data-ttu-id="ea8ec-106">Hinweis: Falls Sie eine niedrigere Version verwenden, sollten Sie Version 1.7.0 installieren.</span><span class="sxs-lookup"><span data-stu-id="ea8ec-106">Note: If you are using an earlier version install version 1.7.0</span></span>

## <a name="install"></a><span data-ttu-id="ea8ec-107">Installieren</span><span class="sxs-lookup"><span data-stu-id="ea8ec-107">Install</span></span>
```
# Remove previous versions of AzureStack and AzureRM modules
Uninstall-Module -Name AzureRM -Force
Uninstall-Module -Name Azure.Storage -Force
Uninstall-Module -Name AzureStack -Force
Get-Module -Name "Azs*" -ListAvailable | Uninstall-Module  -Force 
Get-Module -Name "AzureRm*" -ListAvailable | Uninstall-Module  -Force

# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Install-Module AzureRM -RequiredVersion 2.4.0

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.7.0
```
## <a name="release-notes"></a><span data-ttu-id="ea8ec-108">Versionsinformationen</span><span class="sxs-lookup"><span data-stu-id="ea8ec-108">Release Notes</span></span>
* <span data-ttu-id="ea8ec-109">Wird mit dem 1901-Update unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea8ec-109">Supported with 1901 update</span></span>
* <span data-ttu-id="ea8ec-110">Hierbei handelt es sich um eine Version mit grundlegenden Änderungen (Breaking Changes).</span><span class="sxs-lookup"><span data-stu-id="ea8ec-110">This a breaking change release.</span></span> <span data-ttu-id="ea8ec-111">Details zu Breaking Changes finden Sie unter https://aka.ms/azspshmigration170.</span><span class="sxs-lookup"><span data-stu-id="ea8ec-111">For details on the breaking changes, refer to https://aka.ms/azspshmigration170</span></span>
* <span data-ttu-id="ea8ec-112">Azs.Backup.Admin Module \* Breaking Change: Änderungen am zertifikatbasierten Verschlüsselungsmodus werden gesichert.</span><span class="sxs-lookup"><span data-stu-id="ea8ec-112">Azs.Backup.Admin Module \* Breaking change: Backup changes to cert-based encryption mode.</span></span> <span data-ttu-id="ea8ec-113">Unterstützung für symmetrische Schlüssel ist veraltet.</span><span class="sxs-lookup"><span data-stu-id="ea8ec-113">Support for symmetric keys is deprecated.</span></span>
* <span data-ttu-id="ea8ec-114">Azs.Fabric.Admin Module       \* Eingestellte Unterstützung           \* Get-AzsInfrastructureVolume ist veraltet; wir stellen ein neues Cmdlet bereit: Get-AzsVolume           \* Get-AzsStorageSystem ist veraltet; wir stellen ein neues Cmdlet bereit: Get-AzsStorageSubSystem           \* Get-AzsStoragePool ist veraltet; das StorageSubSystem-Objekt verfügt über die Kapazitätseigenschaft</span><span class="sxs-lookup"><span data-stu-id="ea8ec-114">Azs.Fabric.Admin Module       \* Deprecation           \* Get-AzsInfrastructureVolume has been deprecated, we provide new cmdlet Get-AzsVolume           \* Get-AzsStorageSystem has been deprecated, we provide new cmdlet Get-AzsStorageSubSystem           \* Get-AzsStoragePool has been deprecated, the StorageSubSystem object has the capacity property</span></span>
* <span data-ttu-id="ea8ec-115">Azs.Compute.Admin-Modul           \* BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : „ConvertTo-PlatformImageObject“ wird nur im Erfolgspfad aufgerufen.           \* BugFix: Add-AzsVmExtension, Get-AzsVmExtension : „ConvertTo-VmExtensionObject“ wird nur im Erfolgspfad aufgerufen.</span><span class="sxs-lookup"><span data-stu-id="ea8ec-115">Azs.Compute.Admin Module           \* BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : Calling ConvertTo-PlatformImageObject only in the success path           \* BugFix: Add-AzsVmExtension, Get-AzsVmExtension : Calling ConvertTo-VmExtensionObject only in the success path</span></span>
* <span data-ttu-id="ea8ec-116">Azs.Storage.Admin-Modul           \* Bug fix - Neues Speicherplatzkontingent verwendet Standardwerte, wenn keine angegeben werden.'</span><span class="sxs-lookup"><span data-stu-id="ea8ec-116">Azs.Storage.Admin Module           \* Bug fix - New Storage Quota uses defaults if none provided.'</span></span>

