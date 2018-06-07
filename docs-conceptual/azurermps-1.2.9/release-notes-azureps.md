---
title: Azure PowerShell-Änderungsprotokoll | Microsoft-Dokumentation
description: Hierbei handelt es sich um einen Verlauf der Änderungen, die in der neuesten Version an Azure PowerShell vorgenommen wurden.
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: c57ba563b5a4d4d19944fe8eca2cb4244ee5ed9e
ms.sourcegitcommit: 2eea03b7ac19ad6d7c8097743d33c7ddb9c4df77
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/06/2018
ms.locfileid: "34819710"
---
# <a name="release-notes"></a>Versionshinweise

Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.

## <a name="version-129"></a>Version 1.2.9

Änderungen in dieser Version

* AzureRm.AzureStackAdmin-Modul
    + Am Cmdlet „Add-AzureRmResourceProviderRegistration“ wurden Änderungen vorgenommen, um Teilungsvorgänge für Azure Resource Manager-Administratoren und Azure Resource Manager-Mandanten zu unterstützen. Der neue Parameter „-ResourceManagerType“ wurde hinzugefügt.
    + Die Parameter „-AdminUri“, „-ApiVersion“, „-SubscriptionId“ und „-Token“ wurden aus den einzelnen Cmdlets entfernt. Wir haben mithilfe von Warnungen darauf hingewiesen, dass diese Parameter ausgemustert werden. Nun wurden sie entfernt.
* AzureStackStorage-Modul
    + Zur Unterstützung von Containermigrationsszenarien wurden neue Cmdlets hinzugefügt.
    + Cmdlets, die auf interne Komponenten und zugrunde liegende Features verweisen, wurden entfernt.
* AzureRM.BootStrapper
    + Ein neues Modul wurde erstellt, das zum Verwalten der Versionen von Azure PowerShell-Cmdlets mithilfe von Versionsprofilen dient.