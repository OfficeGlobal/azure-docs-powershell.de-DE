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
ms.sourcegitcommit: 5630030c5cfa9828c3c024b69de59248263ef17f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "56837366"
---
# <a name="migration-guide-for-az-100"></a>Migrationsleitfaden für Az 1.0.0

In diesem Dokument werden die Änderungen beschrieben, die zwischen den 6.x-Versionen von AzureRM und Az-Version 1.0.0 vorgenommen wurden.

## <a name="table-of-contents"></a>Inhaltsverzeichnis
- [Allgemeine grundlegende Änderungen](#general-breaking-changes)
  - [Änderungen von Cmdlet-Nomen](#cmdlet-noun-prefix-changes)
  - [Änderungen von Modulnamen](#module-name-changes)
  - [Entfernte Module](#removed-modules)
  - [Windows PowerShell 5.1 und .NET 4.7.2](#windows-powershell-51-and-net-472)
  - [Vorübergehende Entfernung der Benutzeranmeldung per PSCredential](#temporary-removal-of-user-login-using-pscredential)
  - [Anmeldung per Standardgerätecode anstelle einer Webbrowser-Eingabeaufforderung](#temporary-default-device-code-login-instead-of-web-browser-prompt)
- [Grundlegende Änderungen am Modul](#module-breaking-changes)
  - [Az.ApiManagement (bisher AzureRM.ApiManagement)](#azapimanagement-previously-azurermapimanagement)
  - [Az.Billing (bisher AzureRM.Billing, AzureRM.Consumption und AzureRM.UsageAggregates)](#azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates)
  - [Az.CognitiveServices (bisher AzureRM.CognitiveServices)](#azcognitiveservices-previously-azurermcognitiveservices)
  - [Az.Compute (bisher AzureRM.Compute)](#azcompute-previously-azurermcompute)
  - [Az.DataFactory (bisher AzureRM.DataFactories und AzureRM.DataFactoryV2)](#azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2)
  - [Az.DataLakeAnalytics (bisher AzureRM.DataLakeAnalytics)](#azdatalakeanalytics-previously-azurermdatalakeanalytics)
  - [Az.DataLakeStore (bisher AzureRM.DataLakeStore)](#azdatalakestore-previously-azurermdatalakestore)
  - [Az.KeyVault (bisher AzureRM.KeyVault)](#azkeyvault-previously-azurermkeyvault)
  - [Az.Media (bisher AzureRM.Media)](#azmedia-previously-azurermmedia)
  - [Az.Monitor (bisher AzureRM.Insights)](#azmonitor-previously-azurerminsights)
  - [Az.Network (bisher AzureRM.Network)](#aznetwork-previously-azurermnetwork)
  - [Az.OperationalInsights (bisher AzureRM.OperationalInsights)](#azoperationalinsights-previously-azurermoperationalinsights)
  - [Az.RecoveryServices (bisher AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup und AzureRM.RecoveryServices.SiteRecovery)](#azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery)
  - [Az.Resources (bisher AzureRM.Resources)](#azresources-previously-azurermresources)
  - [Az.ServiceFabric (bisher AzureRM.ServiceFabric)](#azservicefabric-previously-azurermservicefabric)
  - [Az.Sql (bisher AzureRM.Sql)](#azsql-previously-azurermsql)
  - [Az.Storage (bisher Azure.Storage und AzureRM.Storage)](#azstorage-previously-azurestorage-and-azurermstorage)
  - [Az.Websites (bisher AzureRM.Websites)](#azwebsites-previously-azurermwebsites)

## <a name="general-breaking-changes"></a>Allgemeine grundlegende Änderungen
### <a name="cmdlet-noun-prefix-changes"></a>Änderungen von Cmdlet-Nomen
In AzureRM wurde für Cmdlets entweder „AzureRM“ oder „Azure“ als Nomenpräfix verwendet.  Mit Az werden Namen von Cmdlets vereinfacht und normalisiert, damit für alle Cmdlets „Az“ als Nomenpräfix verwendet wird. Beispiel: 
```powershell
Get-AzureRMVM
Get-AzureKeyVaultSecret
```

Geändert in:
```powershell
Get-AzVM
Get-AzKeyVaultSecret
```

Um die Umstellung auf diese neuen Cmdlet-Namen zu vereinfachen, werden mit Az die beiden neuen Cmdlets ```Enable-AzureRmAlias``` und ```Disable-AzureRmAlias``` eingeführt.  Mit ```Enable-AzureRmAlias``` werden aus den älteren Cmdlet-Namen in AzureRM Aliase für die neueren Az-Cmdlet-Namen erstellt.  Das Cmdlet ermöglicht die Erstellung von Aliasen in der aktuellen Sitzung oder übergreifend für alle Sitzungen, indem Ihr Benutzer- oder Computerprofil geändert wird. 

Ein Beispiel hierfür ist das folgende Skript in AzureRM:
```powershell
#Requires -Modules AzureRM.Storage
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

Es kann mit ```Enable-AzureRmAlias``` mit minimalen Änderungen ausgeführt werden:
```powershell
#Requires -Modules Az.Storage
Enable-AzureRmAlias
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

Durch das Ausführen von ```Enable-AzureRmAlias -Scope CurrentUser``` werden die Aliase für alle von Ihnen geöffneten PowerShell-Sitzungen aktiviert. Nach der Ausführung dieses Cmdlets sind für ein Skript dieser Art keinerlei Änderungen erforderlich:
```powershell
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

Führen Sie ```Get-Help -Online Enable-AzureRmAlias``` über die PowerShell-Eingabeaufforderung aus, um ausführliche Informationen zur Nutzung der Alias-Cmdlets zu erhalten.

Mit ```Disable-AzureRmAlias``` werden AzureRM-Cmdlet-Aliase entfernt, die mit ```Enable-AzureRmAlias``` erstellt wurden.  Führen Sie ```Get-Help -Online Disable-AzureRmAlias``` an der PowerShell-Eingabeaufforderung aus, um alle Details anzuzeigen.

### <a name="module-name-changes"></a>Änderungen von Modulnamen
- Die Modulnamen wurden von `AzureRM.*` in `Az.*` geändert, mit Ausnahme der folgenden Module:
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

Die Änderungen der Modulnamen bedeuten, dass alle Skripts, die ```#Requires``` oder ```Import-Module``` zum Laden von bestimmten Modulen nutzen, auf die Verwendung des neuen Moduls umgestellt werden müssen.

#### <a name="migrating-requires-statements"></a>Migrieren von #Requires-Anweisungen
Skripts, für die #Requires zum Deklarieren einer Abhängigkeit von AzureRM-Modulen verwendet wird, sollten aktualisiert werden, damit die neuen Modulnamen genutzt werden.
```powershell
#Requires -Module AzureRM.Compute
```

Änderung erforderlich in:
```powershell
#Requires -Module Az.Compute
```

#### <a name="migrating-import-module-statements"></a>Migrieren von Import-Module-Anweisungen
Skripts, für die ```Import-Module``` zum Laden der AzureRM-Module verwendet wird, müssen aktualisiert werden, damit die neuen Modulnamen widergespiegelt werden.
```powershell
Import-Module -Name AzureRM.Compute
```

Änderung erforderlich in:
```powershell
Import-Module -Name Az.Compute
```

### <a name="migrating-fully-qualified-cmdlet-invocations"></a>Migrieren von vollqualifizierten Cmdlet-Aufrufen
Bei Verwendung von Skripts, für die Cmdlet-Aufrufe mit Modulqualifikation verwendet werden, z.B.:
```powershell
AzureRM.Compute\Get-AzureRmVM
```

Diese sollten geändert werden, damit die neuen Modul- und Cmdlet-Namen verwendet werden:
```powershell
Az.Compute\Get-AzVM
```

### <a name="migrating-module-manifest-dependencies"></a>Migrieren von Modulmanifestabhängigkeiten
Für Module, die Abhängigkeiten von AzureRM-Modulen anhand einer Modulmanifestdatei (.psd1) ausdrücken, müssen die Modulnamen jeweils im Abschnitt „RequiredModules“ aktualisiert werden.

```powershell
RequiredModules = @(@{ModuleName="AzureRM.Profile"; ModuleVersion="5.8.2"})
```

Änderung erforderlich in:

```powershell
RequiredModules = @(@{ModuleName="Az.Profile"; ModuleVersion="1.0.0"})
```

### <a name="removed-modules"></a>Entfernte Module
- `AzureRM.Backup`
- `AzureRM.Compute.ManagedService`
- `AzureRM.Scheduler`

Die Tools für diese Dienste werden nicht mehr aktiv unterstützt.  Kunden wird die zeitnahe Umstellung auf alternative Dienste empfohlen.

### <a name="windows-powershell-51-and-net-472"></a>Windows PowerShell 5.1 und .NET 4.7.2
- Für die Verwendung von Az mit Windows PowerShell 5.1 ist die Installation von .NET 4.7.2 erforderlich. Für die Nutzung von Az mit PowerShell Core wird .NET 4.7.2 aber nicht benötigt. 

### <a name="temporary-removal-of-user-login-using-pscredential"></a>Vorübergehende Entfernung der Benutzeranmeldung per PSCredential
- Aufgrund von Änderungen am Authentifizierungsablauf für .NET Standard entfernen wir die Benutzeranmeldung per PSCredential vorübergehend. Diese Funktion wird mit dem Windows PowerShell 5.1-Release vom 15.01.2019 wieder eingeführt. Eine ausführliche Beschreibung finden Sie unter [diesem Problem](https://github.com/Azure/azure-powershell/issues/7430).

### <a name="default-device-code-login-instead-of-web-browser-prompt"></a>Anmeldung per Standardgerätecode anstelle einer Webbrowser-Eingabeaufforderung
- Aufgrund von Änderungen am Authentifizierungsablauf für .NET Standard nutzen wir die Geräteanmeldung während der interaktiven Anmeldung als Standardanmeldungsablauf. Die Anmeldung per Webbrowser wird im Windows PowerShell 5.1-Release vom 15.01.2019 wieder als Standard eingeführt. Benutzer können dann die Geräteanmeldung mit einem Switch-Parameter wählen.

## <a name="module-breaking-changes"></a>Grundlegende Änderungen am Modul

### <a name="azapimanagement-previously-azurermapimanagement"></a>Az.ApiManagement (bisher AzureRM.ApiManagement)
- Entfernen Sie die folgenden Cmdlets:
  - New-AzureRmApiManagementHostnameConfiguration
  - Set-AzureRmApiManagementHostnames
  - Update-AzureRmApiManagementDeployment
  - Import-AzureRmApiManagementHostnameCertificate
  - Verwenden Sie stattdessen das Cmdlet **Set-AzApiManagement**, um diese Eigenschaften festzulegen.
- Die folgenden Eigenschaften wurden entfernt:
  - Die Eigenschaften `PortalHostnameConfiguration`, `ProxyHostnameConfiguration`, `ManagementHostnameConfiguration` und `ScmHostnameConfiguration` vom Typ `PsApiManagementHostnameConfiguration` wurden aus `PsApiManagementContext` entfernt. Verwenden Sie stattdessen `PortalCustomHostnameConfiguration`, `ProxyCustomHostnameConfiguration`, `ManagementCustomHostnameConfiguration` und `ScmCustomHostnameConfiguration` vom Typ `PsApiManagementCustomHostNameConfiguration`.
  - Die `StaticIPs`-Eigenschaft wurde aus PsApiManagementContext entfernt. Die Eigenschaft wurde in `PublicIPAddresses` und `PrivateIPAddresses` unterteilt.
  - Die erforderliche `Location`-Eigenschaft wurde aus dem Cmdlet New-AzureApiManagementVirtualNetwork entfernt.

### <a name="azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates"></a>Az.Billing (bisher AzureRM.Billing, AzureRM.Consumption und AzureRM.UsageAggregates)
- Der Parameter `InvoiceName` wurde aus dem Cmdlet `Get-AzConsumptionUsageDetail` entfernt.  Für Skripts müssen andere Identitätsparameter für die Rechnung genutzt werden.

### <a name="azcognitiveservices-previously-azurermcognitiveservices"></a>Az.CognitiveServices (bisher AzureRM.CognitiveServices)
- Der Parametersatz `GetSkusWithAccountParamSetName` wurde aus dem Cmdlet `Get-AzCognitiveServicesAccountSkus` entfernt.  Sie müssen SKUs nach Kontotyp und Standort abrufen, anstatt ResourceGroupName und den Kontonamen zu verwenden.

### <a name="azcompute-previously-azurermcompute"></a>Az.Compute (bisher AzureRM.Compute)
- `IdentityIds` wurden aus der `Identity`-Eigenschaft in den Objekten `PSVirtualMachine` und `PSVirtualMachineScaleSet` entfernt. In Skripts sollte der Wert dieses Felds nicht mehr verwendet werden, um Verarbeitungsentscheidungen zu treffen.
- Der Typ der `InstanceView`-Eigenschaft des `PSVirtualMachineScaleSetVM`-Objekts wurde von `VirtualMachineInstanceView` in `VirtualMachineScaleSetVMInstanceView` geändert.
- Die Eigenschaften `AutoOSUpgradePolicy` und `AutomaticOSUpgrade` wurden aus der `UpgradePolicy`-Eigenschaft entfernt.
- Der Typ der `Sku`-Eigenschaft im `PSSnapshotUpdate`-Objekt wurde von `DiskSku` in `SnapshotSku` geändert.
- `VmScaleSetVMParameterSet` wurde aus dem Cmdlet `Add-AzVMDataDisk` entfernt. Sie können einer ScaleSet-VM nicht mehr einzeln einen Datenträger für Daten hinzufügen.

### <a name="azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2"></a>Az.DataFactory (bisher AzureRM.DataFactories und AzureRM.DataFactoryV2)
- Der Parameter `GatewayName` ist im Cmdlet `New-AzDataFactoryEncryptValue` jetzt obligatorisch.
- Das Cmdlet `New-AzDataFactoryGatewayKey` wurde entfernt.
- Der Parameter `LinkedServiceName` wurde aus dem Cmdlet `Get-AzDataFactoryV2ActivityRun` entfernt. In Skripts sollte der Wert dieses Felds nicht mehr verwendet werden, um Verarbeitungsentscheidungen zu treffen.

### <a name="azdatalakeanalytics-previously-azurermdatalakeanalytics"></a>Az.DataLakeAnalytics (bisher AzureRM.DataLakeAnalytics)
- Veraltete Cmdlets wurden entfernt: `New-AzDataLakeAnalyticsCatalogSecret`, `Remove-AzDataLakeAnalyticsCatalogSecret` und `Set-AzDataLakeAnalyticsCatalogSecret`.

### <a name="azdatalakestore-previously-azurermdatalakestore"></a>Az.DataLakeStore (bisher AzureRM.DataLakeStore)
- Für die folgenden Cmdlets wurde der Typ des Parameters `Encoding` von `FileSystemCmdletProviderEncoding` in `System.Text.Encoding` geändert. Bei dieser Änderung wurden die Codierungswerte `String` und `Oem` entfernt. Alle anderen bisherigen Codierungswerte bleiben erhalten.
  - New-AzureRmDataLakeStoreItem
  - Add-AzureRmDataLakeStoreItemContent
  - Get-AzureRmDataLakeStoreItemContent
- Der veraltete Eigenschaftenalias `Tags` wurde aus den Cmdlets `New-AzDataLakeStoreAccount` und `Set-AzDataLakeStoreAccount` entfernt.

  Skripts mit Verwendung von:
  ```powershell
  New-AzureRMDataLakeStoreAccount -Tags @{TagName="TagValue"}
  ```

  Änderung erforderlich in:
  ```powershell
  New-AzDataLakeStoreAccount -Tag @{TagName="TagValue"}
  ```

- Die veralteten Eigenschaften ```Identity```, ```EncryptionState```, ```EncrypotionProvisioningState```, ```EncryptionConfig```, ```FirewallState```, ```FirewallRules```, ```VirtualNetworkRules```, ```TrustedIdProviderState```, ```TrustedIdProviders```, ```DefaultGroup```, ```NewTier```, ```CurrentTier``` und ```FirewallAllowAzureIps``` wurden aus dem ```PSDataLakeStoreAccountBasic```-Objekt entfernt.  Alle Skripts, für die das von ```Get-AzDataLakeStoreAccount``` zurückgegebene ```PSDatalakeStoreAccount```-Objekt verwendet wird, sollten nicht auf diese Eigenschaften verweisen.

### <a name="azkeyvault-previously-azurermkeyvault"></a>Az.KeyVault (bisher AzureRM.KeyVault)
- Die `PurgeDisabled`-Eigenschaft wurde aus den Objekten `PSKeyVaultKeyAttributes`, `PSKeyVaultKeyIdentityItem` und `PSKeyVaultSecretAttributes` entfernt. In Skripts sollte nicht mehr auf die ```PurgeDisabled```-Eigenschaft verwiesen werden, um Verarbeitungsentscheidungen zu treffen.

### <a name="azmedia-previously-azurermmedia"></a>Az.Media (bisher AzureRM.Media)
- Der veraltete Eigenschaftenalias `Tags` wurde aus dem Cmdlet `New-AzMediaService` entfernt. Skripts mit Verwendung von:
  ```powershell
  New-AzureRMMediaService -Tags @{TagName="TagValue"}
  ```

  Änderung erforderlich in:
  ```powershell
  New-AzMMediaService -Tag @{TagName="TagValue"}
  ```
### <a name="azmonitor-previously-azurerminsights"></a>Az.Monitor (bisher AzureRM.Insights)
- Die Plural-Parameternamen `Categories` und `Timegrains` wurden in Singular-Parameternamen aus dem Cmdlet `Set-AzDiagnosticSetting` geändert. Skripts mit Verwendung von:
  ```powershell
  Set-AzureRmDiagnosticSetting -Timegrains PT1M -Categories Category1, Category2
  ```

  Änderung erforderlich in:
  ```powershell
  Set-AzDiagnosticSetting -Timegrain PT1M -Category Category1, Category2
  ```
### <a name="aznetwork-previously-azurermnetwork"></a>Az.Network (bisher AzureRM.Network)
- Der veraltete Parameter `ResourceId` wurde aus dem Cmdlet `Get-AzServiceEndpointPolicyDefinition` entfernt.
- Die verwaltete `EnableVmProtection`-Eigenschaft wurde aus dem `PSVirtualNetwork`-Objekt entfernt.
- Das veraltete Cmdlet `Set-AzVirtualNetworkGatewayVpnClientConfig` wurde entfernt.
  
Für Skripts sollten basierend auf den Werten dieser Felder keine Verarbeitungsentscheidungen mehr getroffen werden.

### <a name="azoperationalinsights-previously-azurermoperationalinsights"></a>Az.OperationalInsights (bisher AzureRM.OperationalInsights)
- Der Standardparametersatz für `Get-AzOperationalInsightsDataSource` wurde entfernt, und `ByWorkspaceNameByKind` ist zum Standardparametersatz geworden.

  Skripts mit Auflistung von Datenquellen mit:
  ```powershell
  Get-AzureRmOperationalInsightsDataSource
  ```

  Änderung mit Angabe der Art erforderlich:
  ```powershell
  Get-AzOperationalInsightsDataSource -Kind AzureActivityLog
  ```

### <a name="azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery"></a>Az.RecoveryServices (bisher AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup und AzureRM.RecoveryServices.SiteRecovery)
- Der Parameter `Encryption` wurde aus dem Cmdlet `New/Set-AzRecoveryServicesAsrPolicy` entfernt.
- Der Parameter `TargetStorageAccountName` ist für Wiederherstellungen von verwalteten Datenträgern im Cmdlet `Restore-AzRecoveryServicesBackupItem` jetzt obligatorisch.
- Die Parameter `StorageAccountName` und `StorageAccountResourceGroupName` im Cmdlet `Restore-AzRecoveryServicesBackupItem` wurden entfernt.
- Der Parameter `Name` im Cmdlet `Get-AzRecoveryServicesBackupContainer` wurde entfernt.

### <a name="azresources-previously-azurermresources"></a>Az.Resources (bisher AzureRM.Resources)
- Der Parameter `Sku` wurde aus dem Cmdlet `New/Set-AzPolicyAssignment` entfernt.
- Der Parameter `Password` wurde aus den Cmdlets `New-AzADServicePrincipal` und `New-AzADSpCredential` entfernt. Die Kennwörter werden automatisch generiert. Bei Verwendung von Skripts mit Bereitstellung des Kennworts:
  ```powershell
  New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476 -Password $secPassword
  ```

  Änderung erforderlich, damit das Kennwort aus der Ausgabe verwendet wird:
  ```powershell
  $credential = New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476
  $secPassword = $credential.Secret
  ```

### <a name="azservicefabric-previously-azurermservicefabric"></a>Az.ServiceFabric (bisher AzureRM.ServiceFabric)
- Die folgenden Cmdlet-Rückgabetypen wurden geändert:
  - Die `SerivceTypeHealthPolicies`-Eigenschaft vom Typ `ApplicationHealthPolicy` wurde entfernt.
  - Die `ApplicationHealthPolicies`-Eigenschaft vom Typ `ClusterUpgradeDeltaHealthPolicy` wurde entfernt.
  - Die `OverrideUserUpgradePolicy`-Eigenschaft vom Typ `ClusterUpgradePolicy` wurde entfernt.
  - Diese Änderungen wirken sich auf die folgenden Cmdlets aus:
    - Add-AzServiceFabricClientCertificate
    - Add-AzServiceFabricClusterCertificate
    - Add-AzServiceFabricNode
    - Add-AzServiceFabricNodeType
    - Get-AzServiceFabricCluster
    - Remove-AzServiceFabricClientCertificate
    - Remove-AzServiceFabricClusterCertificate
    - Remove-AzServiceFabricNode
    - Remove-AzServiceFabricNodeType
    - Remove-AzServiceFabricSetting
    - Set-AzServiceFabricSetting
    - Set-AzServiceFabricUpgradeType
    - Update-AzServiceFabricDurability
    - Update-AzServiceFabricReliability

### <a name="azsql-previously-azurermsql"></a>Az.Sql (bisher AzureRM.Sql)
- Die Parameter `State` und `ResourceId` wurden aus dem Cmdlet `Set-AzSqlDatabaseBackupLongTermRetentionPolicy` entfernt.
- Veraltete Cmdlets wurden entfernt: `Get/Set-AzSqlServerBackupLongTermRetentionVault`, `Get/Start/Stop-AzSqlServerUpgrade`, `Get/Set-AzSqlDatabaseAuditingPolicy`, `Get/Set-AzSqlServerAuditingPolicy`, `Remove-AzSqlDatabaseAuditing` und `Remove-AzSqlServerAuditing`.
- Der veraltete Parameter `Current` wurde aus dem Cmdlet `Get-AzSqlDatabaseBackupLongTermRetentionPolicy` entfernt.
- Der veraltete Parameter `DatabaseName` wurde aus dem Cmdlet `Get-AzSqlServerServiceObjective` entfernt.
- Der veraltete Parameter `PrivilegedLogin` wurde aus dem Cmdlet `Set-AzSqlDatabaseDataMaskingPolicy` entfernt.

### <a name="azstorage-previously-azurestorage-and-azurermstorage"></a>Az.Storage (bisher Azure.Storage und AzureRM.Storage)
- Der Standardparametersatz wurde in `OAuthParameterSet` geändert, um die Erstellung eines OAuth-Speicherkontexts nur mit dem Speicherkontonamen zu unterstützen.
  - Beispiel: `$ctx = New-AzureStorageContext -StorageAccountName $accountName`
- Der Parameter `Location` ist im Cmdlet `Get-AzStorageUsage` jetzt obligatorisch.
- Für die Methoden der Storage-API wird jetzt anstelle von synchronen API-Aufrufen das aufgabenbasierte asynchrone Muster (Task-based Asynchronous Pattern, TAP) verwendet.
#### <a name="1-blob-snapshot"></a>1. Momentaufnahme eines Blobs erstellen
##### <a name="before"></a>Vorher:
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$b.ICloudBlob.Snapshot()
```

##### <a name="after"></a>Nachher:
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$task = $b.ICloudBlob.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="2-share-snapshot"></a>2. Momentaufnahme freigeben
##### <a name="before"></a>Vorher:
```powershell
$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$snapshot = $Share.Snapshot()
```
#####  <a name="after"></a>Nachher:
```powershell

$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$task = $Share.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="3-undelete-a-soft-delete-blob"></a>3. Vorläufig gelöschtes Blob wiederherstellen
##### <a name="before"></a>Vorher:
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$b.ICloudBlob.Undelete()
```
##### <a name="after"></a>Nachher:
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$task = $b.ICloudBlob.UndeleteAsync()
$task.Wait()
```

#### <a name="4-set-blob-tier"></a>4. Blobtarif festlegen
##### <a name="before"></a>Vorher:
```powershell
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$blockBlob.ICloudBlob.SetStandardBlobTier("hot")

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$pageBlob.ICloudBlob.SetPremiumBlobTier("P4")
```

##### <a name="after"></a>Nachher:
```powershell
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$task = $blockBlob.ICloudBlob.SetStandardBlobTierAsync("hot")
$task.Wait()

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$task = $pageBlob.ICloudBlob.SetPremiumBlobTierAsync("P4")
$task.Wait()
```

### <a name="azwebsites-previously-azurermwebsites"></a>Az.Websites (bisher AzureRM.Websites)
- Die veralteten Eigenschaften wurden aus den Objekten `PSAppServicePlan`, `PSCertificate`, `PSCloningInfo` und `PSSite` entfernt.