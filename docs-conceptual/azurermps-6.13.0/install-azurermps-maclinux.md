---
title: Installieren von Azure PowerShell unter macOS oder Linux
description: Anleitung für die Installation von Azure PowerShell unter macOS oder Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/05/2018
ms.openlocfilehash: f60ea1c608be4b1c8319d53303713ba039276abc
ms.sourcegitcommit: 087c588169786c005a3c177624fb3ac6c8870125
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/13/2018
ms.locfileid: "53216669"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a>Installieren von Azure PowerShell unter macOS oder Linux

Bei Windows-fremden Plattformen kann Azure PowerShell in PowerShell Core v6 ausgeführt werden. Diese Version von PowerShell ist für die Verwendung auf allen Plattformen konzipiert, die .NET Core unterstützen. Damit Sie diese Plattformen verwenden können, steht eine .NET Standard-Version von Azure PowerShell zur Verfügung.

> [!NOTE]
> Derzeit befindet sich Azure PowerShell für .NET Standard noch in der Betaphase.
> Sollten bei Ihnen Probleme oder Fehler auftreten, melden Sie dies bitte auf GitHub.
>
> * [Probleme mit Azure PowerShell](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a>Installieren von PowerShell Core

Die Installationsanweisungen für PowerShell Core unterscheiden sich für macOS und die meisten Linux-Distributionen.
Eine ausführliche Anleitung finden Sie in den folgenden Artikeln:

* [Installieren von PowerShell Core unter macOS](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [Installieren von PowerShell Core unter Linux](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-standard"></a>Installieren von Azure PowerShell für .NET Standard

> [!IMPORTANT]
> Das Modul `AzureRM`, das in anderen Artikeln näher beschrieben wird, funktioniert mit PowerShell Core nicht.
> Sie müssen das Modul `Az` installieren, um die Azure PowerShell-Funktionalität in PowerShell Core zu erhalten.

In PowerShell Core ist das PowerShellGet-Modul bereits vorinstalliert. Starten Sie PowerShell mit dem folgenden Befehl:

```bash
pwsh
```

Führen Sie zum Installieren von Azure PowerShell den folgenden Befehl aus:

```powershell-interactive
Install-Module Az
```

> [!NOTE]
> Wenn Sie beim Installieren des Moduls einen Berechtigungsfehler erhalten, müssen Sie PowerShell ggf. im Superuser-Modus ausführen, um Module zu installieren.
>
> ```bash
> sudo pwsh
> ```

Standardmäßig ist der PowerShell-Katalog nicht als vertrauenswürdiges Repository für PowerShellGet konfiguriert. Bei der ersten Verwendung des PowerShell-Katalogs wird die folgende Meldung angezeigt:

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

Antworten Sie mit `Yes` oder `Yes to All`, um die Installation fortzusetzen.

## <a name="enable-aliases"></a>Aktivieren von Aliasen

Zur Erzielung von Kompatibilität mit dem vorhandenen Modul `AzureRM` verfügt das neue Modul `Az` über die Möglichkeit zum Erstellen von abwärtskompatiblen Aliasen für die `AzureRM`-Cmdlets. Richten Sie diese Aliase mit dem folgenden Befehl ein, bevor Sie das Modul zum ersten Mal verwenden:

```powershell-interactive
# Import the module into the PowerShell session
Import-Module Az
# Enable AzureRM aliases for the user
Enable-AzureRmAlias -Scope CurrentUser
```

Aliase werden nur für den aktuellen Benutzer eingerichtet. Überprüfen Sie die Hilfe zum Cmdlet auf weitere Werte, die für `-Scope` angegeben werden können, um die Aliase einzurichten.

> [!NOTE]
> Wenn Sie einen Fehler zu einem Pfadspeicherort erhalten, sollten Sie sicherstellen, dass dieser auf Ihrem lokalen System vorhanden ist. Für den Bereich `CurrentUser` kann dieser Fehler behoben werden, indem in `bash` der folgende Befehl ausgeführt wird:
>
> ```bash
> mkdir -p $HOME/.config/powershell
> ```

## <a name="sign-in"></a>Anmelden

Damit Sie Azure PowerShell verwenden können, müssen Sie `Az` mit dem [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module)-Cmdlet in Ihre PowerShell-Sitzung laden und sich dann mit Ihren Azure-Anmeldeinformationen anmelden. Für das Importieren eines Moduls sind __keine__ erhöhten Rechte erforderlich.

```powershell-interactive
# Import the module into the PowerShell session
Import-Module Az
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

Sie müssen diese Schritte für jede neue gestartete PowerShell-Sitzung wiederholen. Für den automatischen Import des `Az`-Moduls muss ein PowerShell-Profil eingerichtet werden. Informationen hierzu finden Sie unter [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles) (Informationen zu Profilen).
Unter macOS und Linux müssen Sie zur Verwendung Ihres Profils die Umgebungsvariable `$Profile` verwenden. Informationen zum sitzungsübergreifenden Speichern der Azure-Anmeldung finden Sie unter [Persisting user credentials across PowerShell sessions](context-persistence.md) (Speichern von Benutzeranmeldeinformationen zwischen PowerShell-Sitzungen).

## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen zur Verwendung von Azure PowerShell finden Sie im Artikel [Erste Schritte mit Azure PowerShell](get-started-azureps.md).
