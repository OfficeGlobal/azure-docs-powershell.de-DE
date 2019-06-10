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
# <a name="azure-stack-module-172"></a>Azure Stack-Modul 1.7.2

## <a name="requirements"></a>Anforderungen:

Die niedrigste unterstützte Azure Stack-Version ist 1904.

Hinweis: Informationen zur Installation älterer Azure Stack-Versionen finden Sie unter [Installieren von PowerShell für Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell).

## <a name="install-powershell-for-azure-stack"></a>Installieren von PowerShell für Azure Stack

Die Installation umfasst drei Schritte:

1. Installieren der Azure Stack PowerShell, abhängig von Ihrer Version von Azure Stack
2. Aktivieren zusätzlicher Speicherfunktionen
3. Bestätigen der Installation der PowerShell

### <a name="install-azure-stack-powershell"></a>Installieren von Azure Stack-PowerShell

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

### <a name="enable-additional-storage-features"></a>Aktivieren zusätzlicher Speicherfunktionen

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

## <a name="release-notes"></a>Versionsinformationen

* Wird mit dem 1904-Update unterstützt
* Hierbei handelt es sich um eine Version mit grundlegenden Änderungen (Breaking Changes). Details zu Breaking Changes finden Sie unter <https://aka.ms/azspshmigration170>.
* Azs.Backup.Admin Module * Breaking Change: Änderungen am zertifikatbasierten Verschlüsselungsmodus werden gesichert. Unterstützung für symmetrische Schlüssel ist veraltet.
* Azs.Fabric.Admin Module       * Eingestellte Unterstützung           * Get-AzsInfrastructureVolume ist veraltet; wir stellen ein neues Cmdlet bereit: Get-AzsVolume           * Get-AzsStorageSystem ist veraltet; wir stellen ein neues Cmdlet bereit: Get-AzsStorageSubSystem           * Get-AzsStoragePool ist veraltet; das StorageSubSystem-Objekt verfügt über die Kapazitätseigenschaft
* Azs.Compute.Admin-Modul           * BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : „ConvertTo-PlatformImageObject“ wird nur im Erfolgspfad aufgerufen.           * BugFix: Add-AzsVmExtension, Get-AzsVmExtension : „ConvertTo-VmExtensionObject“ wird nur im Erfolgspfad aufgerufen.
* Azs.Storage.Admin-Modul           * Bug fix - Neues Speicherplatzkontingent verwendet Standardwerte, wenn keine angegeben werden.'
