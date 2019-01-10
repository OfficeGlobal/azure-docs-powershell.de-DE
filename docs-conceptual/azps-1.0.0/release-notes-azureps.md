## <a name="100---december-2018"></a>1.0.0 – Dezember 2018
### <a name="general"></a>Allgemein

- Allgemeine Verfügbarkeit des Az-Moduls
- Onlinehilfe für jedes Modul
- Ausführlichere Informationen und eine Roadmap finden Sie auf der [Seite mit der Ankündigung zu Az](https://aka.ms/azps-announce).
- Informationen zur Migration aus AzureRM finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).

### <a name="azaccounts"></a>Az.Accounts
- Geändert von Az.Profile
- Feste Tabellenformate für Profil- und Kontexttypen

### <a name="azapimanagement"></a>Az.ApiManagement
- Korrekturen für #7002
- Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).

### <a name="azbatch"></a>Az.Batch
- Möglichkeit zum Anzeigen der ausgeführten Version des Azure Batch-Knoten-Agents auf den VMs eines Pools mit der neuen `NodeAgentInformation`-Eigenschaft für `PSComputeNode` hinzugefügt.
- Der `Caching`-Standardwert für `PSDataDisk` lautet jetzt nicht mehr `None`, sondern `ReadWrite`.
- Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).

### <a name="azbilling"></a>Az.Billing
- Kombination von Billing-, Consumption- und UsageAggregates-Cmdlets. Ausführliche Informationen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).

### <a name="azcognitivservices"></a>Az.CognitivServices
- Vervollständigungen für SkuName und Typem für den Vorgang New-AzureRmCognitiveServicesAccount hinzugefügt
- GetSkusWithAccountParamSetName-Parametersatz aus Get-AzCognitiveServicesAccountSkus entfernt

### <a name="azcontainerinstance"></a>Az.ContainerInstance
- ManagedIdentity-Unterstützung hinzugefügt

### <a name="azdatalakeanalytics"></a>Az.DataLakeAnalytics
- Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).

### <a name="azdatalakestore"></a>Az.DataLakeStore
- Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).

### <a name="azmonitor"></a>Az.Monitor
- Az.Insights in Az.Monitor umbenannt und weitere weniger wichtige grundlegende Änderungen durchgeführt. Informationen hierzu finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).

### <a name="azkeyvault"></a>Az.KeyVault
- Veraltete PurgeDisabled-Eigenschaft aus Ausgabetypen entfernt

### <a name="azmachinelearning"></a>Az.MachineLearning
- Cmdlets des Az.MachineLearningCompute-Moduls eingebunden

### <a name="azmedia"></a>Az.Media
- Veralteten -Tags-Alias aus New-AzMediaService entfernt

### <a name="aznetwork"></a>Az.Network
Unterstützung für das Konfigurieren von RewriteRuleSets im Application Gateway hinzugefügt
    - Neu hinzugefügte Cmdlets:
        - Add-AzureRmApplicationGatewayRewriteRuleSet
        - Get-AzureRmApplicationGatewayRewriteRuleSet
        - New-AzureRmApplicationGatewayRewriteRuleSet
        - Remove-AzureRmApplicationGatewayRewriteRuleSet
        - Set-AzureRmApplicationGatewayRewriteRuleSet
        - New-AzureRmApplicationGatewayRewriteRule
        - New-AzureRmApplicationGatewayRewriteRuleActionSet
        - New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration
    - Cmdlets mit optionalem Parameter -RewriteRuleSet aktualisiert
        - New-AzureRmApplicationGateway
        - New-AzureRmApplicationGatewayRequestRoutingRule
        - Add-AzureRmApplicationGatewayRequestRoutingRule
        - New-AzureRmApplicationGatewayPathRuleConfig
        - Add-AzureRmApplicationGatewayUrlPathMapConfig
        - New-AzureRmApplicationGatewayUrlPathMapConfig: KeyVault-Unterstützung mithilfe von Identität zum Application Gateway hinzugefügt.
    - Cmdlets mit optionalem Parameter aktualisiert: -KeyVaultSecretId, -KeyVaultSecret
        - Add-AzApplicationGatewaySslCertificate
        - New-AzApplicationGatewaySslCertificate
        - Set-AzApplicationGatewaySslCertificate
    - Cmdlet New-AzApplicationGateway mit optionalem Parameter -UserAssignedIdentity aktualisiert
- Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).

### <a name="azoperationalinsights"></a>Az.OperationalInsights
- Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).

