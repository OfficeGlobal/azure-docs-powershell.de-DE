---
title: Ausführen von Azure PowerShell in einem Docker-Container
description: Es wird beschrieben, wie Sie Azure PowerShell in einem Docker-Container ausführen.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/20/2018
ms.openlocfilehash: b224beb95809d0e48c6f1dd5985de45b3b4df816
ms.sourcegitcommit: 4c775721461210431bd913f28d1f1e6f1976880a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2018
ms.locfileid: "37091597"
---
## <a name="run-azure-powershell-in-a-docker-container"></a>Ausführen von Azure PowerShell in einem Docker-Container

Es gibt eine Reihe von Docker-Images, die bereits für Azure PowerShell vorkonfiguriert sind. Zwei Arten von Containern sind verfügbar: Container mit herkömmlicher PowerShell-Instanz unter Windows und ein Container mit PowerShell Core unter Windows oder Linux.

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