---
title: Azure PowerShell-Änderungsprotokoll | Microsoft-Dokumentation
description: Hierbei handelt es sich um einen Verlauf der Änderungen, die in der neuesten Version an Azure PowerShell vorgenommen wurden.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 5/1/2018
ms.openlocfilehash: 5bc3c9079cb4019bdb2255ab1f947e8ad35ae4cc
ms.sourcegitcommit: c98e3a21037ebd82936828bcb544eed902b24212
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/08/2018
ms.locfileid: "34853456"
---
# <a name="release-notes"></a>Versionshinweise

Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.

---
## <a name="620---june-2018"></a>6.2.0: Juni 2018
#### <a name="azurermprofile"></a>AzureRM.Profile
* Beheben des Problems, aufgrund dessen Version 10.0.3 von Newtonsoft.Json beim Modulimport nicht geladen wurde

#### <a name="azurermcompute"></a>AzureRM.Compute
* Feature zum Aktualisieren von virtuellen VMSS-Computern
    - Cmdlets „Update-AzureRmVmssVM“ und „New-AzureRmVMDataDisk“ hinzugefügt
    - Fügen Sie den Parameter „VirtualMachineScaleSetVM“ zum Cmdlet „Add-AzureRmVMDataDisk“ hinzu, um das Hinzufügen eines Datenträgers zum virtuellen VMSS-Computer zu unterstützen.

#### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* Aktualisierung der ADF .Net SDK-Version auf 0.8.0-preview mit den folgenden Änderungen:
    - Vorgang zum Konfigurieren des Factoryrepositorys hinzugefügt
    - Der verknüpfte QuickBooks-Dienst wurde aktualisiert, um die Eigenschaften „consumerKey“ und „consumerSecret“ verfügbar zu machen.
    - Aktualisierung verschiedener Modelltypen von „SecretBase“ auf „Object“
    - Blobereignisauslöser hinzugefügt

### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Aktualisierung der Dokumentation mit Beispielausgabe

### <a name="azurermnetwork"></a>AzureRM.Network
* Aktivierung der Traffic Analytics-Parameter für Network Watcher-Cmdlets

#### <a name="azurermresources"></a>AzureRM.Resources
* Behebung des Problems mit der Eigenschaft „Properties“ von PSResource-Objekten, die von „Get-AzureRmResource“ zurückgegeben wurden

#### <a name="azurermscheduler"></a>AzureRM.Scheduler
* Behebung des Problems, dass beim Aktualisieren von „ServiceBusQueueJob“ keine neuen Authentifizierungswerte festgelegt wurden

### <a name="azurermsql"></a>AzureRM.Sql
* Aktualisierung der folgenden Cmdlets mit dem optionalen LicenseType-Parameter
    - New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase
    - New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool
    - New-AzureRmSqlDatabaseCopy
    - New-AzureRmSqlDatabaseSecondary
    - Restore-AzureRmSqlDatabase

#### <a name="azurermwebsites"></a>AzureRM.Websites
* „New-AzureRMWebApp“ aktualisiert, um allgemeine Algorithmen aus der Strategiebibliothek zu verwenden.

## <a name="610---may-2018"></a>6.1.0 – Mai 2018
#### <a name="azurermprofile"></a>AzureRM.Profile
* Behebung eines Problems, durch das beim Ausführen von „Clear-AzureRmContext“ ein leerer Kontext mit dem Namen des vorherigen Standardkontexts beibehalten wurde und der Benutzer dadurch keinen neuen Kontext mit dem alten Namen erstellen konnte

#### <a name="azurermanalysisservices"></a>AzureRM.AnalysisServices
* Ermöglichung der Zuordnung von Gateways/Aufhebung der Gatewayzuordnung in AS

#### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* Unterstützung für „ApiVersions“, „ApiReleases“ und „ApiRevisions“ hinzugefügt
* Unterstützung für ServiceFabric-Back-End hinzugefügt
* Unterstützung für Application Insights-Protokollierung hinzugefügt
* Unterstützung für die Erkennung von SKUs vom Typ „Basic“ als gültige SKU des API Management-Diensts hinzugefügt
* Unterstützung hinzugefügt, damit Zertifikate, die von der privaten Zertifizierungsstelle ausgestellt wurden, als Stamm- oder ZS-Zertifikate installiert werden können
* Unterstützung für die Akzeptierung benutzerdefinierter SSL-Zertifikate über KeyVault und mehrere Proxyhostnamen hinzugefügt
* Unterstützung für die verwaltete Dienstidentität hinzugefügt
* Unterstützung für die Annahme von Richtlinien über URL hinzugefügt; HINWEIS: Folgende Cmdlets werden in einem zukünftigen Release als veraltet gekennzeichnet:
   - Import-AzureRmApiManagementHostnameCertificate
   - New-AzureRmApiManagementHostnameConfiguration
   - Set-AzureRmApiManagementHostnames
   - Update-AzureRmApiManagementDeployment

#### <a name="azurermbatch"></a>AzureRM.Batch
* Veröffentlichung des neuen Cmdlets „Get-AzureBatchPoolNodeCounts“
* Veröffentlichung des neuen Cmdlets „Start-AzureBatchComputeNodeServiceLogUpload“

#### <a name="azurermconsumption"></a>AzureRM.Consumption
* Hinzufügung neuer Parameter („Expand“, „ResourceGroup“, „InstanceName“, „InstanceId“, „Tags“ und „Top“) für das Cmdlet „Get-AzureRmConsumptionUsageDetail“

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* Korrektur des Beispiels für „Export AzureRmDataLakeStoreChildItemProperties“
* Korrektur der NULL-Parameterausnahme für rekursiven Fall in „Set-AzureRmDataLakeStoreItemAclEntry“ 
* Korrektur der Hilfedateien für „Set-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAcl“ und „Remove-AzureRmDataLakeStoreItemAclEntry“ 

#### <a name="azurermnetwork"></a>AzureRM.Network
* Erhöhung der Network SDK-Version von 18.0.0-preview auf 19.0.0-preview
* Cmdlet zum Erstellen der Protokollkonfiguration hinzugefügt
    - New-AzureRmNetworkWatcherProtocolConfiguration
* Cmdlet zum Hinzufügen einer neuen Leitungsverbindung zu einer vorhandenen ExpressRoute-Leitung hinzugefügt
    - Add-AzureRmExpressRouteCircuitConnectionConfig
* Cmdlet zum Entfernen einer Leitungsverbindung aus einer vorhandenen ExpressRoute-Leitung hinzugefügt
    - Remove-AzureRmExpressRouteCircuitConnectionConfig
* Cmdlet zum Abrufen einer Leitungsverbindung hinzugefügt
    - Get-AzureRmExpressRouteCircuitConnectionConfig

#### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* Verwendung der Serverauthentifizierung mit generierten Zertifikaten korrigiert (Problemnr. 5998)

#### <a name="azurermsql"></a>AzureRM.Sql
* Überwachungscmdlets korrigiert, um das Entfernen von „AuditActions“ oder „AuditActionGroups“ zu ermöglichen
* Problem mit „Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy“ behoben, das beim Festlegen einer neuen flexiblen Aufbewahrungsrichtlinie zu folgendem Fehler führte: „Configure long term retention policy with azure recovery service vault and policy is no longer supported. Please submit request with the new flexible retention policy“ (Das Konfigurieren einer langfristigen Aufbewahrungsrichtlinie mit Azure Recovery Service-Tresor und -Richtlinie wird nicht mehr unterstützt. Übermitteln Sie eine Anforderung mit der neuen flexiblen Aufbewahrungsrichtlinie.)
* Aktualisierung aller Cmdlets für Azure SQL-Datenbank, für die Erstellung von Pools für elastische Datenbanken und für die Aktualisierung, sodass sie die neue Datenbank-API verwenden. Diese unterstützt die Sku-Eigenschaft für skalierungs- und tarifbezogene Eigenschaften.
* Aktualisierte Cmdlets: 
    - New-AzureRmSqlDatabase, Set-AzureRmSqlDatabase
    - New-AzureRmSqlElasticPool, Set-AzureRmSqlElasticPool
    - New-AzureRmSqlDatabaseCopy
    - New-AzureRmSqlDatabaseSecondary
    - Restore-AzureRmSqlDatabase

#### <a name="azurermtrafficmanager"></a>AzureRM.TrafficManager
* Aktualisierung der Parameter für „Get-AzureRmTrafficManagerProfile“, sodass bei Verwendung des Parameters „-Name“ der Parameter „-ResourceGroupName“ erforderlich ist