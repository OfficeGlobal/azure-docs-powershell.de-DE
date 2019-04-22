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
ms.openlocfilehash: 6568dc4e6c51e8f250aad2c4dd765c065fe6a8bf
ms.sourcegitcommit: ae4540a90508db73335a54408dfd6cdf3712a1e9
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/18/2019
ms.locfileid: "58808055"
---
# <a name="azure-stack-module-171"></a>Azure Stack-Modul 1.7.1

## <a name="requirements"></a>Anforderungen:

Die niedrigste unterstützte Azure Stack-Version ist 1901.

Hinweis: Informationen zur Installation älterer Azure Stack-Versionen finden Sie unter [Installieren von PowerShell für Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell).

## <a name="install"></a>Installieren

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Install-Module -Name AzureRM -RequiredVersion 2.4.0

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.7.1
```

## <a name="release-notes"></a>Versionsinformationen

* Wird mit dem 1901-Update unterstützt
* Hierbei handelt es sich um eine Version mit grundlegenden Änderungen (Breaking Changes). Details zu Breaking Changes finden Sie unter <https://aka.ms/azspshmigration170>.
* Azs.Backup.Admin Module * Breaking Change: Änderungen am zertifikatbasierten Verschlüsselungsmodus werden gesichert. Unterstützung für symmetrische Schlüssel ist veraltet.
* Azs.Fabric.Admin Module       * Eingestellte Unterstützung           * Get-AzsInfrastructureVolume ist veraltet; wir stellen ein neues Cmdlet bereit: Get-AzsVolume           * Get-AzsStorageSystem ist veraltet; wir stellen ein neues Cmdlet bereit: Get-AzsStorageSubSystem           * Get-AzsStoragePool ist veraltet; das StorageSubSystem-Objekt verfügt über die Kapazitätseigenschaft
* Azs.Compute.Admin-Modul           * BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : „ConvertTo-PlatformImageObject“ wird nur im Erfolgspfad aufgerufen.           * BugFix: Add-AzsVmExtension, Get-AzsVmExtension : „ConvertTo-VmExtensionObject“ wird nur im Erfolgspfad aufgerufen.
* Azs.Storage.Admin-Modul           * Bug fix - Neues Speicherplatzkontingent verwendet Standardwerte, wenn keine angegeben werden.'
