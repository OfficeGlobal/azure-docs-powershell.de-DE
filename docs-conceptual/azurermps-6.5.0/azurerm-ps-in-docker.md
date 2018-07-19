---
title: Ausführen von Azure PowerShell in einem Docker-Container
description: Es wird beschrieben, wie Sie Azure PowerShell in einem Docker-Container ausführen.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/20/2018
ms.openlocfilehash: 656c58fbb7cafb539736a0083d6aed1f46b7b98d
ms.sourcegitcommit: 8b882d1c27d9e323447ff85f56d11bbf5e244d7f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/18/2018
ms.locfileid: "39110329"
---
# <a name="run-azure-powershell-in-a-docker-container"></a><span data-ttu-id="ca6e5-103">Ausführen von Azure PowerShell in einem Docker-Container</span><span class="sxs-lookup"><span data-stu-id="ca6e5-103">Run Azure PowerShell in a Docker container</span></span>

<span data-ttu-id="ca6e5-104">Es gibt eine Reihe von Docker-Images, die bereits für Azure PowerShell vorkonfiguriert sind.</span><span class="sxs-lookup"><span data-stu-id="ca6e5-104">There are a set of Docker images preconfigured with Azure PowerShell.</span></span> <span data-ttu-id="ca6e5-105">Zwei Arten von Containern sind verfügbar: Container mit herkömmlicher PowerShell-Instanz unter Windows und ein Container mit PowerShell Core unter Windows oder Linux.</span><span class="sxs-lookup"><span data-stu-id="ca6e5-105">Two types of containers are available: Those running traditional PowerShell on Windows, and a container running PowerShell Core on either Windows or Linux.</span></span>

| <span data-ttu-id="ca6e5-106">Environment</span><span class="sxs-lookup"><span data-stu-id="ca6e5-106">Environment</span></span> | <span data-ttu-id="ca6e5-107">Docker-Image</span><span class="sxs-lookup"><span data-stu-id="ca6e5-107">Docker image</span></span> |
|-------------|--------------|
| <span data-ttu-id="ca6e5-108">PowerShell unter Windows</span><span class="sxs-lookup"><span data-stu-id="ca6e5-108">PowerShell on Windows</span></span> | [<span data-ttu-id="ca6e5-109">azuresdk/azure-powershell</span><span class="sxs-lookup"><span data-stu-id="ca6e5-109">azuresdk/azure-powershell</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| <span data-ttu-id="ca6e5-110">PowerShell Core unter Windows</span><span class="sxs-lookup"><span data-stu-id="ca6e5-110">PowerShell Core on Windows</span></span> | [<span data-ttu-id="ca6e5-111">azuresdk/azure-powershell-core:nanoserver</span><span class="sxs-lookup"><span data-stu-id="ca6e5-111">azuresdk/azure-powershell-core:nanoserver</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| <span data-ttu-id="ca6e5-112">PowerShell Core unter Linux</span><span class="sxs-lookup"><span data-stu-id="ca6e5-112">PowerShell Core on Linux</span></span> | [<span data-ttu-id="ca6e5-113">azuresdk/azure-powershell-core:latest</span><span class="sxs-lookup"><span data-stu-id="ca6e5-113">azuresdk/azure-powershell-core:latest</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

<span data-ttu-id="ca6e5-114">Wenn Sie einen dieser Container ausführen möchten, verwenden Sie `docker run -it $ImageName`, um ein interaktives Terminal zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="ca6e5-114">To run any of these containers, you use `docker run -it $ImageName` to get an interactive terminal.</span></span> <span data-ttu-id="ca6e5-115">Verwenden Sie also beispielsweise Folgendes, wenn Sie den Container „PowerShell Core unter Linux“ ausführen möchten:</span><span class="sxs-lookup"><span data-stu-id="ca6e5-115">For example, to run the PowerShell Core on Linux container, use:</span></span>

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> <span data-ttu-id="ca6e5-116">Wenn Sie einen Windows-Container in Docker ausführen möchten, muss Windows als Hostbetriebssystem verwendet werden, und Docker muss für die Ausführung von Windows-Containern konfiguriert sein.</span><span class="sxs-lookup"><span data-stu-id="ca6e5-116">To run a Windows container in Docker, your host OS must be Windows and Docker must be set to run Windows containers.</span></span> <span data-ttu-id="ca6e5-117">Informationen zum Wechseln zwischen Windows- und Linux-Umgebungen in Docker finden Sie in der Docker-Dokumentation unter [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers) (Wechseln zwischen Windows und Linux-Containern).</span><span class="sxs-lookup"><span data-stu-id="ca6e5-117">To learn about switching between Windows and Linux environments in Docker, see the Docker documentation [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).</span></span>

## <a name="use-a-powershell-core-container"></a><span data-ttu-id="ca6e5-118">Verwenden eines PowerShell Core-Containers</span><span class="sxs-lookup"><span data-stu-id="ca6e5-118">Use a PowerShell Core container</span></span>

<span data-ttu-id="ca6e5-119">Die PowerShell Core-Container werden mit PowerShell Core v6 bereitgestellt, und das Modul `AzureRM.NetCore` ist vorinstalliert.</span><span class="sxs-lookup"><span data-stu-id="ca6e5-119">The PowerShell Core containers come with PowerShell Core v6 and the `AzureRM.NetCore` module pre-installed.</span></span> <span data-ttu-id="ca6e5-120">Führen Sie das [Import-Module](/powershell/module/microsoft.powershell.core/import-module)-Cmdlet aus, und melden Sie sich dann mit Ihrem Azure-Konto an:</span><span class="sxs-lookup"><span data-stu-id="ca6e5-120">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM.NetCore
Connect-AzureRmAccount
```

## <a name="use-the-windows-container-with-powershell"></a><span data-ttu-id="ca6e5-121">Verwenden des Windows-Containers mit PowerShell</span><span class="sxs-lookup"><span data-stu-id="ca6e5-121">Use the Windows container with PowerShell</span></span>

<span data-ttu-id="ca6e5-122">Für den Windows-Container ist das Modul `AzureRM` vorinstalliert.</span><span class="sxs-lookup"><span data-stu-id="ca6e5-122">The Windows container has the `AzureRM` module pre-installed.</span></span> <span data-ttu-id="ca6e5-123">Führen Sie das [Import-Module](/powershell/module/microsoft.powershell.core/import-module)-Cmdlet aus, und melden Sie sich dann mit Ihrem Azure-Konto an:</span><span class="sxs-lookup"><span data-stu-id="ca6e5-123">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM
Connect-AzureRmAccount
```