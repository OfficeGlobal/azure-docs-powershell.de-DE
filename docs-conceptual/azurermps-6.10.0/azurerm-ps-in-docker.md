---
title: Ausführen von Azure PowerShell in einem Docker-Container
description: Es wird beschrieben, wie Sie Azure PowerShell in einem Docker-Container ausführen.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/09/2018
ms.openlocfilehash: 0ed8f50abbcb2aa00192196f19004446dc696b5d
ms.sourcegitcommit: a749eb729f583c9d0dd86141bbd04984d77ae9ab
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/11/2018
ms.locfileid: "48882100"
---
# <a name="run-azure-powershell-in-a-docker-container"></a>Ausführen von Azure PowerShell in einem Docker-Container

Microsoft veröffentlicht Docker-Images, für die Azure PowerShell vorinstalliert ist. Diese Images können für das Experimentieren mit Azure PowerShell oder das Ausführen in einer isolierten Umgebung verwendet werden. Es sind auch Images mit PowerShell Core und PowerShell 5 vorhanden. 

| Environment | Docker-Image |
|-------------|--------------|
| PowerShell unter Windows | [azuresdk/azure-powershell](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| PowerShell Core unter Windows | [azuresdk/azure-powershell-core:nanoserver](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| PowerShell Core unter Linux | [azuresdk/azure-powershell-core:latest](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

Verwenden Sie `docker run -it $ImageName`, um ein interaktives Terminal zu erhalten, wenn Sie einen dieser Container ausführen möchten. Beispiel für die Ausführung eines Linux-Containers mit PowerShell Core:

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> Wenn Sie einen Windows-Container in Docker ausführen möchten, muss Windows als Hostbetriebssystem verwendet werden, und Docker muss für die Ausführung von Windows-Containern konfiguriert sein. Informationen zum Wechseln zwischen Windows- und Linux-Umgebungen in Docker finden Sie in der Docker-Dokumentation unter [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers) (Wechseln zwischen Windows und Linux-Containern).

## <a name="use-a-powershell-core-container"></a>Verwenden eines PowerShell Core-Containers

Die PowerShell Core-Container werden mit PowerShell Core v6 bereitgestellt, und das Modul `AzureRM.NetCore` ist vorinstalliert. Führen Sie das [Import-Module](/powershell/module/microsoft.powershell.core/import-module)-Cmdlet aus, und melden Sie sich dann mit Ihrem Azure-Konto an:

```powershell
Import-Module AzureRM.NetCore
Connect-AzureRmAccount
```

## <a name="use-the-windows-container-with-powershell"></a>Verwenden des Windows-Containers mit PowerShell

Für den Windows-Container ist das Modul `AzureRM` vorinstalliert. Führen Sie das [Import-Module](/powershell/module/microsoft.powershell.core/import-module)-Cmdlet aus, und melden Sie sich dann mit Ihrem Azure-Konto an:

```powershell
Import-Module AzureRM
Connect-AzureRmAccount
```