### <a name="azprofile"></a>Az.Profile
- Modulnamen in Az.Accounts geändert

### <a name="azrecoveryservices"></a>Az.RecoveryServices
- Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).

### <a name="azresources"></a>Az.Resources
- Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).

### <a name="azservicefabric"></a>Az.ServiceFabric
- Unterstützung für das Angeben des Zertifikats anhand des allgemeinen Namens und Fingerabdrucks
- Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).

### <a name="azsignalr"></a>Az.SIgnalR
- Allgemeine Verfügbarkeit für PowerShell-Cmdlets für SIgnalR

### <a name="azsql"></a>Az.Sql
- Neue Erkennungstypen Data_Exfiltration und Unsafe_Action zu Cmdlets für Bedrohungserkennung hinzugefügt
- Dokumentationsbeispiele für Cmdlets für SQL-Überwachung aktualisiert
- Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).

### <a name="azstorage"></a>Az.Storage
- Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).

### <a name="azwebsites"></a>Az.Websites
- Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).

## <a name="070---december-2018"></a>0.7.0 – Dezember 2018

### <a name="general"></a>Allgemein

* Geringe Änderungen für anstehenden Übergang von AzureRM zu Az

### <a name="azcompute"></a>Az.Compute

* Unterstützung für UltraSSD und Katalogimages in einfachen Parametersätzen für `New-AzVm(ss)`-Cmdlets hinzugefügt.

### <a name="azdatalakestore"></a>Az.DataLakeStore

* Nachgestellten Schrägstrich für die Domäne des ADLS-Kontos korrigiert

### <a name="azfrontdoor"></a>Az.FrontDoor

* Einige fehlerhafte Links behoben
    - In den Artikeln zu New-AzureRmFrontDoor und Set-AzureRmFrontDoor den Artikel-Link zum Cmdlet „New-AzureRmFrontDoorHealthProbeSettingObject“ korrigiert.
    - Im Artikel zu New-AzureRmFrontDoorManagedRuleObject den Artikel-Link zum Cmdlet „New-AzureRmFrontDoorRuleGroupOverrideObject“ korrigiert.

### <a name="azrecoveryservices"></a>Az.RecoveryServices

* Clientseitige Validierungen für Wiederherstellungsvorgänge von Azure-Dateifreigaben hinzugefügt.
* storageAccountName und storageAccountResourceGroupName für AFS-Wiederherstellung optional gemacht.

### <a name="azresources"></a>Az.Resources

* Fehlerbehebung für https://github.com/Azure/azure-powershell/issues/7679
    - Get-AzureRmRoleAssignment für die Verwendung des Abonnementbereichs aktualisiert, wenn dieser beim Anfordern von klassischen Administratoren angegeben wird.

### <a name="azsql"></a>Az.Sql

* Geringe Änderungen für anstehenden Übergang von AzureRM zu Az
* Problem mit der Verwendung von Get-AzureRmSqlDatabaseVulnerabilityAssessment mit .NET Core behoben
* Dokumentation mit Hilfemeldungen zu Cmdlets für die SQL-Überwachung geändert.

### <a name="azstorage"></a>Az.Storage

* -EnableHierarchicalNamespace zu New-AzureRmStorageAccount hinzugefügt
* Problem behoben, bei dem für das Copy File-Cmdlet am Ziel kein Quellkontext wiederverwendet werden kann, wenn -DestContext nicht eingegeben wird
    - Start-AzureStorageFileCopy
* Unterstützung der Konfiguration von statischen Websites
    - Enable-AzureStorageStaticWebsite
    - Disable-AzureStorageStaticWebsite

### <a name="azwebsites"></a>Az.Websites

* Set-AzureRmWebApp und Set-AzureRmWebAppSlot 
    - Neuen Parameter (-AzureStoragePath) zum Angeben von Azure Storage-Pfaden hinzugefügt, die in Windows- und Linux-Container-Apps bereitgestellt werden sollen. Verwenden Sie die Ausgabe des neuen Cmdlets New-AzureRmWebAppAzureStoragePath als Parameter zum Festlegen der Azure Storage-Pfade.

## <a name="061---november-2018"></a>0.6.1 – November 2018

### <a name="azapimanagement"></a>Az.ApiManagement
* Abhängigkeiten für Typzuordnungsproblem aktualisiert

### <a name="azautomation"></a>Az.Automation
* Swagger-basierte Azure Automation-Cmdlets
* Cmdlets zur Updateverwaltung hinzugefügt
* Cmdlets zur Quellcodeverwaltung hinzugefügt
* Cmdlet „Remove-AzureRmAutomationHybridWorkerGroup“ hinzugefügt
* DSC-Befehl für die Knotenregistrierung korrigiert

