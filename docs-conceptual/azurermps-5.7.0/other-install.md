---
title: Andere Installationsmöglichkeiten für Azure PowerShell
description: Installieren von Azure PowerShell ohne PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/20/2018
ms.openlocfilehash: 7c6446a66cd3ab9fe8f5d8adf13fed36ee093340
ms.sourcegitcommit: cb1fd248920d7efca67bd6c738a3b47206df7890
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/13/2018
ms.locfileid: "39025309"
---
# <a name="install-azure-powershell-on-windows-with-msi-or-web-platform-installer"></a>Installieren von Azure PowerShell unter Windows per MSI oder Webplattform-Installer

In diesem Artikel erfahren Sie, wie Sie Azure PowerShell unter Windows mit einem MSI-Paket oder mit dem Webplattform-Installer (WebPI) installieren.  
Verwenden Sie diese Installationsmethoden nur, wenn sie für Ihr System erforderlich sind. Die empfohlene Vorgehensweise zum Installieren von Azure PowerShell unter Windows ist die Verwendung von PowerShellGet. Eine Anleitung für die Installation von Azure PowerShell unter Verwendung von PowerShellGet finden Sie unter [Installieren von Azure PowerShell mit PowerShellGet](install-azurerm-ps.md).

Informationen zur Ausführung von Azure PowerShell in einem Docker-Container finden Sie unter [Run Azure PowerShell in a Docker container](azurerm-ps-in-docker.md) (Ausführen von Azure PowerShell in einem Docker-Container).

Informationen zur Installation in Linux- oder macOS-Umgebungen finden Sie unter [Installieren von Azure PowerShell unter macOS oder Linux](install-azurermps-maclinux.md).

## <a name="install-or-update-on-windows-using-the-msi-package"></a>Installieren oder Aktualisieren unter Windows mithilfe des MSI-Pakets

Azure PowerShell kann mithilfe der bei [GitHub](https://github.com/Azure/azure-powershell/releases/tag/v5.7.0-April2018) verfügbaren MSI-Datei installiert werden. Ältere per MSI installierte Versionen von Azure-Modulen werden vom Installationsprogramm automatisch entfernt. Mit dem MSI-Paket werden Module unter `${env:ProgramFiles}\WindowsPowerShell\Modules` installiert. Sowohl das Modul `AzureRM` als auch das Modul `Azure` werden installiert.

> [!NOTE]
> Verwenden Sie das Modul `Azure` nur, wenn Sie mit dem klassischen Azure-Bereitstellungsmodell arbeiten.

Damit Sie Azure PowerShell verwenden können, müssen Sie `AzureRM` mit dem [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module)-Cmdlet in Ihre aktuelle PowerShell-Sitzung laden und sich dann mit Ihren Azure-Anmeldeinformationen anmelden.

```powershell
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

Sie müssen diese Schritte für jede neue PowerShell-Sitzung wiederholen, die Sie starten. Für den automatischen Import des Moduls `AzureRM` muss ein PowerShell-Profil eingerichtet werden. Informationen hierzu finden Sie unter [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles) (Informationen zu Profilen).
Informationen zum sitzungsübergreifenden Speichern der Azure-Anmeldung finden Sie unter [Persisting user credentials across PowerShell sessions](context-persistence.md) (Speichern von Benutzeranmeldeinformationen zwischen PowerShell-Sitzungen).

## <a name="install-or-update-on-windows-using-the-web-platform-installer"></a>Installieren oder Aktualisieren unter Windows mit dem Webplattform-Installer

Laden Sie das [Azure PowerShell-WebPI-Paket](http://aka.ms/webpi-azps) herunter, und starten Sie die Installation. Ältere per MSI oder WebPI installierte Versionen von Azure-Modulen werden vom Installationsprogramm automatisch entfernt. Die Module werden unter `${env:ProgramFiles}\WindowsPowerShell\Modules` installiert. Sowohl das Modul `AzureRM` als auch das Modul `Azure` werden installiert.

> [!NOTE]
> Verwenden Sie das Modul `Azure` nur, wenn Sie mit dem klassischen Azure-Bereitstellungsmodell arbeiten.

Damit Sie Azure PowerShell verwenden können, müssen Sie `AzureRM` mit dem [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module)-Cmdlet in Ihre aktuelle PowerShell-Sitzung laden und sich dann mit Ihren Azure-Anmeldeinformationen anmelden.

```powershell
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

Sie müssen diese Schritte für jede neue PowerShell-Sitzung wiederholen, die Sie starten. Für den automatischen Import des Moduls `AzureRM` muss ein PowerShell-Profil eingerichtet werden. Informationen hierzu finden Sie unter [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles) (Informationen zu Profilen).
Informationen zum sitzungsübergreifenden Speichern der Azure-Anmeldung finden Sie unter [Persisting user credentials across PowerShell sessions](context-persistence.md) (Speichern von Benutzeranmeldeinformationen zwischen PowerShell-Sitzungen).