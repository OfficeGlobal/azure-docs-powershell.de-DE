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
ms.locfileid: "35323321"
---
# <a name="other-installation-methods"></a><span data-ttu-id="dff06-103">Andere Installationsmethoden</span><span class="sxs-lookup"><span data-stu-id="dff06-103">Other installation methods</span></span>

<span data-ttu-id="dff06-104">In diesem Artikel erfahren Sie, wie Sie Azure PowerShell mithilfe eines MSI-Pakets oder mithilfe des Webplattform-Installers (WebPI) installieren.</span><span class="sxs-lookup"><span data-stu-id="dff06-104">This article explains how to install Azure PowerShell using an MSI or Web Platform Installer (WebPI).</span></span> <span data-ttu-id="dff06-105">Azure PowerShell kann auch innerhalb eines Docker-Containers ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="dff06-105">You can also run Azure PowerShell from inside of a Docker container.</span></span> <span data-ttu-id="dff06-106">Verwenden Sie diese Installationsmethoden nur, wenn sie für Ihr System erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="dff06-106">Use these installation methods only if they're necessary for your system.</span></span> <span data-ttu-id="dff06-107">Grundsätzlich sollte Azure PowerShell mithilfe von PowerShellGet installiert werden.</span><span class="sxs-lookup"><span data-stu-id="dff06-107">The canonical way to install Azure PowerShell is through PowerShellGet.</span></span> <span data-ttu-id="dff06-108">Eine Anleitung für die Installation von Azure PowerShell unter Verwendung von PowerShellGet finden Sie unter [Installieren von Azure PowerShell mit PowerShellGet](install-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="dff06-108">For instructions on using PowerShellGet to install Azure PowerShell, see [Install Azure PowerShell with PowerShellGet](install-azurerm-ps.md).</span></span>

<span data-ttu-id="dff06-109">Informationen zur Installation in Linux- oder macOS-Umgebungen finden Sie unter [Installieren von Azure PowerShell unter macOS oder Linux](install-azurermps-maclinux.md).</span><span class="sxs-lookup"><span data-stu-id="dff06-109">To install on Linux or macOS environments, see [Install Azure PowerShell on macOS or Linux](install-azurermps-maclinux.md).</span></span>

## <a name="install-or-update-on-windows-using-the-web-platform-installer"></a><span data-ttu-id="dff06-110">Installieren oder Aktualisieren unter Windows mit dem Webplattform-Installer</span><span class="sxs-lookup"><span data-stu-id="dff06-110">Install or update on Windows using the Web Platform Installer</span></span>

