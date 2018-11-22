---
title: Installieren von Azure PowerShell unter macOS oder Linux
description: Anleitung für die Installation von Azure PowerShell unter macOS oder Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 47611281f67d68c9fc2686e0c6156b060a225158
ms.sourcegitcommit: 80a3da199954d0ab78765715fb49793e89a30f12
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/22/2018
ms.locfileid: "52258688"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a>Installieren von Azure PowerShell unter macOS oder Linux

Bei Windows-fremden Plattformen kann Azure PowerShell in PowerShell Core v6 ausgeführt werden. Diese Version von PowerShell ist für die Verwendung auf allen Plattformen konzipiert, die .NET Core unterstützen. Damit Sie diese Plattformen verwenden können, steht eine spezielle .NET Core-Version von Azure PowerShell zur Verfügung.

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

```powershell-interactive
Install-Module AzureRM.NetCore
```

> [!IMPORTANT]
> Das in einem anderen Artikel behandelte `AzureRM`-Modul ist nicht für .NET Core konzipiert und kann nicht mit PowerShell Core verwendet werden. `AzureRM` und `AzureRM.NetCore` verwenden die gleichen Cmdlet-Namen. Der einzige Unterschied besteht also im Namen des Rollupmoduls und der .NET-Version, für die sie erstellt wurden.

Standardmäßig ist der PowerShell-Katalog nicht als vertrauenswürdiges Repository für PowerShellGet konfiguriert. Bei der ersten Verwendung des PowerShell-Katalogs wird die folgende Meldung angezeigt:

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

Antworten Sie mit `Yes` oder `Yes to All`, um die Installation fortzusetzen.

## <a name="sign-in"></a>Anmelden

Damit Sie Azure PowerShell verwenden können, müssen Sie `AzureRM.Netcore` mit dem [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module)-Cmdlet in Ihre PowerShell-Sitzung laden und sich dann mit Ihren Azure-Anmeldeinformationen anmelden. Für das Importieren eines Moduls sind __keine__ erhöhten Rechte erforderlich.

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM.Netcore
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

Sie müssen diese Schritte für jede neue gestartete PowerShell-Sitzung wiederholen. Für den automatischen Import des `AzureRM`-Moduls muss ein PowerShell-Profil eingerichtet werden. Informationen hierzu finden Sie unter [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles) (Informationen zu Profilen).
Unter macOS und Linux müssen Sie zur Verwendung Ihres Profils die Umgebungsvariable `$Profile` verwenden. Informationen zum sitzungsübergreifenden Speichern der Azure-Anmeldung finden Sie unter [Persisting user credentials across PowerShell sessions](context-persistence.md) (Speichern von Benutzeranmeldeinformationen zwischen PowerShell-Sitzungen).

## <a name="available-cmdlets"></a>Verfügbare Cmdlets

Die Azure PowerShell-Module für .NET Core befinden sich noch in der Entwicklungsphase. Diese Module bieten nicht den vollständigen Satz der Cmdlets, die für die Windows-Version der Module verfügbar sind. Die folgenden Funktionen werden in AzureRM.Netcore-Module implementiert:

* Kontenverwaltung
  * Anmelden mit einem Microsoft-Konto, Unternehmenskonto oder Dienstprinzipal über Microsoft Azure Active Directory
  * Speichern Sie die Anmeldeinformationen mit Save-AzureRmContext auf einem Datenträger, und laden Sie gespeicherte Anmeldeinformationen mit Import-AzureRmContext.
* Environment
  * Abrufen der verschiedenen vorkonfigurierten Microsoft Azure-Umgebungen
  * Hinzufügen/Einrichten/Entfernen angepasster Umgebungen (z.B. Ihrer Azure Stack- oder Windows Azure Pack-Umgebungen)
* Cmdlets auf Verwaltungsebene für Azure-Dienste, die Resource Manager- und Service Management-Schnittstellen nutzen.
  * Virtual Machine
  * App Service (Websites)
  * SQL-Datenbank
  * Speicher
  * Netzwerk

## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen zur Verwendung von Azure PowerShell finden Sie im Artikel [Erste Schritte mit Azure PowerShell](get-started-azureps.md).
