---
ms.openlocfilehash: 911e1f7ff56feab2735f397a0128aab4aa7757c7
ms.sourcegitcommit: 0c012450805bef75472f48c74fe488baf6ba53bb
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/04/2019
ms.locfileid: "66498674"
---
## <a name="220---june-2019"></a><span data-ttu-id="08dbc-101">2.2.0 – Juni 2019</span><span class="sxs-lookup"><span data-stu-id="08dbc-101">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="08dbc-102">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="08dbc-102">Az.Cdn</span></span>
* <span data-ttu-id="08dbc-103">Es wurden Cmdlets aktualisiert, um das rulesEngine-Feature basierend auf der API-Version 2019-04-15 zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="08dbc-103">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08dbc-104">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08dbc-104">Az.Compute</span></span>
* <span data-ttu-id="08dbc-105">Der Parameter `NoWait` wurde hinzugefügt, der den Vorgang startet und sofort zurückkehrt, bevor der Vorgang abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="08dbc-105">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="08dbc-106">Aktualisierte Cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="08dbc-106">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="08dbc-107">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="08dbc-107">Az.EventHub</span></span>
* <span data-ttu-id="08dbc-108">Fehlerbehebung für #9231 – Get-AzEventHubNamespace gibt keine Tags zurück</span><span class="sxs-lookup"><span data-stu-id="08dbc-108">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="08dbc-109">Fehlerbehebung für #9230 – Get-AzEventHubNamespace gibt ResourceGroup anstelle von ResourceGroupName zurück</span><span class="sxs-lookup"><span data-stu-id="08dbc-109">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08dbc-110">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08dbc-110">Az.Network</span></span>
* <span data-ttu-id="08dbc-111">ResourceId und InputObject wurden für NAT Gateway aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-111">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="08dbc-112">Es wurde ein Alias für ResourceId und InputObjectr hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-112">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="08dbc-113">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="08dbc-113">Az.PolicyInsights</span></span>
* <span data-ttu-id="08dbc-114">Fehlerbehebung für Nullverweis in Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="08dbc-114">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08dbc-115">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-115">Az.RecoveryServices</span></span>
* <span data-ttu-id="08dbc-116">Minimale Aufbewahrung in Tagen für IaaSVM-Richtlinie wurde von 1 in 7 geändert</span><span class="sxs-lookup"><span data-stu-id="08dbc-116">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="08dbc-117">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="08dbc-117">Az.ServiceBus</span></span>
* <span data-ttu-id="08dbc-118">Fehlerbehebung für #9182 – Get-AzServiceBusNamespace gibt ResourceGroup anstelle von ResourceGroupName zurück</span><span class="sxs-lookup"><span data-stu-id="08dbc-118">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="08dbc-119">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="08dbc-119">Az.ServiceFabric</span></span>
* <span data-ttu-id="08dbc-120">Tippfehler in Fehlermeldung für Update-AzServiceFabricReliability wurde behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-120">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="08dbc-121">Fehlendes Zeichen in Service Fabric-Befehlszeilen wurde behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-121">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="08dbc-122">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08dbc-122">Az.Sql</span></span>
* <span data-ttu-id="08dbc-123">Der DnsZonePartner-Parameter für das Cmdlet New-AzureSqlInstance wurde hinzugefügt, um AutoDr für verwaltete Instanzen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="08dbc-123">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="08dbc-124">Das Cmdlet Get-AzSqlDatabaseSecureConnectionPolicy wird eingestellt</span><span class="sxs-lookup"><span data-stu-id="08dbc-124">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="08dbc-125">Cmdlets zum Schutz vor Bedrohungen werden in „Advanced Threat Protection“ (Erweiterter Schutz vor Bedrohungen) umbenannt</span><span class="sxs-lookup"><span data-stu-id="08dbc-125">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="08dbc-126">New-AzSqlInstance – Die Parameter StorageSizeInGB und LicenseType sind jetzt optional</span><span class="sxs-lookup"><span data-stu-id="08dbc-126">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08dbc-127">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08dbc-127">Az.Websites</span></span>
* <span data-ttu-id="08dbc-128">Das Problem, bei dem die Verwendung von Set-AzWebApp und Set-AzWebAppSlot mit der -WebApp-Eigenschaft die Tags entfernt hat, wurde behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-128">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="08dbc-129">2.1.0 – Mai 2019</span><span class="sxs-lookup"><span data-stu-id="08dbc-129">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="08dbc-130">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="08dbc-130">Az.ApiManagement</span></span>
* <span data-ttu-id="08dbc-131">Es wurden neue Cmdlets zum Verwalten der Diagnose im globalen sowie im API-Bereich erstellt</span><span class="sxs-lookup"><span data-stu-id="08dbc-131">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="08dbc-132">**Get-AzApiManagementDiagnostic**: Abrufen der Diagnose, die im globalen oder im API-Bereich konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="08dbc-132">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="08dbc-133">**New-AzApiManagementDiagnostic**: Erstellen neuer Diagnosen im globalen oder API-Bereich</span><span class="sxs-lookup"><span data-stu-id="08dbc-133">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="08dbc-134">**New-AzApiManagementHttpMessageDiagnostic**: Erstellen einer Diagnoseeinstellung für die zu protokollierenden Kopfzeilen und für die Größe der Bytes für den Text</span><span class="sxs-lookup"><span data-stu-id="08dbc-134">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="08dbc-135">**New-AzApiManagementPipelineDiagnosticSetting**: Erstellen von Diagnoseeinstellungen für ein-/ausgehende HTTP-Nachrichten für das Gateway</span><span class="sxs-lookup"><span data-stu-id="08dbc-135">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="08dbc-136">**New-AzApiManagementSamplingSetting**: Erstellen der Einstellung „Sampling“ für die Anforderungen/Antworten für eine Diagnose</span><span class="sxs-lookup"><span data-stu-id="08dbc-136">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="08dbc-137">**Remove-AzApiManagementDiagnostic**: Entfernen einer Diagnoseentität im globalen oder API-Bereich</span><span class="sxs-lookup"><span data-stu-id="08dbc-137">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="08dbc-138">**Set-AzApiManagementDiagnostic**: Aktualisieren einer Diagnoseentität im globalen oder API-Bereich</span><span class="sxs-lookup"><span data-stu-id="08dbc-138">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="08dbc-139">Es wurden neue Cmdlets für die Cacheverwaltung im ApiManagement-Dienst erstellt</span><span class="sxs-lookup"><span data-stu-id="08dbc-139">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="08dbc-140">**Get-AzApiManagementCache**: Abrufen der Details des durch den Bezeichner angegebenen Caches oder aller Caches</span><span class="sxs-lookup"><span data-stu-id="08dbc-140">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="08dbc-141">**New-AzApiManagementCache**: Erstellen eines neuen „standardmäßigen“ Caches oder eines Caches in einer bestimmten „Region“ von Azure</span><span class="sxs-lookup"><span data-stu-id="08dbc-141">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="08dbc-142">**Remove-AzApiManagementCache**: Entfernen eines Caches</span><span class="sxs-lookup"><span data-stu-id="08dbc-142">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="08dbc-143">**Update-AzApiManagementCache**: Aktualisieren eines Caches</span><span class="sxs-lookup"><span data-stu-id="08dbc-143">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="08dbc-144">Es wurden neue Cmdlets zur Verwaltung von API-Schemas erstellt</span><span class="sxs-lookup"><span data-stu-id="08dbc-144">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="08dbc-145">**New-AzApiManagementSchema**: Erstellen eines neuen Schemas für eine API</span><span class="sxs-lookup"><span data-stu-id="08dbc-145">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="08dbc-146">**Get-AzApiManagementSchema**: Abrufen des in der API konfigurierten Schemas</span><span class="sxs-lookup"><span data-stu-id="08dbc-146">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="08dbc-147">**Remove-AzApiManagementSchema**: Entfernen des in der API konfigurierten Schemas</span><span class="sxs-lookup"><span data-stu-id="08dbc-147">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="08dbc-148">**Set-AzApiManagementSchema**: Aktualisieren des in der API konfigurierten Schemas</span><span class="sxs-lookup"><span data-stu-id="08dbc-148">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="08dbc-149">Es wurde ein neues Cmdlet zum Generieren eines Benutzertokens erstellt</span><span class="sxs-lookup"><span data-stu-id="08dbc-149">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="08dbc-150">**New-AzApiManagementUserToken**: Generieren eines neuen Benutzertokens, das standardmäßig für acht Stunden gültig ist. Mit diesem Cmdlet kann das Token für den „GIT“-Benutzer generiert werden./</span><span class="sxs-lookup"><span data-stu-id="08dbc-150">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="08dbc-151">Es wurde ein neues Cmdlet zum Abrufen des Netzwerkstatus erstellt</span><span class="sxs-lookup"><span data-stu-id="08dbc-151">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="08dbc-152">**Get-AzApiManagementNetworkStatus**: Abrufen der Netzwerkstatuskonnektivität von Ressourcen, von denen der API Management-Dienst abhängig ist</span><span class="sxs-lookup"><span data-stu-id="08dbc-152">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="08dbc-153">Dies ist hilfreich, wenn Sie den ApiManagement-Dienst in einem virtuellen Netzwerk bereitstellen und überprüfen, ob eine der Abhängigkeiten fehlerhaft ist.</span><span class="sxs-lookup"><span data-stu-id="08dbc-153">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="08dbc-154">Das Cmdlet **New-AzApiManagement** wurde zum Verwalten des ApiManagement-Diensts aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-154">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="08dbc-155">Die Unterstützung für die neue SKU „Consumption“ wurde hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-155">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="08dbc-156">Die Unterstützung zum Aktivieren des Flags „EnableClientCertificate“ für die neue SKU „Consumption“ wurde hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-156">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="08dbc-157">Das neue Cmdlet **New-AzApiManagementSslSetting** ermöglicht die Konfiguration der „TLS/SSL“-Einstellung für „Back-End“ und „Front-End“</span><span class="sxs-lookup"><span data-stu-id="08dbc-157">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="08dbc-158">Dies kann auch dazu verwendet werden, um „Verschlüsselungen“ wie „3DES“ und „ServerProtokolle“ wie „Http2“ für das „Front-End“ eines ApiManagement-Diensts zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="08dbc-158">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="08dbc-159">Die Unterstützung für die Konfiguration des Hostnamens „DeveloperPortal“ wurde zum ApiManagement-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-159">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="08dbc-160">Die **Get-AzApiManagementSsoToken**-Cmdlets wurden aktualisiert, um das Objekt „PsApiManagement“ als Eingabe zu übernehmen</span><span class="sxs-lookup"><span data-stu-id="08dbc-160">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="08dbc-161">Das Cmdlet wurde aktualisiert, um Fehlermeldungen inline anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="08dbc-161">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="08dbc-162">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Fehlercode: ValidationError-Fehlermeldung: Mindestens ein Feld enthält ungültige Werte: Fehlerdetails: [Code=ValidationError, Message=Fehler in Element 'log-to-eventhub' in Zeile 3, Spalte 10: Protokollierungstool nicht gefunden, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="08dbc-162">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="08dbc-163">Cmdlet **Export-AzApiManagementApi** wurde für den Export von APIs im Format „OpenApi 3.0“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-163">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="08dbc-164">Cmdlet **Import-AzApiManagementApi** wurde aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-164">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="08dbc-165">Zum Importieren der API aus der „OpenApi 3.0“-Dokumentspezifikation</span><span class="sxs-lookup"><span data-stu-id="08dbc-165">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="08dbc-166">Zur Außerkraftsetzung der „PsApiManagementSchema“-Eigenschaft, die in einem beliebigen Dokument („Swagger“, „Wadl“, „Wsdl“, „OpenApi“) angegeben ist</span><span class="sxs-lookup"><span data-stu-id="08dbc-166">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="08dbc-167">Zur Außerkraftsetzung der „ServiceUrl“-Eigenschaft, die in einem beliebigen Dokument angegeben ist</span><span class="sxs-lookup"><span data-stu-id="08dbc-167">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="08dbc-168">Cmdlet **Get-AzApiManagementPolicy** wurde aktualisiert, um die Richtlinie im Format ohne XML-Escapezeichen mit „rawxml“ zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="08dbc-168">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="08dbc-169">Cmdlet **Set-AzApiManagementPolicy** wurde aktualisiert, um die Richtlinie im Format ohne XML-Escapezeichen mit „rawxml“ und im Format mit XML-Escapezeichen mit „xml“ zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="08dbc-169">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="08dbc-170">Cmdlet **New-AzApiManagementApi** wurde aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-170">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="08dbc-171">Zum Konfigurieren der API mit dem „OpenId“-Autorisierungsserver</span><span class="sxs-lookup"><span data-stu-id="08dbc-171">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="08dbc-172">Zum Erstellen einer API in einem „ApiVersionSet“</span><span class="sxs-lookup"><span data-stu-id="08dbc-172">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="08dbc-173">Zum Klonen einer API mithilfe von „SourceApiId“ und „SourceApiRevision“</span><span class="sxs-lookup"><span data-stu-id="08dbc-173">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="08dbc-174">Möglichkeit zum Konfigurieren von „SubscriptionRequired“ im API-Bereich</span><span class="sxs-lookup"><span data-stu-id="08dbc-174">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="08dbc-175">Cmdlet **Set-AzApiManagementApi** wurde aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-175">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="08dbc-176">Zum Konfigurieren der API mit dem „OpenId“-Autorisierungsserver</span><span class="sxs-lookup"><span data-stu-id="08dbc-176">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="08dbc-177">Zum Aktualisieren einer API in einem „ApiVersionSet“</span><span class="sxs-lookup"><span data-stu-id="08dbc-177">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="08dbc-178">Möglichkeit zum Konfigurieren von „SubscriptionRequired“ im API-Bereich</span><span class="sxs-lookup"><span data-stu-id="08dbc-178">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="08dbc-179">Cmdlet **New-AzApiManagementRevision** wurde aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-179">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="08dbc-180">Zum Klonen (Kopiertags, Produkte, Vorgänge und Richtlinien) einer vorhandenen Version mithilfe von „SourceApiRevision“</span><span class="sxs-lookup"><span data-stu-id="08dbc-180">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="08dbc-181">Die neue Version übernimmt die „ApiId“ des übergeordneten Elements</span><span class="sxs-lookup"><span data-stu-id="08dbc-181">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="08dbc-182">Zum Bereitstellen einer „ApiRevisionDescription“</span><span class="sxs-lookup"><span data-stu-id="08dbc-182">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="08dbc-183">Zur Außerkraftsetzung der „ServiceUrl“ beim Klonen einer API</span><span class="sxs-lookup"><span data-stu-id="08dbc-183">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="08dbc-184">Cmdlet **New-AzApiManagementIdentityProvider** wurde aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-184">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="08dbc-185">Zum Konfigurieren von „AAD“ oder „AADB2C“ mit einer „Authority“</span><span class="sxs-lookup"><span data-stu-id="08dbc-185">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="08dbc-186">Zum Einrichten von „SignupPolicy“, „SigninPolicy“, „ProfileEditingPolicy“ und „PasswordResetPolicy“</span><span class="sxs-lookup"><span data-stu-id="08dbc-186">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="08dbc-187">Cmdlet **New-AzApiManagementSubscription** wurde aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-187">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="08dbc-188">Zum Berücksichtigen für das neue „SubscriptonModel“ mithilfe von „Scope“ und „UserId“</span><span class="sxs-lookup"><span data-stu-id="08dbc-188">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="08dbc-189">Zum Berücksichtigen für das alte Abonnementmodell mithilfe von „ProductId“ und „UserId“</span><span class="sxs-lookup"><span data-stu-id="08dbc-189">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="08dbc-190">Die Unterstützung zum Aktivieren von „AllowTracing“ auf Abonnementebene wurde hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-190">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="08dbc-191">Cmdlet **Set-AzApiManagementSubscription** wurde aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-191">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="08dbc-192">Zum Berücksichtigen für das neue „SubscriptonModel“ mithilfe von „Scope“ und „UserId“</span><span class="sxs-lookup"><span data-stu-id="08dbc-192">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="08dbc-193">Zum Berücksichtigen für das alte Abonnementmodell mithilfe von „ProductId“ und „UserId“</span><span class="sxs-lookup"><span data-stu-id="08dbc-193">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="08dbc-194">Die Unterstützung zum Aktivieren von „AllowTracing“ auf Abonnementebene wurde hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-194">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="08dbc-195">Folgende Cmdlets wurden aktualisiert, um „ResourceId“ als Eingabe zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="08dbc-195">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="08dbc-196">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="08dbc-196">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="08dbc-197">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="08dbc-197">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="08dbc-198">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="08dbc-198">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="08dbc-199">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="08dbc-199">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="08dbc-200">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="08dbc-200">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="08dbc-201">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="08dbc-201">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="08dbc-202">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="08dbc-202">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="08dbc-203">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="08dbc-203">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="08dbc-204">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="08dbc-204">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="08dbc-205">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="08dbc-205">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="08dbc-206">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="08dbc-206">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="08dbc-207">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="08dbc-207">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="08dbc-208">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="08dbc-208">Az.Automation</span></span>
* <span data-ttu-id="08dbc-209">Get-AzAutomationJobOutputRecord wurde aktualisiert, um JSON- und Textdatensatzwerte zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="08dbc-209">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="08dbc-210">Behebung des Problems: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="08dbc-210">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="08dbc-211">Behebung des Problems: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="08dbc-211">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="08dbc-212">Das Verhalten von Start-AzAutomationDscCompilationJob wurde geändert, um den Auftrag einfach zu starten, anstatt auf dessen Abschluss zu warten</span><span class="sxs-lookup"><span data-stu-id="08dbc-212">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="08dbc-213">Behebung des Problems: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="08dbc-213">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="08dbc-214">Fehlerbehebung für Get-AzAutomationDscNode, wenn die Verwendung von „-Name“ alle Knoten zurückgibt</span><span class="sxs-lookup"><span data-stu-id="08dbc-214">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="08dbc-215">Jetzt wird nur der übereinstimmende Knoten zurückgegeben</span><span class="sxs-lookup"><span data-stu-id="08dbc-215">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08dbc-216">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08dbc-216">Az.Compute</span></span>
* <span data-ttu-id="08dbc-217">Parameter „ProtectFromScaleIn“ und „ProtectFromScaleSetAction“ wurden zum Cmdlet „Update-AzVmssVM“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-217">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="08dbc-218">Der jetzt festgelegte wimple-Parameter „New-AzVM“ verwendet standardmäßig einen verfügbaren Standort, wenn „East US“ (USA, Osten) nicht unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="08dbc-218">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="08dbc-219">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08dbc-219">Az.DataLakeStore</span></span>
* <span data-ttu-id="08dbc-220">Das ADLS-SDK wurde aktualisiert, um „HttpClient“ zu verwenden und Datenebenentests wurden mit dem Azure-Framework integriert</span><span class="sxs-lookup"><span data-stu-id="08dbc-220">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="08dbc-221">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="08dbc-221">Az.Monitor</span></span>
* <span data-ttu-id="08dbc-222">Fehlerbehebung bei falschen Parameternamen in Hilfebeispielen</span><span class="sxs-lookup"><span data-stu-id="08dbc-222">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08dbc-223">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08dbc-223">Az.Network</span></span>
* <span data-ttu-id="08dbc-224">DisableBgpRoutePropagation-Flag wurde zur Ausgabe der effektiven Routentabelle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-224">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="08dbc-225">Aktualisiertes Cmdlet:</span><span class="sxs-lookup"><span data-stu-id="08dbc-225">Updated cmdlet:</span></span>
        - <span data-ttu-id="08dbc-226">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="08dbc-226">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="08dbc-227">Fehlerbehebung von doppeltem Bindestrich in Dokumentation von New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="08dbc-227">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="08dbc-228">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08dbc-228">Az.Resources</span></span>
* <span data-ttu-id="08dbc-229">Neues Cmdlet „Get-AzureRmDenyAssignment“ zum Abrufen von Ablehnungszuweisungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-229">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="08dbc-230">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08dbc-230">Az.Sql</span></span>
* <span data-ttu-id="08dbc-231">„Advanced Threat Protection“-Cmdlets in „Advanced Data Security“ umbenennen und Sicherheitsrisikobewertung standardmäßig aktivieren</span><span class="sxs-lookup"><span data-stu-id="08dbc-231">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="08dbc-232">2.0.0: Mai 2019</span><span class="sxs-lookup"><span data-stu-id="08dbc-232">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="08dbc-233">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08dbc-233">Az.Accounts</span></span>
* <span data-ttu-id="08dbc-234">Authentifizierungsbibliothek aktualisiert, um ADFS-Probleme mit der Authentifizierung per Benutzername/Kennwort zu beheben</span><span class="sxs-lookup"><span data-stu-id="08dbc-234">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="08dbc-235">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-235">Az.CognitiveServices</span></span>
* <span data-ttu-id="08dbc-236">Ausschließliche Anzeige des Bing-Haftungsausschlusses für Bing-Suchdienste</span><span class="sxs-lookup"><span data-stu-id="08dbc-236">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="08dbc-237">Fehler behoben, der zu einem Fehler bei der Kontoerstellung führte</span><span class="sxs-lookup"><span data-stu-id="08dbc-237">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08dbc-238">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08dbc-238">Az.Compute</span></span>
* <span data-ttu-id="08dbc-239">Feature für die Näherungsplatzierungsgruppe</span><span class="sxs-lookup"><span data-stu-id="08dbc-239">Proximity placement group feature.</span></span>
    - <span data-ttu-id="08dbc-240">Die folgenden neuen Cmdlets wurden hinzugefügt:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="08dbc-240">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="08dbc-241">Der neue Parameter „ProximityPlacementGroupId“ wurde zu den folgenden Cmdlets hinzugefügt:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="08dbc-241">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="08dbc-242">Der Parameter „StorageAccountType“ wurde zu „New-AzGalleryImageVersion“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="08dbc-242">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="08dbc-243">„TargetRegion“ von „New-AzGalleryImageVersion“ kann „StorageAccountType“ enthalten.</span><span class="sxs-lookup"><span data-stu-id="08dbc-243">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="08dbc-244">Switch-Parameter „SkipShutdown“ wurde zu „Stop-AzVM“ und „Stop-AzVmss“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="08dbc-244">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="08dbc-245">Wichtige Änderungen</span><span class="sxs-lookup"><span data-stu-id="08dbc-245">Breaking changes</span></span>
    - <span data-ttu-id="08dbc-246">„Set-AzVMBootDiagnostics“ in „Set-AzVMBootDiagnostic“ geändert</span><span class="sxs-lookup"><span data-stu-id="08dbc-246">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="08dbc-247">„Export-AzLogAnalyticThrottledRequests“ in „Export-AzLogAnalyticThrottledRequests“ geändert</span><span class="sxs-lookup"><span data-stu-id="08dbc-247">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="08dbc-248">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="08dbc-248">Az.DeploymentManager</span></span>
* <span data-ttu-id="08dbc-249">Erste allgemein verfügbare Version der Azure-Bereitstellungs-Manager-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="08dbc-249">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="08dbc-250">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="08dbc-250">Az.Dns</span></span>
* <span data-ttu-id="08dbc-251">Automatische Delegierung des DNS-Namenservers</span><span class="sxs-lookup"><span data-stu-id="08dbc-251">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="08dbc-252">Das Cmdlet zum Erstellen einer DNS-Zone akzeptiert den übergeordneten Zonennamen als zusätzlichen optionalen Parameter.</span><span class="sxs-lookup"><span data-stu-id="08dbc-252">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="08dbc-253">NS-Einträge in der übergeordneten Zone für neu erstellte untergeordnete Zone hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-253">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="08dbc-254">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="08dbc-254">Az.FrontDoor</span></span>
* <span data-ttu-id="08dbc-255">Erste allgemein verfügbare Version der Azure Frontdoor-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="08dbc-255">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="08dbc-256">WAF-Cmdlets so umbenannt, dass sie „Waf“ enthalten</span><span class="sxs-lookup"><span data-stu-id="08dbc-256">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="08dbc-257">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="08dbc-257">Az.HDInsight</span></span>
* <span data-ttu-id="08dbc-258">Zwei Cmdlets entfernt:</span><span class="sxs-lookup"><span data-stu-id="08dbc-258">Removed two cmdlets:</span></span>
    - <span data-ttu-id="08dbc-259">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="08dbc-259">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="08dbc-260">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="08dbc-260">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="08dbc-261">Neues Cmdlet „Set-AzHDInsightGatewayCredential“ hinzugefügt, um „Grant-AzHDInsightHttpServicesAccess“ zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="08dbc-261">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="08dbc-262">Cmdlet „Get-AzHDInsightJobOutput“ aktualisiert, um zwischen Leserrolle und HDInsight-Bedienerrolle zu unterscheiden:</span><span class="sxs-lookup"><span data-stu-id="08dbc-262">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="08dbc-263">Benutzer mit der Rolle „Leser“ müssen den Parameter „DefaultStorageAccountKey“ explizit angeben, andernfalls treten Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="08dbc-263">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="08dbc-264">Benutzer mit der Rolle des HDInsight-Bedieners sind nicht betroffen.</span><span class="sxs-lookup"><span data-stu-id="08dbc-264">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="08dbc-265">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="08dbc-265">Az.Monitor</span></span>
* <span data-ttu-id="08dbc-266">Neue Cmdlets für SQR-API (Scheduled Query Rule, geplante Abfrageregel)</span><span class="sxs-lookup"><span data-stu-id="08dbc-266">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="08dbc-267">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="08dbc-267">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="08dbc-268">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="08dbc-268">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="08dbc-269">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="08dbc-269">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="08dbc-270">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="08dbc-270">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="08dbc-271">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="08dbc-271">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="08dbc-272">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="08dbc-272">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="08dbc-273">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="08dbc-273">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="08dbc-274">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="08dbc-274">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="08dbc-275">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="08dbc-275">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="08dbc-276">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="08dbc-276">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="08dbc-277">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="08dbc-277">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="08dbc-278">[Weitere Informationen](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules) zur SQR-API</span><span class="sxs-lookup"><span data-stu-id="08dbc-278">[More](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="08dbc-279">„Az.Monitor.md“ aktualisiert, um Cmdlets für metrikbasierte GenV2-Warnungsregel (nicht klassisch) einzuschließen</span><span class="sxs-lookup"><span data-stu-id="08dbc-279">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08dbc-280">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08dbc-280">Az.Network</span></span>
* <span data-ttu-id="08dbc-281">Unterstützung für NAT-Gatewayressource hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-281">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="08dbc-282">Neue Cmdlets</span><span class="sxs-lookup"><span data-stu-id="08dbc-282">New cmdlets</span></span>
        - <span data-ttu-id="08dbc-283">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="08dbc-283">New-AzNatGateway</span></span>
        - <span data-ttu-id="08dbc-284">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="08dbc-284">Get-AzNatGateway</span></span>
        - <span data-ttu-id="08dbc-285">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="08dbc-285">Set-AzNatGateway</span></span>
        - <span data-ttu-id="08dbc-286">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="08dbc-286">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="08dbc-287">Aktualisierte Cmdlets</span><span class="sxs-lookup"><span data-stu-id="08dbc-287">Updated cmdlets</span></span>
        - <span data-ttu-id="08dbc-288">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="08dbc-288">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="08dbc-289">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="08dbc-289">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="08dbc-290">Folgende Befehle für das Feature aktualisiert: Benutzerdefinierte Routen für Brooklyn-Gateway festgelegt/entfernt</span><span class="sxs-lookup"><span data-stu-id="08dbc-290">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="08dbc-291">„New-AzVirtualNetworkGateway“ aktualisiert: Zusätzlicher optionaler Parameter „-CustomRoute“ hinzugefügt, um die Adresspräfixe als benutzerdefinierte Routen für das Gateway festlegen zu können.</span><span class="sxs-lookup"><span data-stu-id="08dbc-291">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="08dbc-292">„Set-AzVirtualNetworkGateway“ aktualisiert: Zusätzlicher optionaler Parameter „-CustomRoute“ hinzugefügt, um die Adresspräfixe als benutzerdefinierte Routen für das Gateway festlegen zu können.</span><span class="sxs-lookup"><span data-stu-id="08dbc-292">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="08dbc-293">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="08dbc-293">Az.PolicyInsights</span></span>
* <span data-ttu-id="08dbc-294">Unterstützung für die Abfrage von Richtlinienauswertungsdetails</span><span class="sxs-lookup"><span data-stu-id="08dbc-294">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="08dbc-295">Parameter „-Expand“ zu „Get-AzPolicyState“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-295">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="08dbc-296">Unterstützung für „-Expand PolicyEvaluationDetails“</span><span class="sxs-lookup"><span data-stu-id="08dbc-296">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08dbc-297">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-297">Az.RecoveryServices</span></span>
* <span data-ttu-id="08dbc-298">Unterstützung für abonnementübergreifende Azure-zu-Azure-Sitewiederherstellung</span><span class="sxs-lookup"><span data-stu-id="08dbc-298">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="08dbc-299">Markierung anstehender wichtiger Änderungen für Azure Site Recovery</span><span class="sxs-lookup"><span data-stu-id="08dbc-299">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="08dbc-300">Fehlerbehebung für Azure Site Recovery-Wiederherstellungsplan und -Aktionsplan</span><span class="sxs-lookup"><span data-stu-id="08dbc-300">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="08dbc-301">Fehlerbehebung für die Aktualisierung der Azure Site Recovery-Netzwerkzuordnung für Azure zu Azure</span><span class="sxs-lookup"><span data-stu-id="08dbc-301">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="08dbc-302">Fehlerbehebung für die Aktualisierung der Azure Site Recovery-Schutzrichtung für Azure zu Azure für verwaltete Datenträger</span><span class="sxs-lookup"><span data-stu-id="08dbc-302">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="08dbc-303">Weitere kleinere Korrekturen</span><span class="sxs-lookup"><span data-stu-id="08dbc-303">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="08dbc-304">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="08dbc-304">Az.Relay</span></span>
* <span data-ttu-id="08dbc-305">Korrektur von Tippfehlern in Kundennachrichten</span><span class="sxs-lookup"><span data-stu-id="08dbc-305">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="08dbc-306">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="08dbc-306">Az.ServiceBus</span></span>
* <span data-ttu-id="08dbc-307">Neue Cmdlets für „NetworkRuleSet“ des Namespace hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-307">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08dbc-308">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08dbc-308">Az.Storage</span></span>
* <span data-ttu-id="08dbc-309">Upgrade auf Speicherclientbibliothek 10.0.1 (Namespace aller Objekte von diesem SDK von „Microsoft.WindowsAzure.Storage. *“ in „Microsoft.Azure.Storage.* “ geändert)</span><span class="sxs-lookup"><span data-stu-id="08dbc-309">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="08dbc-310">Upgrade auf Microsoft.Azure.Management.Storage 11.0.0, um die neue API-Version 2019-04-01 zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="08dbc-310">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="08dbc-311">Art des Standardspeicherkontos bei der Speicherkontoerstellung von „Storage“ in „StorageV2“ geändert</span><span class="sxs-lookup"><span data-stu-id="08dbc-311">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="08dbc-312">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="08dbc-312">New-AzStorageAccount</span></span>
* <span data-ttu-id="08dbc-313">Vom Speicherkonto-Cmdlet ausgegebener SKU-Name (Sku.Name) durch Hinzufügen eines Unterstrichs an SKU-Eingabename angepasst (Beispiel: „StandardLRS“ > „Standard_LRS“).</span><span class="sxs-lookup"><span data-stu-id="08dbc-313">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="08dbc-314">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="08dbc-314">New-AzStorageAccount</span></span>
    - <span data-ttu-id="08dbc-315">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="08dbc-315">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="08dbc-316">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="08dbc-316">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08dbc-317">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08dbc-317">Az.Websites</span></span>
* <span data-ttu-id="08dbc-318">Die Eigenschaft „Kind“ wird nun für PSSite-Objekte festgelegt, die von „Get-AzWebApp“ zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="08dbc-318">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="08dbc-319">„Get-AzWebApp\*Metrics“ und „Get-AzAppServicePlanMetrics“ als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-319">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="08dbc-320">1.8.0: April 2019</span><span class="sxs-lookup"><span data-stu-id="08dbc-320">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="08dbc-321">Highlights seit der letzten Hauptversion</span><span class="sxs-lookup"><span data-stu-id="08dbc-321">Highlights since the last major release</span></span>
* <span data-ttu-id="08dbc-322">Allgemeine Verfügbarkeit des `Az`-Moduls</span><span class="sxs-lookup"><span data-stu-id="08dbc-322">General availability of `Az` module</span></span>
* <span data-ttu-id="08dbc-323">Weitere Informationen zum `Az`-Modul finden Sie unter folgendem Link: https://aka.ms/azps-announce.</span><span class="sxs-lookup"><span data-stu-id="08dbc-323">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="08dbc-324">Vervollständigung für Location, ResourceGroup und ResourceName hinzugefügt: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/.</span><span class="sxs-lookup"><span data-stu-id="08dbc-324">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="08dbc-325">Unterstützung für Platzhalter zu Get-Cmdlets für Az.Compute und Az.Network hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-325">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="08dbc-326">Interaktive und Benutzername/Kennwort-Authentifizierung ausschließlich für Windows PowerShell 5.1 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-326">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="08dbc-327">Unterstützung für Python 2-Runbooks in Az.Automation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-327">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="08dbc-328">Az.LogicApp: Neue Cmdlets für Integrationskonto-Assemblys und -Batchkonfiguration</span><span class="sxs-lookup"><span data-stu-id="08dbc-328">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="08dbc-329">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08dbc-329">Az.Accounts</span></span>
* <span data-ttu-id="08dbc-330">„Uninstall-AzureRm“ aktualisiert, um Module unter Mac ordnungsgemäß zu löschen</span><span class="sxs-lookup"><span data-stu-id="08dbc-330">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="08dbc-331">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="08dbc-331">Az.Batch</span></span>
* <span data-ttu-id="08dbc-332">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="08dbc-332">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="08dbc-333">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="08dbc-333">Az.Cdn</span></span>
* <span data-ttu-id="08dbc-334">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="08dbc-334">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="08dbc-335">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-335">Az.CognitiveServices</span></span>
* <span data-ttu-id="08dbc-336">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="08dbc-336">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08dbc-337">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08dbc-337">Az.Compute</span></span>
* <span data-ttu-id="08dbc-338">Problem mit der AEM-Installation behoben, wenn die Ressourcen-IDs von Datenträgern Ressourcengruppen in Kleinbuchstaben enthielten</span><span class="sxs-lookup"><span data-stu-id="08dbc-338">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="08dbc-339">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="08dbc-339">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="08dbc-340">Dokumentation für Platzhalter korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-340">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="08dbc-341">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="08dbc-341">Az.DataFactory</span></span>
* <span data-ttu-id="08dbc-342">„SsisProperties“ hinzugefügt, falls „NodeCount“ für verwaltete Integration Runtime nicht NULL ist</span><span class="sxs-lookup"><span data-stu-id="08dbc-342">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="08dbc-343">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08dbc-343">Az.DataLakeStore</span></span>
* <span data-ttu-id="08dbc-344">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="08dbc-344">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="08dbc-345">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="08dbc-345">Az.EventGrid</span></span>
* <span data-ttu-id="08dbc-346">Hilfetext für Endpunkt aktualisiert, um anzugeben, dass Ressourcen erstellt werden müssen, bevor die Cmdlets zum Erstellen/Aktualisieren von Ereignisabonnements verwendet werden</span><span class="sxs-lookup"><span data-stu-id="08dbc-346">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="08dbc-347">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="08dbc-347">Az.EventHub</span></span>
* <span data-ttu-id="08dbc-348">Neue Cmdlets für „NetworkRuleSet“ des Namespace hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-348">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="08dbc-349">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="08dbc-349">Az.HDInsight</span></span>
* <span data-ttu-id="08dbc-350">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="08dbc-350">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="08dbc-351">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="08dbc-351">Az.IotHub</span></span>
* <span data-ttu-id="08dbc-352">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="08dbc-352">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="08dbc-353">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="08dbc-353">Az.KeyVault</span></span>
* <span data-ttu-id="08dbc-354">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="08dbc-354">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="08dbc-355">Dokumentation für Platzhalter korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-355">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="08dbc-356">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="08dbc-356">Az.MachineLearning</span></span>
* <span data-ttu-id="08dbc-357">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="08dbc-357">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="08dbc-358">Az.Media</span><span class="sxs-lookup"><span data-stu-id="08dbc-358">Az.Media</span></span>
* <span data-ttu-id="08dbc-359">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="08dbc-359">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="08dbc-360">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="08dbc-360">Az.Monitor</span></span>
  * <span data-ttu-id="08dbc-361">Neue Cmdlets für metrikbasierte GenV2-Warnungsregel (nicht klassisch)</span><span class="sxs-lookup"><span data-stu-id="08dbc-361">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="08dbc-362">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="08dbc-362">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="08dbc-363">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="08dbc-363">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="08dbc-364">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="08dbc-364">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="08dbc-365">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="08dbc-365">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="08dbc-366">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="08dbc-366">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="08dbc-367">Monitor SDK auf Version 0.22.0-preview aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-367">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08dbc-368">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08dbc-368">Az.Network</span></span>
* <span data-ttu-id="08dbc-369">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="08dbc-369">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="08dbc-370">Dokumentation für Platzhalter korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-370">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="08dbc-371">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="08dbc-371">Az.NotificationHubs</span></span>
* <span data-ttu-id="08dbc-372">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="08dbc-372">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="08dbc-373">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="08dbc-373">Az.OperationalInsights</span></span>
* <span data-ttu-id="08dbc-374">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="08dbc-374">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="08dbc-375">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="08dbc-375">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="08dbc-376">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="08dbc-376">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08dbc-377">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-377">Az.RecoveryServices</span></span>
* <span data-ttu-id="08dbc-378">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="08dbc-378">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="08dbc-379">Tabellenformat für SQL auf Azure-VM aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-379">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="08dbc-380">Alternative Methode zum Abrufen des Speicherorts in „AzureFileShare“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-380">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="08dbc-381">„ScheduleRunDays“ in SchedulePolicy-Objekt gemäß Zeitzone aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-381">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="08dbc-382">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="08dbc-382">Az.RedisCache</span></span>
* <span data-ttu-id="08dbc-383">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="08dbc-383">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="08dbc-384">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08dbc-384">Az.Resources</span></span>
* <span data-ttu-id="08dbc-385">Dokumentation für Platzhalter korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-385">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="08dbc-386">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08dbc-386">Az.Sql</span></span>
* <span data-ttu-id="08dbc-387">Abhängigkeit vom Monitor SDK durch allgemeinen Code ersetzt</span><span class="sxs-lookup"><span data-stu-id="08dbc-387">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="08dbc-388">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="08dbc-388">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="08dbc-389">Verbesserter Prozess für Klassifizierung mehrerer Spalten</span><span class="sxs-lookup"><span data-stu-id="08dbc-389">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="08dbc-390">SKU-Eigenschaften (SKU-Name, Familie, Kapazität) in Antwort von „Get-AzSqlServerServiceObjective“ aufgenommen und standardmäßig als Tabelle formatiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-390">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="08dbc-391">Möglichkeit zum Ausführen von „Get-AzSqlServerServiceObjective“ nach Standort, ohne dass bereits ein Server in der Region vorhanden sein muss</span><span class="sxs-lookup"><span data-stu-id="08dbc-391">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="08dbc-392">Unterstützung für Zeitzonenparameter bei der Erstellung einer verwalteten Instanz</span><span class="sxs-lookup"><span data-stu-id="08dbc-392">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="08dbc-393">Dokumentation für Platzhalter korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-393">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08dbc-394">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08dbc-394">Az.Websites</span></span>
* <span data-ttu-id="08dbc-395">„Set-AzWebApp“ und „Set-AzWebAppSlot“ korrigiert, sodass die Tags bei der Ausführung nicht entfernt werden</span><span class="sxs-lookup"><span data-stu-id="08dbc-395">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="08dbc-396">Cmdlets, die Nomen im Plural enthalten, auf Nomen im Singular aktualisiert. Namen im Plural wurden als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="08dbc-396">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="08dbc-397">WebSites SDK aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-397">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="08dbc-398">AdminSiteName-Eigenschaft aus „PSAppServicePlan“ entfernt</span><span class="sxs-lookup"><span data-stu-id="08dbc-398">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="08dbc-399">1.7.0: April 2019</span><span class="sxs-lookup"><span data-stu-id="08dbc-399">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="08dbc-400">Highlights seit der letzten Hauptversion</span><span class="sxs-lookup"><span data-stu-id="08dbc-400">Highlights since the last major release</span></span>
* <span data-ttu-id="08dbc-401">Allgemeine Verfügbarkeit des `Az`-Moduls</span><span class="sxs-lookup"><span data-stu-id="08dbc-401">General availability of `Az` module</span></span>
* <span data-ttu-id="08dbc-402">Weitere Informationen zum `Az`-Modul finden Sie unter folgendem Link: https://aka.ms/azps-announce.</span><span class="sxs-lookup"><span data-stu-id="08dbc-402">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="08dbc-403">Vervollständigung für Location, ResourceGroup und ResourceName hinzugefügt: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/.</span><span class="sxs-lookup"><span data-stu-id="08dbc-403">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="08dbc-404">Unterstützung für Platzhalter zu Get-Cmdlets für Az.Compute und Az.Network hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-404">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="08dbc-405">Interaktive und Benutzername/Kennwort-Authentifizierung ausschließlich für Windows PowerShell 5.1 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-405">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="08dbc-406">Unterstützung für Python 2-Runbooks in Az.Automation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-406">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="08dbc-407">Az.LogicApp: Neue Cmdlets für Integrationskonto-Assemblys und -Batchkonfiguration</span><span class="sxs-lookup"><span data-stu-id="08dbc-407">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="08dbc-408">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08dbc-408">Az.Accounts</span></span>
* <span data-ttu-id="08dbc-409">„Add-AzEnvironment“ und „Set-AzEnvironment“ aktualisiert, um den Parameter „AzureAnalysisServicesEndpointResourceId“ zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="08dbc-409">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="08dbc-410">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-410">Az.AnalysisServices</span></span>
* <span data-ttu-id="08dbc-411">ServiceClient wird in Cmdlets für die Datenebene verwendet, und die ursprüngliche Authentifizierungslogik wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="08dbc-411">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="08dbc-412">„Add-AzureASAccount“ wird als Wrapper von „Connect-AzAccount“ festgelegt, um einen Breaking Change zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="08dbc-412">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="08dbc-413">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="08dbc-413">Az.Automation</span></span>
* <span data-ttu-id="08dbc-414">Fehler des Cmdlets „Fixed New-AzAutomationSoftwareUpdateConfiguration“ für Einschlüsse behoben.</span><span class="sxs-lookup"><span data-stu-id="08dbc-414">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="08dbc-415">Die Parameter „IncludedKbNumber“ und „IncludedPackageNameMask“ sollten nun funktionieren.</span><span class="sxs-lookup"><span data-stu-id="08dbc-415">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="08dbc-416">Fehlerbehebung für eine dynamische Gruppe der Azure Automation-Updateverwaltung</span><span class="sxs-lookup"><span data-stu-id="08dbc-416">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08dbc-417">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08dbc-417">Az.Compute</span></span>
* <span data-ttu-id="08dbc-418">Parameter „HyperVGeneration“ zu „New-AzDiskConfig“ und „New-AzSnapshotConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-418">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="08dbc-419">Zulassen der VM-Erstellung mit einem Katalogimage aus anderen Mandanten</span><span class="sxs-lookup"><span data-stu-id="08dbc-419">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="08dbc-420">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="08dbc-420">Az.ContainerInstance</span></span>
* <span data-ttu-id="08dbc-421">Problem im Parameter „-Command“ von „New-AzContainerGroup“ behoben, das dazu führte, dass ein nachgestelltes leeres Argument hinzugefügt wurde</span><span class="sxs-lookup"><span data-stu-id="08dbc-421">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="08dbc-422">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="08dbc-422">Az.DataFactory</span></span>
* <span data-ttu-id="08dbc-423">Version des ADF .NET SDK auf 3.0.2 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-423">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="08dbc-424">Cmdlet „Set-AzDataFactoryV2“ mit zusätzlichen Parametern für RepoConfiguration-Einstellungen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-424">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="08dbc-425">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08dbc-425">Az.Resources</span></span>
* <span data-ttu-id="08dbc-426">Verarbeitung von Anbietern für „Get-AzResource“ bei der Angabe der Parameter „-ResourceId“ oder „-ResourceGroupName“, „-Name“ und „-ResourceType“ verbessert</span><span class="sxs-lookup"><span data-stu-id="08dbc-426">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="08dbc-427">Fehlerbehandlung für „Test-AzDeployment“ und „Test-AzResourceGroupDeployment“ verbessert</span><span class="sxs-lookup"><span data-stu-id="08dbc-427">Improve error handling for for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="08dbc-428">Behandlung von außerhalb der Bereitstellungsüberprüfung aufgetretenen Fehlern und stattdessen Aufnahme in die Ausgabe des Befehls</span><span class="sxs-lookup"><span data-stu-id="08dbc-428">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="08dbc-429">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="08dbc-429">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="08dbc-430">Switch-Parameter „-IgnoreDynamicParameters“ zu Bereitstellungs-Cmdlets hinzugefügt, um Aufforderung in Skript- und Auftragsszenarien zu überspringen</span><span class="sxs-lookup"><span data-stu-id="08dbc-430">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="08dbc-431">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="08dbc-431">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="08dbc-432">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08dbc-432">Az.Sql</span></span>
* <span data-ttu-id="08dbc-433">Unterstützung für Klassifizierung von Datenbankdaten</span><span class="sxs-lookup"><span data-stu-id="08dbc-433">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08dbc-434">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08dbc-434">Az.Storage</span></span>
* <span data-ttu-id="08dbc-435">Melden eines ausführlichen Fehlers beim Erstellen des Storage-Kontexts mit dem Parameter „-UseConnectedAccount“, aber ohne Azure-Anmeldekonto</span><span class="sxs-lookup"><span data-stu-id="08dbc-435">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="08dbc-436">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="08dbc-436">New-AzStorageContext</span></span>
* <span data-ttu-id="08dbc-437">Unterstützung für das Verwalten von Blobdiensteigenschaften eines bestimmten Storage-Kontos mit einer API der Verwaltungsebene</span><span class="sxs-lookup"><span data-stu-id="08dbc-437">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="08dbc-438">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="08dbc-438">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="08dbc-439">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="08dbc-439">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="08dbc-440">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="08dbc-440">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="08dbc-441">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="08dbc-441">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="08dbc-442">Unterstützung von „-AsJob“ für Cmdlets für den Upload und Download von Blobs und Dateien</span><span class="sxs-lookup"><span data-stu-id="08dbc-442">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="08dbc-443">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="08dbc-443">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="08dbc-444">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="08dbc-444">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="08dbc-445">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="08dbc-445">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="08dbc-446">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="08dbc-446">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="08dbc-447">1.6.0: März 2019</span><span class="sxs-lookup"><span data-stu-id="08dbc-447">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="08dbc-448">Highlights seit der letzten Hauptversion</span><span class="sxs-lookup"><span data-stu-id="08dbc-448">Highlights since the last major release</span></span>
* <span data-ttu-id="08dbc-449">Allgemeine Verfügbarkeit des `Az`-Moduls</span><span class="sxs-lookup"><span data-stu-id="08dbc-449">General availability of `Az` module</span></span>
* <span data-ttu-id="08dbc-450">Weitere Informationen zum `Az`-Modul finden Sie unter folgendem Link: https://aka.ms/azps-announce.</span><span class="sxs-lookup"><span data-stu-id="08dbc-450">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="08dbc-451">Vervollständigung für Location, ResourceGroup und ResourceName hinzugefügt: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/.</span><span class="sxs-lookup"><span data-stu-id="08dbc-451">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="08dbc-452">Unterstützung für Platzhalter zu Get-Cmdlets für Az.Compute und Az.Network hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-452">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="08dbc-453">Interaktive und Benutzername/Kennwort-Authentifizierung ausschließlich für Windows PowerShell 5.1 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-453">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="08dbc-454">Unterstützung für Python 2-Runbooks in Az.Automation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-454">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="08dbc-455">Az.LogicApp: Neue Cmdlets für Integrationskonto-Assemblys und -Batchkonfiguration</span><span class="sxs-lookup"><span data-stu-id="08dbc-455">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="08dbc-456">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="08dbc-456">Az.Automation</span></span>
* <span data-ttu-id="08dbc-457">Änderung an der Azure Automation-Updateverwaltung, um die folgenden neuen Features zu unterstützen:</span><span class="sxs-lookup"><span data-stu-id="08dbc-457">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="08dbc-458">Dynamische Gruppierung</span><span class="sxs-lookup"><span data-stu-id="08dbc-458">Dynamic grouping</span></span>
    * <span data-ttu-id="08dbc-459">Pre-/Post-Skripts</span><span class="sxs-lookup"><span data-stu-id="08dbc-459">Pre-Post script</span></span>
    * <span data-ttu-id="08dbc-460">Neustarteinstellung</span><span class="sxs-lookup"><span data-stu-id="08dbc-460">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08dbc-461">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08dbc-461">Az.Compute</span></span>
* <span data-ttu-id="08dbc-462">Problem mit der Pfadauflösung in „Get-AzVmBootDiagnosticsData“ behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-462">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="08dbc-463">Computeclientbibliothek auf 25.0.0. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-463">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="08dbc-464">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="08dbc-464">Az.KeyVault</span></span>
* <span data-ttu-id="08dbc-465">Unterstützung für Platzhalterzeichen zu KeyVault-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-465">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08dbc-466">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08dbc-466">Az.Network</span></span>
* <span data-ttu-id="08dbc-467">Threat Intelligence-Unterstützung für Azure Firewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-467">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="08dbc-468">Ressource der obersten Ebene für Application Gateway-Firewallrichtlinie und benutzerdefinierte Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-468">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08dbc-469">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-469">Az.RecoveryServices</span></span>
* <span data-ttu-id="08dbc-470">SnapshotRetentionInDays in Azure-VM-Richtlinie hinzugefügt, um sofortigen Wiederherstellungspunkt zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="08dbc-470">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="08dbc-471">Pipe-Unterstützung für das Aufheben der Registrierung eines Containers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-471">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="08dbc-472">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08dbc-472">Az.Resources</span></span>
* <span data-ttu-id="08dbc-473">Unterstützung für Platzhalterzeichen für Get-AzResource und Get-AzResourceGroup aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-473">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="08dbc-474">Anmeldeinformationen aktualisiert, die beim Senden generischer Aufrufe an ARM verwendet werden</span><span class="sxs-lookup"><span data-stu-id="08dbc-474">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="08dbc-475">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08dbc-475">Az.Sql</span></span>
* <span data-ttu-id="08dbc-476">Der Cmdlet-Parameter der Bedrohungserkennung (ExcludeDetectionType) wurde von „DetectionType“ in „string[]“ geändert, um ihn zukunftssicher zu machen, wenn neue DetectionTypes-Elemente hinzugefügt werden, und um AutoVervollständigen zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="08dbc-476">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08dbc-477">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08dbc-477">Az.Storage</span></span>
* <span data-ttu-id="08dbc-478">Unterstützung von Get-/Set-/Remove-Verwaltungsrichtlinien für Speicherkonto hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-478">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="08dbc-479">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="08dbc-479">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="08dbc-480">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="08dbc-480">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="08dbc-481">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="08dbc-481">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="08dbc-482">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="08dbc-482">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="08dbc-483">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="08dbc-483">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="08dbc-484">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="08dbc-484">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08dbc-485">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08dbc-485">Az.Websites</span></span>
* <span data-ttu-id="08dbc-486">ARM-Vorlagenfehler behoben, der zu einem Problem beim Klonen aller Slots mithilfe von „New-AzWebApp -IncludeSourceWebAppSlots“ führte</span><span class="sxs-lookup"><span data-stu-id="08dbc-486">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="08dbc-487">1.5.0: März 2019</span><span class="sxs-lookup"><span data-stu-id="08dbc-487">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="08dbc-488">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08dbc-488">Az.Accounts</span></span>
* <span data-ttu-id="08dbc-489">Der Befehl „Register-AzModule“ wurde hinzugefügt, um von AutoRest generierte Cmdlets zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="08dbc-489">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="08dbc-490">Beispiele für „Connect-AzAccount“ wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="08dbc-490">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="08dbc-491">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="08dbc-491">Az.Automation</span></span>
* <span data-ttu-id="08dbc-492">Problem behoben, das beim Abrufen bestimmter monatlicher Zeitpläne in verschiedenen Azure Automation-Cmdlets auftrat</span><span class="sxs-lookup"><span data-stu-id="08dbc-492">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="08dbc-493">„Get-AzAutomationDscNode“ wurde korrigiert, da nur die 20 obersten Knoten zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="08dbc-493">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="08dbc-494">Jetzt werden alle Knoten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="08dbc-494">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="08dbc-495">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="08dbc-495">Az.Cdn</span></span>
* <span data-ttu-id="08dbc-496">Neue Powershell-Cmdlets zum Aktivieren/Deaktivieren von HTTPS für benutzerdefinierte Domänen hinzugefügt und alte Cmdlets außer Betrieb genommen</span><span class="sxs-lookup"><span data-stu-id="08dbc-496">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08dbc-497">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08dbc-497">Az.Compute</span></span>
* <span data-ttu-id="08dbc-498">Unterstützung für Platzhalterzeichen zu Get-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-498">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="08dbc-499">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="08dbc-499">Az.DataFactory</span></span>
* <span data-ttu-id="08dbc-500">Version des ADF .NET SDK auf 3.0.1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-500">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="08dbc-501">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="08dbc-501">Az.LogicApp</span></span>
* <span data-ttu-id="08dbc-502">„ListWorkflows“ wurde korrigiert, da nur die erste Seite mit Ergebnissen abgerufen wurde.</span><span class="sxs-lookup"><span data-stu-id="08dbc-502">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08dbc-503">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08dbc-503">Az.Network</span></span>
* <span data-ttu-id="08dbc-504">Unterstützung für Platzhalterzeichen zu Network-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-504">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08dbc-505">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-505">Az.RecoveryServices</span></span>
* <span data-ttu-id="08dbc-506">SQL Server jetzt in Azure-VM-Support enthalten</span><span class="sxs-lookup"><span data-stu-id="08dbc-506">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="08dbc-507">SDK-Update</span><span class="sxs-lookup"><span data-stu-id="08dbc-507">SDK Update</span></span>
* <span data-ttu-id="08dbc-508">VMappContainer-Überprüfung in „Get-ProtectableItem“ entfernt</span><span class="sxs-lookup"><span data-stu-id="08dbc-508">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="08dbc-509">„Name“ und „ServerName“ als Parameter für „Get-ProtectableItem“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-509">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="08dbc-510">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08dbc-510">Az.Resources</span></span>
* <span data-ttu-id="08dbc-511">Parameter `-TemplateObject` zu Bereitstellungs-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-511">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="08dbc-512">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="08dbc-512">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="08dbc-513">Problem beim Piping des Ergebnisses von `Get-AzResource` an `Set-AzResource` behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-513">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="08dbc-514">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="08dbc-514">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="08dbc-515">Problem mit JSON-Datentypänderung beim Ausführen von `Set-AzResource` behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-515">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="08dbc-516">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="08dbc-516">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="08dbc-517">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08dbc-517">Az.Sql</span></span>
* <span data-ttu-id="08dbc-518">„AuditingEndpointsCommunicator“ wird aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="08dbc-518">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="08dbc-519">Das Verhalten eines Grenzfalls beim Erstellen neuer Diagnoseeinstellungen wurde korrigiert.</span><span class="sxs-lookup"><span data-stu-id="08dbc-519">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08dbc-520">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08dbc-520">Az.Storage</span></span>
* <span data-ttu-id="08dbc-521">Unterstützung von „Kind BlockBlobStorage“ beim Erstellen eines Speicherkontos: New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="08dbc-521">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="08dbc-522">1.4.0 – Februar 2019</span><span class="sxs-lookup"><span data-stu-id="08dbc-522">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="08dbc-523">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-523">Az.AnalysisServices</span></span>
* <span data-ttu-id="08dbc-524">Cmdlet „AddAzureASAccount“ als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-524">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="08dbc-525">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="08dbc-525">Az.Automation</span></span>
* <span data-ttu-id="08dbc-526">Hilfe für „Import-AzAutomationDscNodeConfiguration“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-526">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="08dbc-527">Überprüfung des Konfigurationsnamens zu Cmdlet „Import-AzAutomationDscConfiguration“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-527">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="08dbc-528">Fehlerbehandlung für Cmdlet „Import-AzAutomationDscConfiguration“ verbessert</span><span class="sxs-lookup"><span data-stu-id="08dbc-528">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="08dbc-529">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-529">Az.CognitiveServices</span></span>
* <span data-ttu-id="08dbc-530">„CustomSubdomainName“ als neuer optionaler Parameter für Cmdlet „New-AzCognitiveServicesAccount“ hinzugefügt, das zum Angeben der Unterdomäne für die Ressource verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="08dbc-530">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08dbc-531">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08dbc-531">Az.Compute</span></span>
* <span data-ttu-id="08dbc-532">Problem mit ID-Parametersätzen behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-532">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="08dbc-533">„Get-AzVMExtension“ aktualisiert, sodass alle installierten Erweiterungen aufgelistet werden, wenn der Name-Parameter nicht angegeben ist</span><span class="sxs-lookup"><span data-stu-id="08dbc-533">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="08dbc-534">Parameter „Tag“ und „ResourceId“ zum Cmdlet „Update-AzImage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-534">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="08dbc-535">„Get-AzVmssVM“ ohne Instanz-ID und mit „InstanceView“ können virtuelle VMSS-Computer mit Instanzansicht auflisten.</span><span class="sxs-lookup"><span data-stu-id="08dbc-535">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="08dbc-536">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08dbc-536">Az.DataLakeStore</span></span>
* <span data-ttu-id="08dbc-537">Cmdlets zum Auflisten und Wiederherstellen gelöschter ADL-Elemente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-537">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="08dbc-538">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="08dbc-538">Az.EventHub</span></span>
* <span data-ttu-id="08dbc-539">Neue boolesche Eigenschaft „SkipEmptyArchives“ zum Überspringen leerer Archive in Klasse „CaptureDescription“ von EventHub hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-539">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="08dbc-540">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="08dbc-540">Az.KeyVault</span></span>
* <span data-ttu-id="08dbc-541">Kennzeichnung in „Set-AzKeyVaultSecret“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-541">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="08dbc-542">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="08dbc-542">Az.LogicApp</span></span>
* <span data-ttu-id="08dbc-543">SKU „Basic“ für Integrationskonten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-543">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="08dbc-544">XSLT 2.0, XSLT 3.0 und Liquid-Zuordnungstypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-544">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="08dbc-545">Neue Cmdlets für Integrationskonto-Assemblys</span><span class="sxs-lookup"><span data-stu-id="08dbc-545">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="08dbc-546">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="08dbc-546">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="08dbc-547">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="08dbc-547">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="08dbc-548">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="08dbc-548">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="08dbc-549">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="08dbc-549">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="08dbc-550">Neue Cmdlets für Integrationskonto-Batchkonfiguration</span><span class="sxs-lookup"><span data-stu-id="08dbc-550">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="08dbc-551">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="08dbc-551">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="08dbc-552">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="08dbc-552">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="08dbc-553">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="08dbc-553">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="08dbc-554">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="08dbc-554">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="08dbc-555">Logik-App-SDK auf Version 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-555">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="08dbc-556">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="08dbc-556">Az.Monitor</span></span>
* <span data-ttu-id="08dbc-557">Hilfe für „Get-AzMetric“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-557">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08dbc-558">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08dbc-558">Az.Network</span></span>
* <span data-ttu-id="08dbc-559">Hilfebeispiel für „Add-AzApplicationGatewayCustomError“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-559">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="08dbc-560">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="08dbc-560">Az.OperationalInsights</span></span>
* <span data-ttu-id="08dbc-561">Zusätzliche Unterstützung für Datenquelle von „New-ApplicationInsights“ und „Get-ApplicationInsights“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="08dbc-561">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="08dbc-562">Neue Art von „ApplicationInsights“ zum Abrufen von bestimmten und von allen ApplicationInsights-Datenquellen für einen Workspace hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="08dbc-562">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="08dbc-563">Cmdlet „New-AzOperationalInsightsApplicationInsightsDataSource“ zum Erstellen einer Datenquelle anhand des angegebenen Ressourcenparameters für „Application-Insights“ hinzugefügt: „subscriptionId“, „resourceGroupName“ und „name“.</span><span class="sxs-lookup"><span data-stu-id="08dbc-563">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="08dbc-564">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08dbc-564">Az.Resources</span></span>
* <span data-ttu-id="08dbc-565">Behebung des Problems: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="08dbc-565">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="08dbc-566">Behebung des Problems: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="08dbc-566">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="08dbc-567">Behebung des Problems: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="08dbc-567">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="08dbc-568">Fehler korrigiert, der die wiederholte Erstellung von „KeyCredentials“ verhindert</span><span class="sxs-lookup"><span data-stu-id="08dbc-568">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="08dbc-569">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08dbc-569">Az.Sql</span></span>
* <span data-ttu-id="08dbc-570">Unterstützung für SQL DB Hyperscale-Tarif hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-570">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="08dbc-571">Fehler korrigiert, aufgrund dessen die Wiederherstellung wegen der Festlegung unnötiger Eigenschaften in der Wiederherstellungsanforderung fehlschlagen konnte</span><span class="sxs-lookup"><span data-stu-id="08dbc-571">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08dbc-572">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08dbc-572">Az.Websites</span></span>
* <span data-ttu-id="08dbc-573">Beispiel in „Get-AzWebAppSlotMetrics“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-573">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="08dbc-574">1.3.0: Februar 2019</span><span class="sxs-lookup"><span data-stu-id="08dbc-574">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="08dbc-575">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08dbc-575">Az.Accounts</span></span>
* <span data-ttu-id="08dbc-576">Update auf die aktuelle Version von ClientRuntime durchgeführt</span><span class="sxs-lookup"><span data-stu-id="08dbc-576">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="08dbc-577">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-577">Az.AnalysisServices</span></span>
<span data-ttu-id="08dbc-578">Allgemeine Verfügbarkeit für Az.AnalysisServices-Modul</span><span class="sxs-lookup"><span data-stu-id="08dbc-578">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08dbc-579">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08dbc-579">Az.Compute</span></span>
* <span data-ttu-id="08dbc-580">AEM-Erweiterung: Unterstützung für UltraSSD und P60-, P70- und P80-Datenträger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-580">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="08dbc-581">Hilfebeschreibung für „Set-AzVMBootDiagnostics“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-581">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="08dbc-582">Hilfebeschreibung und Beispiel für „Update-AzImage“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-582">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08dbc-583">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-583">Az.RecoveryServices</span></span>
<span data-ttu-id="08dbc-584">Allgemeine Verfügbarkeit für Az.RecoveryServices-Modul.</span><span class="sxs-lookup"><span data-stu-id="08dbc-584">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="08dbc-585">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08dbc-585">Az.Resources</span></span>
* <span data-ttu-id="08dbc-586">Kennzeichnung für Ressourcengruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-586">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="08dbc-587">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="08dbc-587">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="08dbc-588">Problem behoben, bei dem „-ErrorAction“ von `Get-AzureRmRoleAssignment` nicht berücksichtigt wird</span><span class="sxs-lookup"><span data-stu-id="08dbc-588">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="08dbc-589">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="08dbc-589">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="08dbc-590">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08dbc-590">Az.Sql</span></span>
* <span data-ttu-id="08dbc-591">Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-591">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="08dbc-592">Problem behoben, bei dem eine fehlende Anmeldung am Azure-Konto bei der Ausführung von SQL-Cmdlets zu einer nullref-Ausnahme führt</span><span class="sxs-lookup"><span data-stu-id="08dbc-592">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="08dbc-593">nullref-Ausnahme in Get-AzSqlCapability korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-593">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="08dbc-594">1.2.1: Januar 2019</span><span class="sxs-lookup"><span data-stu-id="08dbc-594">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="08dbc-595">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08dbc-595">Az.Accounts</span></span>
* <span data-ttu-id="08dbc-596">Release mit richtiger Version der Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="08dbc-596">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="08dbc-597">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-597">Az.AnalysisServices</span></span>
* <span data-ttu-id="08dbc-598">Release mit aktualisierter Authentifizierungsabhängigkeit</span><span class="sxs-lookup"><span data-stu-id="08dbc-598">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08dbc-599">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-599">Az.RecoveryServices</span></span>
* <span data-ttu-id="08dbc-600">Release mit aktualisierter Authentifizierungsabhängigkeit</span><span class="sxs-lookup"><span data-stu-id="08dbc-600">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="08dbc-601">1.2.0: Januar 2019</span><span class="sxs-lookup"><span data-stu-id="08dbc-601">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="08dbc-602">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08dbc-602">Az.Accounts</span></span>
* <span data-ttu-id="08dbc-603">Interaktive und Benutzername/Kennwort-Authentifizierung ausschließlich für Windows PowerShell 5.1 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-603">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="08dbc-604">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-604">Update incorrect online help URLs</span></span>
* <span data-ttu-id="08dbc-605">Warnmeldung in PS Core für „Uninstall-AzureRm“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-605">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="08dbc-606">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="08dbc-606">Az.Aks</span></span>
* <span data-ttu-id="08dbc-607">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-607">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="08dbc-608">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="08dbc-608">Az.Automation</span></span>
* <span data-ttu-id="08dbc-609">Unterstützung für Python 2-Runbooks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-609">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="08dbc-610">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-610">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="08dbc-611">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="08dbc-611">Az.Cdn</span></span>
* <span data-ttu-id="08dbc-612">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-612">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08dbc-613">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08dbc-613">Az.Compute</span></span>
* <span data-ttu-id="08dbc-614">Cmdlet „Invoke-AzVMReimage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-614">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="08dbc-615">Parameter „TempDisk“ zu „Set-AzVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-615">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="08dbc-616">Warnmeldung von „New-AzVM“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-616">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="08dbc-617">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="08dbc-617">Az.ContainerRegistry</span></span>
* <span data-ttu-id="08dbc-618">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-618">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="08dbc-619">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="08dbc-619">Az.DataFactory</span></span>
* <span data-ttu-id="08dbc-620">Version des ADF .NET SDK auf 3.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-620">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="08dbc-621">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08dbc-621">Az.DataLakeStore</span></span>
* <span data-ttu-id="08dbc-622">Problem mit ADLS-Endpunkt bei Verwendung von MSI behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-622">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="08dbc-623">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="08dbc-623">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="08dbc-624">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-624">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="08dbc-625">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="08dbc-625">Az.IotHub</span></span>
* <span data-ttu-id="08dbc-626">Codierungsformat zu Cmdlet „Add-IotHubRoutingEndpoint“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-626">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="08dbc-627">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="08dbc-627">Az.KeyVault</span></span>
* <span data-ttu-id="08dbc-628">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-628">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08dbc-629">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08dbc-629">Az.Network</span></span>
* <span data-ttu-id="08dbc-630">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-630">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="08dbc-631">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08dbc-631">Az.Resources</span></span>
* <span data-ttu-id="08dbc-632">Fehlerhafte Beispiele in Referenzdokumentation zu „New-AzADAppCredential“ und „New-AzADSpCredential“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-632">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="08dbc-633">Problem behoben, bei dem der Pfad für den Parameter „-TemplateFile“ nicht aufgelöst wurde, bevor Cmdlets für die Bereitstellung von Ressourcengruppen ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="08dbc-633">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="08dbc-634">Az.Resources: Richtige Dokumentation für Standardwert von „New-AzureRmPolicyDefinition -Mode“ bereitgestellt</span><span class="sxs-lookup"><span data-stu-id="08dbc-634">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="08dbc-635">Az.Resources: Behebung des Problems: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="08dbc-635">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="08dbc-636">Az.Resources: Behebung des Problems: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="08dbc-636">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="08dbc-637">Formatierungsproblem für Objekt „PSResourceGroupDeployment“ behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-637">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="08dbc-638">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="08dbc-638">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="08dbc-639">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="08dbc-639">Az.ServiceFabric</span></span>
* <span data-ttu-id="08dbc-640">Rollback beim Hinzufügen eines Zertifikats zum VMSS-Modell, Auslösung einer Ausnahme. Fehlerbehebung: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="08dbc-640">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="08dbc-641">Einige Fehlermeldungen wurden korrigiert.</span><span class="sxs-lookup"><span data-stu-id="08dbc-641">Fix some error messages.</span></span>
* <span data-ttu-id="08dbc-642">Fehler bei Clustererstellung mit ARM-Standardvorlage für „New-AzServiceFabriCluster“ behoben, bei dem die Migration zu Az nicht funktioniert hat.</span><span class="sxs-lookup"><span data-stu-id="08dbc-642">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="08dbc-643">Fehler behoben beim Hinzufügen eines Cluster-/Anwendungszertifikats ausschließlich zu VM Scale Sets, die zum Cluster gehören, indem die Cluster-ID in der Erweiterung überprüft wird.</span><span class="sxs-lookup"><span data-stu-id="08dbc-643">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="08dbc-644">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="08dbc-644">Az.SignalR</span></span>
* <span data-ttu-id="08dbc-645">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-645">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="08dbc-646">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08dbc-646">Az.Sql</span></span>
* <span data-ttu-id="08dbc-647">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-647">Update incorrect online help URLs</span></span>
* <span data-ttu-id="08dbc-648">Parameterbeschreibung für den Parameter „LicenseType“ mit möglichen Werten aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-648">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="08dbc-649">Fehler behoben, bei dem die Aktualisierung der Identität der verwalteten Instanz nicht funktioniert hat, wenn es sich um die einzige aktualisierte Eigenschaft gehandelt hat</span><span class="sxs-lookup"><span data-stu-id="08dbc-649">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="08dbc-650">Unterstützung für die benutzerdefinierte Sortierung auf verwalteter Instanz</span><span class="sxs-lookup"><span data-stu-id="08dbc-650">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08dbc-651">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08dbc-651">Az.Storage</span></span>
* <span data-ttu-id="08dbc-652">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-652">Update incorrect online help URLs</span></span>
* <span data-ttu-id="08dbc-653">Ausführliche Fehlermeldung beim Abrufen/Festlegen der klassischen Protokollierung bzw. Metriken für Storage Premium-Konto, da für das Storage Premium-Konto die klassische Protokollierung bzw. Metriken nicht unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="08dbc-653">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="08dbc-654">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="08dbc-654">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="08dbc-655">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="08dbc-655">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="08dbc-656">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="08dbc-656">Az.TrafficManager</span></span>
* <span data-ttu-id="08dbc-657">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-657">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08dbc-658">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08dbc-658">Az.Websites</span></span>
* <span data-ttu-id="08dbc-659">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-659">Update incorrect online help URLs</span></span>
* <span data-ttu-id="08dbc-660">„New-AzWebAppSSLBinding“ korrigiert, damit das Zertifikat in die richtige Ressourcengruppe bzw. an den richtigen Speicherort hochgeladen wird, wenn die App in einer ASE gehostet wird.</span><span class="sxs-lookup"><span data-stu-id="08dbc-660">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="08dbc-661">„New-AzWebAppSSLBinding“ korrigiert, damit die Tags beim Binden eines SSL-Zertifikats an eine App nicht überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="08dbc-661">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="08dbc-662">1.1.0 – Januar 2019</span><span class="sxs-lookup"><span data-stu-id="08dbc-662">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="08dbc-663">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08dbc-663">Az.Accounts</span></span>
* <span data-ttu-id="08dbc-664">Bereich „Local“ zu „Enable-AzureRmAlias“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-664">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08dbc-665">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08dbc-665">Az.Compute</span></span>
* <span data-ttu-id="08dbc-666">Name ist jetzt optional im ID-Parametersatz für „Restart/Start/Stop/Remove/Set-AzVM“ und „Save-AzVMImage“</span><span class="sxs-lookup"><span data-stu-id="08dbc-666">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="08dbc-667">Beschreibung der ID in Hilfedateien aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-667">Updated the description of ID in help files</span></span>
* <span data-ttu-id="08dbc-668">Problem mit der Abwärtskompatibilität beim Az.Accounts-Modul behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-668">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="08dbc-669">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08dbc-669">Az.DataLakeStore</span></span>
* <span data-ttu-id="08dbc-670">Aktualisierung der SDK-Version der Datenebene auf 1.1.14 für SDK-Fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="08dbc-670">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="08dbc-671">Behandlung von negativen acesstime- and modificationtime-Werten für „getfilestatus“ und „liststatus“ korrigiert, asynchrones Abbruchtoken korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-671">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="08dbc-672">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="08dbc-672">Az.EventGrid</span></span>
* <span data-ttu-id="08dbc-673">Zur Verwendung der API-Version 2019-01-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-673">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="08dbc-674">Aktualisierung der folgenden Cmdlets zur Unterstützung des neuen Szenarios in der API-Version 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="08dbc-674">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="08dbc-675">New-AzureRmEventGridSubscription: Neue optionale Parameter zum Angeben folgender Werte hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="08dbc-675">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="08dbc-676">Gültigkeitsdauer des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="08dbc-676">Event Time-To-Live,</span></span>
        - <span data-ttu-id="08dbc-677">Maximale Anzahl von Übermittlungsversuchen für die Ereignisse</span><span class="sxs-lookup"><span data-stu-id="08dbc-677">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="08dbc-678">Endpunkt für unzustellbare Nachrichten</span><span class="sxs-lookup"><span data-stu-id="08dbc-678">Dead letter endpoint.</span></span>
    - <span data-ttu-id="08dbc-679">Update-AzureRmEventGridSubscription: Neue optionale Parameter zum Angeben folgender Werte hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="08dbc-679">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="08dbc-680">Gültigkeitsdauer des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="08dbc-680">Event Time-To-Live,</span></span>
        - <span data-ttu-id="08dbc-681">Maximale Anzahl von Übermittlungsversuchen für die Ereignisse</span><span class="sxs-lookup"><span data-stu-id="08dbc-681">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="08dbc-682">Endpunkt für unzustellbare Nachrichten</span><span class="sxs-lookup"><span data-stu-id="08dbc-682">Dead letter endpoint.</span></span>
* <span data-ttu-id="08dbc-683">Neue Enumerationswerte („storageQueue“ und „hybridConnection“) für die EndpointType-Option in den Cmdlets „New-AzureRmEventGridSubscription“ und „Update-AzureRmEventGridSubscription“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-683">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="08dbc-684">Anzeige einer Warnmeldung, wenn das Erstellen oder Aktualisieren des Ereignisabonnements voraussichtlich eine manuelle Aktion des Benutzers zur Folge hat</span><span class="sxs-lookup"><span data-stu-id="08dbc-684">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="08dbc-685">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="08dbc-685">Az.IotHub</span></span>
* <span data-ttu-id="08dbc-686">Auf die aktuelle Version des Iot Hub SDK aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-686">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="08dbc-687">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="08dbc-687">Az.LogicApp</span></span>
* <span data-ttu-id="08dbc-688">„Get-AzLogicApp“ listet alle Apps ohne angegebenen Namen auf</span><span class="sxs-lookup"><span data-stu-id="08dbc-688">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="08dbc-689">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08dbc-689">Az.Resources</span></span>
* <span data-ttu-id="08dbc-690">Problem mit dem Parametersatz bei Angabe der Parameter „-ODataQuery“ und „-ResourceId“ für „Get-AzResource“ behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-690">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="08dbc-691">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="08dbc-691">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="08dbc-692">Behandlung des Parameters „-Custom“ in „New/Set-AzPolicyDefinition“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-692">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="08dbc-693">Tippfehler in der Dokumentation für „New-AzDeployment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-693">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="08dbc-694">Parameter „-MailNickname“ als obligatorisch festgelegt für „New-AzADUser“</span><span class="sxs-lookup"><span data-stu-id="08dbc-694">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="08dbc-695">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="08dbc-695">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="08dbc-696">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="08dbc-696">Az.SignalR</span></span>
* <span data-ttu-id="08dbc-697">Problem mit der Abwärtskompatibilität beim Az.Accounts-Modul behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-697">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="08dbc-698">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08dbc-698">Az.Sql</span></span>
* <span data-ttu-id="08dbc-699">Abhängigkeit des Speicherverwaltungsclients zur allgemeinen SDK-Implementierung konvertiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-699">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08dbc-700">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08dbc-700">Az.Storage</span></span>
* <span data-ttu-id="08dbc-701">Festlegung des „StorageAccountName“ des Speicherkontexts als tatsächlichen Namen des Speicherkontos, wenn dieser mit „SAS-Token“, „OAuth“ oder „Anonym“ erstellt wird</span><span class="sxs-lookup"><span data-stu-id="08dbc-701">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="08dbc-702">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="08dbc-702">New-AzStorageContext</span></span>
* <span data-ttu-id="08dbc-703">Erstellen von SAS-Token des Blob-Momentaufnahmeobjekts mit dem Parameter „-FullUri“, Festlegung des zurückgegebenen URI als Momentaufnahme-URI</span><span class="sxs-lookup"><span data-stu-id="08dbc-703">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="08dbc-704">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="08dbc-704">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08dbc-705">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08dbc-705">Az.Websites</span></span>
* <span data-ttu-id="08dbc-706">Fehler bei der Datumsanalyse in „Get-AzDeletedWebApp“ behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-706">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="08dbc-707">Problem mit der Abwärtskompatibilität beim Az.Accounts-Modul behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-707">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="08dbc-708">1.0.0 – Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="08dbc-708">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="08dbc-709">Allgemein</span><span class="sxs-lookup"><span data-stu-id="08dbc-709">General</span></span>

- <span data-ttu-id="08dbc-710">Allgemeine Verfügbarkeit des Az-Moduls</span><span class="sxs-lookup"><span data-stu-id="08dbc-710">General Availability of Az Module</span></span>
- <span data-ttu-id="08dbc-711">Onlinehilfe für jedes Modul</span><span class="sxs-lookup"><span data-stu-id="08dbc-711">Online help for each module</span></span>
- <span data-ttu-id="08dbc-712">Ausführlichere Informationen und eine Roadmap finden Sie auf der [Seite mit der Ankündigung zu Az](https://aka.ms/azps-announce).</span><span class="sxs-lookup"><span data-stu-id="08dbc-712">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="08dbc-713">Informationen zur Migration aus AzureRM finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="08dbc-713">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="08dbc-714">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08dbc-714">Az.Accounts</span></span>
- <span data-ttu-id="08dbc-715">Geändert von Az.Profile</span><span class="sxs-lookup"><span data-stu-id="08dbc-715">Changed from Az.Profile</span></span>
- <span data-ttu-id="08dbc-716">Feste Tabellenformate für Profil- und Kontexttypen</span><span class="sxs-lookup"><span data-stu-id="08dbc-716">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="08dbc-717">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="08dbc-717">Az.ApiManagement</span></span>
- <span data-ttu-id="08dbc-718">Korrekturen für #7002</span><span class="sxs-lookup"><span data-stu-id="08dbc-718">Fixes for #7002</span></span>
- <span data-ttu-id="08dbc-719">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="08dbc-719">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="08dbc-720">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="08dbc-720">Az.Batch</span></span>
- <span data-ttu-id="08dbc-721">Möglichkeit zum Anzeigen der ausgeführten Version des Azure Batch-Knoten-Agents auf den VMs eines Pools mit der neuen `NodeAgentInformation`-Eigenschaft für `PSComputeNode` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="08dbc-721">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="08dbc-722">Der `Caching`-Standardwert für `PSDataDisk` lautet jetzt nicht mehr `None`, sondern `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="08dbc-722">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="08dbc-723">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="08dbc-723">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="08dbc-724">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="08dbc-724">Az.Billing</span></span>
- <span data-ttu-id="08dbc-725">Kombination von Billing-, Consumption- und UsageAggregates-Cmdlets. Ausführliche Informationen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="08dbc-725">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="08dbc-726">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-726">Az.CognitivServices</span></span>
- <span data-ttu-id="08dbc-727">Vervollständigungen für SkuName und Typem für den Vorgang New-AzureRmCognitiveServicesAccount hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-727">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="08dbc-728">GetSkusWithAccountParamSetName-Parametersatz aus Get-AzCognitiveServicesAccountSkus entfernt</span><span class="sxs-lookup"><span data-stu-id="08dbc-728">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="08dbc-729">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="08dbc-729">Az.ContainerInstance</span></span>
- <span data-ttu-id="08dbc-730">ManagedIdentity-Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-730">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="08dbc-731">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="08dbc-731">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="08dbc-732">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="08dbc-732">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="08dbc-733">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08dbc-733">Az.DataLakeStore</span></span>
- <span data-ttu-id="08dbc-734">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="08dbc-734">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="08dbc-735">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="08dbc-735">Az.Monitor</span></span>
- <span data-ttu-id="08dbc-736">Az.Insights in Az.Monitor umbenannt und weitere weniger wichtige grundlegende Änderungen durchgeführt. Informationen hierzu finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="08dbc-736">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="08dbc-737">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="08dbc-737">Az.KeyVault</span></span>
- <span data-ttu-id="08dbc-738">Veraltete PurgeDisabled-Eigenschaft aus Ausgabetypen entfernt</span><span class="sxs-lookup"><span data-stu-id="08dbc-738">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="08dbc-739">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="08dbc-739">Az.MachineLearning</span></span>
- <span data-ttu-id="08dbc-740">Cmdlets des Az.MachineLearningCompute-Moduls eingebunden</span><span class="sxs-lookup"><span data-stu-id="08dbc-740">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="08dbc-741">Az.Media</span><span class="sxs-lookup"><span data-stu-id="08dbc-741">Az.Media</span></span>
- <span data-ttu-id="08dbc-742">Veralteten -Tags-Alias aus New-AzMediaService entfernt</span><span class="sxs-lookup"><span data-stu-id="08dbc-742">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="08dbc-743">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08dbc-743">Az.Network</span></span>
<span data-ttu-id="08dbc-744">Unterstützung für das Konfigurieren von RewriteRuleSets im Application Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-744">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="08dbc-745">Neu hinzugefügte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="08dbc-745">New cmdlets added:</span></span>
        - <span data-ttu-id="08dbc-746">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="08dbc-746">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="08dbc-747">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="08dbc-747">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="08dbc-748">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="08dbc-748">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="08dbc-749">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="08dbc-749">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="08dbc-750">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="08dbc-750">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="08dbc-751">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="08dbc-751">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="08dbc-752">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="08dbc-752">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="08dbc-753">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="08dbc-753">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="08dbc-754">Cmdlets mit optionalem Parameter -RewriteRuleSet aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-754">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="08dbc-755">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="08dbc-755">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="08dbc-756">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="08dbc-756">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="08dbc-757">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="08dbc-757">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="08dbc-758">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="08dbc-758">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="08dbc-759">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="08dbc-759">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="08dbc-760">New-AzureRmApplicationGatewayUrlPathMapConfig: KeyVault-Unterstützung mithilfe von Identität zum Application Gateway hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="08dbc-760">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="08dbc-761">Cmdlets mit optionalem Parameter aktualisiert: -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="08dbc-761">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="08dbc-762">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="08dbc-762">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="08dbc-763">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="08dbc-763">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="08dbc-764">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="08dbc-764">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="08dbc-765">Cmdlet New-AzApplicationGateway mit optionalem Parameter -UserAssignedIdentity aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-765">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="08dbc-766">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="08dbc-766">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="08dbc-767">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="08dbc-767">Az.OperationalInsights</span></span>
- <span data-ttu-id="08dbc-768">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="08dbc-768">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="08dbc-769">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="08dbc-769">Az.Profile</span></span>
- <span data-ttu-id="08dbc-770">Modulnamen in Az.Accounts geändert</span><span class="sxs-lookup"><span data-stu-id="08dbc-770">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="08dbc-771">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-771">Az.RecoveryServices</span></span>
- <span data-ttu-id="08dbc-772">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="08dbc-772">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="08dbc-773">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08dbc-773">Az.Resources</span></span>
- <span data-ttu-id="08dbc-774">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="08dbc-774">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="08dbc-775">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="08dbc-775">Az.ServiceFabric</span></span>
- <span data-ttu-id="08dbc-776">Unterstützung für das Angeben des Zertifikats anhand des allgemeinen Namens und Fingerabdrucks</span><span class="sxs-lookup"><span data-stu-id="08dbc-776">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="08dbc-777">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="08dbc-777">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="08dbc-778">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="08dbc-778">Az.SIgnalR</span></span>
- <span data-ttu-id="08dbc-779">Allgemeine Verfügbarkeit für PowerShell-Cmdlets für SIgnalR</span><span class="sxs-lookup"><span data-stu-id="08dbc-779">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="08dbc-780">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08dbc-780">Az.Sql</span></span>
- <span data-ttu-id="08dbc-781">Neue Erkennungstypen Data_Exfiltration und Unsafe_Action zu Cmdlets für Bedrohungserkennung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-781">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="08dbc-782">Dokumentationsbeispiele für Cmdlets für SQL-Überwachung aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-782">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="08dbc-783">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="08dbc-783">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="08dbc-784">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08dbc-784">Az.Storage</span></span>
- <span data-ttu-id="08dbc-785">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="08dbc-785">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="08dbc-786">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08dbc-786">Az.Websites</span></span>
- <span data-ttu-id="08dbc-787">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="08dbc-787">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="08dbc-788">0.7.0 – Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="08dbc-788">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="08dbc-789">Allgemein</span><span class="sxs-lookup"><span data-stu-id="08dbc-789">General</span></span>

* <span data-ttu-id="08dbc-790">Geringe Änderungen für anstehenden Übergang von AzureRM zu Az</span><span class="sxs-lookup"><span data-stu-id="08dbc-790">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="08dbc-791">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08dbc-791">Az.Compute</span></span>

* <span data-ttu-id="08dbc-792">Unterstützung für UltraSSD und Katalogimages in einfachen Parametersätzen für `New-AzVm(ss)`-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="08dbc-792">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="08dbc-793">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08dbc-793">Az.DataLakeStore</span></span>

* <span data-ttu-id="08dbc-794">Nachgestellten Schrägstrich für die Domäne des ADLS-Kontos korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-794">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="08dbc-795">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="08dbc-795">Az.FrontDoor</span></span>

* <span data-ttu-id="08dbc-796">Einige fehlerhafte Links behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-796">Fixed some broken links</span></span>
    - <span data-ttu-id="08dbc-797">In den Artikeln zu New-AzureRmFrontDoor und Set-AzureRmFrontDoor den Artikel-Link zum Cmdlet „New-AzureRmFrontDoorHealthProbeSettingObject“ korrigiert.</span><span class="sxs-lookup"><span data-stu-id="08dbc-797">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="08dbc-798">Im Artikel zu New-AzureRmFrontDoorManagedRuleObject den Artikel-Link zum Cmdlet „New-AzureRmFrontDoorRuleGroupOverrideObject“ korrigiert.</span><span class="sxs-lookup"><span data-stu-id="08dbc-798">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="08dbc-799">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-799">Az.RecoveryServices</span></span>

* <span data-ttu-id="08dbc-800">Clientseitige Validierungen für Wiederherstellungsvorgänge von Azure-Dateifreigaben hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="08dbc-800">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="08dbc-801">storageAccountName und storageAccountResourceGroupName für AFS-Wiederherstellung optional gemacht.</span><span class="sxs-lookup"><span data-stu-id="08dbc-801">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="08dbc-802">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08dbc-802">Az.Resources</span></span>

* <span data-ttu-id="08dbc-803">Fehlerbehebung für https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="08dbc-803">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="08dbc-804">Get-AzureRmRoleAssignment für die Verwendung des Abonnementbereichs aktualisiert, wenn dieser beim Anfordern von klassischen Administratoren angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="08dbc-804">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="08dbc-805">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08dbc-805">Az.Sql</span></span>

* <span data-ttu-id="08dbc-806">Geringe Änderungen für anstehenden Übergang von AzureRM zu Az</span><span class="sxs-lookup"><span data-stu-id="08dbc-806">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="08dbc-807">Problem mit der Verwendung von Get-AzureRmSqlDatabaseVulnerabilityAssessment mit .NET Core behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-807">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="08dbc-808">Dokumentation mit Hilfemeldungen zu Cmdlets für die SQL-Überwachung geändert.</span><span class="sxs-lookup"><span data-stu-id="08dbc-808">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="08dbc-809">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08dbc-809">Az.Storage</span></span>

* <span data-ttu-id="08dbc-810">-EnableHierarchicalNamespace zu New-AzureRmStorageAccount hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-810">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="08dbc-811">Problem behoben, bei dem für das Copy File-Cmdlet am Ziel kein Quellkontext wiederverwendet werden kann, wenn -DestContext nicht eingegeben wird</span><span class="sxs-lookup"><span data-stu-id="08dbc-811">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="08dbc-812">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="08dbc-812">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="08dbc-813">Unterstützung der Konfiguration von statischen Websites</span><span class="sxs-lookup"><span data-stu-id="08dbc-813">Support Static Website configuration</span></span>
    - <span data-ttu-id="08dbc-814">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="08dbc-814">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="08dbc-815">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="08dbc-815">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="08dbc-816">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08dbc-816">Az.Websites</span></span>

* <span data-ttu-id="08dbc-817">Set-AzureRmWebApp und Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="08dbc-817">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="08dbc-818">Neuen Parameter (-AzureStoragePath) zum Angeben von Azure Storage-Pfaden hinzugefügt, die in Windows- und Linux-Container-Apps bereitgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="08dbc-818">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="08dbc-819">Verwenden Sie die Ausgabe des neuen Cmdlets New-AzureRmWebAppAzureStoragePath als Parameter zum Festlegen der Azure Storage-Pfade.</span><span class="sxs-lookup"><span data-stu-id="08dbc-819">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="08dbc-820">0.6.1 – November 2018</span><span class="sxs-lookup"><span data-stu-id="08dbc-820">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="08dbc-821">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="08dbc-821">Az.ApiManagement</span></span>
* <span data-ttu-id="08dbc-822">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-822">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="08dbc-823">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="08dbc-823">Az.Automation</span></span>
* <span data-ttu-id="08dbc-824">Swagger-basierte Azure Automation-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="08dbc-824">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="08dbc-825">Cmdlets zur Updateverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-825">Added Update Management cmdlets</span></span>
* <span data-ttu-id="08dbc-826">Cmdlets zur Quellcodeverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-826">Added Source Control cmdlets</span></span>
* <span data-ttu-id="08dbc-827">Cmdlet „Remove-AzureRmAutomationHybridWorkerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-827">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="08dbc-828">DSC-Befehl für die Knotenregistrierung korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-828">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="08dbc-829">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08dbc-829">Az.Compute</span></span>
* <span data-ttu-id="08dbc-830">Identitätsproblem für SystemAssigned-Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-830">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="08dbc-831">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-831">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="08dbc-832">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="08dbc-832">Az.ContainerInstance</span></span>
* <span data-ttu-id="08dbc-833">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-833">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="08dbc-834">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="08dbc-834">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="08dbc-835">Beschreibung der Beispiele für Marketplace-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-835">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="08dbc-836">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08dbc-836">Az.Network</span></span>
* <span data-ttu-id="08dbc-837">Folgende Cmdlets hinzugefügt: New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="08dbc-837">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="08dbc-838">ICMP wieder unterstützten AzureFirewall-Netzwerkprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-838">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="08dbc-839">Cmdlet „Test-AzureRmNetworkWatcherConnectivity“ aktualisiert und Überprüfung für Ziel-ID, Adresse und Port hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-839">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="08dbc-840">Probleme mit Arbeitsspeicherauslastung in der VirtualNetwork-Zuordnung behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-840">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="08dbc-841">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="08dbc-841">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="08dbc-842">Problem beim Ändern der Richtlinie für eine geschützte Dateifreigabe behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-842">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="08dbc-843">Richtlinienzeitzone in Großschreibung geändert</span><span class="sxs-lookup"><span data-stu-id="08dbc-843">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="08dbc-844">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="08dbc-844">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="08dbc-845">Korrigiertes Beispiel in „New-AzureRmRecoveryServicesAsrProtectableItem“</span><span class="sxs-lookup"><span data-stu-id="08dbc-845">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="08dbc-846">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-846">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="08dbc-847">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="08dbc-847">Az.Relay</span></span>
* <span data-ttu-id="08dbc-848">Optionaler Parameter „-KeyValue“ zu Cmdlet „New-AzureRmRelayKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht</span><span class="sxs-lookup"><span data-stu-id="08dbc-848">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="08dbc-849">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08dbc-849">Az.Resources</span></span>
* <span data-ttu-id="08dbc-850">Hilfedokumentation für ressourcenidentitätsbezogene Parameter in `New-AzureRmPolicyAssignment` und `Set-AzureRmPolicyAssignment` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-850">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="08dbc-851">Beispiel für „New-AzureRmPolicyDefinition“ hinzugefügt, das „-Metadata“ nutzt</span><span class="sxs-lookup"><span data-stu-id="08dbc-851">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="08dbc-852">Korrektur, um Beibehaltung von Groß-/Kleinschreibung in Tagschlüsseln in „NetStandard“ zu ermöglichen: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="08dbc-852">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="08dbc-853">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="08dbc-853">Az.ServiceFabric</span></span>
* <span data-ttu-id="08dbc-854">Benachrichtigung über veraltete Elemente für anstehende wichtige Änderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-854">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="08dbc-855">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08dbc-855">Az.Sql</span></span>
* <span data-ttu-id="08dbc-856">Neue Cmdlets für CRUD-Vorgänge in verwalteten Azure SQL-Datenbank-Instanzen und verwalteten Azure SQL-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-856">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="08dbc-857">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="08dbc-857">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="08dbc-858">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="08dbc-858">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="08dbc-859">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="08dbc-859">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="08dbc-860">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="08dbc-860">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="08dbc-861">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="08dbc-861">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="08dbc-862">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="08dbc-862">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="08dbc-863">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="08dbc-863">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="08dbc-864">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="08dbc-864">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="08dbc-865">Erweiterte Verwaltung von Überwachungsrichtlinien auf einem Server oder in einer Datenbank aktiviert</span><span class="sxs-lookup"><span data-stu-id="08dbc-865">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="08dbc-866">Neuer Parameter (PredicateExpression) hinzugefügt, um die Filterung von Überwachungsprotokollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="08dbc-866">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="08dbc-867">Cmdlets wurden angepasst, sodass sie SQL-Clients anstelle von Legacyclients verwenden.</span><span class="sxs-lookup"><span data-stu-id="08dbc-867">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="08dbc-868">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="08dbc-868">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="08dbc-869">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="08dbc-869">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="08dbc-870">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="08dbc-870">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="08dbc-871">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="08dbc-871">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="08dbc-872">Problem bei Verwendung von „Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings“ mit festgelegtem Parameter für den Speicherkontonamen behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-872">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="08dbc-873">0.5.0 – November 2018</span><span class="sxs-lookup"><span data-stu-id="08dbc-873">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="08dbc-874">Allgemein</span><span class="sxs-lookup"><span data-stu-id="08dbc-874">General</span></span>
* <span data-ttu-id="08dbc-875">Ressourcenvervollständigungen für viele Kern-Cmdlets hinzugefügt (diese ermöglichen das Durchlaufen von vorhandenen Ressourcennamen per TAB-TASTE, wenn Cmdlets interaktiv aufgerufen werden)</span><span class="sxs-lookup"><span data-stu-id="08dbc-875">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="08dbc-876">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="08dbc-876">Az.Profile</span></span>
* <span data-ttu-id="08dbc-877">Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="08dbc-877">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="08dbc-878">Parameter „TenantId“ im Cmdlet „Connect-AzAccount“ in „Tenant“ umbenannt und Alias für „TenantId“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-878">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="08dbc-879">Beschreibung von „TenantId“ für „Connect-AzAccount“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-879">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="08dbc-880">Fehlermeldung für fehlgeschlagene Anmeldung bei Angabe der Mandantendomäne korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-880">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="08dbc-881">Problem in Bezug auf Kontextnamenskonflikt für Konten ohne Abonnements im Mandanten behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-881">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="08dbc-882">Problem mit DataLake-Endpunkten bei Verwendung von MSI behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-882">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="08dbc-883">Problem behoben, das zur Auslösung von „Disconnect-AzAccount“ führte, wenn keine Verbindung bestand</span><span class="sxs-lookup"><span data-stu-id="08dbc-883">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="08dbc-884">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-884">Az.CognitiveServices</span></span>
* <span data-ttu-id="08dbc-885">Vorgang „Get-AzCognitiveServicesAccountSkus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-885">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08dbc-886">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08dbc-886">Az.Compute</span></span>
* <span data-ttu-id="08dbc-887">Cmdlets Add-AzVmssVMDataDisk und Remove-AzVmssVMDataDisk hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-887">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="08dbc-888">„Get-AzVMImage“ zeigt „AutomaticOSUpgradeProperties“ an</span><span class="sxs-lookup"><span data-stu-id="08dbc-888">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="08dbc-889">Problem behoben, aufgrund dessen die Optionswerte „SetAzVMChefExtension -BootstrapOptions“ und „-JsonAttribute“ nicht im JSON-Format festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="08dbc-889">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="08dbc-890">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08dbc-890">Az.DataLakeStore</span></span>
* <span data-ttu-id="08dbc-891">Aktualisierung des DataLake-Pakets auf 1.1.10</span><span class="sxs-lookup"><span data-stu-id="08dbc-891">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="08dbc-892">Standardmäßige Parallelität zu Multithreadvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-892">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="08dbc-893">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="08dbc-893">Az.Insights</span></span>
* <span data-ttu-id="08dbc-894">Problem Nr. 7267 behoben (Bereich für automatische Skalierung)</span><span class="sxs-lookup"><span data-stu-id="08dbc-894">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="08dbc-895">Probleme beim Erstellen einer neuen Regel für die automatische Skalierung, aufgrund derer die aufgelisteten Parameter nicht richtig festgelegt wurden (Es wurde stets der Standardwert festgelegt.)</span><span class="sxs-lookup"><span data-stu-id="08dbc-895">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="08dbc-896">Problem Nr. 7513 behoben [Insights] „Set-AzDiagnosticSetting“ erfordert die explizite Angabe von Kategorien während der Erstellung der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="08dbc-896">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="08dbc-897">Nun erfordert das Cmdlet nicht die explizite Angabe der Kategorien, die während der Erstellung aktiviert werden sollen. Das bedeutet, es funktioniert wie dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="08dbc-897">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08dbc-898">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08dbc-898">Az.Network</span></span>
* <span data-ttu-id="08dbc-899">„PeeringType“ wurde geändert und ist nun ein erforderlicher Parameter für die folgenden Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="08dbc-899">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="08dbc-900">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="08dbc-900">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="08dbc-901">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="08dbc-901">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="08dbc-902">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="08dbc-902">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="08dbc-903">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="08dbc-903">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="08dbc-904">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="08dbc-904">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="08dbc-905">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="08dbc-905">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="08dbc-906">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="08dbc-906">Az.PolicyInsights</span></span>
* <span data-ttu-id="08dbc-907">Cmdlets für Richtlinienwartung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-907">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="08dbc-908">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08dbc-908">Az.Resources</span></span>
* <span data-ttu-id="08dbc-909">Fehlerbehebung für https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="08dbc-909">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="08dbc-910">Zulassen der Auflistung von Ressourcen mithilfe des Parameters „-ResourceId“ für „Get-AzResource“</span><span class="sxs-lookup"><span data-stu-id="08dbc-910">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="08dbc-911">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="08dbc-911">Az.ServiceBus</span></span>
* <span data-ttu-id="08dbc-912">Schreibgeschützte Eigenschaft „MigrationState“ zu „PSServiceBusMigrationConfigurationAttributes“ hinzugefügt, was das Ermitteln des Migrationsstatus ermöglicht</span><span class="sxs-lookup"><span data-stu-id="08dbc-912">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="08dbc-913">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="08dbc-913">Az.ServiceFabric</span></span>
* <span data-ttu-id="08dbc-914">Hinzufügen des Zertifikats zu Linux VMSS korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-914">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="08dbc-915">„Add-AzServiceFabricClusterCertificate“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="08dbc-915">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="08dbc-916">Verwenden des richtigen Fingerabdrucks aus dem neuen Zertifikat (Azure/service-fabric-issues#932)</span><span class="sxs-lookup"><span data-stu-id="08dbc-916">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="08dbc-917">Richtige Anzeige von Ausnahmen (Azure/service-fabric-issues#1054)</span><span class="sxs-lookup"><span data-stu-id="08dbc-917">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="08dbc-918">„Update-AzServiceFabricDurability“ korrigiert, um die Clusterkonfiguration zu aktualisieren, bevor der VMSS-Vorgang „CreateOrUpdate“ gestartet wird</span><span class="sxs-lookup"><span data-stu-id="08dbc-918">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="08dbc-919">0.4.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="08dbc-919">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="08dbc-920">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="08dbc-920">Az.Profile</span></span>
* <span data-ttu-id="08dbc-921">Problem mit „Get-AzSubscription“ in Cloud Shell behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-921">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="08dbc-922">Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="08dbc-922">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08dbc-923">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08dbc-923">Az.Compute</span></span>
* <span data-ttu-id="08dbc-924">Neue Größen zur Whitelist von VM-Größen hinzugefügt, für die bei Verwendung des einfachen Parametersatzes für „New-AzVm“ der beschleunigte Netzwerkbetrieb aktiviert wird</span><span class="sxs-lookup"><span data-stu-id="08dbc-924">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="08dbc-925">ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="08dbc-925">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="08dbc-926">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08dbc-926">Az.DataLakeStore</span></span>
* <span data-ttu-id="08dbc-927">Unterstützung für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-927">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="08dbc-928">Get-AzDataLakeStoreVirtualNetworkRule: Dient zum Abrufen oder Auflisten der Azure Data Lake Store-Regel für das virtuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="08dbc-928">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="08dbc-929">Add-AzDataLakeStoreVirtualNetworkRule: Fügt dem angegebenen Data Lake Store-Konto eine Regel für das virtuelle Netzwerk hinzu.</span><span class="sxs-lookup"><span data-stu-id="08dbc-929">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="08dbc-930">Set-AzDataLakeStoreVirtualNetworkRule: Ändert die angegebene Regel für das virtuelle Netzwerk in das angegebene Data Lake Store-Konto.</span><span class="sxs-lookup"><span data-stu-id="08dbc-930">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="08dbc-931">Remove-AzDataLakeStoreVirtualNetworkRule: Dient zum Löschen der Azure Data Lake Store-Regel für das virtuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="08dbc-931">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08dbc-932">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08dbc-932">Az.Network</span></span>
* <span data-ttu-id="08dbc-933">Cmdlet „Test-AzNetworkWatcherConnectivity“ aktualisiert, Protokollwert wird jetzt an Back-End übergeben.</span><span class="sxs-lookup"><span data-stu-id="08dbc-933">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="08dbc-934">ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="08dbc-934">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="08dbc-935">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08dbc-935">Az.Resources</span></span>
* <span data-ttu-id="08dbc-936">Problem behoben, aufgrund dessen „Get-AzRoleDefinition“ eine unverständliche Ausnahme auslöst (wenn das Standardprofil kein Abonnement enthält und kein Bereich festgelegt ist), indem im Szenario eine aussagekräftige Ausnahme hinzugefügt wurde.</span><span class="sxs-lookup"><span data-stu-id="08dbc-936">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="08dbc-937">Außerdem wurde der Standardparametersatz auf „RoleDefinitionNameParameterSet“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="08dbc-937">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="08dbc-938">0.3.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="08dbc-938">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="08dbc-939">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="08dbc-939">Azure.Storage</span></span>
* <span data-ttu-id="08dbc-940">Fehler beim Kopieren von Blobs/Dateien behoben, aufgrund dessen bei einem Metadatenproblem des Ziels keine Metadaten kopiert wurden</span><span class="sxs-lookup"><span data-stu-id="08dbc-940">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="08dbc-941">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="08dbc-941">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="08dbc-942">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="08dbc-942">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="08dbc-943">Der Abruf der Speicherressourcennutzung eines bestimmten Standorts wird jetzt unterstützt, und das Hinzufügen einer Warnmeldung für den Abruf der globalen Speicherressourcennutzung ist überflüssig.</span><span class="sxs-lookup"><span data-stu-id="08dbc-943">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="08dbc-944">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="08dbc-944">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="08dbc-945">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="08dbc-945">Az.CognitiveServices</span></span>
* <span data-ttu-id="08dbc-946">„Get-AzCognitiveServicesAccountSkus“ wird ohne vorhandenes Konto unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08dbc-946">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08dbc-947">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08dbc-947">Az.Compute</span></span>
* <span data-ttu-id="08dbc-948">Korrektur von „Get-AzVM -ResourceGroupName <rg>“, sodass ggf. mehr als 50 Ergebnisse zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="08dbc-948">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="08dbc-949">Der Cmdlet-Hilfe zu „New-AzVmss“ wurde ein Beispiel für „SimpleParameterSet“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="08dbc-949">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="08dbc-950">Tippfehler in der Azure Disk Encryption-Statusmeldung behoben</span><span class="sxs-lookup"><span data-stu-id="08dbc-950">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="08dbc-951">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="08dbc-951">Az.DataFactoryV2</span></span>
* <span data-ttu-id="08dbc-952">Die Version des ADF .Net-SDK wurde auf 2.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="08dbc-952">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08dbc-953">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08dbc-953">Az.Network</span></span>
* <span data-ttu-id="08dbc-954">NetworkProfile-Funktionalität wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="08dbc-954">Added NetworkProfile functionality.</span></span> <span data-ttu-id="08dbc-955">Neue Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-955">new cmdlets added</span></span>
    - <span data-ttu-id="08dbc-956">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="08dbc-956">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="08dbc-957">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="08dbc-957">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="08dbc-958">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="08dbc-958">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="08dbc-959">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="08dbc-959">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="08dbc-960">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="08dbc-960">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="08dbc-961">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="08dbc-961">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="08dbc-962">Dienstzuordnungslink in Subnetzmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-962">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="08dbc-963">Cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-963">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="08dbc-964">Cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-964">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="08dbc-965">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="08dbc-965">Az.RedisCache</span></span>
* <span data-ttu-id="08dbc-966">Künftig sind beliebige Zeichenfolgen als Größenparameter zulässig.</span><span class="sxs-lookup"><span data-stu-id="08dbc-966">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="08dbc-967">P5 in Popup „PSArgumentCompleter“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-967">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="08dbc-968">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08dbc-968">Az.Resources</span></span>
* <span data-ttu-id="08dbc-969">Fehlender Parameter „-Mode“ zu „Set-AzPolicyDefinition“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="08dbc-969">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="08dbc-970">Cmdlet-Fehler bei „Get-AzProviderOperation“ für Vorgänge mit Ursprung behoben, der den Benutzer enthält</span><span class="sxs-lookup"><span data-stu-id="08dbc-970">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="08dbc-971">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08dbc-971">Az.Sql</span></span>
* <span data-ttu-id="08dbc-972">Problem behoben, aufgrund dessen einige Sicherungs-Cmdlets das aktuelle Azure-Abonnements nicht erkannt haben</span><span class="sxs-lookup"><span data-stu-id="08dbc-972">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08dbc-973">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08dbc-973">Az.Websites</span></span>
* <span data-ttu-id="08dbc-974">Neues Cmdlet „Get-AzWebAppContainerContinuousDeploymentUrl“ zum Abrufen der Webhook-URL von Continuous Deployment für Container</span><span class="sxs-lookup"><span data-stu-id="08dbc-974">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="08dbc-975">Neue Cmdlets „New-AzWebAppContainerPSSession“ und „Enter-WebAppContainerPSSession“ zum Initiieren einer PowerShell-Remotesitzung in einer Windows-Container-App</span><span class="sxs-lookup"><span data-stu-id="08dbc-975">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="08dbc-976">0.2.0 – September 2018</span><span class="sxs-lookup"><span data-stu-id="08dbc-976">0.2.0 - September 2018</span></span>
 <span data-ttu-id="08dbc-977">Erste Version</span><span class="sxs-lookup"><span data-stu-id="08dbc-977">Initial Release</span></span>