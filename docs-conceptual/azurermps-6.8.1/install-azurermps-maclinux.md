---
title: Installieren von Azure PowerShell unter macOS oder Linux
description: Anleitung für die Installation von Azure PowerShell unter macOS oder Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: f014d62e898da195a38052db6b7e37a2cd96dfdd
ms.sourcegitcommit: 3a02e0c85c83de873981dd392500bc82c1cf9286
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/24/2018
ms.locfileid: "46560115"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a>Installieren von Azure PowerShell unter macOS oder Linux

Bei Windows-fremden Plattformen kann Azure PowerShell in PowerShell Core v6 ausgeführt werden. Diese Version von PowerShell ist für die Verwendung auf allen Plattformen konzipiert, die .NET Core unterstützen. Damit Sie diese Plattformen verwenden können, steht eine .NET Standard-Version von Azure PowerShell zur Verfügung.

> [!NOTE]
> PowerShell Core v6 und Azure PowerShell für .NET Core befinden sich derzeit noch in der Betaphase.
> Der Support für diese Produkte ist eingeschränkt. Sollten bei Ihnen Probleme oder Fehler auftreten, melden Sie dies bitte auf GitHub.
>
> * [Probleme mit PowerShell Core v6](https://github.com/PowerShell/PowerShell/issues)
> * [Probleme mit Azure PowerShell](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a>Installieren von PowerShell Core

Die Installationsanweisungen für PowerShell Core unterscheiden sich für macOS und die meisten Linux-Distributionen.
Eine ausführliche Anleitung finden Sie in den folgenden Artikeln:

* [Installieren von PowerShell Core unter macOS](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [Installieren von PowerShell Core unter Linux](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a>Installieren von Azure PowerShell für .NET Core

In PowerShell Core ist das PowerShellGet-Modul bereits vorinstalliert. Für die Installation der Module in PowerShell sind erhöhte Rechte erforderlich, daher müssen Sie Ihre Sitzung als Superuser starten:

```bash
sudo pwsh
```

Führen Sie zum Installieren von Azure PowerShell den folgenden Befehl aus:

```powershell
Install-Module Az
```

> [!IMPORTANT]
> Das in einem anderen Artikel behandelte `AzureRM`-Modul ist nicht für .NET Core konzipiert und kann nicht mit PowerShell Core verwendet werden. Die `Az`-Module enthalten Befehlsaliase für alle `AzureRM`-Cmdlets, sodass die gesamte Dokumentation für `AzureRM` gilt.

Standardmäßig ist der PowerShell-Katalog nicht als vertrauenswürdiges Repository für PowerShellGet konfiguriert. Bei der ersten Verwendung des PowerShell-Katalogs wird die folgende Meldung angezeigt:

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

Antworten Sie mit `Yes` oder `Yes to All`, um die Installation fortzusetzen.

## <a name="sign-in"></a>Anmelden

Damit Sie Azure PowerShell verwenden können, müssen Sie `Az` mit dem [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module)-Cmdlet in Ihre PowerShell-Sitzung laden und sich dann mit Ihren Azure-Anmeldeinformationen anmelden. Für das Importieren eines Moduls sind __keine__ erhöhten Rechte erforderlich.

```powershell
# Import the module into the PowerShell session
Import-Module Az
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

Sie müssen diese Schritte für jede neue gestartete PowerShell-Sitzung wiederholen. Für den automatischen Import des `Az`-Moduls muss ein PowerShell-Profil eingerichtet werden. Informationen hierzu finden Sie unter [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles) (Informationen zu Profilen).
Unter macOS und Linux müssen Sie zur Verwendung Ihres Profils die Umgebungsvariable `$Profile` verwenden. Informationen zum sitzungsübergreifenden Speichern der Azure-Anmeldung finden Sie unter [Persisting user credentials across PowerShell sessions](context-persistence.md) (Speichern von Benutzeranmeldeinformationen zwischen PowerShell-Sitzungen).

## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen zur Verwendung von Azure PowerShell finden Sie im Artikel [Erste Schritte mit Azure PowerShell](get-started-azureps.md).
