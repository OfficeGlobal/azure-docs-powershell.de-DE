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
# <a name="azure-stack-module-170"></a>Azure Stack-Modul 1.7.0

## <a name="requirements"></a>Anforderungen:
Die niedrigste unterstützte Azure Stack-Version ist 1901.

Hinweis: Falls Sie eine niedrigere Version verwenden, sollten Sie Version 1.7.0 installieren.

## <a name="install"></a>Installieren
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
## <a name="release-notes"></a>Versionsinformationen
* Wird mit dem 1901-Update unterstützt
* Hierbei handelt es sich um eine Version mit grundlegenden Änderungen (Breaking Changes). Details zu Breaking Changes finden Sie unter https://aka.ms/azspshmigration170.
* Azs.Backup.Admin Module * Breaking Change: Änderungen am zertifikatbasierten Verschlüsselungsmodus werden gesichert. Unterstützung für symmetrische Schlüssel ist veraltet.
* Azs.Fabric.Admin Module       * Eingestellte Unterstützung           * Get-AzsInfrastructureVolume ist veraltet; wir stellen ein neues Cmdlet bereit: Get-AzsVolume           * Get-AzsStorageSystem ist veraltet; wir stellen ein neues Cmdlet bereit: Get-AzsStorageSubSystem           * Get-AzsStoragePool ist veraltet; das StorageSubSystem-Objekt verfügt über die Kapazitätseigenschaft
* Azs.Compute.Admin-Modul           * BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : „ConvertTo-PlatformImageObject“ wird nur im Erfolgspfad aufgerufen.           * BugFix: Add-AzsVmExtension, Get-AzsVmExtension : „ConvertTo-VmExtensionObject“ wird nur im Erfolgspfad aufgerufen.
* Azs.Storage.Admin-Modul           * Bug fix - Neues Speicherplatzkontingent verwendet Standardwerte, wenn keine angegeben werden.'

