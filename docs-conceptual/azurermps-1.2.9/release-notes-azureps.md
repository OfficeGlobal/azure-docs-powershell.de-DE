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
# <a name="release-notes"></a><span data-ttu-id="fb9f3-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="fb9f3-103">Release notes</span></span>

<span data-ttu-id="fb9f3-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="fb9f3-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-129"></a><span data-ttu-id="fb9f3-105">Version 1.2.9</span><span class="sxs-lookup"><span data-stu-id="fb9f3-105">Version 1.2.9</span></span>

<span data-ttu-id="fb9f3-106">Änderungen in dieser Version</span><span class="sxs-lookup"><span data-stu-id="fb9f3-106">Changes This Release</span></span>

* <span data-ttu-id="fb9f3-107">AzureRm.AzureStackAdmin-Modul</span><span class="sxs-lookup"><span data-stu-id="fb9f3-107">AzureRm.AzureStackAdmin Module</span></span>
    + <span data-ttu-id="fb9f3-108">Am Cmdlet „Add-AzureRmResourceProviderRegistration“ wurden Änderungen vorgenommen, um Teilungsvorgänge für Azure Resource Manager-Administratoren und Azure Resource Manager-Mandanten zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="fb9f3-108">Changes in the Add-AzureRmResourceProviderRegistration cmdlet for the support of Admin Azure resource manager and tenant azure resource manager split.</span></span> <span data-ttu-id="fb9f3-109">Der neue Parameter „-ResourceManagerType“ wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fb9f3-109">A new parameter -ResourceManagerType has been added.</span></span>
    + <span data-ttu-id="fb9f3-110">Die Parameter „-AdminUri“, „-ApiVersion“, „-SubscriptionId“ und „-Token“ wurden aus den einzelnen Cmdlets entfernt.</span><span class="sxs-lookup"><span data-stu-id="fb9f3-110">Removal of the parameters -AdminUri, -ApiVersion, -SubscriptionId and -Token from each cmdlets.</span></span> <span data-ttu-id="fb9f3-111">Wir haben mithilfe von Warnungen darauf hingewiesen, dass diese Parameter ausgemustert werden. Nun wurden sie entfernt.</span><span class="sxs-lookup"><span data-stu-id="fb9f3-111">We have been printing warnings that these parameters will be deprecated and now they got removed.</span></span>
* <span data-ttu-id="fb9f3-112">AzureStackStorage-Modul</span><span class="sxs-lookup"><span data-stu-id="fb9f3-112">AzureStackStorage module</span></span>
    + <span data-ttu-id="fb9f3-113">Zur Unterstützung von Containermigrationsszenarien wurden neue Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fb9f3-113">Added new cmdlets to support container migration scenarios.</span></span>
    + <span data-ttu-id="fb9f3-114">Cmdlets, die auf interne Komponenten und zugrunde liegende Features verweisen, wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="fb9f3-114">Removed cmdlets referring to internal components and underlying features.</span></span>
* <span data-ttu-id="fb9f3-115">AzureRM.BootStrapper</span><span class="sxs-lookup"><span data-stu-id="fb9f3-115">AzureRM.BootStrapper</span></span>
    + <span data-ttu-id="fb9f3-116">Ein neues Modul wurde erstellt, das zum Verwalten der Versionen von Azure PowerShell-Cmdlets mithilfe von Versionsprofilen dient.</span><span class="sxs-lookup"><span data-stu-id="fb9f3-116">Created new module to manage versions of Azure PowerShell cmdlets through the use of version profiles</span></span>