### <a name="azcompute"></a>Az.Compute
* Identitätsproblem für SystemAssigned-Identität korrigiert
* Abhängigkeiten für Typzuordnungsproblem aktualisiert

### <a name="azcontainerinstance"></a>Az.ContainerInstance
* Abhängigkeiten für Typzuordnungsproblem aktualisiert

### <a name="azmarketplaceordering"></a>Az.MarketplaceOrdering
* Beschreibung der Beispiele für Marketplace-Cmdlets aktualisiert

### <a name="aznetwork"></a>Az.Network
* Folgende Cmdlets hinzugefügt: New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError
* ICMP wieder unterstützten AzureFirewall-Netzwerkprotokollen hinzugefügt
* Cmdlet „Test-AzureRmNetworkWatcherConnectivity“ aktualisiert und Überprüfung für Ziel-ID, Adresse und Port hinzugefügt 
* Probleme mit Arbeitsspeicherauslastung in der VirtualNetwork-Zuordnung behoben

### <a name="azrecoveryservicesbackup"></a>Az.RecoveryServices.Backup
* Problem beim Ändern der Richtlinie für eine geschützte Dateifreigabe behoben
* Richtlinienzeitzone in Großschreibung geändert

### <a name="azrecoveryservicessiterecovery"></a>Az.RecoveryServices.SiteRecovery
* Korrigiertes Beispiel in „New-AzureRmRecoveryServicesAsrProtectableItem“
* Abhängigkeiten für Typzuordnungsproblem aktualisiert

### <a name="azrelay"></a>Az.Relay
* Optionaler Parameter „-KeyValue“ zu Cmdlet „New-AzureRmRelayKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht

### <a name="azresources"></a>Az.Resources
* Hilfedokumentation für ressourcenidentitätsbezogene Parameter in `New-AzureRmPolicyAssignment` und `Set-AzureRmPolicyAssignment` aktualisiert
* Beispiel für „New-AzureRmPolicyDefinition“ hinzugefügt, das „-Metadata“ nutzt
* Korrektur, um Beibehaltung von Groß-/Kleinschreibung in Tagschlüsseln in „NetStandard“ zu ermöglichen: #7678 #7703

### <a name="azservicefabric"></a>Az.ServiceFabric
* Benachrichtigung über veraltete Elemente für anstehende wichtige Änderungen hinzugefügt

### <a name="azsql"></a>Az.Sql
* Neue Cmdlets für CRUD-Vorgänge in verwalteten Azure SQL-Datenbank-Instanzen und verwalteten Azure SQL-Datenbanken hinzugefügt
    - Get-AzureRmSqlInstance
    - New-AzureRmSqlInstance
    - Set-AzureRmSqlInstance
    - Remove-AzureRmSqlInstance
    - Get-AzureRmSqlInstanceDatabase
    - New-AzureRmSqlInstanceDatabase
    - Restore-AzureRmSqlInstanceDatabase
    - Remove-AzureRmSqlInstanceDatabase
* Erweiterte Verwaltung von Überwachungsrichtlinien auf einem Server oder in einer Datenbank aktiviert
    - Neuer Parameter (PredicateExpression) hinzugefügt, um die Filterung von Überwachungsprotokollen zu ermöglichen
    - Cmdlets wurden angepasst, sodass sie SQL-Clients anstelle von Legacyclients verwenden.
    - Set-AzureRmSqlServerAuditing
    - Get-AzureRmSqlServerAuditing
    - Set-AzureRmSqlDatabaseAuditing
    - Get-AzureRmSqlDatabaseAuditing
* Problem bei Verwendung von „Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings“ mit festgelegtem Parameter für den Speicherkontonamen behoben

## <a name="050---november-2018"></a>0.5.0 – November 2018
#### <a name="general"></a>Allgemein
* Ressourcenvervollständigungen für viele Kern-Cmdlets hinzugefügt (diese ermöglichen das Durchlaufen von vorhandenen Ressourcennamen per TAB-TASTE, wenn Cmdlets interaktiv aufgerufen werden)

#### <a name="azprofile"></a>Az.Profile
* Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird
* Parameter „TenantId“ im Cmdlet „Connect-AzAccount“ in „Tenant“ umbenannt und Alias für „TenantId“ hinzugefügt
* Beschreibung von „TenantId“ für „Connect-AzAccount“ aktualisiert
* Fehlermeldung für fehlgeschlagene Anmeldung bei Angabe der Mandantendomäne korrigiert
    - https://github.com/Azure/azure-powershell/issues/6936
