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
ms.openlocfilehash: af0343e5ad92fa7f2b5c10e3e67cb7e10feb81c6
ms.sourcegitcommit: 0fdccb57a356b6e7c35a77b1f76e01fb96ef582b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/17/2019
ms.locfileid: "65855787"
---
# <a name="azure-stack-module-172"></a><span data-ttu-id="080c7-103">Azure Stack-Modul 1.7.2</span><span class="sxs-lookup"><span data-stu-id="080c7-103">Azure Stack Module 1.7.2</span></span>

## <a name="requirements"></a><span data-ttu-id="080c7-104">Anforderungen:</span><span class="sxs-lookup"><span data-stu-id="080c7-104">Requirements:</span></span>

<span data-ttu-id="080c7-105">Die niedrigste unterstützte Azure Stack-Version ist 1904.</span><span class="sxs-lookup"><span data-stu-id="080c7-105">Minimum supported Azure Stack version is 1904.</span></span>

<span data-ttu-id="080c7-106">Hinweis: Informationen zur Installation älterer Azure Stack-Versionen finden Sie unter [Installieren von PowerShell für Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell).</span><span class="sxs-lookup"><span data-stu-id="080c7-106">Note: For earlier versions of Azure Stack check [Install Azure Stack Powershell](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span></span>

## <a name="install-powershell-for-azure-stack"></a><span data-ttu-id="080c7-107">Installieren von PowerShell für Azure Stack</span><span class="sxs-lookup"><span data-stu-id="080c7-107">Install PowerShell for Azure Stack</span></span>

<span data-ttu-id="080c7-108">Die Installation umfasst drei Schritte:</span><span class="sxs-lookup"><span data-stu-id="080c7-108">Installation has three steps:</span></span>

1. <span data-ttu-id="080c7-109">Installieren der Azure Stack PowerShell, abhängig von Ihrer Version von Azure Stack</span><span class="sxs-lookup"><span data-stu-id="080c7-109">Install Azure Stack PowerShell depending on your version of Azure Stack</span></span>
2. <span data-ttu-id="080c7-110">Aktivieren zusätzlicher Speicherfunktionen</span><span class="sxs-lookup"><span data-stu-id="080c7-110">Enable additional storage features</span></span>
3. <span data-ttu-id="080c7-111">Bestätigen der Installation der PowerShell</span><span class="sxs-lookup"><span data-stu-id="080c7-111">Confirm the installation of PowerShell</span></span>

### <a name="install-azure-stack-powershell"></a><span data-ttu-id="080c7-112">Installieren von Azure Stack-PowerShell</span><span class="sxs-lookup"><span data-stu-id="080c7-112">Install Azure Stack PowerShell</span></span>

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install the AzureRM.BootStrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRM.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Get-AzureRmProfile -Update
Use-AzureRmProfile -Profile 2019-03-01-hybrid -Force
Install-Module -Name AzureStack -RequiredVersion 1.7.2
```

### <a name="enable-additional-storage-features"></a><span data-ttu-id="080c7-113">Aktivieren zusätzlicher Speicherfunktionen</span><span class="sxs-lookup"><span data-stu-id="080c7-113">Enable additional storage features</span></span>

```
# Install the Azure.Storage module version 4.5.0
Install-Module -Name Azure.Storage -RequiredVersion 4.5.0 -Force -AllowClobber

# Install the AzureRm.Storage module version 5.0.4
Install-Module -Name AzureRM.Storage -RequiredVersion 5.0.4 -Force -AllowClobber

# Remove incompatible storage module installed by AzureRM.Storage
Uninstall-Module Azure.Storage -RequiredVersion 4.6.1 -Force

# Load the modules explicitly specifying the versions
Import-Module -Name Azure.Storage -RequiredVersion 4.5.0
Import-Module -Name AzureRM.Storage -RequiredVersion 5.0.4
```

## <a name="release-notes"></a><span data-ttu-id="080c7-114">Versionsinformationen</span><span class="sxs-lookup"><span data-stu-id="080c7-114">Release Notes</span></span>

* <span data-ttu-id="080c7-115">Wird mit dem 1904-Update unterstützt</span><span class="sxs-lookup"><span data-stu-id="080c7-115">Supported with 1904 update</span></span>
* <span data-ttu-id="080c7-116">Hierbei handelt es sich um eine Version mit grundlegenden Änderungen (Breaking Changes).</span><span class="sxs-lookup"><span data-stu-id="080c7-116">This a breaking change release.</span></span> <span data-ttu-id="080c7-117">Details zu Breaking Changes finden Sie unter <https://aka.ms/azspshmigration170>.</span><span class="sxs-lookup"><span data-stu-id="080c7-117">For details on the breaking changes, refer to <https://aka.ms/azspshmigration170></span></span>
* <span data-ttu-id="080c7-118">Azs.Backup.Admin Module \* Breaking Change: Änderungen am zertifikatbasierten Verschlüsselungsmodus werden gesichert.</span><span class="sxs-lookup"><span data-stu-id="080c7-118">Azs.Backup.Admin Module \* Breaking change: Backup changes to cert-based encryption mode.</span></span> <span data-ttu-id="080c7-119">Unterstützung für symmetrische Schlüssel ist veraltet.</span><span class="sxs-lookup"><span data-stu-id="080c7-119">Support for symmetric keys is deprecated.</span></span>
* <span data-ttu-id="080c7-120">Azs.Fabric.Admin Module       \* Eingestellte Unterstützung           \* Get-AzsInfrastructureVolume ist veraltet; wir stellen ein neues Cmdlet bereit: Get-AzsVolume           \* Get-AzsStorageSystem ist veraltet; wir stellen ein neues Cmdlet bereit: Get-AzsStorageSubSystem           \* Get-AzsStoragePool ist veraltet; das StorageSubSystem-Objekt verfügt über die Kapazitätseigenschaft</span><span class="sxs-lookup"><span data-stu-id="080c7-120">Azs.Fabric.Admin Module       \* Deprecation           \* Get-AzsInfrastructureVolume has been deprecated, we provide new cmdlet Get-AzsVolume           \* Get-AzsStorageSystem has been deprecated, we provide new cmdlet Get-AzsStorageSubSystem           \* Get-AzsStoragePool has been deprecated, the StorageSubSystem object has the capacity property</span></span>
* <span data-ttu-id="080c7-121">Azs.Compute.Admin-Modul           \* BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : „ConvertTo-PlatformImageObject“ wird nur im Erfolgspfad aufgerufen.           \* BugFix: Add-AzsVmExtension, Get-AzsVmExtension : „ConvertTo-VmExtensionObject“ wird nur im Erfolgspfad aufgerufen.</span><span class="sxs-lookup"><span data-stu-id="080c7-121">Azs.Compute.Admin Module           \* BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : Calling ConvertTo-PlatformImageObject only in the success path           \* BugFix: Add-AzsVmExtension, Get-AzsVmExtension : Calling ConvertTo-VmExtensionObject only in the success path</span></span>
* <span data-ttu-id="080c7-122">Azs.Storage.Admin-Modul           \* Bug fix - Neues Speicherplatzkontingent verwendet Standardwerte, wenn keine angegeben werden.'</span><span class="sxs-lookup"><span data-stu-id="080c7-122">Azs.Storage.Admin Module           \* Bug fix - New Storage Quota uses defaults if none provided.'</span></span>
