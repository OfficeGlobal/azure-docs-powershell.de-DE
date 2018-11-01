---
title: Installieren von Azure PowerShell unter macOS oder Linux
description: Anleitung für die Installation von Azure PowerShell unter macOS oder Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/05/2018
ms.openlocfilehash: e7d27c6f6d980c54e45620b179cf2e26ffed17f0
ms.sourcegitcommit: ff44dec6418a449757bded3c6ebe0a7d4c05ee6e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/01/2018
ms.locfileid: "50738375"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a><span data-ttu-id="888b9-103">Installieren von Azure PowerShell unter macOS oder Linux</span><span class="sxs-lookup"><span data-stu-id="888b9-103">Install Azure PowerShell on macOS or Linux</span></span>

<span data-ttu-id="888b9-104">Bei Windows-fremden Plattformen kann Azure PowerShell in PowerShell Core v6 ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="888b9-104">For non-Windows platforms, it's possible to run Azure PowerShell in PowerShell Core v6.</span></span> <span data-ttu-id="888b9-105">Diese Version von PowerShell ist für die Verwendung auf allen Plattformen konzipiert, die .NET Core unterstützen.</span><span class="sxs-lookup"><span data-stu-id="888b9-105">This version of PowerShell is built for use on any platform that supports .NET Core.</span></span> <span data-ttu-id="888b9-106">Damit Sie diese Plattformen verwenden können, steht eine .NET Standard-Version von Azure PowerShell zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="888b9-106">To work with these platforms, there's a .NET Standard version of Azure PowerShell available.</span></span>

