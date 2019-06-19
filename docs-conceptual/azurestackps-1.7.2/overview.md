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
ms.openlocfilehash: b77e09f6fcd5b7752af9f51a42d357db4f1b13db
ms.sourcegitcommit: febbbd3f75c8dd1a296281d265289f015b6cb537
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/12/2019
ms.locfileid: "67037672"
---
# <a name="azure-stack-module-172"></a>Azure Stack-Modul 1.7.2

## <a name="requirements"></a>Anforderungen:

Die niedrigste unterstützte Azure Stack-Version ist 1904.

Hinweis: Informationen zur Installation älterer Azure Stack-Versionen finden Sie unter [Installieren von PowerShell für Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell).

## <a name="install"></a>Installieren

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Install-Module -Name AzureRM -RequiredVersion 2.5.0

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.7.2
```

## <a name="release-notes"></a>Versionsinformationen

* Wird mit dem 1904-Update unterstützt
* Hierbei handelt es sich um eine Version mit grundlegenden Änderungen (Breaking Changes). Details zu Breaking Changes finden Sie unter <https://aka.ms/azspshmigration170>.
* Wichtige Änderung: Änderungen am zertifikatbasierten Verschlüsselungsmodus werden gesichert. Unterstützung für symmetrische Schlüssel ist veraltet.
* Details zu Breaking Changes finden Sie unter https://aka.ms/azspshmigration170.
* Azs.Storage.Admin Module 
* Fehlerbehebung: Neues Speicherplatzkontingent verwendet Standardwerte, wenn keine angegeben werden.
