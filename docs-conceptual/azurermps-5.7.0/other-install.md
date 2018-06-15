---
title: Andere Installationsmöglichkeiten für Azure PowerShell
description: Hier erfahren Sie, wie Sie Azure PowerShell mithilfe des MSI-Pakets oder des Webplattform-Installers installieren.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 0919583d9cb05a75fae3b812eed84109be8b28aa
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323270"
---
# <a name="other-installation-methods"></a>Andere Installationsmethoden

In diesem Artikel erfahren Sie, wie Sie Azure PowerShell mithilfe eines MSI-Pakets oder mithilfe des Webplattform-Installers (WebPI) installieren. Azure PowerShell kann auch innerhalb eines Docker-Containers ausgeführt werden. Verwenden Sie diese Installationsmethoden nur, wenn sie für Ihr System erforderlich sind. Grundsätzlich sollte Azure PowerShell mithilfe von PowerShellGet installiert werden. Eine Anleitung für die Installation von Azure PowerShell unter Verwendung von PowerShellGet finden Sie unter [Installieren von Azure PowerShell mit PowerShellGet](install-azurerm-ps.md).

Informationen zur Installation in Linux- oder macOS-Umgebungen finden Sie unter [Installieren von Azure PowerShell unter macOS oder Linux](install-azurermps-maclinux.md).

## <a name="install-or-update-on-windows-using-the-web-platform-installer"></a>Installieren oder Aktualisieren unter Windows mit dem Webplattform-Installer

Die Vorgehensweise zum Installieren der neuesten Azure PowerShell-Version über WebPI hat sich im Vergleich zu früheren Versionen nicht geändert.
Laden Sie das [Azure PowerShell-WebPI-Paket](http://aka.ms/webpi-azps) herunter, und starten Sie die Installation.

> [!NOTE]
> Wenn Sie bereits Azure-Module aus dem PowerShell-Katalog installiert haben, entfernt das Installationsprogramm diese automatisch. Dadurch wird sichergestellt, dass nur eine einzelne Version von Azure PowerShell installiert ist, was Ihre Umgebung vereinfacht. Es gibt jedoch Szenarien, in denen mehrere gleichzeitig installierte Versionen benötigt werden.
>
> PowerShell-Katalogmodule werden unter `$env:ProgramFiles\WindowsPowerShell\Modules` installiert. Der WebPI-Installer installiert Azure-Module dagegen unter `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.
>
> Im Falle eines Installationsfehlers können Sie die `Azure*` Ordner aus dem Ordner `$env:ProgramFiles\WindowsPowerShell\Modules` entfernen und die Installation wiederholen.

Nach Abschluss der Installation sollte Ihre `$env:PSModulePath` -Einstellung die Verzeichnisse mit den Azure PowerShell-Cmdlets enthalten. Mit dem folgenden Befehl können Sie überprüfen, ob Azure PowerShell ordnungsgemäß installiert wurde:

```powershell
# To make sure the Azure PowerShell module is available after you install
Get-Module -ListAvailable Azure* | Select-Object Name, Version, Path
```

> [!NOTE]
> Es gibt ein bekanntes Problem, das bei der Installation per WebPI auftreten kann. Wenn Ihr Computer aufgrund von Systemupdates oder anderen Installationen neu gestartet werden muss, wird bei Updates für `$env:PSModulePath` unter Umständen der Installationspfad von Azure PowerShell nicht einbezogen.

Nach der Installation wird beim Ladevorgang oder beim Ausführen von Cmdlets möglicherweise folgende Fehlermeldung angezeigt:

```
PS C:\> Connect-AzureRmAccount
Connect-AzureRmAccount : The term 'Connect-AzureRmAccount' is not recognized as the name of a cmdlet,
function, script file, or operable program. Check the spelling of the name, or if a path was
included, verify that the path is correct and try again.
At line:1 char:1
+ Connect-AzureRmAccount
+ ~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (Connect-AzureRmAccount:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
```

Starten Sie zum Beheben dieses Fehlers den Computer neu, oder importieren Sie das Modul unter Verwendung des vollqualifizierten Pfads.

```powershell
Import-Module "$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\AzureRM.psd1"
```

## <a name="install-or-update-on-windows-using-the-msi-package"></a>Installieren oder Aktualisieren unter Windows mithilfe des MSI-Pakets

Azure PowerShell kann mithilfe der bei [GitHub](https://aka.ms/azps-release) verfügbaren MSI-Datei installiert werden. Ältere installierte Versionen von Azure-Modulen werden vom Installationsprogramm automatisch entfernt. Das MSI-Paket installiert Module unter `$env:ProgramFiles\WindowsPowerShell\Modules`, erstellt aber keine versionsspezifischen Ordner.

## <a name="run-in-a-docker-container"></a>Ausführen in einem Docker-Container

Wir pflegen eine Reihe von Docker-Images, die bereits mit Azure PowerShell vorkonfiguriert sind. Zur Verfügung stehen zwei Arten von Containern: Container mit herkömmlicher PowerShell-Instanz unter Windows und ein Container mit PowerShell Core unter Windows oder Linux.

| Environment | Docker-Image |
|-------------|--------------|
| PowerShell unter Windows | [azuresdk/azure-powershell](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| PowerShell Core unter Windows | [azuresdk/azure-powershell-core:nanoserver](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| PowerShell Core unter Linux | [azuresdk/azure-powershell-core:latest](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

Wenn Sie einen dieser Container ausführen möchten, verwenden Sie `docker run -it $ImageName`, um ein interaktives Terminal zu erhalten. Verwenden Sie also beispielsweise Folgendes, wenn Sie den Container „PowerShell Core unter Linux“ ausführen möchten:

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> Wenn Sie einen Windows-Container in Docker ausführen möchten, muss Windows als Hostbetriebssystem verwendet werden, und Docker muss für die Ausführung von Windows-Containern konfiguriert sein. Informationen zum Wechseln zwischen Windows- und Linux-Umgebungen in Docker finden Sie in der Docker-Dokumentation unter [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers) (Wechseln zwischen Windows und Linux-Containern).