> [!NOTE]
> <span data-ttu-id="888b9-107">Derzeit befindet sich Azure PowerShell für .NET Standard noch in der Betaphase.</span><span class="sxs-lookup"><span data-stu-id="888b9-107">At this time, Azure PowerShell for .NET Standard is still in beta.</span></span>
> <span data-ttu-id="888b9-108">Sollten bei Ihnen Probleme oder Fehler auftreten, melden Sie dies bitte auf GitHub.</span><span class="sxs-lookup"><span data-stu-id="888b9-108">If you have problems or discover bugs, please file an issue on GitHub.</span></span>
>
> * [<span data-ttu-id="888b9-109">Probleme mit Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="888b9-109">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a><span data-ttu-id="888b9-110">Installieren von PowerShell Core</span><span class="sxs-lookup"><span data-stu-id="888b9-110">Install PowerShell Core</span></span>

<span data-ttu-id="888b9-111">Die Installationsanweisungen für PowerShell Core unterscheiden sich für macOS und die meisten Linux-Distributionen.</span><span class="sxs-lookup"><span data-stu-id="888b9-111">The installation instructions for PowerShell Core are different for macOS and most Linux distributions.</span></span>
<span data-ttu-id="888b9-112">Eine ausführliche Anleitung finden Sie in den folgenden Artikeln:</span><span class="sxs-lookup"><span data-stu-id="888b9-112">Detailed instructions can be found in the following articles:</span></span>

* [<span data-ttu-id="888b9-113">Installieren von PowerShell Core unter macOS</span><span class="sxs-lookup"><span data-stu-id="888b9-113">Install PowerShell Core on macOS</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [<span data-ttu-id="888b9-114">Installieren von PowerShell Core unter Linux</span><span class="sxs-lookup"><span data-stu-id="888b9-114">Install PowerShell Core on Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-standard"></a><span data-ttu-id="888b9-115">Installieren von Azure PowerShell für .NET Standard</span><span class="sxs-lookup"><span data-stu-id="888b9-115">Install Azure PowerShell for .NET Standard</span></span>

> [!IMPORTANT]
> <span data-ttu-id="888b9-116">Das Modul `AzureRM`, das in anderen Artikeln näher beschrieben wird, funktioniert mit PowerShell Core nicht.</span><span class="sxs-lookup"><span data-stu-id="888b9-116">The `AzureRM` module detailed in other articles does not work with PowerShell Core.</span></span>
> <span data-ttu-id="888b9-117">Sie müssen das Modul `Az` installieren, um die Azure PowerShell-Funktionalität in PowerShell Core zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="888b9-117">You must install the `Az` module to get Azure PowerShell functionality in PowerShell Core.</span></span>

<span data-ttu-id="888b9-118">In PowerShell Core ist das PowerShellGet-Modul bereits vorinstalliert.</span><span class="sxs-lookup"><span data-stu-id="888b9-118">PowerShell Core comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="888b9-119">Starten Sie PowerShell mit dem folgenden Befehl:</span><span class="sxs-lookup"><span data-stu-id="888b9-119">Start PowerShell with the command:</span></span>

```bash
pwsh
```

<span data-ttu-id="888b9-120">Führen Sie zum Installieren von Azure PowerShell den folgenden Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="888b9-120">To install Azure PowerShell, run the following command:</span></span>

```powershell
Install-Module Az
```

> [!NOTE]
> <span data-ttu-id="888b9-121">Wenn Sie beim Installieren des Moduls einen Berechtigungsfehler erhalten, müssen Sie PowerShell ggf. im Superuser-Modus ausführen, um Module zu installieren.</span><span class="sxs-lookup"><span data-stu-id="888b9-121">If you encounter a permissions error when attempting to install the module, you may need to run PowerShell in superuser mode to install modules.</span></span>
>
> ```bash
> sudo pwsh
> ```

<span data-ttu-id="888b9-122">Standardmäßig ist der PowerShell-Katalog nicht als vertrauenswürdiges Repository für PowerShellGet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="888b9-122">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="888b9-123">Bei der ersten Verwendung des PowerShell-Katalogs wird die folgende Meldung angezeigt:</span><span class="sxs-lookup"><span data-stu-id="888b9-123">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="888b9-124">Antworten Sie mit `Yes` oder `Yes to All`, um die Installation fortzusetzen.</span><span class="sxs-lookup"><span data-stu-id="888b9-124">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

## <a name="enable-aliases"></a><span data-ttu-id="888b9-125">Aktivieren von Aliasen</span><span class="sxs-lookup"><span data-stu-id="888b9-125">Enable aliases</span></span>

<span data-ttu-id="888b9-126">Zur Erzielung von Kompatibilität mit dem vorhandenen Modul `AzureRM` verfügt das neue Modul `Az` über die Möglichkeit zum Erstellen von abwärtskompatiblen Aliasen für die `AzureRM`-Cmdlets.</span><span class="sxs-lookup"><span data-stu-id="888b9-126">For compatibility with the existing `AzureRM` module, the new `Az` module has the ability to create backwards compatible aliases for the `AzureRM` cmdlets.</span></span> <span data-ttu-id="888b9-127">Richten Sie diese Aliase mit dem folgenden Befehl ein, bevor Sie das Modul zum ersten Mal verwenden:</span><span class="sxs-lookup"><span data-stu-id="888b9-127">Before using the module for the first time, set up these aliases with the following command:</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module Az
# Enable AzureRM aliases for the user
Enable-AzureRmAlias -Scope CurrentUser
```

<span data-ttu-id="888b9-128">Aliase werden nur für den aktuellen Benutzer eingerichtet.</span><span class="sxs-lookup"><span data-stu-id="888b9-128">This sets up aliases for the current user only.</span></span> <span data-ttu-id="888b9-129">Überprüfen Sie die Hilfe zum Cmdlet auf weitere Werte, die für `-Scope` angegeben werden können, um die Aliase einzurichten.</span><span class="sxs-lookup"><span data-stu-id="888b9-129">Check the cmdlet help for other values that can be provided to `-Scope` to set up the aliases.</span></span>

> [!NOTE]
> <span data-ttu-id="888b9-130">Wenn Sie einen Fehler zu einem Pfadspeicherort erhalten, sollten Sie sicherstellen, dass dieser auf Ihrem lokalen System vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="888b9-130">If you encounter an error about a path location, make sure that it exists on your local system.</span></span> <span data-ttu-id="888b9-131">Für den Bereich `CurrentUser` kann dieser Fehler behoben werden, indem in `bash` der folgende Befehl ausgeführt wird:</span><span class="sxs-lookup"><span data-stu-id="888b9-131">For the `CurrentUser` scope, this error can be resolved by running the following command in `bash`:</span></span>
>
> ```bash
> mkdir -p $HOME/.config/powershell
> ```

## <a name="sign-in"></a><span data-ttu-id="888b9-132">Anmelden</span><span class="sxs-lookup"><span data-stu-id="888b9-132">Sign in</span></span>

<span data-ttu-id="888b9-133">Damit Sie Azure PowerShell verwenden können, müssen Sie `Az` mit dem [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module)-Cmdlet in Ihre PowerShell-Sitzung laden und sich dann mit Ihren Azure-Anmeldeinformationen anmelden.</span><span class="sxs-lookup"><span data-stu-id="888b9-133">To start working with Azure PowerShell, you need to load `Az` into your PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span> <span data-ttu-id="888b9-134">Für das Importieren eines Moduls sind __keine__ erhöhten Rechte erforderlich.</span><span class="sxs-lookup"><span data-stu-id="888b9-134">Importing a module does __not__ require elevated privileges.</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module Az
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="888b9-135">Sie müssen diese Schritte für jede neue gestartete PowerShell-Sitzung wiederholen.</span><span class="sxs-lookup"><span data-stu-id="888b9-135">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="888b9-136">Für den automatischen Import des `Az`-Moduls muss ein PowerShell-Profil eingerichtet werden. Informationen hierzu finden Sie unter [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles) (Informationen zu Profilen).</span><span class="sxs-lookup"><span data-stu-id="888b9-136">Automatically importing the `Az` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="888b9-137">Unter macOS und Linux müssen Sie zur Verwendung Ihres Profils die Umgebungsvariable `$Profile` verwenden.</span><span class="sxs-lookup"><span data-stu-id="888b9-137">On macOS and Linux, you should work with your profile through the `$Profile` environment variable.</span></span> <span data-ttu-id="888b9-138">Informationen zum sitzungsübergreifenden Speichern der Azure-Anmeldung finden Sie unter [Persisting user credentials across PowerShell sessions](context-persistence.md) (Speichern von Benutzeranmeldeinformationen zwischen PowerShell-Sitzungen).</span><span class="sxs-lookup"><span data-stu-id="888b9-138">To learn how to persist your Azure sign-in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="888b9-139">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="888b9-139">Next Steps</span></span>

<span data-ttu-id="888b9-140">Weitere Informationen zur Verwendung von Azure PowerShell finden Sie im Artikel [Erste Schritte mit Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="888b9-140">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
