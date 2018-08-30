---
title: Ausführen von Azure PowerShell in einem Docker-Container
description: Es wird beschrieben, wie Sie Azure PowerShell in einem Docker-Container ausführen.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/20/2018
ms.openlocfilehash: 27ac176d8bd0b142b7740b2ba6793edb500a8af3
ms.sourcegitcommit: dca906e73e943aac207cee23b79915773419c673
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/30/2018
ms.locfileid: "43250624"
---
# <a name="run-azure-powershell-in-a-docker-container"></a><span data-ttu-id="095ea-103">Ausführen von Azure PowerShell in einem Docker-Container</span><span class="sxs-lookup"><span data-stu-id="095ea-103">Run Azure PowerShell in a Docker container</span></span>

<span data-ttu-id="095ea-104">Microsoft veröffentlicht Docker-Images mit vorinstallierter Azure PowerShell-Umgebung, um die Ausführung von Azure PowerShell in portablen Umgebungen zu erleichtern.</span><span class="sxs-lookup"><span data-stu-id="095ea-104">To make running Azure PowerShell in portable environments easy, Microsoft publishes Docker images with Azure PowerShell pre-installed.</span></span> <span data-ttu-id="095ea-105">Diese Images bieten einen Linux-Gast unter PowerShell Core oder einen Windows-Gast mit PowerShell Core oder PowerShell 5.</span><span class="sxs-lookup"><span data-stu-id="095ea-105">These images offer a Linux guest running PowerShell Core, or a Windows guest with either PowerShell Core or PowerShell 5.</span></span>

| <span data-ttu-id="095ea-106">Environment</span><span class="sxs-lookup"><span data-stu-id="095ea-106">Environment</span></span> | <span data-ttu-id="095ea-107">Docker-Image</span><span class="sxs-lookup"><span data-stu-id="095ea-107">Docker image</span></span> |
|-------------|--------------|
| <span data-ttu-id="095ea-108">PowerShell unter Windows</span><span class="sxs-lookup"><span data-stu-id="095ea-108">PowerShell on Windows</span></span> | [<span data-ttu-id="095ea-109">azuresdk/azure-powershell</span><span class="sxs-lookup"><span data-stu-id="095ea-109">azuresdk/azure-powershell</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| <span data-ttu-id="095ea-110">PowerShell Core unter Windows</span><span class="sxs-lookup"><span data-stu-id="095ea-110">PowerShell Core on Windows</span></span> | [<span data-ttu-id="095ea-111">azuresdk/azure-powershell-core:nanoserver</span><span class="sxs-lookup"><span data-stu-id="095ea-111">azuresdk/azure-powershell-core:nanoserver</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| <span data-ttu-id="095ea-112">PowerShell Core unter Linux</span><span class="sxs-lookup"><span data-stu-id="095ea-112">PowerShell Core on Linux</span></span> | [<span data-ttu-id="095ea-113">azuresdk/azure-powershell-core:latest</span><span class="sxs-lookup"><span data-stu-id="095ea-113">azuresdk/azure-powershell-core:latest</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

<span data-ttu-id="095ea-114">Wenn Sie einen dieser Container ausführen möchten, verwenden Sie `docker run -it $ImageName`, um ein interaktives Terminal zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="095ea-114">To run any of these containers, you use `docker run -it $ImageName` to get an interactive terminal.</span></span> <span data-ttu-id="095ea-115">Verwenden Sie also beispielsweise Folgendes, wenn Sie den Container „PowerShell Core unter Linux“ ausführen möchten:</span><span class="sxs-lookup"><span data-stu-id="095ea-115">For example, to run the PowerShell Core on Linux container, use:</span></span>

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> <span data-ttu-id="095ea-116">Wenn Sie einen Windows-Container in Docker ausführen möchten, muss Windows als Hostbetriebssystem verwendet werden, und Docker muss für die Ausführung von Windows-Containern konfiguriert sein.</span><span class="sxs-lookup"><span data-stu-id="095ea-116">To run a Windows container in Docker, your host OS must be Windows and Docker must be set to run Windows containers.</span></span> <span data-ttu-id="095ea-117">Informationen zum Wechseln zwischen Windows- und Linux-Umgebungen in Docker finden Sie in der Docker-Dokumentation unter [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers) (Wechseln zwischen Windows und Linux-Containern).</span><span class="sxs-lookup"><span data-stu-id="095ea-117">To learn about switching between Windows and Linux environments in Docker, see the Docker documentation [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).</span></span>

## <a name="use-a-powershell-core-container"></a><span data-ttu-id="095ea-118">Verwenden eines PowerShell Core-Containers</span><span class="sxs-lookup"><span data-stu-id="095ea-118">Use a PowerShell Core container</span></span>

<span data-ttu-id="095ea-119">Die PowerShell Core-Container werden mit PowerShell Core v6 bereitgestellt, und das Modul `AzureRM.NetCore` ist vorinstalliert.</span><span class="sxs-lookup"><span data-stu-id="095ea-119">The PowerShell Core containers come with PowerShell Core v6 and the `AzureRM.NetCore` module pre-installed.</span></span> <span data-ttu-id="095ea-120">Führen Sie das [Import-Module](/powershell/module/microsoft.powershell.core/import-module)-Cmdlet aus, und melden Sie sich dann mit Ihrem Azure-Konto an:</span><span class="sxs-lookup"><span data-stu-id="095ea-120">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM.NetCore
Connect-AzureRmAccount
```

## <a name="use-the-windows-container-with-powershell"></a><span data-ttu-id="095ea-121">Verwenden des Windows-Containers mit PowerShell</span><span class="sxs-lookup"><span data-stu-id="095ea-121">Use the Windows container with PowerShell</span></span>

<span data-ttu-id="095ea-122">Für den Windows-Container ist das Modul `AzureRM` vorinstalliert.</span><span class="sxs-lookup"><span data-stu-id="095ea-122">The Windows container has the `AzureRM` module pre-installed.</span></span> <span data-ttu-id="095ea-123">Führen Sie das [Import-Module](/powershell/module/microsoft.powershell.core/import-module)-Cmdlet aus, und melden Sie sich dann mit Ihrem Azure-Konto an:</span><span class="sxs-lookup"><span data-stu-id="095ea-123">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM
Connect-AzureRmAccount
```
