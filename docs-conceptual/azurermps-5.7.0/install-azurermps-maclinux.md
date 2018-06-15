---
title: Installieren von Azure PowerShell unter macOS oder Linux
description: Anleitung für die Installation von Azure PowerShell unter macOS oder Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 17912c155255b6fdfd3cfb9242163b67d405dc03
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323253"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a>Installieren von Azure PowerShell unter macOS oder Linux

Bei Windows-fremden Plattformen kann Azure PowerShell auf der Grundlage von PowerShell Core v6 ausgeführt werden. Im Gegensatz zur Standardversion von Azure PowerShell, die auf .NET Framework für Windows basiert, wurde dieses Produkt für .NET Core konzipiert und kann auf einer beliebigen Plattform ausgeführt werden, die die .NET Core-Laufzeit unterstützt.

> [!NOTE]
> PowerShell Core v6 und Azure PowerShell für .NET Core befinden sich derzeit noch in der Betaphase.
> Der Support für diese Produkte ist eingeschränkt. Sollten bei Ihnen Probleme oder Fehler auftreten, melden Sie dies bitte auf GitHub.
>
> * [Probleme mit PowerShell Core v6](https://github.com/PowerShell/PowerShell/issues)
> * [Probleme mit Azure PowerShell](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core-v6"></a>Installieren von PowerShell Core v6

Die Installation von PowerShell Core v6 unter Linux oder macOS variiert je nach Linux-Distribution und Betriebssystemversion.
Eine ausführliche Anleitung finden Sie in den folgenden Artikeln:

- [Installieren von PowerShell Core unter macOS](/powershell/scripting/setup/installing-powershell-core-on-macos)
- [Installieren von PowerShell Core unter Linux](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a>Installieren von Azure PowerShell für .NET Core

In PowerShell Core v6 ist das PowerShellGet-Modul bereits vorinstalliert. Dies vereinfacht die Installation eines beliebigen, im PowerShell-Katalog veröffentlichten Moduls. Um Azure PowerShell zu installieren, öffnen Sie eine neue PowerShell-Sitzung, und führen Sie den folgenden Befehl aus:

```powershell
Install-Module AzureRM.NetCore
```

## <a name="load-the-azurermnetcore-module"></a>Laden des AzureRM.Netcore-Moduls

Nach der Installation des Moduls müssen Sie das Modul in der PowerShell-Sitzung laden. Module werden wie folgt mit dem Cmdlet `Import-Module` geladen:

```powershell
Import-Module AzureRM.Netcore
Import-Module AzureRM.Profile.Netcore
```

Nach Abschluss des Imports können Sie das neu installierte Modul testen, indem Sie versuchen, sich mithilfe des folgenden Befehls bei Azure anzumelden:

```powershell
Connect-AzureRmAccount
```

Der obige Befehl sollte Sie auffordern, zu `https://aka.ms/devicelogin` zu wechseln und den bereitgestellten Code einzugeben.

## <a name="available-cmdlets"></a>Verfügbare Cmdlets

Die Azure PowerShell-Module für .NET Standard sind immer noch in der Entwicklungsphase. Diese Module bieten nicht den vollständigen Satz der Cmdlets, die für die Windows-Version der Module verfügbar sind. Die folgenden Funktionen werden in AzureRM.Netcore-Module implementiert:

* Kontenverwaltung
  - Melden Sie sich mit dem Microsoft-Konto, Unternehmenskonto oder einem Dienstprinzipal über Microsoft Azure Active Directory an.
  - Speichern Sie die Anmeldeinformationen mit Save-AzureRmContext auf einem Datenträger, und laden Sie gespeicherte Anmeldeinformationen mit Import-AzureRmContext.
* Environment
  - Abrufen der verschiedenen vorkonfigurierten Microsoft Azure-Umgebungen
  - Hinzufügen/Einrichten/Entfernen angepasster Umgebungen (z.B. Ihrer Azure Stack- oder Windows Azure Pack-Umgebungen)
* Cmdlets auf Verwaltungsebene für Azure-Dienste, die Resource Manager- und Service Management-Schnittstellen nutzen.
  - Virtual Machine
  - App Service (Websites)
  - SQL-Datenbank
  - Speicher
  - Netzwerk

## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen zur Verwendung von Azure PowerShell finden Sie im Artikel [Erste Schritte mit Azure PowerShell](get-started-azureps.md).