* Problem in Bezug auf Kontextnamenskonflikt für Konten ohne Abonnements im Mandanten behoben
    - https://github.com/Azure/azure-powershell/issues/7453
* Problem mit DataLake-Endpunkten bei Verwendung von MSI behoben
    - https://github.com/Azure/azure-powershell/issues/7462
* Problem behoben, das zur Auslösung von „Disconnect-AzAccount“ führte, wenn keine Verbindung bestand
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* Vorgang „Get-AzCognitiveServicesAccountSkus“ hinzugefügt

#### <a name="azcompute"></a>Az.Compute
* Cmdlets Add-AzVmssVMDataDisk und Remove-AzVmssVMDataDisk hinzugefügt
* „Get-AzVMImage“ zeigt „AutomaticOSUpgradeProperties“ an
* Problem behoben, aufgrund dessen die Optionswerte „SetAzVMChefExtension -BootstrapOptions“ und „-JsonAttribute“ nicht im JSON-Format festgelegt wurden

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* Aktualisierung des DataLake-Pakets auf 1.1.10
* Standardmäßige Parallelität zu Multithreadvorgängen hinzugefügt

#### <a name="azinsights"></a>Az.Insights
* Problem Nr. 7267 behoben (Bereich für automatische Skalierung)
    - Probleme beim Erstellen einer neuen Regel für die automatische Skalierung, aufgrund derer die aufgelisteten Parameter nicht richtig festgelegt wurden (Es wurde stets der Standardwert festgelegt.)
* Problem Nr. 7513 behoben [Insights] „Set-AzDiagnosticSetting“ erfordert die explizite Angabe von Kategorien während der Erstellung der Einstellung.
    - Nun erfordert das Cmdlet nicht die explizite Angabe der Kategorien, die während der Erstellung aktiviert werden sollen. Das bedeutet, es funktioniert wie dokumentiert.

#### <a name="aznetwork"></a>Az.Network
* „PeeringType“ wurde geändert und ist nun ein erforderlicher Parameter für die folgenden Cmdlets:
    - Get-AzExpressRouteCircuitRouteTable
    - Get-AzExpressRouteCircuitARPTable
    - Get-AzExpressRouteCircuitRouteTableSummary
    - Get-AzExpressRouteCrossConnectionArpTable
    - Get-AzExpressRouteCrossConnectionRouteTable
    - Get-AzExpressRouteCrossConnectionRouteTableSummary

#### <a name="azpolicyinsights"></a>Az.PolicyInsights
* Cmdlets für Richtlinienwartung hinzugefügt

#### <a name="azresources"></a>Az.Resources
* Fehlerbehebung für https://github.com/Azure/azure-powershell/issues/7402
    - Zulassen der Auflistung von Ressourcen mithilfe des Parameters „-ResourceId“ für „Get-AzResource“

#### <a name="azservicebus"></a>Az.ServiceBus
* Schreibgeschützte Eigenschaft „MigrationState“ zu „PSServiceBusMigrationConfigurationAttributes“ hinzugefügt, was das Ermitteln des Migrationsstatus ermöglicht