<span data-ttu-id="dff06-111">Die Vorgehensweise zum Installieren der neuesten Azure PowerShell-Version über WebPI hat sich im Vergleich zu früheren Versionen nicht geändert.</span><span class="sxs-lookup"><span data-stu-id="dff06-111">Installing the latest Azure PowerShell from WebPI is the same as it was for previous versions.</span></span>
<span data-ttu-id="dff06-112">Laden Sie das [Azure PowerShell-WebPI-Paket](http://aka.ms/webpi-azps) herunter, und starten Sie die Installation.</span><span class="sxs-lookup"><span data-stu-id="dff06-112">Download the [Azure PowerShell WebPI package](http://aka.ms/webpi-azps) and start the install.</span></span>

> [!NOTE]
> <span data-ttu-id="dff06-113">Wenn Sie bereits Azure-Module aus dem PowerShell-Katalog installiert haben, entfernt das Installationsprogramm diese automatisch.</span><span class="sxs-lookup"><span data-stu-id="dff06-113">If you have previously installed Azure modules from the PowerShell Gallery, the installer automatically removes them.</span></span> <span data-ttu-id="dff06-114">Dadurch wird sichergestellt, dass nur eine einzelne Version von Azure PowerShell installiert ist, was Ihre Umgebung vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="dff06-114">This simplifies your environment by ensuring that only one version of Azure PowerShell is installed.</span></span> <span data-ttu-id="dff06-115">Es gibt jedoch Szenarien, in denen mehrere gleichzeitig installierte Versionen benötigt werden.</span><span class="sxs-lookup"><span data-stu-id="dff06-115">However, there are scenarios where you may need multiple versions installed at the same time.</span></span>
>
> <span data-ttu-id="dff06-116">PowerShell-Katalogmodule werden unter `$env:ProgramFiles\WindowsPowerShell\Modules` installiert.</span><span class="sxs-lookup"><span data-stu-id="dff06-116">PowerShell Gallery modules install modules in `$env:ProgramFiles\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="dff06-117">Der WebPI-Installer installiert Azure-Module dagegen unter `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.</span><span class="sxs-lookup"><span data-stu-id="dff06-117">In contrast, the WebPI installer installs the Azure modules in `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.</span></span>
>
> <span data-ttu-id="dff06-118">Im Falle eines Installationsfehlers können Sie die `Azure*` Ordner aus dem Ordner `$env:ProgramFiles\WindowsPowerShell\Modules` entfernen und die Installation wiederholen.</span><span class="sxs-lookup"><span data-stu-id="dff06-118">If an error occurs during install, you can manually remove the `Azure*` folders in your `$env:ProgramFiles\WindowsPowerShell\Modules` folder, and try the installation again.</span></span>

<span data-ttu-id="dff06-119">Nach Abschluss der Installation sollte Ihre `$env:PSModulePath` -Einstellung die Verzeichnisse mit den Azure PowerShell-Cmdlets enthalten.</span><span class="sxs-lookup"><span data-stu-id="dff06-119">Once the installation completes, your `$env:PSModulePath` setting should include the directories containing the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="dff06-120">Mit dem folgenden Befehl können Sie überprüfen, ob Azure PowerShell ordnungsgemäß installiert wurde:</span><span class="sxs-lookup"><span data-stu-id="dff06-120">The following command can be used to verify that the Azure PowerShell is installed properly:</span></span>

```powershell
# To make sure the Azure PowerShell module is available after you install
Get-Module -ListAvailable Azure* | Select-Object Name, Version, Path
```

> [!NOTE]
> <span data-ttu-id="dff06-121">Es gibt ein bekanntes Problem, das bei der Installation per WebPI auftreten kann.</span><span class="sxs-lookup"><span data-stu-id="dff06-121">There is a known issue that can occur when installing from WebPI.</span></span> <span data-ttu-id="dff06-122">Wenn Ihr Computer aufgrund von Systemupdates oder anderen Installationen neu gestartet werden muss, wird bei Updates für `$env:PSModulePath` unter Umständen der Installationspfad von Azure PowerShell nicht einbezogen.</span><span class="sxs-lookup"><span data-stu-id="dff06-122">If your computer requires a restart due to system updates or other installations, it may cause updates to `$env:PSModulePath` to fail to include the path where Azure PowerShell is installed.</span></span>

<span data-ttu-id="dff06-123">Nach der Installation wird beim Ladevorgang oder beim Ausführen von Cmdlets möglicherweise folgende Fehlermeldung angezeigt:</span><span class="sxs-lookup"><span data-stu-id="dff06-123">When attempting to load or execute cmdlets after installation, you can receive the following error message:</span></span>

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

<span data-ttu-id="dff06-124">Starten Sie zum Beheben dieses Fehlers den Computer neu, oder importieren Sie das Modul unter Verwendung des vollqualifizierten Pfads.</span><span class="sxs-lookup"><span data-stu-id="dff06-124">This error can be corrected by restarting the machine or importing the module using the fully qualified path.</span></span>

```powershell
Import-Module "$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\AzureRM.psd1"
```

## <a name="install-or-update-on-windows-using-the-msi-package"></a><span data-ttu-id="dff06-125">Installieren oder Aktualisieren unter Windows mithilfe des MSI-Pakets</span><span class="sxs-lookup"><span data-stu-id="dff06-125">Install or update on Windows using the MSI Package</span></span>

<span data-ttu-id="dff06-126">Azure PowerShell kann mithilfe der bei [GitHub](https://aka.ms/azps-release) verfügbaren MSI-Datei installiert werden.</span><span class="sxs-lookup"><span data-stu-id="dff06-126">Azure PowerShell can be installed using the MSI file available from [GitHub](https://aka.ms/azps-release).</span></span> <span data-ttu-id="dff06-127">Ältere installierte Versionen von Azure-Modulen werden vom Installationsprogramm automatisch entfernt.</span><span class="sxs-lookup"><span data-stu-id="dff06-127">If you have installed previous versions of Azure modules, the installer automatically removes them.</span></span> <span data-ttu-id="dff06-128">Das MSI-Paket installiert Module unter `$env:ProgramFiles\WindowsPowerShell\Modules`, erstellt aber keine versionsspezifischen Ordner.</span><span class="sxs-lookup"><span data-stu-id="dff06-128">The MSI package installs modules in `$env:ProgramFiles\WindowsPowerShell\Modules` but does not create version-specific folders.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="dff06-129">Ausführen in einem Docker-Container</span><span class="sxs-lookup"><span data-stu-id="dff06-129">Run in a Docker container</span></span>

<span data-ttu-id="dff06-130">Wir pflegen eine Reihe von Docker-Images, die bereits mit Azure PowerShell vorkonfiguriert sind.</span><span class="sxs-lookup"><span data-stu-id="dff06-130">We maintain a set of Docker images preconfigured with Azure PowerShell.</span></span> <span data-ttu-id="dff06-131">Zur Verfügung stehen zwei Arten von Containern: Container mit herkömmlicher PowerShell-Instanz unter Windows und ein Container mit PowerShell Core unter Windows oder Linux.</span><span class="sxs-lookup"><span data-stu-id="dff06-131">There are two types of containers available: Those running traditional PowerShell on Windows, and a container running PowerShell Core on either Windows or Linux.</span></span>

| <span data-ttu-id="dff06-132">Environment</span><span class="sxs-lookup"><span data-stu-id="dff06-132">Environment</span></span> | <span data-ttu-id="dff06-133">Docker-Image</span><span class="sxs-lookup"><span data-stu-id="dff06-133">Docker image</span></span> |
|-------------|--------------|
| <span data-ttu-id="dff06-134">PowerShell unter Windows</span><span class="sxs-lookup"><span data-stu-id="dff06-134">PowerShell on Windows</span></span> | [<span data-ttu-id="dff06-135">azuresdk/azure-powershell</span><span class="sxs-lookup"><span data-stu-id="dff06-135">azuresdk/azure-powershell</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| <span data-ttu-id="dff06-136">PowerShell Core unter Windows</span><span class="sxs-lookup"><span data-stu-id="dff06-136">PowerShell Core on Windows</span></span> | [<span data-ttu-id="dff06-137">azuresdk/azure-powershell-core:nanoserver</span><span class="sxs-lookup"><span data-stu-id="dff06-137">azuresdk/azure-powershell-core:nanoserver</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| <span data-ttu-id="dff06-138">PowerShell Core unter Linux</span><span class="sxs-lookup"><span data-stu-id="dff06-138">PowerShell Core on Linux</span></span> | [<span data-ttu-id="dff06-139">azuresdk/azure-powershell-core:latest</span><span class="sxs-lookup"><span data-stu-id="dff06-139">azuresdk/azure-powershell-core:latest</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

<span data-ttu-id="dff06-140">Wenn Sie einen dieser Container ausführen möchten, verwenden Sie `docker run -it $ImageName`, um ein interaktives Terminal zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="dff06-140">To run any of these containers, you use `docker run -it $ImageName` to get an interactive terminal.</span></span> <span data-ttu-id="dff06-141">Verwenden Sie also beispielsweise Folgendes, wenn Sie den Container „PowerShell Core unter Linux“ ausführen möchten:</span><span class="sxs-lookup"><span data-stu-id="dff06-141">For example, to run the PowerShell Core on Linux container, use:</span></span>

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> <span data-ttu-id="dff06-142">Wenn Sie einen Windows-Container in Docker ausführen möchten, muss Windows als Hostbetriebssystem verwendet werden, und Docker muss für die Ausführung von Windows-Containern konfiguriert sein.</span><span class="sxs-lookup"><span data-stu-id="dff06-142">To run a Windows container in Docker, your host OS must be Windows and Docker must be set to run Windows containers.</span></span> <span data-ttu-id="dff06-143">Informationen zum Wechseln zwischen Windows- und Linux-Umgebungen in Docker finden Sie in der Docker-Dokumentation unter [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers) (Wechseln zwischen Windows und Linux-Containern).</span><span class="sxs-lookup"><span data-stu-id="dff06-143">To learn about switching between Windows and Linux environments in Docker, see the Docker documentation [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).</span></span>