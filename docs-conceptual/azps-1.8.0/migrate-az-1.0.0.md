---
title: Grundlegende Änderungen für Microsoft Azure PowerShell Az 1.0.0
description: Dieser Migrationsleitfaden enthält eine Liste mit grundlegenden Änderungen, die in Az-Version 1 an Azure PowerShell vorgenommen wurden.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/14/2018
ms.openlocfilehash: be3e19dc4b689adbc63b933dd9f3454122d5344a
ms.sourcegitcommit: 43f4bdf2a59dd82fd881512aa9761bf72eb5703c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "63068845"
---
# <a name="migration-guide-for-az-100"></a><span data-ttu-id="25a88-103">Migrationsleitfaden für Az 1.0.0</span><span class="sxs-lookup"><span data-stu-id="25a88-103">Migration Guide for Az 1.0.0</span></span>

<span data-ttu-id="25a88-104">In diesem Dokument werden die Änderungen beschrieben, die zwischen den 6.x-Versionen von AzureRM und Az-Version 1.0.0 vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="25a88-104">This document describes the changes between the 6.x versions of AzureRM and Az version 1.0.0.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="25a88-105">Inhaltsverzeichnis</span><span class="sxs-lookup"><span data-stu-id="25a88-105">Table of Contents</span></span>
- [<span data-ttu-id="25a88-106">Allgemeine grundlegende Änderungen</span><span class="sxs-lookup"><span data-stu-id="25a88-106">General breaking changes</span></span>](#general-breaking-changes)
  - [<span data-ttu-id="25a88-107">Änderungen von Cmdlet-Nomen</span><span class="sxs-lookup"><span data-stu-id="25a88-107">Cmdlet Noun Prefix Changes</span></span>](#cmdlet-noun-prefix-changes)
  - [<span data-ttu-id="25a88-108">Änderungen von Modulnamen</span><span class="sxs-lookup"><span data-stu-id="25a88-108">Module name changes</span></span>](#module-name-changes)
  - [<span data-ttu-id="25a88-109">Entfernte Module</span><span class="sxs-lookup"><span data-stu-id="25a88-109">Removed modules</span></span>](#removed-modules)
  - [<span data-ttu-id="25a88-110">Windows PowerShell 5.1 und .NET 4.7.2</span><span class="sxs-lookup"><span data-stu-id="25a88-110">Windows PowerShell 5.1 and .NET 4.7.2</span></span>](#windows-powershell-51-and-net-472)
  - [<span data-ttu-id="25a88-111">Vorübergehende Entfernung der Benutzeranmeldung per PSCredential</span><span class="sxs-lookup"><span data-stu-id="25a88-111">Temporary removal of User login using PSCredential</span></span>](#temporary-removal-of-user-login-using-pscredential)
  - [<span data-ttu-id="25a88-112">Anmeldung per Standardgerätecode anstelle einer Webbrowser-Eingabeaufforderung</span><span class="sxs-lookup"><span data-stu-id="25a88-112">Default Device Code login instead of Web Browser prompt</span></span>](#temporary-default-device-code-login-instead-of-web-browser-prompt)
- [<span data-ttu-id="25a88-113">Grundlegende Änderungen am Modul</span><span class="sxs-lookup"><span data-stu-id="25a88-113">Module breaking changes</span></span>](#module-breaking-changes)
  - [<span data-ttu-id="25a88-114">Az.ApiManagement (bisher AzureRM.ApiManagement)</span><span class="sxs-lookup"><span data-stu-id="25a88-114">Az.ApiManagement (previously AzureRM.ApiManagement)</span></span>](#azapimanagement-previously-azurermapimanagement)
  - [<span data-ttu-id="25a88-115">Az.Billing (bisher AzureRM.Billing, AzureRM.Consumption und AzureRM.UsageAggregates)</span><span class="sxs-lookup"><span data-stu-id="25a88-115">Az.Billing (previously AzureRM.Billing, AzureRM.Consumption, and AzureRM.UsageAggregates)</span></span>](#azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates)
  - [<span data-ttu-id="25a88-116">Az.CognitiveServices (bisher AzureRM.CognitiveServices)</span><span class="sxs-lookup"><span data-stu-id="25a88-116">Az.CognitiveServices (previously AzureRM.CognitiveServices)</span></span>](#azcognitiveservices-previously-azurermcognitiveservices)
  - [<span data-ttu-id="25a88-117">Az.Compute (bisher AzureRM.Compute)</span><span class="sxs-lookup"><span data-stu-id="25a88-117">Az.Compute (previously AzureRM.Compute)</span></span>](#azcompute-previously-azurermcompute)
  - [<span data-ttu-id="25a88-118">Az.DataFactory (bisher AzureRM.DataFactories und AzureRM.DataFactoryV2)</span><span class="sxs-lookup"><span data-stu-id="25a88-118">Az.DataFactory (previously AzureRM.DataFactories and AzureRM.DataFactoryV2)</span></span>](#azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2)
  - [<span data-ttu-id="25a88-119">Az.DataLakeAnalytics (bisher AzureRM.DataLakeAnalytics)</span><span class="sxs-lookup"><span data-stu-id="25a88-119">Az.DataLakeAnalytics (previously AzureRM.DataLakeAnalytics)</span></span>](#azdatalakeanalytics-previously-azurermdatalakeanalytics)
  - [<span data-ttu-id="25a88-120">Az.DataLakeStore (bisher AzureRM.DataLakeStore)</span><span class="sxs-lookup"><span data-stu-id="25a88-120">Az.DataLakeStore (previously AzureRM.DataLakeStore)</span></span>](#azdatalakestore-previously-azurermdatalakestore)
  - [<span data-ttu-id="25a88-121">Az.KeyVault (bisher AzureRM.KeyVault)</span><span class="sxs-lookup"><span data-stu-id="25a88-121">Az.KeyVault (previously AzureRM.KeyVault)</span></span>](#azkeyvault-previously-azurermkeyvault)
  - [<span data-ttu-id="25a88-122">Az.Media (bisher AzureRM.Media)</span><span class="sxs-lookup"><span data-stu-id="25a88-122">Az.Media (previously AzureRM.Media)</span></span>](#azmedia-previously-azurermmedia)
  - [<span data-ttu-id="25a88-123">Az.Monitor (bisher AzureRM.Insights)</span><span class="sxs-lookup"><span data-stu-id="25a88-123">Az.Monitor (previously AzureRM.Insights)</span></span>](#azmonitor-previously-azurerminsights)
  - [<span data-ttu-id="25a88-124">Az.Network (bisher AzureRM.Network)</span><span class="sxs-lookup"><span data-stu-id="25a88-124">Az.Network (previously AzureRM.Network)</span></span>](#aznetwork-previously-azurermnetwork)
  - [<span data-ttu-id="25a88-125">Az.OperationalInsights (bisher AzureRM.OperationalInsights)</span><span class="sxs-lookup"><span data-stu-id="25a88-125">Az.OperationalInsights (previously AzureRM.OperationalInsights)</span></span>](#azoperationalinsights-previously-azurermoperationalinsights)
  - [<span data-ttu-id="25a88-126">Az.RecoveryServices (bisher AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup und AzureRM.RecoveryServices.SiteRecovery)</span><span class="sxs-lookup"><span data-stu-id="25a88-126">Az.RecoveryServices (previously AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup, and AzureRM.RecoveryServices.SiteRecovery)</span></span>](#azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery)
  - [<span data-ttu-id="25a88-127">Az.Resources (bisher AzureRM.Resources)</span><span class="sxs-lookup"><span data-stu-id="25a88-127">Az.Resources (previously AzureRM.Resources)</span></span>](#azresources-previously-azurermresources)
  - [<span data-ttu-id="25a88-128">Az.ServiceFabric (bisher AzureRM.ServiceFabric)</span><span class="sxs-lookup"><span data-stu-id="25a88-128">Az.ServiceFabric (previously AzureRM.ServiceFabric)</span></span>](#azservicefabric-previously-azurermservicefabric)
  - [<span data-ttu-id="25a88-129">Az.Sql (bisher AzureRM.Sql)</span><span class="sxs-lookup"><span data-stu-id="25a88-129">Az.Sql (previously AzureRM.Sql)</span></span>](#azsql-previously-azurermsql)
  - [<span data-ttu-id="25a88-130">Az.Storage (bisher Azure.Storage und AzureRM.Storage)</span><span class="sxs-lookup"><span data-stu-id="25a88-130">Az.Storage (previously Azure.Storage and AzureRM.Storage)</span></span>](#azstorage-previously-azurestorage-and-azurermstorage)
  - [<span data-ttu-id="25a88-131">Az.Websites (bisher AzureRM.Websites)</span><span class="sxs-lookup"><span data-stu-id="25a88-131">Az.Websites (previously AzureRM.Websites)</span></span>](#azwebsites-previously-azurermwebsites)

## <a name="general-breaking-changes"></a><span data-ttu-id="25a88-132">Allgemeine grundlegende Änderungen</span><span class="sxs-lookup"><span data-stu-id="25a88-132">General breaking changes</span></span>
### <a name="cmdlet-noun-prefix-changes"></a><span data-ttu-id="25a88-133">Änderungen von Cmdlet-Nomen</span><span class="sxs-lookup"><span data-stu-id="25a88-133">Cmdlet Noun Prefix Changes</span></span>
<span data-ttu-id="25a88-134">In AzureRM wurde für Cmdlets entweder „AzureRM“ oder „Azure“ als Nomenpräfix verwendet.</span><span class="sxs-lookup"><span data-stu-id="25a88-134">In AzureRM, cmdlets used either 'AzureRM' or 'Azure' as a noun prefix.</span></span>  <span data-ttu-id="25a88-135">Mit Az werden Namen von Cmdlets vereinfacht und normalisiert, damit für alle Cmdlets „Az“ als Nomenpräfix verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="25a88-135">Az simplifies and normalizes cmndlet names, so that all cmdlets use 'Az' as their cmdlet noun prefix.</span></span> <span data-ttu-id="25a88-136">Beispiel: </span><span class="sxs-lookup"><span data-stu-id="25a88-136">For example:</span></span>
```powershell
Get-AzureRMVM
Get-AzureKeyVaultSecret
```

<span data-ttu-id="25a88-137">Geändert in:</span><span class="sxs-lookup"><span data-stu-id="25a88-137">Have changed to</span></span>
```powershell
Get-AzVM
Get-AzKeyVaultSecret
```

<span data-ttu-id="25a88-138">Um die Umstellung auf diese neuen Cmdlet-Namen zu vereinfachen, werden mit Az die beiden neuen Cmdlets ```Enable-AzureRmAlias``` und ```Disable-AzureRmAlias``` eingeführt.</span><span class="sxs-lookup"><span data-stu-id="25a88-138">To make the transition to these new cmdlet names simpler, Az introduces two new cmdlets, ```Enable-AzureRmAlias``` and ```Disable-AzureRmAlias```.</span></span>  <span data-ttu-id="25a88-139">Mit ```Enable-AzureRmAlias``` werden aus den älteren Cmdlet-Namen in AzureRM Aliase für die neueren Az-Cmdlet-Namen erstellt.</span><span class="sxs-lookup"><span data-stu-id="25a88-139">```Enable-AzureRmAlias``` creates aliases from the older cmdlet names in AzureRM to the newer Az cmdlet names.</span></span>  <span data-ttu-id="25a88-140">Das Cmdlet ermöglicht die Erstellung von Aliasen in der aktuellen Sitzung oder übergreifend für alle Sitzungen, indem Ihr Benutzer- oder Computerprofil geändert wird.</span><span class="sxs-lookup"><span data-stu-id="25a88-140">The cmdlet allows creating aliases in the current session, or across all sessions by changing your user or machine profile.</span></span> 

<span data-ttu-id="25a88-141">Ein Beispiel hierfür ist das folgende Skript in AzureRM:</span><span class="sxs-lookup"><span data-stu-id="25a88-141">For example, the following script in AzureRM:</span></span>
```powershell
#Requires -Modules AzureRM.Storage
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="25a88-142">Es kann mit ```Enable-AzureRmAlias``` mit minimalen Änderungen ausgeführt werden:</span><span class="sxs-lookup"><span data-stu-id="25a88-142">Could be run with minimal changes using ```Enable-AzureRmAlias```:</span></span>
```powershell
#Requires -Modules Az.Storage
Enable-AzureRmAlias
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="25a88-143">Durch das Ausführen von ```Enable-AzureRmAlias -Scope CurrentUser``` werden die Aliase für alle von Ihnen geöffneten PowerShell-Sitzungen aktiviert. Nach der Ausführung dieses Cmdlets sind für ein Skript dieser Art keinerlei Änderungen erforderlich:</span><span class="sxs-lookup"><span data-stu-id="25a88-143">Running ```Enable-AzureRmAlias -Scope CurrentUser``` will enable the aliases for all powershell sessions you open, so that after executing this cmdlet, a script like this would not need to be changed at all:</span></span>
```powershell
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="25a88-144">Führen Sie ```Get-Help -Online Enable-AzureRmAlias``` über die PowerShell-Eingabeaufforderung aus, um ausführliche Informationen zur Nutzung der Alias-Cmdlets zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="25a88-144">For complete details on the usage of the alias cmdlets, execute ```Get-Help -Online Enable-AzureRmAlias``` from the powershell prompt.</span></span>

<span data-ttu-id="25a88-145">Mit ```Disable-AzureRmAlias``` werden AzureRM-Cmdlet-Aliase entfernt, die mit ```Enable-AzureRmAlias``` erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="25a88-145">```Disable-AzureRmAlias``` removes AzureRM cmdlet aliases created by ```Enable-AzureRmAlias```.</span></span>  <span data-ttu-id="25a88-146">Führen Sie ```Get-Help -Online Disable-AzureRmAlias``` an der PowerShell-Eingabeaufforderung aus, um alle Details anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="25a88-146">For complete details, execute ```Get-Help -Online Disable-AzureRmAlias``` from the powershell prompt.</span></span>

### <a name="module-name-changes"></a><span data-ttu-id="25a88-147">Änderungen von Modulnamen</span><span class="sxs-lookup"><span data-stu-id="25a88-147">Module Name Changes</span></span>
- <span data-ttu-id="25a88-148">Die Modulnamen wurden von `AzureRM.*` in `Az.*` geändert, mit Ausnahme der folgenden Module:</span><span class="sxs-lookup"><span data-stu-id="25a88-148">The module names have changed from `AzureRM.*` to `Az.*`, except for the following modules:</span></span>
```
AzureRM.Profile                       -> Az.Accounts
Azure.AnalysisServices                -> Az.AnalysisServices
AzureRM.Consumption                   -> Az.Billing
AzureRM.UsageAggregates               -> Az.Billing
AzureRM.DataFactories                 -> Az.DataFactory
AzureRM.DataFactoryV2                 -> Az.DataFactory
AzureRM.MachineLearningCompute        -> Az.MachineLearning
AzureRM.Insights                      -> Az.Monitor
AzureRM.RecoveryServices.Backup       -> Az.RecoveryServices
AzureRM.RecoveryServices.SiteRecovery -> Az.RecoveryServices
AzureRM.Tags                          -> Az.Resources
Azure.Storage                         -> Az.Storage
```

<span data-ttu-id="25a88-149">Die Änderungen der Modulnamen bedeuten, dass alle Skripts, die ```#Requires``` oder ```Import-Module``` zum Laden von bestimmten Modulen nutzen, auf die Verwendung des neuen Moduls umgestellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="25a88-149">The changes in module names mean that any script that uses ```#Requires``` or ```Import-Module``` to load specific modules will need to be changed to use the new module instead.</span></span>

#### <a name="migrating-requires-statements"></a><span data-ttu-id="25a88-150">Migrieren von #Requires-Anweisungen</span><span class="sxs-lookup"><span data-stu-id="25a88-150">Migrating #Requires Statements</span></span>
<span data-ttu-id="25a88-151">Skripts, für die #Requires zum Deklarieren einer Abhängigkeit von AzureRM-Modulen verwendet wird, sollten aktualisiert werden, damit die neuen Modulnamen genutzt werden.</span><span class="sxs-lookup"><span data-stu-id="25a88-151">Scripts that use #Requires to declare a dependency on AzureRM modules should be updated to use the new module names</span></span>
```powershell
#Requires -Module AzureRM.Compute
```

<span data-ttu-id="25a88-152">Änderung erforderlich in:</span><span class="sxs-lookup"><span data-stu-id="25a88-152">Should be changed to</span></span>
```powershell
#Requires -Module Az.Compute
```

#### <a name="migrating-import-module-statements"></a><span data-ttu-id="25a88-153">Migrieren von Import-Module-Anweisungen</span><span class="sxs-lookup"><span data-stu-id="25a88-153">Migrating Import-Module Statements</span></span>
<span data-ttu-id="25a88-154">Skripts, für die ```Import-Module``` zum Laden der AzureRM-Module verwendet wird, müssen aktualisiert werden, damit die neuen Modulnamen widergespiegelt werden.</span><span class="sxs-lookup"><span data-stu-id="25a88-154">Scripts that use ```Import-Module``` to load AzureRM modules will need to be updated to reflect the new module names.</span></span>
```powershell
Import-Module -Name AzureRM.Compute
```

<span data-ttu-id="25a88-155">Änderung erforderlich in:</span><span class="sxs-lookup"><span data-stu-id="25a88-155">Should be changed to</span></span>
```powershell
Import-Module -Name Az.Compute
```

### <a name="migrating-fully-qualified-cmdlet-invocations"></a><span data-ttu-id="25a88-156">Migrieren von vollqualifizierten Cmdlet-Aufrufen</span><span class="sxs-lookup"><span data-stu-id="25a88-156">Migrating Fully-Qualified Cmdlet Invocations</span></span>
<span data-ttu-id="25a88-157">Bei Verwendung von Skripts, für die Cmdlet-Aufrufe mit Modulqualifikation verwendet werden, z.B.:</span><span class="sxs-lookup"><span data-stu-id="25a88-157">Scripts that use module-qualified cmdlet invocations, like</span></span>
```powershell
AzureRM.Compute\Get-AzureRmVM
```

<span data-ttu-id="25a88-158">Diese sollten geändert werden, damit die neuen Modul- und Cmdlet-Namen verwendet werden:</span><span class="sxs-lookup"><span data-stu-id="25a88-158">Should be changed to use the new module and cmdlet names</span></span>
```powershell
Az.Compute\Get-AzVM
```

### <a name="migrating-module-manifest-dependencies"></a><span data-ttu-id="25a88-159">Migrieren von Modulmanifestabhängigkeiten</span><span class="sxs-lookup"><span data-stu-id="25a88-159">Migrating Module Manifest Dependencies</span></span>
<span data-ttu-id="25a88-160">Für Module, die Abhängigkeiten von AzureRM-Modulen anhand einer Modulmanifestdatei (.psd1) ausdrücken, müssen die Modulnamen jeweils im Abschnitt „RequiredModules“ aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="25a88-160">Modules that express dependencies on AzureRM modules through a module manifest (.psd1) file will need to updated the module names in their 'RequiredModules' section</span></span>

```powershell
RequiredModules = @(@{ModuleName="AzureRM.Profile"; ModuleVersion="5.8.2"})
```

<span data-ttu-id="25a88-161">Änderung erforderlich in:</span><span class="sxs-lookup"><span data-stu-id="25a88-161">Should be changed to</span></span>

```powershell
RequiredModules = @(@{ModuleName="Az.Profile"; ModuleVersion="1.0.0"})
```

### <a name="removed-modules"></a><span data-ttu-id="25a88-162">Entfernte Module</span><span class="sxs-lookup"><span data-stu-id="25a88-162">Removed modules</span></span>
- `AzureRM.Backup`
- `AzureRM.Compute.ManagedService`
- `AzureRM.Scheduler`

<span data-ttu-id="25a88-163">Die Tools für diese Dienste werden nicht mehr aktiv unterstützt.</span><span class="sxs-lookup"><span data-stu-id="25a88-163">The tooling for these services are no longer actively supported.</span></span>  <span data-ttu-id="25a88-164">Kunden wird die zeitnahe Umstellung auf alternative Dienste empfohlen.</span><span class="sxs-lookup"><span data-stu-id="25a88-164">Customers are encouraged to move to alternative services as soon as it is convenient.</span></span>

### <a name="windows-powershell-51-and-net-472"></a><span data-ttu-id="25a88-165">Windows PowerShell 5.1 und .NET 4.7.2</span><span class="sxs-lookup"><span data-stu-id="25a88-165">Windows PowerShell 5.1 and .NET 4.7.2</span></span>
- <span data-ttu-id="25a88-166">Für die Verwendung von Az mit Windows PowerShell 5.1 ist die Installation von .NET 4.7.2 erforderlich.</span><span class="sxs-lookup"><span data-stu-id="25a88-166">Using Az with Windows PowerShell 5.1 requires the installation of .NET 4.7.2.</span></span> <span data-ttu-id="25a88-167">Für die Nutzung von Az mit PowerShell Core wird .NET 4.7.2 aber nicht benötigt.</span><span class="sxs-lookup"><span data-stu-id="25a88-167">However, using Az with PowerShell Core does not require .NET 4.7.2.</span></span> 

### <a name="temporary-removal-of-user-login-using-pscredential"></a><span data-ttu-id="25a88-168">Vorübergehende Entfernung der Benutzeranmeldung per PSCredential</span><span class="sxs-lookup"><span data-stu-id="25a88-168">Temporary removal of User login using PSCredential</span></span>
- <span data-ttu-id="25a88-169">Aufgrund von Änderungen am Authentifizierungsablauf für .NET Standard entfernen wir die Benutzeranmeldung per PSCredential vorübergehend.</span><span class="sxs-lookup"><span data-stu-id="25a88-169">Due to changes in the authentication flow for .NET Standard, we are temporarily removing user login via PSCredential.</span></span> <span data-ttu-id="25a88-170">Diese Funktion wird mit dem Windows PowerShell 5.1-Release vom 15.01.2019 wieder eingeführt.</span><span class="sxs-lookup"><span data-stu-id="25a88-170">This capability will be re-introduced in the 1/15/2019 release for Windows PowerShell 5.1.</span></span> <span data-ttu-id="25a88-171">Eine ausführliche Beschreibung finden Sie unter [diesem Problem](https://github.com/Azure/azure-powershell/issues/7430).</span><span class="sxs-lookup"><span data-stu-id="25a88-171">This is duscussed in detail in [this issue.](https://github.com/Azure/azure-powershell/issues/7430)</span></span>

### <a name="default-device-code-login-instead-of-web-browser-prompt"></a><span data-ttu-id="25a88-172">Anmeldung per Standardgerätecode anstelle einer Webbrowser-Eingabeaufforderung</span><span class="sxs-lookup"><span data-stu-id="25a88-172">Default Device Code login instead of Web Browser prompt</span></span>
- <span data-ttu-id="25a88-173">Aufgrund von Änderungen am Authentifizierungsablauf für .NET Standard nutzen wir die Geräteanmeldung während der interaktiven Anmeldung als Standardanmeldungsablauf.</span><span class="sxs-lookup"><span data-stu-id="25a88-173">Due to changes in the authentication flow for .NET Standard, we are using device login as the default login flow during interactive login.</span></span> <span data-ttu-id="25a88-174">Die Anmeldung per Webbrowser wird im Windows PowerShell 5.1-Release vom 15.01.2019 wieder als Standard eingeführt.</span><span class="sxs-lookup"><span data-stu-id="25a88-174">Web browser based login will be re-introduced for Windows PowerShell 5.1 as the default in the 1/15/2019 release.</span></span> <span data-ttu-id="25a88-175">Benutzer können dann die Geräteanmeldung mit einem Switch-Parameter wählen.</span><span class="sxs-lookup"><span data-stu-id="25a88-175">At that time, users will be able to choose device login using a Switch parameter.</span></span>

## <a name="module-breaking-changes"></a><span data-ttu-id="25a88-176">Grundlegende Änderungen am Modul</span><span class="sxs-lookup"><span data-stu-id="25a88-176">Module breaking changes</span></span>

### <a name="azapimanagement-previously-azurermapimanagement"></a><span data-ttu-id="25a88-177">Az.ApiManagement (bisher AzureRM.ApiManagement)</span><span class="sxs-lookup"><span data-stu-id="25a88-177">Az.ApiManagement (previously AzureRM.ApiManagement)</span></span>
- <span data-ttu-id="25a88-178">Entfernen Sie die folgenden Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="25a88-178">Removing the following cmdlets:</span></span>
  - <span data-ttu-id="25a88-179">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="25a88-179">New-AzureRmApiManagementHostnameConfiguration</span></span>
  - <span data-ttu-id="25a88-180">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="25a88-180">Set-AzureRmApiManagementHostnames</span></span>
  - <span data-ttu-id="25a88-181">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="25a88-181">Update-AzureRmApiManagementDeployment</span></span>
  - <span data-ttu-id="25a88-182">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="25a88-182">Import-AzureRmApiManagementHostnameCertificate</span></span>
  - <span data-ttu-id="25a88-183">Verwenden Sie stattdessen das Cmdlet **Set-AzApiManagement**, um diese Eigenschaften festzulegen.</span><span class="sxs-lookup"><span data-stu-id="25a88-183">Use **Set-AzApiManagement** cmdlet to set these properites instead</span></span>
- <span data-ttu-id="25a88-184">Die folgenden Eigenschaften wurden entfernt:</span><span class="sxs-lookup"><span data-stu-id="25a88-184">Following properties were removed</span></span>
  - <span data-ttu-id="25a88-185">Die Eigenschaften `PortalHostnameConfiguration`, `ProxyHostnameConfiguration`, `ManagementHostnameConfiguration` und `ScmHostnameConfiguration` vom Typ `PsApiManagementHostnameConfiguration` wurden aus `PsApiManagementContext` entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-185">Removed property `PortalHostnameConfiguration`, `ProxyHostnameConfiguration`, `ManagementHostnameConfiguration` and `ScmHostnameConfiguration` of type `PsApiManagementHostnameConfiguration` from `PsApiManagementContext`.</span></span> <span data-ttu-id="25a88-186">Verwenden Sie stattdessen `PortalCustomHostnameConfiguration`, `ProxyCustomHostnameConfiguration`, `ManagementCustomHostnameConfiguration` und `ScmCustomHostnameConfiguration` vom Typ `PsApiManagementCustomHostNameConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="25a88-186">Instead use `PortalCustomHostnameConfiguration`, `ProxyCustomHostnameConfiguration`, `ManagementCustomHostnameConfiguration` and `ScmCustomHostnameConfiguration` of type `PsApiManagementCustomHostNameConfiguration`.</span></span>
  - <span data-ttu-id="25a88-187">Die `StaticIPs`-Eigenschaft wurde aus PsApiManagementContext entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-187">Removed property `StaticIPs` from PsApiManagementContext.</span></span> <span data-ttu-id="25a88-188">Die Eigenschaft wurde in `PublicIPAddresses` und `PrivateIPAddresses` unterteilt.</span><span class="sxs-lookup"><span data-stu-id="25a88-188">The property has been split into `PublicIPAddresses` and `PrivateIPAddresses`.</span></span>
  - <span data-ttu-id="25a88-189">Die erforderliche `Location`-Eigenschaft wurde aus dem Cmdlet New-AzureApiManagementVirtualNetwork entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-189">Removed required property `Location` from New-AzureApiManagementVirtualNetwork cmdlet.</span></span>

### <a name="azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates"></a><span data-ttu-id="25a88-190">Az.Billing (bisher AzureRM.Billing, AzureRM.Consumption und AzureRM.UsageAggregates)</span><span class="sxs-lookup"><span data-stu-id="25a88-190">Az.Billing (previously AzureRM.Billing, AzureRM.Consumption, and AzureRM.UsageAggregates)</span></span>
- <span data-ttu-id="25a88-191">Der Parameter `InvoiceName` wurde aus dem Cmdlet `Get-AzConsumptionUsageDetail` entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-191">The `InvoiceName` parameter was removed from the `Get-AzConsumptionUsageDetail` cmdlet.</span></span>  <span data-ttu-id="25a88-192">Für Skripts müssen andere Identitätsparameter für die Rechnung genutzt werden.</span><span class="sxs-lookup"><span data-stu-id="25a88-192">Scripts will need to use other identity parameters for the invoice.</span></span>

### <a name="azcognitiveservices-previously-azurermcognitiveservices"></a><span data-ttu-id="25a88-193">Az.CognitiveServices (bisher AzureRM.CognitiveServices)</span><span class="sxs-lookup"><span data-stu-id="25a88-193">Az.CognitiveServices (previously AzureRM.CognitiveServices)</span></span>
- <span data-ttu-id="25a88-194">Der Parametersatz `GetSkusWithAccountParamSetName` wurde aus dem Cmdlet `Get-AzCognitiveServicesAccountSkus` entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-194">Removed `GetSkusWithAccountParamSetName` parameter set from `Get-AzCognitiveServicesAccountSkus` cmdlet.</span></span>  <span data-ttu-id="25a88-195">Sie müssen SKUs nach Kontotyp und Standort abrufen, anstatt ResourceGroupName und den Kontonamen zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="25a88-195">You must get Skus by Account Type and Location, instead of using ResourceGroupName and Account Name.</span></span>

### <a name="azcompute-previously-azurermcompute"></a><span data-ttu-id="25a88-196">Az.Compute (bisher AzureRM.Compute)</span><span class="sxs-lookup"><span data-stu-id="25a88-196">Az.Compute (previously AzureRM.Compute)</span></span>
- <span data-ttu-id="25a88-197">`IdentityIds` wurden aus der `Identity`-Eigenschaft in den Objekten `PSVirtualMachine` und `PSVirtualMachineScaleSet` entfernt. In Skripts sollte der Wert dieses Felds nicht mehr verwendet werden, um Verarbeitungsentscheidungen zu treffen.</span><span class="sxs-lookup"><span data-stu-id="25a88-197">`IdentityIds` are removed from `Identity` property in `PSVirtualMachine` and `PSVirtualMachineScaleSet` objects Scripts should no longer use the value of this field to make processing decisions.</span></span>
- <span data-ttu-id="25a88-198">Der Typ der `InstanceView`-Eigenschaft des `PSVirtualMachineScaleSetVM`-Objekts wurde von `VirtualMachineInstanceView` in `VirtualMachineScaleSetVMInstanceView` geändert.</span><span class="sxs-lookup"><span data-stu-id="25a88-198">The type of `InstanceView` property of `PSVirtualMachineScaleSetVM` object is changed from `VirtualMachineInstanceView` to `VirtualMachineScaleSetVMInstanceView`</span></span>
- <span data-ttu-id="25a88-199">Die Eigenschaften `AutoOSUpgradePolicy` und `AutomaticOSUpgrade` wurden aus der `UpgradePolicy`-Eigenschaft entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-199">`AutoOSUpgradePolicy` and `AutomaticOSUpgrade` properties are removed from `UpgradePolicy` property</span></span>
- <span data-ttu-id="25a88-200">Der Typ der `Sku`-Eigenschaft im `PSSnapshotUpdate`-Objekt wurde von `DiskSku` in `SnapshotSku` geändert.</span><span class="sxs-lookup"><span data-stu-id="25a88-200">The type of `Sku` property in `PSSnapshotUpdate` object is changed from `DiskSku` to `SnapshotSku`</span></span>
- <span data-ttu-id="25a88-201">`VmScaleSetVMParameterSet` wurde aus dem Cmdlet `Add-AzVMDataDisk` entfernt. Sie können einer ScaleSet-VM nicht mehr einzeln einen Datenträger für Daten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="25a88-201">`VmScaleSetVMParameterSet` is removed from `Add-AzVMDataDisk` cmdlet, you cna no longer add a data disk individually to a ScaleSet VM.</span></span>

### <a name="azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2"></a><span data-ttu-id="25a88-202">Az.DataFactory (bisher AzureRM.DataFactories und AzureRM.DataFactoryV2)</span><span class="sxs-lookup"><span data-stu-id="25a88-202">Az.DataFactory (previously AzureRM.DataFactories and AzureRM.DataFactoryV2)</span></span>
- <span data-ttu-id="25a88-203">Der Parameter `GatewayName` ist im Cmdlet `New-AzDataFactoryEncryptValue` jetzt obligatorisch.</span><span class="sxs-lookup"><span data-stu-id="25a88-203">The `GatewayName` parameter has become mandatory in the `New-AzDataFactoryEncryptValue` cmdlet</span></span>
- <span data-ttu-id="25a88-204">Das Cmdlet `New-AzDataFactoryGatewayKey` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-204">Removed `New-AzDataFactoryGatewayKey` cmdlet</span></span>
- <span data-ttu-id="25a88-205">Der Parameter `LinkedServiceName` wurde aus dem Cmdlet `Get-AzDataFactoryV2ActivityRun` entfernt. In Skripts sollte der Wert dieses Felds nicht mehr verwendet werden, um Verarbeitungsentscheidungen zu treffen.</span><span class="sxs-lookup"><span data-stu-id="25a88-205">Removed `LinkedServiceName` parameter from `Get-AzDataFactoryV2ActivityRun` cmdlet Scripts should no longer use the value of this field to make processing decisions.</span></span>

### <a name="azdatalakeanalytics-previously-azurermdatalakeanalytics"></a><span data-ttu-id="25a88-206">Az.DataLakeAnalytics (bisher AzureRM.DataLakeAnalytics)</span><span class="sxs-lookup"><span data-stu-id="25a88-206">Az.DataLakeAnalytics (previously AzureRM.DataLakeAnalytics)</span></span>
- <span data-ttu-id="25a88-207">Veraltete Cmdlets wurden entfernt: `New-AzDataLakeAnalyticsCatalogSecret`, `Remove-AzDataLakeAnalyticsCatalogSecret` und `Set-AzDataLakeAnalyticsCatalogSecret`.</span><span class="sxs-lookup"><span data-stu-id="25a88-207">Removed deprecated cmdlets: `New-AzDataLakeAnalyticsCatalogSecret`, `Remove-AzDataLakeAnalyticsCatalogSecret`, and `Set-AzDataLakeAnalyticsCatalogSecret`</span></span>

### <a name="azdatalakestore-previously-azurermdatalakestore"></a><span data-ttu-id="25a88-208">Az.DataLakeStore (bisher AzureRM.DataLakeStore)</span><span class="sxs-lookup"><span data-stu-id="25a88-208">Az.DataLakeStore (previously AzureRM.DataLakeStore)</span></span>
- <span data-ttu-id="25a88-209">Für die folgenden Cmdlets wurde der Typ des Parameters `Encoding` von `FileSystemCmdletProviderEncoding` in `System.Text.Encoding` geändert.</span><span class="sxs-lookup"><span data-stu-id="25a88-209">The following cmdlets have had the `Encoding` parameter changed from the type `FileSystemCmdletProviderEncoding` to `System.Text.Encoding`.</span></span> <span data-ttu-id="25a88-210">Bei dieser Änderung wurden die Codierungswerte `String` und `Oem` entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-210">This change removes the encoding values `String` and `Oem`.</span></span> <span data-ttu-id="25a88-211">Alle anderen bisherigen Codierungswerte bleiben erhalten.</span><span class="sxs-lookup"><span data-stu-id="25a88-211">All the other prior encoding values remain.</span></span>
  - <span data-ttu-id="25a88-212">New-AzureRmDataLakeStoreItem</span><span class="sxs-lookup"><span data-stu-id="25a88-212">New-AzureRmDataLakeStoreItem</span></span>
  - <span data-ttu-id="25a88-213">Add-AzureRmDataLakeStoreItemContent</span><span class="sxs-lookup"><span data-stu-id="25a88-213">Add-AzureRmDataLakeStoreItemContent</span></span>
  - <span data-ttu-id="25a88-214">Get-AzureRmDataLakeStoreItemContent</span><span class="sxs-lookup"><span data-stu-id="25a88-214">Get-AzureRmDataLakeStoreItemContent</span></span>
- <span data-ttu-id="25a88-215">Der veraltete Eigenschaftenalias `Tags` wurde aus den Cmdlets `New-AzDataLakeStoreAccount` und `Set-AzDataLakeStoreAccount` entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-215">Removed deprecated `Tags` property alias from `New-AzDataLakeStoreAccount` and `Set-AzDataLakeStoreAccount` cmdlets</span></span>

  <span data-ttu-id="25a88-216">Skripts mit Verwendung von:</span><span class="sxs-lookup"><span data-stu-id="25a88-216">Scripts using</span></span>
  ```powershell
  New-AzureRMDataLakeStoreAccount -Tags @{TagName="TagValue"}
  ```

  <span data-ttu-id="25a88-217">Änderung erforderlich in:</span><span class="sxs-lookup"><span data-stu-id="25a88-217">Should be changed to</span></span>
  ```powershell
  New-AzDataLakeStoreAccount -Tag @{TagName="TagValue"}
  ```

- <span data-ttu-id="25a88-218">Die veralteten Eigenschaften ```Identity```, ```EncryptionState```, ```EncrypotionProvisioningState```, ```EncryptionConfig```, ```FirewallState```, ```FirewallRules```, ```VirtualNetworkRules```, ```TrustedIdProviderState```, ```TrustedIdProviders```, ```DefaultGroup```, ```NewTier```, ```CurrentTier``` und ```FirewallAllowAzureIps``` wurden aus dem ```PSDataLakeStoreAccountBasic```-Objekt entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-218">Removed deprecated properties ```Identity```, ```EncryptionState```, ```EncrypotionProvisioningState```, ```EncryptionConfig```, ```FirewallState```, ```FirewallRules```, ```VirtualNetworkRules```, ```TrustedIdProviderState```, ```TrustedIdProviders```, ```DefaultGroup```, ```NewTier```, ```CurrentTier```, ```FirewallAllowAzureIps``` from ```PSDataLakeStoreAccountBasic``` object.</span></span>  <span data-ttu-id="25a88-219">Alle Skripts, für die das von ```Get-AzDataLakeStoreAccount``` zurückgegebene ```PSDatalakeStoreAccount```-Objekt verwendet wird, sollten nicht auf diese Eigenschaften verweisen.</span><span class="sxs-lookup"><span data-stu-id="25a88-219">Any script that uses the ```PSDatalakeStoreAccount``` returned from ```Get-AzDataLakeStoreAccount``` should not reference these properties.</span></span>

### <a name="azkeyvault-previously-azurermkeyvault"></a><span data-ttu-id="25a88-220">Az.KeyVault (bisher AzureRM.KeyVault)</span><span class="sxs-lookup"><span data-stu-id="25a88-220">Az.KeyVault (previously AzureRM.KeyVault)</span></span>
- <span data-ttu-id="25a88-221">Die `PurgeDisabled`-Eigenschaft wurde aus den Objekten `PSKeyVaultKeyAttributes`, `PSKeyVaultKeyIdentityItem` und `PSKeyVaultSecretAttributes` entfernt. In Skripts sollte nicht mehr auf die ```PurgeDisabled```-Eigenschaft verwiesen werden, um Verarbeitungsentscheidungen zu treffen.</span><span class="sxs-lookup"><span data-stu-id="25a88-221">The `PurgeDisabled` property was removed from the `PSKeyVaultKeyAttributes`, `PSKeyVaultKeyIdentityItem`, and `PSKeyVaultSecretAttributes` objects Scripts shoudl no longer reference the ```PurgeDisabled``` property to make processing decisions.</span></span>

### <a name="azmedia-previously-azurermmedia"></a><span data-ttu-id="25a88-222">Az.Media (bisher AzureRM.Media)</span><span class="sxs-lookup"><span data-stu-id="25a88-222">Az.Media (previously AzureRM.Media)</span></span>
- <span data-ttu-id="25a88-223">Der veraltete Eigenschaftenalias `Tags` wurde aus dem Cmdlet `New-AzMediaService` entfernt. Skripts mit Verwendung von:</span><span class="sxs-lookup"><span data-stu-id="25a88-223">Remove deprecated `Tags` property alias from `New-AzMediaService` cmdlet Scripts using</span></span>
  ```powershell
  New-AzureRMMediaService -Tags @{TagName="TagValue"}
  ```

  <span data-ttu-id="25a88-224">Änderung erforderlich in:</span><span class="sxs-lookup"><span data-stu-id="25a88-224">Should be changed to</span></span>
  ```powershell
  New-AzMMediaService -Tag @{TagName="TagValue"}
  ```
### <a name="azmonitor-previously-azurerminsights"></a><span data-ttu-id="25a88-225">Az.Monitor (bisher AzureRM.Insights)</span><span class="sxs-lookup"><span data-stu-id="25a88-225">Az.Monitor (previously AzureRM.Insights)</span></span>
- <span data-ttu-id="25a88-226">Die Plural-Parameternamen `Categories` und `Timegrains` wurden in Singular-Parameternamen aus dem Cmdlet `Set-AzDiagnosticSetting` geändert. Skripts mit Verwendung von:</span><span class="sxs-lookup"><span data-stu-id="25a88-226">Removed plural names `Categories` and `Timegrains` parameter in favor of singular parameter names from `Set-AzDiagnosticSetting` cmdlet Scripts using</span></span>
  ```powershell
  Set-AzureRmDiagnosticSetting -Timegrains PT1M -Categories Category1, Category2
  ```

  <span data-ttu-id="25a88-227">Änderung erforderlich in:</span><span class="sxs-lookup"><span data-stu-id="25a88-227">Should be changed to</span></span>
  ```powershell
  Set-AzDiagnosticSetting -Timegrain PT1M -Category Category1, Category2
  ```
### <a name="aznetwork-previously-azurermnetwork"></a><span data-ttu-id="25a88-228">Az.Network (bisher AzureRM.Network)</span><span class="sxs-lookup"><span data-stu-id="25a88-228">Az.Network (previously AzureRM.Network)</span></span>
- <span data-ttu-id="25a88-229">Der veraltete Parameter `ResourceId` wurde aus dem Cmdlet `Get-AzServiceEndpointPolicyDefinition` entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-229">Removed deprecated `ResourceId` parameter from `Get-AzServiceEndpointPolicyDefinition` cmdlet</span></span>
- <span data-ttu-id="25a88-230">Die verwaltete `EnableVmProtection`-Eigenschaft wurde aus dem `PSVirtualNetwork`-Objekt entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-230">Removed deprecated `EnableVmProtection` property from `PSVirtualNetwork` object</span></span>
- <span data-ttu-id="25a88-231">Das veraltete Cmdlet `Set-AzVirtualNetworkGatewayVpnClientConfig` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-231">Removed deprecated `Set-AzVirtualNetworkGatewayVpnClientConfig` cmdlet</span></span>
  
<span data-ttu-id="25a88-232">Für Skripts sollten basierend auf den Werten dieser Felder keine Verarbeitungsentscheidungen mehr getroffen werden.</span><span class="sxs-lookup"><span data-stu-id="25a88-232">Scripts shoudl no longer make processing decisions based on the values fo these fields.</span></span>

### <a name="azoperationalinsights-previously-azurermoperationalinsights"></a><span data-ttu-id="25a88-233">Az.OperationalInsights (bisher AzureRM.OperationalInsights)</span><span class="sxs-lookup"><span data-stu-id="25a88-233">Az.OperationalInsights (previously AzureRM.OperationalInsights)</span></span>
- <span data-ttu-id="25a88-234">Der Standardparametersatz für `Get-AzOperationalInsightsDataSource` wurde entfernt, und `ByWorkspaceNameByKind` ist zum Standardparametersatz geworden.</span><span class="sxs-lookup"><span data-stu-id="25a88-234">Default parameter set for `Get-AzOperationalInsightsDataSource` is removed, and `ByWorkspaceNameByKind` has become the default parameter set</span></span>

  <span data-ttu-id="25a88-235">Skripts mit Auflistung von Datenquellen mit:</span><span class="sxs-lookup"><span data-stu-id="25a88-235">Scripts that listed data sources using</span></span>
  ```powershell
  Get-AzureRmOperationalInsightsDataSource
  ```

  <span data-ttu-id="25a88-236">Änderung mit Angabe der Art erforderlich:</span><span class="sxs-lookup"><span data-stu-id="25a88-236">Should be changed to specify a Kind</span></span>
  ```powershell
  Get-AzOperationalInsightsDataSource -Kind AzureActivityLog
  ```

### <a name="azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery"></a><span data-ttu-id="25a88-237">Az.RecoveryServices (bisher AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup und AzureRM.RecoveryServices.SiteRecovery)</span><span class="sxs-lookup"><span data-stu-id="25a88-237">Az.RecoveryServices (previously AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup, and AzureRM.RecoveryServices.SiteRecovery)</span></span>
- <span data-ttu-id="25a88-238">Der Parameter `Encryption` wurde aus dem Cmdlet `New/Set-AzRecoveryServicesAsrPolicy` entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-238">Removed `Encryption` parameter from `New/Set-AzRecoveryServicesAsrPolicy` cmdlet</span></span>
- <span data-ttu-id="25a88-239">Der Parameter `TargetStorageAccountName` ist für Wiederherstellungen von verwalteten Datenträgern im Cmdlet `Restore-AzRecoveryServicesBackupItem` jetzt obligatorisch.</span><span class="sxs-lookup"><span data-stu-id="25a88-239">`TargetStorageAccountName` parameter is now mandatory for managed disk restores in `Restore-AzRecoveryServicesBackupItem` cmdlet</span></span>
- <span data-ttu-id="25a88-240">Die Parameter `StorageAccountName` und `StorageAccountResourceGroupName` im Cmdlet `Restore-AzRecoveryServicesBackupItem` wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-240">Removed `StorageAccountName` and `StorageAccountResourceGroupName` parameters in `Restore-AzRecoveryServicesBackupItem` cmdlet</span></span>
- <span data-ttu-id="25a88-241">Der Parameter `Name` im Cmdlet `Get-AzRecoveryServicesBackupContainer` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-241">Removed `Name`parameter in `Get-AzRecoveryServicesBackupContainer` cmdlet</span></span>

### <a name="azresources-previously-azurermresources"></a><span data-ttu-id="25a88-242">Az.Resources (bisher AzureRM.Resources)</span><span class="sxs-lookup"><span data-stu-id="25a88-242">Az.Resources (previously AzureRM.Resources)</span></span>
- <span data-ttu-id="25a88-243">Der Parameter `Sku` wurde aus dem Cmdlet `New/Set-AzPolicyAssignment` entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-243">Removed `Sku` parameter from `New/Set-AzPolicyAssignment` cmdlet</span></span>
- <span data-ttu-id="25a88-244">Der Parameter `Password` wurde aus den Cmdlets `New-AzADServicePrincipal` und `New-AzADSpCredential` entfernt. Die Kennwörter werden automatisch generiert. Bei Verwendung von Skripts mit Bereitstellung des Kennworts:</span><span class="sxs-lookup"><span data-stu-id="25a88-244">Removed `Password` parameter from `New-AzADServicePrincipal` and `New-AzADSpCredential` cmdlet Passwords are automatically generated, scripts that provided the password:</span></span>
  ```powershell
  New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476 -Password $secPassword
  ```

  <span data-ttu-id="25a88-245">Änderung erforderlich, damit das Kennwort aus der Ausgabe verwendet wird:</span><span class="sxs-lookup"><span data-stu-id="25a88-245">Should be changed to retriedve the password from the output:</span></span>
  ```powershell
  $credential = New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476
  $secPassword = $credential.Secret
  ```

### <a name="azservicefabric-previously-azurermservicefabric"></a><span data-ttu-id="25a88-246">Az.ServiceFabric (bisher AzureRM.ServiceFabric)</span><span class="sxs-lookup"><span data-stu-id="25a88-246">Az.ServiceFabric (previously AzureRM.ServiceFabric)</span></span>
- <span data-ttu-id="25a88-247">Die folgenden Cmdlet-Rückgabetypen wurden geändert:</span><span class="sxs-lookup"><span data-stu-id="25a88-247">The following cmdlet return types have been changed:</span></span>
  - <span data-ttu-id="25a88-248">Die `SerivceTypeHealthPolicies`-Eigenschaft vom Typ `ApplicationHealthPolicy` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-248">The property `SerivceTypeHealthPolicies` of type `ApplicationHealthPolicy` has been removed.</span></span>
  - <span data-ttu-id="25a88-249">Die `ApplicationHealthPolicies`-Eigenschaft vom Typ `ClusterUpgradeDeltaHealthPolicy` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-249">The property `ApplicationHealthPolicies` of type `ClusterUpgradeDeltaHealthPolicy` has been removed.</span></span>
  - <span data-ttu-id="25a88-250">Die `OverrideUserUpgradePolicy`-Eigenschaft vom Typ `ClusterUpgradePolicy` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-250">The property `OverrideUserUpgradePolicy` of type `ClusterUpgradePolicy` has been removed.</span></span>
  - <span data-ttu-id="25a88-251">Diese Änderungen wirken sich auf die folgenden Cmdlets aus:</span><span class="sxs-lookup"><span data-stu-id="25a88-251">These changes affect the following cmdlets:</span></span>
    - <span data-ttu-id="25a88-252">Add-AzServiceFabricClientCertificate</span><span class="sxs-lookup"><span data-stu-id="25a88-252">Add-AzServiceFabricClientCertificate</span></span>
    - <span data-ttu-id="25a88-253">Add-AzServiceFabricClusterCertificate</span><span class="sxs-lookup"><span data-stu-id="25a88-253">Add-AzServiceFabricClusterCertificate</span></span>
    - <span data-ttu-id="25a88-254">Add-AzServiceFabricNode</span><span class="sxs-lookup"><span data-stu-id="25a88-254">Add-AzServiceFabricNode</span></span>
    - <span data-ttu-id="25a88-255">Add-AzServiceFabricNodeType</span><span class="sxs-lookup"><span data-stu-id="25a88-255">Add-AzServiceFabricNodeType</span></span>
    - <span data-ttu-id="25a88-256">Get-AzServiceFabricCluster</span><span class="sxs-lookup"><span data-stu-id="25a88-256">Get-AzServiceFabricCluster</span></span>
    - <span data-ttu-id="25a88-257">Remove-AzServiceFabricClientCertificate</span><span class="sxs-lookup"><span data-stu-id="25a88-257">Remove-AzServiceFabricClientCertificate</span></span>
    - <span data-ttu-id="25a88-258">Remove-AzServiceFabricClusterCertificate</span><span class="sxs-lookup"><span data-stu-id="25a88-258">Remove-AzServiceFabricClusterCertificate</span></span>
    - <span data-ttu-id="25a88-259">Remove-AzServiceFabricNode</span><span class="sxs-lookup"><span data-stu-id="25a88-259">Remove-AzServiceFabricNode</span></span>
    - <span data-ttu-id="25a88-260">Remove-AzServiceFabricNodeType</span><span class="sxs-lookup"><span data-stu-id="25a88-260">Remove-AzServiceFabricNodeType</span></span>
    - <span data-ttu-id="25a88-261">Remove-AzServiceFabricSetting</span><span class="sxs-lookup"><span data-stu-id="25a88-261">Remove-AzServiceFabricSetting</span></span>
    - <span data-ttu-id="25a88-262">Set-AzServiceFabricSetting</span><span class="sxs-lookup"><span data-stu-id="25a88-262">Set-AzServiceFabricSetting</span></span>
    - <span data-ttu-id="25a88-263">Set-AzServiceFabricUpgradeType</span><span class="sxs-lookup"><span data-stu-id="25a88-263">Set-AzServiceFabricUpgradeType</span></span>
    - <span data-ttu-id="25a88-264">Update-AzServiceFabricDurability</span><span class="sxs-lookup"><span data-stu-id="25a88-264">Update-AzServiceFabricDurability</span></span>
    - <span data-ttu-id="25a88-265">Update-AzServiceFabricReliability</span><span class="sxs-lookup"><span data-stu-id="25a88-265">Update-AzServiceFabricReliability</span></span>

### <a name="azsql-previously-azurermsql"></a><span data-ttu-id="25a88-266">Az.Sql (bisher AzureRM.Sql)</span><span class="sxs-lookup"><span data-stu-id="25a88-266">Az.Sql (previously AzureRM.Sql)</span></span>
- <span data-ttu-id="25a88-267">Die Parameter `State` und `ResourceId` wurden aus dem Cmdlet `Set-AzSqlDatabaseBackupLongTermRetentionPolicy` entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-267">Removed `State` and `ResourceId` parameters from `Set-AzSqlDatabaseBackupLongTermRetentionPolicy` cmdlet</span></span>
- <span data-ttu-id="25a88-268">Veraltete Cmdlets wurden entfernt: `Get/Set-AzSqlServerBackupLongTermRetentionVault`, `Get/Start/Stop-AzSqlServerUpgrade`, `Get/Set-AzSqlDatabaseAuditingPolicy`, `Get/Set-AzSqlServerAuditingPolicy`, `Remove-AzSqlDatabaseAuditing` und `Remove-AzSqlServerAuditing`.</span><span class="sxs-lookup"><span data-stu-id="25a88-268">Removed deprecated cmdlets: `Get/Set-AzSqlServerBackupLongTermRetentionVault`, `Get/Start/Stop-AzSqlServerUpgrade`, `Get/Set-AzSqlDatabaseAuditingPolicy`, `Get/Set-AzSqlServerAuditingPolicy`, `Remove-AzSqlDatabaseAuditing`, `Remove-AzSqlServerAuditing`</span></span>
- <span data-ttu-id="25a88-269">Der veraltete Parameter `Current` wurde aus dem Cmdlet `Get-AzSqlDatabaseBackupLongTermRetentionPolicy` entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-269">Removed deprecated parameter `Current` from `Get-AzSqlDatabaseBackupLongTermRetentionPolicy` cmdlet</span></span>
- <span data-ttu-id="25a88-270">Der veraltete Parameter `DatabaseName` wurde aus dem Cmdlet `Get-AzSqlServerServiceObjective` entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-270">Removed deprecated parameter `DatabaseName` from `Get-AzSqlServerServiceObjective` cmdlet</span></span>
- <span data-ttu-id="25a88-271">Der veraltete Parameter `PrivilegedLogin` wurde aus dem Cmdlet `Set-AzSqlDatabaseDataMaskingPolicy` entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-271">Removed deprecated parameter `PrivilegedLogin` from `Set-AzSqlDatabaseDataMaskingPolicy` cmdlet</span></span>

### <a name="azstorage-previously-azurestorage-and-azurermstorage"></a><span data-ttu-id="25a88-272">Az.Storage (bisher Azure.Storage und AzureRM.Storage)</span><span class="sxs-lookup"><span data-stu-id="25a88-272">Az.Storage (previously Azure.Storage and AzureRM.Storage)</span></span>
- <span data-ttu-id="25a88-273">Der Standardparametersatz wurde in `OAuthParameterSet` geändert, um die Erstellung eines OAuth-Speicherkontexts nur mit dem Speicherkontonamen zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="25a88-273">To support creating an Oauth storage context with only the storage account name, the default parameter set has been changed to `OAuthParameterSet`</span></span>
  - <span data-ttu-id="25a88-274">Beispiel: `$ctx = New-AzureStorageContext -StorageAccountName $accountName`</span><span class="sxs-lookup"><span data-stu-id="25a88-274">Example: `$ctx = New-AzureStorageContext -StorageAccountName $accountName`</span></span>
- <span data-ttu-id="25a88-275">Der Parameter `Location` ist im Cmdlet `Get-AzStorageUsage` jetzt obligatorisch.</span><span class="sxs-lookup"><span data-stu-id="25a88-275">The `Location` parameter has become mandatory in the `Get-AzStorageUsage` cmdlet</span></span>
- <span data-ttu-id="25a88-276">Für die Methoden der Storage-API wird jetzt anstelle von synchronen API-Aufrufen das aufgabenbasierte asynchrone Muster (Task-based Asynchronous Pattern, TAP) verwendet.</span><span class="sxs-lookup"><span data-stu-id="25a88-276">The Storage API methods now use the Task-based Asynchronous Pattern (TAP), instead of synchronous API calls.</span></span>
#### <a name="1-blob-snapshot"></a><span data-ttu-id="25a88-277">1. Momentaufnahme eines Blobs erstellen</span><span class="sxs-lookup"><span data-stu-id="25a88-277">1. Blob Snapshot</span></span>
##### <a name="before"></a><span data-ttu-id="25a88-278">Vorher:</span><span class="sxs-lookup"><span data-stu-id="25a88-278">Before:</span></span>
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$b.ICloudBlob.Snapshot()
```

##### <a name="after"></a><span data-ttu-id="25a88-279">Nachher:</span><span class="sxs-lookup"><span data-stu-id="25a88-279">After:</span></span>
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$task = $b.ICloudBlob.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="2-share-snapshot"></a><span data-ttu-id="25a88-280">2. Momentaufnahme freigeben</span><span class="sxs-lookup"><span data-stu-id="25a88-280">2. Share Snapshot</span></span>
##### <a name="before"></a><span data-ttu-id="25a88-281">Vorher:</span><span class="sxs-lookup"><span data-stu-id="25a88-281">Before:</span></span>
```powershell
$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$snapshot = $Share.Snapshot()
```
#####  <a name="after"></a><span data-ttu-id="25a88-282">Nachher:</span><span class="sxs-lookup"><span data-stu-id="25a88-282">After:</span></span>
```powershell

$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$task = $Share.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="3-undelete-a-soft-delete-blob"></a><span data-ttu-id="25a88-283">3. Vorläufig gelöschtes Blob wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="25a88-283">3. Undelete a soft delete blob</span></span>
##### <a name="before"></a><span data-ttu-id="25a88-284">Vorher:</span><span class="sxs-lookup"><span data-stu-id="25a88-284">Before:</span></span>
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$b.ICloudBlob.Undelete()
```
##### <a name="after"></a><span data-ttu-id="25a88-285">Nachher:</span><span class="sxs-lookup"><span data-stu-id="25a88-285">After:</span></span>
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$task = $b.ICloudBlob.UndeleteAsync()
$task.Wait()
```

#### <a name="4-set-blob-tier"></a><span data-ttu-id="25a88-286">4. Blobtarif festlegen</span><span class="sxs-lookup"><span data-stu-id="25a88-286">4. Set Blob Tier</span></span>
##### <a name="before"></a><span data-ttu-id="25a88-287">Vorher:</span><span class="sxs-lookup"><span data-stu-id="25a88-287">Before:</span></span>
```powershell
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$blockBlob.ICloudBlob.SetStandardBlobTier("hot")

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$pageBlob.ICloudBlob.SetPremiumBlobTier("P4")
```

##### <a name="after"></a><span data-ttu-id="25a88-288">Nachher:</span><span class="sxs-lookup"><span data-stu-id="25a88-288">After:</span></span>
```powershell
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$task = $blockBlob.ICloudBlob.SetStandardBlobTierAsync("hot")
$task.Wait()

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$task = $pageBlob.ICloudBlob.SetPremiumBlobTierAsync("P4")
$task.Wait()
```

### <a name="azwebsites-previously-azurermwebsites"></a><span data-ttu-id="25a88-289">Az.Websites (bisher AzureRM.Websites)</span><span class="sxs-lookup"><span data-stu-id="25a88-289">Az.Websites (previously AzureRM.Websites)</span></span>
- <span data-ttu-id="25a88-290">Die veralteten Eigenschaften wurden aus den Objekten `PSAppServicePlan`, `PSCertificate`, `PSCloningInfo` und `PSSite` entfernt.</span><span class="sxs-lookup"><span data-stu-id="25a88-290">Removed deprecated properties from the `PSAppServicePlan`, `PSCertificate`, `PSCloningInfo`, and `PSSite` objects</span></span>