#### <a name="azservicefabric"></a>Az.ServiceFabric
* Hinzufügen des Zertifikats zu Linux VMSS korrigiert
* „Add-AzServiceFabricClusterCertificate“ korrigiert
    - Verwenden des richtigen Fingerabdrucks aus dem neuen Zertifikat (Azure/service-fabric-issues#932)
    - Richtige Anzeige von Ausnahmen (Azure/service-fabric-issues#1054)
* „Update-AzServiceFabricDurability“ korrigiert, um die Clusterkonfiguration zu aktualisieren, bevor der VMSS-Vorgang „CreateOrUpdate“ gestartet wird

## <a name="040---october-2018"></a>0.4.0 – Oktober 2018
#### <a name="azprofile"></a>Az.Profile
* Problem mit „Get-AzSubscription“ in Cloud Shell behoben
* Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird

#### <a name="azcompute"></a>Az.Compute
* Neue Größen zur Whitelist von VM-Größen hinzugefügt, für die bei Verwendung des einfachen Parametersatzes für „New-AzVm“ der beschleunigte Netzwerkbetrieb aktiviert wird
* ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* Unterstützung für Regeln für virtuelle Netzwerke hinzugefügt
    - Get-AzDataLakeStoreVirtualNetworkRule: Dient zum Abrufen oder Auflisten der Azure Data Lake Store-Regel für das virtuelle Netzwerk.
    - Add-AzDataLakeStoreVirtualNetworkRule: Fügt dem angegebenen Data Lake Store-Konto eine Regel für das virtuelle Netzwerk hinzu.
    - Set-AzDataLakeStoreVirtualNetworkRule: Ändert die angegebene Regel für das virtuelle Netzwerk in das angegebene Data Lake Store-Konto.
    - Remove-AzDataLakeStoreVirtualNetworkRule: Dient zum Löschen der Azure Data Lake Store-Regel für das virtuelle Netzwerk.

#### <a name="aznetwork"></a>Az.Network
* Cmdlet „Test-AzNetworkWatcherConnectivity“ aktualisiert, Protokollwert wird jetzt an Back-End übergeben.
* ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.

#### <a name="azresources"></a>Az.Resources
* Problem behoben, aufgrund dessen „Get-AzRoleDefinition“ eine unverständliche Ausnahme auslöst (wenn das Standardprofil kein Abonnement enthält und kein Bereich festgelegt ist), indem im Szenario eine aussagekräftige Ausnahme hinzugefügt wurde. Außerdem wurde der Standardparametersatz auf „RoleDefinitionNameParameterSet“ festgelegt.

## <a name="030---october-2018"></a>0.3.0 – Oktober 2018
#### <a name="azurestorage"></a>Azure.Storage
* Fehler beim Kopieren von Blobs/Dateien behoben, aufgrund dessen bei einem Metadatenproblem des Ziels keine Metadaten kopiert wurden
    - Start-AzureStorageBlobCopy
    - Start-AzureStorageFileCopy
* Der Abruf der Speicherressourcennutzung eines bestimmten Standorts wird jetzt unterstützt, und das Hinzufügen einer Warnmeldung für den Abruf der globalen Speicherressourcennutzung ist überflüssig.
    - Get-AzStorageUsage
    
#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* „Get-AzCognitiveServicesAccountSkus“ wird ohne vorhandenes Konto unterstützt.

#### <a name="azcompute"></a>Az.Compute
* Korrektur von „Get-AzVM -ResourceGroupName <rg>“, sodass ggf. mehr als 50 Ergebnisse zurückgegeben werden
* Der Cmdlet-Hilfe zu „New-AzVmss“ wurde ein Beispiel für „SimpleParameterSet“ hinzugefügt.
* Tippfehler in der Azure Disk Encryption-Statusmeldung behoben

#### <a name="azdatafactoryv2"></a>Az.DataFactoryV2
* Die Version des ADF .Net-SDK wurde auf 2.3.0 aktualisiert.

#### <a name="aznetwork"></a>Az.Network
* NetworkProfile-Funktionalität wurde hinzugefügt. Neue Cmdlets hinzugefügt
    - Get-AzNetworkProfile
    - New-AzNetworkProfile
    - Remove-AzNetworkProfile
    - Set-AzNetworkProfile
    - New-AzContainerNicConfig
    - New-AzContainerNicConfigIpConfig
* Dienstzuordnungslink in Subnetzmodell hinzugefügt
* Cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap hinzugefügt
* Cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig hinzugefügt

#### <a name="azrediscache"></a>Az.RedisCache
* Künftig sind beliebige Zeichenfolgen als Größenparameter zulässig. P5 in Popup „PSArgumentCompleter“ hinzugefügt

#### <a name="azresources"></a>Az.Resources
* Fehlender Parameter „-Mode“ zu „Set-AzPolicyDefinition“ hinzugefügt
* Cmdlet-Fehler bei „Get-AzProviderOperation“ für Vorgänge mit Ursprung behoben, der den Benutzer enthält

#### <a name="azsql"></a>Az.Sql
* Problem behoben, aufgrund dessen einige Sicherungs-Cmdlets das aktuelle Azure-Abonnements nicht erkannt haben

#### <a name="azwebsites"></a>Az.Websites
* Neues Cmdlet „Get-AzWebAppContainerContinuousDeploymentUrl“ zum Abrufen der Webhook-URL von Continuous Deployment für Container
* Neue Cmdlets „New-AzWebAppContainerPSSession“ und „Enter-WebAppContainerPSSession“ zum Initiieren einer PowerShell-Remotesitzung in einer Windows-Container-App

## <a name="020---september-2018"></a>0.2.0 – September 2018
 Erste Version