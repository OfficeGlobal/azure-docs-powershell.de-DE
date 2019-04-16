---
ms.openlocfilehash: 54d7a9da878e085e90479fb229876c9be6dafd74
ms.sourcegitcommit: 89066b7c4b527357bb2024e1ad708df84c131804
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/09/2019
ms.locfileid: "59364140"
---
## <a name="170---april-2019"></a><span data-ttu-id="28f95-101">1.7.0: April 2019</span><span class="sxs-lookup"><span data-stu-id="28f95-101">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="28f95-102">Highlights seit der letzten Hauptversion</span><span class="sxs-lookup"><span data-stu-id="28f95-102">Highlights since the last major release</span></span>
* <span data-ttu-id="28f95-103">Allgemeine Verfügbarkeit des `Az`-Moduls</span><span class="sxs-lookup"><span data-stu-id="28f95-103">General availability of `Az` module</span></span>
* <span data-ttu-id="28f95-104">Weitere Informationen zum `Az`-Modul finden Sie unter folgendem Link: https://aka.ms/azps-announce.</span><span class="sxs-lookup"><span data-stu-id="28f95-104">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="28f95-105">Vervollständigung für Location, ResourceGroup und ResourceName hinzugefügt: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/.</span><span class="sxs-lookup"><span data-stu-id="28f95-105">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="28f95-106">Unterstützung für Platzhalter zu Get-Cmdlets für Az.Compute und Az.Network hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-106">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="28f95-107">Interaktive und Benutzername/Kennwort-Authentifizierung ausschließlich für Windows PowerShell 5.1 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-107">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="28f95-108">Unterstützung für Python 2-Runbooks in Az.Automation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-108">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="28f95-109">Az.LogicApp: Neue Cmdlets für Integrationskonto-Assemblys und -Batchkonfiguration</span><span class="sxs-lookup"><span data-stu-id="28f95-109">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="28f95-110">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="28f95-110">Az.Accounts</span></span>
* <span data-ttu-id="28f95-111">„Add-AzEnvironment“ und „Set-AzEnvironment“ aktualisiert, um den Parameter „AzureAnalysisServicesEndpointResourceId“ zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="28f95-111">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="28f95-112">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="28f95-112">Az.AnalysisServices</span></span>
* <span data-ttu-id="28f95-113">ServiceClient wird in Cmdlets für die Datenebene verwendet, und die ursprüngliche Authentifizierungslogik wird entfernt.</span><span class="sxs-lookup"><span data-stu-id="28f95-113">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="28f95-114">„Add-AzureASAccount“ wird als Wrapper von „Connect-AzAccount“ festgelegt, um einen Breaking Change zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="28f95-114">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="28f95-115">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="28f95-115">Az.Automation</span></span>
* <span data-ttu-id="28f95-116">Fehler des Cmdlets „Fixed New-AzAutomationSoftwareUpdateConfiguration“ für Einschlüsse behoben.</span><span class="sxs-lookup"><span data-stu-id="28f95-116">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="28f95-117">Die Parameter „IncludedKbNumber“ und „IncludedPackageNameMask“ sollten nun funktionieren.</span><span class="sxs-lookup"><span data-stu-id="28f95-117">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="28f95-118">Fehlerbehebung für eine dynamische Gruppe der Azure Automation-Updateverwaltung</span><span class="sxs-lookup"><span data-stu-id="28f95-118">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="28f95-119">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="28f95-119">Az.Compute</span></span>
* <span data-ttu-id="28f95-120">Parameter „HyperVGeneration“ zu „New-AzDiskConfig“ und „New-AzSnapshotConfig“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-120">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="28f95-121">Zulassen der VM-Erstellung mit einem Katalogimage aus anderen Mandanten</span><span class="sxs-lookup"><span data-stu-id="28f95-121">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="28f95-122">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="28f95-122">Az.ContainerInstance</span></span>
* <span data-ttu-id="28f95-123">Problem im Parameter „-Command“ von „New-AzContainerGroup“ behoben, das dazu führte, dass ein nachgestelltes leeres Argument hinzugefügt wurde</span><span class="sxs-lookup"><span data-stu-id="28f95-123">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="28f95-124">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="28f95-124">Az.DataFactory</span></span>
* <span data-ttu-id="28f95-125">Version des ADF .NET SDK auf 3.0.2 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-125">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="28f95-126">Cmdlet „Set-AzDataFactoryV2“ mit zusätzlichen Parametern für RepoConfiguration-Einstellungen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-126">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="28f95-127">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="28f95-127">Az.Resources</span></span>
* <span data-ttu-id="28f95-128">Verarbeitung von Anbietern für „Get-AzResource“ bei der Angabe der Parameter „-ResourceId“ oder „-ResourceGroupName“, „-Name“ und „-ResourceType“ verbessert</span><span class="sxs-lookup"><span data-stu-id="28f95-128">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="28f95-129">Fehlerbehandlung für „Test-AzDeployment“ und „Test-AzResourceGroupDeployment“ verbessert</span><span class="sxs-lookup"><span data-stu-id="28f95-129">Improve error handling for for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="28f95-130">Behandlung von außerhalb der Bereitstellungsüberprüfung aufgetretenen Fehlern und stattdessen Aufnahme in die Ausgabe des Befehls</span><span class="sxs-lookup"><span data-stu-id="28f95-130">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="28f95-131">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="28f95-131">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="28f95-132">Switch-Parameter „-IgnoreDynamicParameters“ zu Bereitstellungs-Cmdlets hinzugefügt, um Aufforderung in Skript- und Auftragsszenarien zu überspringen</span><span class="sxs-lookup"><span data-stu-id="28f95-132">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="28f95-133">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="28f95-133">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="28f95-134">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="28f95-134">Az.Sql</span></span>
* <span data-ttu-id="28f95-135">Unterstützung für Klassifizierung von Datenbankdaten</span><span class="sxs-lookup"><span data-stu-id="28f95-135">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="28f95-136">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="28f95-136">Az.Storage</span></span>
* <span data-ttu-id="28f95-137">Melden eines ausführlichen Fehlers beim Erstellen des Storage-Kontexts mit dem Parameter „-UseConnectedAccount“, aber ohne Azure-Anmeldekonto</span><span class="sxs-lookup"><span data-stu-id="28f95-137">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="28f95-138">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="28f95-138">New-AzStorageContext</span></span>
* <span data-ttu-id="28f95-139">Unterstützung für das Verwalten von Blobdiensteigenschaften eines bestimmten Storage-Kontos mit einer API der Verwaltungsebene</span><span class="sxs-lookup"><span data-stu-id="28f95-139">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="28f95-140">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="28f95-140">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="28f95-141">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="28f95-141">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="28f95-142">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="28f95-142">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="28f95-143">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="28f95-143">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="28f95-144">Unterstützung von „-AsJob“ für Cmdlets für den Upload und Download von Blobs und Dateien</span><span class="sxs-lookup"><span data-stu-id="28f95-144">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="28f95-145">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="28f95-145">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="28f95-146">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="28f95-146">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="28f95-147">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="28f95-147">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="28f95-148">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="28f95-148">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="28f95-149">1.6.0: März 2019</span><span class="sxs-lookup"><span data-stu-id="28f95-149">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="28f95-150">Highlights seit der letzten Hauptversion</span><span class="sxs-lookup"><span data-stu-id="28f95-150">Highlights since the last major release</span></span>
* <span data-ttu-id="28f95-151">Allgemeine Verfügbarkeit des `Az`-Moduls</span><span class="sxs-lookup"><span data-stu-id="28f95-151">General availability of `Az` module</span></span>
* <span data-ttu-id="28f95-152">Weitere Informationen zum `Az`-Modul finden Sie unter folgendem Link: https://aka.ms/azps-announce.</span><span class="sxs-lookup"><span data-stu-id="28f95-152">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="28f95-153">Vervollständigung für Location, ResourceGroup und ResourceName hinzugefügt: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/.</span><span class="sxs-lookup"><span data-stu-id="28f95-153">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="28f95-154">Unterstützung für Platzhalter zu Get-Cmdlets für Az.Compute und Az.Network hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-154">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="28f95-155">Interaktive und Benutzername/Kennwort-Authentifizierung ausschließlich für Windows PowerShell 5.1 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-155">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="28f95-156">Unterstützung für Python 2-Runbooks in Az.Automation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-156">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="28f95-157">Az.LogicApp: Neue Cmdlets für Integrationskonto-Assemblys und -Batchkonfiguration</span><span class="sxs-lookup"><span data-stu-id="28f95-157">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="28f95-158">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="28f95-158">Az.Automation</span></span>
* <span data-ttu-id="28f95-159">Änderung an der Azure Automation-Updateverwaltung, um die folgenden neuen Features zu unterstützen:</span><span class="sxs-lookup"><span data-stu-id="28f95-159">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="28f95-160">Dynamische Gruppierung</span><span class="sxs-lookup"><span data-stu-id="28f95-160">Dynamic grouping</span></span>
    * <span data-ttu-id="28f95-161">Pre-/Post-Skripts</span><span class="sxs-lookup"><span data-stu-id="28f95-161">Pre-Post script</span></span>
    * <span data-ttu-id="28f95-162">Neustarteinstellung</span><span class="sxs-lookup"><span data-stu-id="28f95-162">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="28f95-163">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="28f95-163">Az.Compute</span></span>
* <span data-ttu-id="28f95-164">Problem mit der Pfadauflösung in „Get-AzVmBootDiagnosticsData“ behoben</span><span class="sxs-lookup"><span data-stu-id="28f95-164">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="28f95-165">Computeclientbibliothek auf 25.0.0. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-165">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="28f95-166">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="28f95-166">Az.KeyVault</span></span>
* <span data-ttu-id="28f95-167">Unterstützung für Platzhalterzeichen zu KeyVault-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-167">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="28f95-168">Az.Network</span><span class="sxs-lookup"><span data-stu-id="28f95-168">Az.Network</span></span>
* <span data-ttu-id="28f95-169">Threat Intelligence-Unterstützung für Azure Firewall hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-169">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="28f95-170">Ressource der obersten Ebene für Application Gateway-Firewallrichtlinie und benutzerdefinierte Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-170">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="28f95-171">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="28f95-171">Az.RecoveryServices</span></span>
* <span data-ttu-id="28f95-172">SnapshotRetentionInDays in Azure-VM-Richtlinie hinzugefügt, um sofortigen Wiederherstellungspunkt zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="28f95-172">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="28f95-173">Pipe-Unterstützung für das Aufheben der Registrierung eines Containers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-173">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="28f95-174">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="28f95-174">Az.Resources</span></span>
* <span data-ttu-id="28f95-175">Unterstützung für Platzhalterzeichen für Get-AzResource und Get-AzResourceGroup aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-175">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="28f95-176">Anmeldeinformationen aktualisiert, die beim Senden generischer Aufrufe an ARM verwendet werden</span><span class="sxs-lookup"><span data-stu-id="28f95-176">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="28f95-177">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="28f95-177">Az.Sql</span></span>
* <span data-ttu-id="28f95-178">Der Cmdlet-Parameter der Bedrohungserkennung (ExcludeDetectionType) wurde von „DetectionType“ in „string[]“ geändert, um ihn zukunftssicher zu machen, wenn neue DetectionTypes-Elemente hinzugefügt werden, und um AutoVervollständigen zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="28f95-178">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="28f95-179">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="28f95-179">Az.Storage</span></span>
* <span data-ttu-id="28f95-180">Unterstützung von Get-/Set-/Remove-Verwaltungsrichtlinien für Speicherkonto hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-180">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="28f95-181">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="28f95-181">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="28f95-182">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="28f95-182">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="28f95-183">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="28f95-183">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="28f95-184">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="28f95-184">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="28f95-185">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="28f95-185">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="28f95-186">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="28f95-186">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="28f95-187">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="28f95-187">Az.Websites</span></span>
* <span data-ttu-id="28f95-188">ARM-Vorlagenfehler behoben, der zu einem Problem beim Klonen aller Slots mithilfe von „New-AzWebApp -IncludeSourceWebAppSlots“ führte</span><span class="sxs-lookup"><span data-stu-id="28f95-188">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="28f95-189">1.5.0: März 2019</span><span class="sxs-lookup"><span data-stu-id="28f95-189">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="28f95-190">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="28f95-190">Az.Accounts</span></span>
* <span data-ttu-id="28f95-191">Der Befehl „Register-AzModule“ wurde hinzugefügt, um von AutoRest generierte Cmdlets zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="28f95-191">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="28f95-192">Beispiele für „Connect-AzAccount“ wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="28f95-192">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="28f95-193">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="28f95-193">Az.Automation</span></span>
* <span data-ttu-id="28f95-194">Problem behoben, das beim Abrufen bestimmter monatlicher Zeitpläne in verschiedenen Azure Automation-Cmdlets auftrat</span><span class="sxs-lookup"><span data-stu-id="28f95-194">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="28f95-195">„Get-AzAutomationDscNode“ wurde korrigiert, da nur die 20 obersten Knoten zurückgegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="28f95-195">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="28f95-196">Jetzt werden alle Knoten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28f95-196">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="28f95-197">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="28f95-197">Az.Cdn</span></span>
* <span data-ttu-id="28f95-198">Neue Powershell-Cmdlets zum Aktivieren/Deaktivieren von HTTPS für benutzerdefinierte Domänen hinzugefügt und alte Cmdlets außer Betrieb genommen</span><span class="sxs-lookup"><span data-stu-id="28f95-198">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="28f95-199">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="28f95-199">Az.Compute</span></span>
* <span data-ttu-id="28f95-200">Unterstützung für Platzhalterzeichen zu Get-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-200">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="28f95-201">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="28f95-201">Az.DataFactory</span></span>
* <span data-ttu-id="28f95-202">Version des ADF .NET SDK auf 3.0.1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-202">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="28f95-203">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="28f95-203">Az.LogicApp</span></span>
* <span data-ttu-id="28f95-204">„ListWorkflows“ wurde korrigiert, da nur die erste Seite mit Ergebnissen abgerufen wurde.</span><span class="sxs-lookup"><span data-stu-id="28f95-204">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="28f95-205">Az.Network</span><span class="sxs-lookup"><span data-stu-id="28f95-205">Az.Network</span></span>
* <span data-ttu-id="28f95-206">Unterstützung für Platzhalterzeichen zu Network-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-206">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="28f95-207">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="28f95-207">Az.RecoveryServices</span></span>
* <span data-ttu-id="28f95-208">SQL Server jetzt in Azure-VM-Support enthalten</span><span class="sxs-lookup"><span data-stu-id="28f95-208">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="28f95-209">SDK-Update</span><span class="sxs-lookup"><span data-stu-id="28f95-209">SDK Update</span></span>
* <span data-ttu-id="28f95-210">VMappContainer-Überprüfung in „Get-ProtectableItem“ entfernt</span><span class="sxs-lookup"><span data-stu-id="28f95-210">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="28f95-211">„Name“ und „ServerName“ als Parameter für „Get-ProtectableItem“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-211">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="28f95-212">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="28f95-212">Az.Resources</span></span>
* <span data-ttu-id="28f95-213">Parameter `-TemplateObject` zu Bereitstellungs-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-213">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="28f95-214">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="28f95-214">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="28f95-215">Problem beim Piping des Ergebnisses von `Get-AzResource` an Folgendes behoben:</span><span class="sxs-lookup"><span data-stu-id="28f95-215">Fix issue when piping the result of `Get-AzResource` to</span></span> `Set-AzResource`
    - <span data-ttu-id="28f95-216">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="28f95-216">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="28f95-217">Problem mit JSON-Datentypänderung beim Ausführen des folgenden Cmdlets behoben:</span><span class="sxs-lookup"><span data-stu-id="28f95-217">Fix issue with JSON data type change when running</span></span> `Set-AzResource`
    - <span data-ttu-id="28f95-218">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="28f95-218">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="28f95-219">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="28f95-219">Az.Sql</span></span>
* <span data-ttu-id="28f95-220">„AuditingEndpointsCommunicator“ wird aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="28f95-220">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="28f95-221">Das Verhalten eines Grenzfalls beim Erstellen neuer Diagnoseeinstellungen wurde korrigiert.</span><span class="sxs-lookup"><span data-stu-id="28f95-221">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="28f95-222">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="28f95-222">Az.Storage</span></span>
* <span data-ttu-id="28f95-223">Unterstützung von „Kind BlockBlobStorage“ beim Erstellen eines Speicherkontos: New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="28f95-223">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="28f95-224">1.4.0 – Februar 2019</span><span class="sxs-lookup"><span data-stu-id="28f95-224">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="28f95-225">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="28f95-225">Az.AnalysisServices</span></span>
* <span data-ttu-id="28f95-226">Cmdlet „AddAzureASAccount“ als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="28f95-226">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="28f95-227">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="28f95-227">Az.Automation</span></span>
* <span data-ttu-id="28f95-228">Hilfe für „Import-AzAutomationDscNodeConfiguration“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-228">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="28f95-229">Überprüfung des Konfigurationsnamens zu Cmdlet „Import-AzAutomationDscConfiguration“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-229">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="28f95-230">Fehlerbehandlung für Cmdlet „Import-AzAutomationDscConfiguration“ verbessert</span><span class="sxs-lookup"><span data-stu-id="28f95-230">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="28f95-231">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="28f95-231">Az.CognitiveServices</span></span>
* <span data-ttu-id="28f95-232">„CustomSubdomainName“ als neuer optionaler Parameter für Cmdlet „New-AzCognitiveServicesAccount“ hinzugefügt, das zum Angeben der Unterdomäne für die Ressource verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="28f95-232">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="28f95-233">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="28f95-233">Az.Compute</span></span>
* <span data-ttu-id="28f95-234">Problem mit ID-Parametersätzen behoben</span><span class="sxs-lookup"><span data-stu-id="28f95-234">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="28f95-235">„Get-AzVMExtension“ aktualisiert, sodass alle installierten Erweiterungen aufgelistet werden, wenn der Name-Parameter nicht angegeben ist</span><span class="sxs-lookup"><span data-stu-id="28f95-235">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="28f95-236">Parameter „Tag“ und „ResourceId“ zum Cmdlet „Update-AzImage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-236">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="28f95-237">„Get-AzVmssVM“ ohne Instanz-ID und mit „InstanceView“ können virtuelle VMSS-Computer mit Instanzansicht auflisten.</span><span class="sxs-lookup"><span data-stu-id="28f95-237">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="28f95-238">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="28f95-238">Az.DataLakeStore</span></span>
* <span data-ttu-id="28f95-239">Cmdlets zum Auflisten und Wiederherstellen gelöschter ADL-Elemente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-239">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="28f95-240">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="28f95-240">Az.EventHub</span></span>
* <span data-ttu-id="28f95-241">Neue boolesche Eigenschaft „SkipEmptyArchives“ zum Überspringen leerer Archive in Klasse „CaptureDescription“ von EventHub hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-241">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="28f95-242">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="28f95-242">Az.KeyVault</span></span>
* <span data-ttu-id="28f95-243">Kennzeichnung in „Set-AzKeyVaultSecret“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="28f95-243">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="28f95-244">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="28f95-244">Az.LogicApp</span></span>
* <span data-ttu-id="28f95-245">SKU „Basic“ für Integrationskonten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-245">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="28f95-246">XSLT 2.0, XSLT 3.0 und Liquid-Zuordnungstypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-246">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="28f95-247">Neue Cmdlets für Integrationskonto-Assemblys</span><span class="sxs-lookup"><span data-stu-id="28f95-247">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="28f95-248">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="28f95-248">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="28f95-249">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="28f95-249">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="28f95-250">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="28f95-250">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="28f95-251">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="28f95-251">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="28f95-252">Neue Cmdlets für Integrationskonto-Batchkonfiguration</span><span class="sxs-lookup"><span data-stu-id="28f95-252">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="28f95-253">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="28f95-253">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="28f95-254">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="28f95-254">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="28f95-255">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="28f95-255">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="28f95-256">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="28f95-256">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="28f95-257">Logik-App-SDK auf Version 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-257">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="28f95-258">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="28f95-258">Az.Monitor</span></span>
* <span data-ttu-id="28f95-259">Hilfe für „Get-AzMetric“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-259">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="28f95-260">Az.Network</span><span class="sxs-lookup"><span data-stu-id="28f95-260">Az.Network</span></span>
* <span data-ttu-id="28f95-261">Hilfebeispiel für „Add-AzApplicationGatewayCustomError“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-261">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="28f95-262">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="28f95-262">Az.OperationalInsights</span></span>
* <span data-ttu-id="28f95-263">Zusätzliche Unterstützung für Datenquelle von „New-ApplicationInsights“ und „Get-ApplicationInsights“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="28f95-263">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="28f95-264">Neue Art von „ApplicationInsights“ zum Abrufen von bestimmten und von allen ApplicationInsights-Datenquellen für einen Workspace hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="28f95-264">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="28f95-265">Cmdlet „New-AzOperationalInsightsApplicationInsightsDataSource“ zum Erstellen einer Datenquelle anhand des angegebenen Ressourcenparameters für „Application-Insights“ hinzugefügt: „subscriptionId“, „resourceGroupName“ und „name“.</span><span class="sxs-lookup"><span data-stu-id="28f95-265">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="28f95-266">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="28f95-266">Az.Resources</span></span>
* <span data-ttu-id="28f95-267">Behebung des Problems: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="28f95-267">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="28f95-268">Behebung des Problems: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="28f95-268">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="28f95-269">Behebung des Problems: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="28f95-269">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="28f95-270">Fehler korrigiert, der die wiederholte Erstellung von „KeyCredentials“ verhindert</span><span class="sxs-lookup"><span data-stu-id="28f95-270">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="28f95-271">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="28f95-271">Az.Sql</span></span>
* <span data-ttu-id="28f95-272">Unterstützung für SQL DB Hyperscale-Tarif hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-272">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="28f95-273">Fehler korrigiert, aufgrund dessen die Wiederherstellung wegen der Festlegung unnötiger Eigenschaften in der Wiederherstellungsanforderung fehlschlagen konnte</span><span class="sxs-lookup"><span data-stu-id="28f95-273">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="28f95-274">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="28f95-274">Az.Websites</span></span>
* <span data-ttu-id="28f95-275">Beispiel in „Get-AzWebAppSlotMetrics“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="28f95-275">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="28f95-276">1.3.0: Februar 2019</span><span class="sxs-lookup"><span data-stu-id="28f95-276">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="28f95-277">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="28f95-277">Az.Accounts</span></span>
* <span data-ttu-id="28f95-278">Update auf die aktuelle Version von ClientRuntime durchgeführt</span><span class="sxs-lookup"><span data-stu-id="28f95-278">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="28f95-279">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="28f95-279">Az.AnalysisServices</span></span>
<span data-ttu-id="28f95-280">Allgemeine Verfügbarkeit für Az.AnalysisServices-Modul</span><span class="sxs-lookup"><span data-stu-id="28f95-280">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="28f95-281">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="28f95-281">Az.Compute</span></span>
* <span data-ttu-id="28f95-282">AEM-Erweiterung: Unterstützung für UltraSSD und P60-, P70- und P80-Datenträger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-282">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="28f95-283">Hilfebeschreibung für „Set-AzVMBootDiagnostics“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-283">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="28f95-284">Hilfebeschreibung und Beispiel für „Update-AzImage“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-284">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="28f95-285">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="28f95-285">Az.RecoveryServices</span></span>
<span data-ttu-id="28f95-286">Allgemeine Verfügbarkeit für Az.RecoveryServices-Modul.</span><span class="sxs-lookup"><span data-stu-id="28f95-286">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="28f95-287">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="28f95-287">Az.Resources</span></span>
* <span data-ttu-id="28f95-288">Kennzeichnung für Ressourcengruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="28f95-288">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="28f95-289">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="28f95-289">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="28f95-290">Problem behoben, bei dem „-ErrorAction“ von `Get-AzureRmRoleAssignment` nicht berücksichtigt wird</span><span class="sxs-lookup"><span data-stu-id="28f95-290">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="28f95-291">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="28f95-291">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="28f95-292">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="28f95-292">Az.Sql</span></span>
* <span data-ttu-id="28f95-293">Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-293">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="28f95-294">Problem behoben, bei dem eine fehlende Anmeldung am Azure-Konto bei der Ausführung von SQL-Cmdlets zu einer nullref-Ausnahme führt</span><span class="sxs-lookup"><span data-stu-id="28f95-294">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="28f95-295">nullref-Ausnahme in Get-AzSqlCapability korrigiert</span><span class="sxs-lookup"><span data-stu-id="28f95-295">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="28f95-296">1.2.1: Januar 2019</span><span class="sxs-lookup"><span data-stu-id="28f95-296">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="28f95-297">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="28f95-297">Az.Accounts</span></span>
* <span data-ttu-id="28f95-298">Release mit richtiger Version der Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="28f95-298">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="28f95-299">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="28f95-299">Az.AnalysisServices</span></span>
* <span data-ttu-id="28f95-300">Release mit aktualisierter Authentifizierungsabhängigkeit</span><span class="sxs-lookup"><span data-stu-id="28f95-300">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="28f95-301">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="28f95-301">Az.RecoveryServices</span></span>
* <span data-ttu-id="28f95-302">Release mit aktualisierter Authentifizierungsabhängigkeit</span><span class="sxs-lookup"><span data-stu-id="28f95-302">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="28f95-303">1.2.0: Januar 2019</span><span class="sxs-lookup"><span data-stu-id="28f95-303">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="28f95-304">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="28f95-304">Az.Accounts</span></span>
* <span data-ttu-id="28f95-305">Interaktive und Benutzername/Kennwort-Authentifizierung ausschließlich für Windows PowerShell 5.1 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-305">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="28f95-306">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-306">Update incorrect online help URLs</span></span>
* <span data-ttu-id="28f95-307">Warnmeldung in PS Core für „Uninstall-AzureRm“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-307">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="28f95-308">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="28f95-308">Az.Aks</span></span>
* <span data-ttu-id="28f95-309">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-309">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="28f95-310">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="28f95-310">Az.Automation</span></span>
* <span data-ttu-id="28f95-311">Unterstützung für Python 2-Runbooks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-311">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="28f95-312">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-312">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="28f95-313">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="28f95-313">Az.Cdn</span></span>
* <span data-ttu-id="28f95-314">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-314">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="28f95-315">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="28f95-315">Az.Compute</span></span>
* <span data-ttu-id="28f95-316">Cmdlet „Invoke-AzVMReimage“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-316">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="28f95-317">Parameter „TempDisk“ zu „Set-AzVmss“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-317">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="28f95-318">Warnmeldung von „New-AzVM“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="28f95-318">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="28f95-319">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="28f95-319">Az.ContainerRegistry</span></span>
* <span data-ttu-id="28f95-320">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-320">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="28f95-321">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="28f95-321">Az.DataFactory</span></span>
* <span data-ttu-id="28f95-322">Version des ADF .NET SDK auf 3.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-322">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="28f95-323">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="28f95-323">Az.DataLakeStore</span></span>
* <span data-ttu-id="28f95-324">Problem mit ADLS-Endpunkt bei Verwendung von MSI behoben</span><span class="sxs-lookup"><span data-stu-id="28f95-324">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="28f95-325">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="28f95-325">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="28f95-326">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-326">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="28f95-327">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="28f95-327">Az.IotHub</span></span>
* <span data-ttu-id="28f95-328">Codierungsformat zu Cmdlet „Add-IotHubRoutingEndpoint“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-328">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="28f95-329">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="28f95-329">Az.KeyVault</span></span>
* <span data-ttu-id="28f95-330">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-330">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="28f95-331">Az.Network</span><span class="sxs-lookup"><span data-stu-id="28f95-331">Az.Network</span></span>
* <span data-ttu-id="28f95-332">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-332">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="28f95-333">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="28f95-333">Az.Resources</span></span>
* <span data-ttu-id="28f95-334">Fehlerhafte Beispiele in Referenzdokumentation zu „New-AzADAppCredential“ und „New-AzADSpCredential“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="28f95-334">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="28f95-335">Problem behoben, bei dem der Pfad für den Parameter „-TemplateFile“ nicht aufgelöst wurde, bevor Cmdlets für die Bereitstellung von Ressourcengruppen ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="28f95-335">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="28f95-336">Az.Resources: Richtige Dokumentation für Standardwert von „New-AzureRmPolicyDefinition -Mode“ bereitgestellt</span><span class="sxs-lookup"><span data-stu-id="28f95-336">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="28f95-337">Az.Resources: Behebung des Problems: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="28f95-337">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="28f95-338">Az.Resources: Behebung des Problems: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="28f95-338">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="28f95-339">Formatierungsproblem für Objekt „PSResourceGroupDeployment“ behoben</span><span class="sxs-lookup"><span data-stu-id="28f95-339">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="28f95-340">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="28f95-340">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="28f95-341">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="28f95-341">Az.ServiceFabric</span></span>
* <span data-ttu-id="28f95-342">Rollback beim Hinzufügen eines Zertifikats zum VMSS-Modell, Auslösung einer Ausnahme. Fehlerbehebung: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="28f95-342">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="28f95-343">Einige Fehlermeldungen wurden korrigiert.</span><span class="sxs-lookup"><span data-stu-id="28f95-343">Fix some error messages.</span></span>
* <span data-ttu-id="28f95-344">Fehler bei Clustererstellung mit ARM-Standardvorlage für „New-AzServiceFabriCluster“ behoben, bei dem die Migration zu Az nicht funktioniert hat.</span><span class="sxs-lookup"><span data-stu-id="28f95-344">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="28f95-345">Fehler behoben beim Hinzufügen eines Cluster-/Anwendungszertifikats ausschließlich zu VM Scale Sets, die zum Cluster gehören, indem die Cluster-ID in der Erweiterung überprüft wird.</span><span class="sxs-lookup"><span data-stu-id="28f95-345">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="28f95-346">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="28f95-346">Az.SignalR</span></span>
* <span data-ttu-id="28f95-347">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-347">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="28f95-348">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="28f95-348">Az.Sql</span></span>
* <span data-ttu-id="28f95-349">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-349">Update incorrect online help URLs</span></span>
* <span data-ttu-id="28f95-350">Parameterbeschreibung für den Parameter „LicenseType“ mit möglichen Werten aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-350">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="28f95-351">Fehler behoben, bei dem die Aktualisierung der Identität der verwalteten Instanz nicht funktioniert hat, wenn es sich um die einzige aktualisierte Eigenschaft gehandelt hat</span><span class="sxs-lookup"><span data-stu-id="28f95-351">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="28f95-352">Unterstützung für die benutzerdefinierte Sortierung auf verwalteter Instanz</span><span class="sxs-lookup"><span data-stu-id="28f95-352">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="28f95-353">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="28f95-353">Az.Storage</span></span>
* <span data-ttu-id="28f95-354">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-354">Update incorrect online help URLs</span></span>
* <span data-ttu-id="28f95-355">Ausführliche Fehlermeldung beim Abrufen/Festlegen der klassischen Protokollierung bzw. Metriken für Storage Premium-Konto, da für das Storage Premium-Konto die klassische Protokollierung bzw. Metriken nicht unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="28f95-355">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="28f95-356">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="28f95-356">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="28f95-357">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="28f95-357">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="28f95-358">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="28f95-358">Az.TrafficManager</span></span>
* <span data-ttu-id="28f95-359">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-359">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="28f95-360">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="28f95-360">Az.Websites</span></span>
* <span data-ttu-id="28f95-361">Fehlerhafte URLs für Onlinehilfe aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-361">Update incorrect online help URLs</span></span>
* <span data-ttu-id="28f95-362">„New-AzWebAppSSLBinding“ korrigiert, damit das Zertifikat in die richtige Ressourcengruppe bzw. an den richtigen Speicherort hochgeladen wird, wenn die App in einer ASE gehostet wird.</span><span class="sxs-lookup"><span data-stu-id="28f95-362">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="28f95-363">„New-AzWebAppSSLBinding“ korrigiert, damit die Tags beim Binden eines SSL-Zertifikats an eine App nicht überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="28f95-363">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="28f95-364">1.1.0 – Januar 2019</span><span class="sxs-lookup"><span data-stu-id="28f95-364">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="28f95-365">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="28f95-365">Az.Accounts</span></span>
* <span data-ttu-id="28f95-366">Bereich „Local“ zu „Enable-AzureRmAlias“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-366">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="28f95-367">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="28f95-367">Az.Compute</span></span>
* <span data-ttu-id="28f95-368">Name ist jetzt optional im ID-Parametersatz für „Restart/Start/Stop/Remove/Set-AzVM“ und „Save-AzVMImage“</span><span class="sxs-lookup"><span data-stu-id="28f95-368">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="28f95-369">Beschreibung der ID in Hilfedateien aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-369">Updated the description of ID in help files</span></span>
* <span data-ttu-id="28f95-370">Problem mit der Abwärtskompatibilität beim Az.Accounts-Modul behoben</span><span class="sxs-lookup"><span data-stu-id="28f95-370">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="28f95-371">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="28f95-371">Az.DataLakeStore</span></span>
* <span data-ttu-id="28f95-372">Aktualisierung der SDK-Version der Datenebene auf 1.1.14 für SDK-Fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="28f95-372">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="28f95-373">Behandlung von negativen acesstime- and modificationtime-Werten für „getfilestatus“ und „liststatus“ korrigiert, asynchrones Abbruchtoken korrigiert</span><span class="sxs-lookup"><span data-stu-id="28f95-373">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="28f95-374">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="28f95-374">Az.EventGrid</span></span>
* <span data-ttu-id="28f95-375">Zur Verwendung der API-Version 2019-01-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-375">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="28f95-376">Aktualisierung der folgenden Cmdlets zur Unterstützung des neuen Szenarios in der API-Version 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="28f95-376">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="28f95-377">New-AzureRmEventGridSubscription: Neue optionale Parameter zum Angeben folgender Werte hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="28f95-377">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="28f95-378">Gültigkeitsdauer des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="28f95-378">Event Time-To-Live,</span></span>
        - <span data-ttu-id="28f95-379">Maximale Anzahl von Übermittlungsversuchen für die Ereignisse</span><span class="sxs-lookup"><span data-stu-id="28f95-379">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="28f95-380">Endpunkt für unzustellbare Nachrichten</span><span class="sxs-lookup"><span data-stu-id="28f95-380">Dead letter endpoint.</span></span>
    - <span data-ttu-id="28f95-381">Update-AzureRmEventGridSubscription: Neue optionale Parameter zum Angeben folgender Werte hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="28f95-381">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="28f95-382">Gültigkeitsdauer des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="28f95-382">Event Time-To-Live,</span></span>
        - <span data-ttu-id="28f95-383">Maximale Anzahl von Übermittlungsversuchen für die Ereignisse</span><span class="sxs-lookup"><span data-stu-id="28f95-383">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="28f95-384">Endpunkt für unzustellbare Nachrichten</span><span class="sxs-lookup"><span data-stu-id="28f95-384">Dead letter endpoint.</span></span>
* <span data-ttu-id="28f95-385">Neue Enumerationswerte („storageQueue“ und „hybridConnection“) für die EndpointType-Option in den Cmdlets „New-AzureRmEventGridSubscription“ und „Update-AzureRmEventGridSubscription“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-385">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="28f95-386">Anzeige einer Warnmeldung, wenn das Erstellen oder Aktualisieren des Ereignisabonnements voraussichtlich eine manuelle Aktion des Benutzers zur Folge hat</span><span class="sxs-lookup"><span data-stu-id="28f95-386">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="28f95-387">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="28f95-387">Az.IotHub</span></span>
* <span data-ttu-id="28f95-388">Auf die aktuelle Version des Iot Hub SDK aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-388">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="28f95-389">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="28f95-389">Az.LogicApp</span></span>
* <span data-ttu-id="28f95-390">„Get-AzLogicApp“ listet alle Apps ohne angegebenen Namen auf</span><span class="sxs-lookup"><span data-stu-id="28f95-390">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="28f95-391">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="28f95-391">Az.Resources</span></span>
* <span data-ttu-id="28f95-392">Problem mit dem Parametersatz bei Angabe der Parameter „-ODataQuery“ und „-ResourceId“ für „Get-AzResource“ behoben</span><span class="sxs-lookup"><span data-stu-id="28f95-392">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="28f95-393">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="28f95-393">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="28f95-394">Behandlung des Parameters „-Custom“ in „New/Set-AzPolicyDefinition“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="28f95-394">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="28f95-395">Tippfehler in der Dokumentation für „New-AzDeployment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="28f95-395">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="28f95-396">Parameter „-MailNickname“ als obligatorisch festgelegt für „New-AzADUser“</span><span class="sxs-lookup"><span data-stu-id="28f95-396">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="28f95-397">Weitere Informationen finden Sie hier: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="28f95-397">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="28f95-398">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="28f95-398">Az.SignalR</span></span>
* <span data-ttu-id="28f95-399">Problem mit der Abwärtskompatibilität beim Az.Accounts-Modul behoben</span><span class="sxs-lookup"><span data-stu-id="28f95-399">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="28f95-400">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="28f95-400">Az.Sql</span></span>
* <span data-ttu-id="28f95-401">Abhängigkeit des Speicherverwaltungsclients zur allgemeinen SDK-Implementierung konvertiert</span><span class="sxs-lookup"><span data-stu-id="28f95-401">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="28f95-402">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="28f95-402">Az.Storage</span></span>
* <span data-ttu-id="28f95-403">Festlegung des „StorageAccountName“ des Speicherkontexts als tatsächlichen Namen des Speicherkontos, wenn dieser mit „SAS-Token“, „OAuth“ oder „Anonym“ erstellt wird</span><span class="sxs-lookup"><span data-stu-id="28f95-403">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="28f95-404">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="28f95-404">New-AzStorageContext</span></span>
* <span data-ttu-id="28f95-405">Erstellen von SAS-Token des Blob-Momentaufnahmeobjekts mit dem Parameter „-FullUri“, Festlegung des zurückgegebenen URI als Momentaufnahme-URI</span><span class="sxs-lookup"><span data-stu-id="28f95-405">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="28f95-406">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="28f95-406">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="28f95-407">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="28f95-407">Az.Websites</span></span>
* <span data-ttu-id="28f95-408">Fehler bei der Datumsanalyse in „Get-AzDeletedWebApp“ behoben</span><span class="sxs-lookup"><span data-stu-id="28f95-408">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="28f95-409">Problem mit der Abwärtskompatibilität beim Az.Accounts-Modul behoben</span><span class="sxs-lookup"><span data-stu-id="28f95-409">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="28f95-410">1.0.0 – Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="28f95-410">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="28f95-411">Allgemein</span><span class="sxs-lookup"><span data-stu-id="28f95-411">General</span></span>

- <span data-ttu-id="28f95-412">Allgemeine Verfügbarkeit des Az-Moduls</span><span class="sxs-lookup"><span data-stu-id="28f95-412">General Availability of Az Module</span></span>
- <span data-ttu-id="28f95-413">Onlinehilfe für jedes Modul</span><span class="sxs-lookup"><span data-stu-id="28f95-413">Online help for each module</span></span>
- <span data-ttu-id="28f95-414">Ausführlichere Informationen und eine Roadmap finden Sie auf der [Seite mit der Ankündigung zu Az](https://aka.ms/azps-announce).</span><span class="sxs-lookup"><span data-stu-id="28f95-414">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="28f95-415">Informationen zur Migration aus AzureRM finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="28f95-415">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="28f95-416">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="28f95-416">Az.Accounts</span></span>
- <span data-ttu-id="28f95-417">Geändert von Az.Profile</span><span class="sxs-lookup"><span data-stu-id="28f95-417">Changed from Az.Profile</span></span>
- <span data-ttu-id="28f95-418">Feste Tabellenformate für Profil- und Kontexttypen</span><span class="sxs-lookup"><span data-stu-id="28f95-418">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="28f95-419">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="28f95-419">Az.ApiManagement</span></span>
- <span data-ttu-id="28f95-420">Korrekturen für #7002</span><span class="sxs-lookup"><span data-stu-id="28f95-420">Fixes for #7002</span></span>
- <span data-ttu-id="28f95-421">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="28f95-421">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="28f95-422">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="28f95-422">Az.Batch</span></span>
- <span data-ttu-id="28f95-423">Möglichkeit zum Anzeigen der ausgeführten Version des Azure Batch-Knoten-Agents auf den VMs eines Pools mit der neuen `NodeAgentInformation`-Eigenschaft für `PSComputeNode` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="28f95-423">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="28f95-424">Der `Caching`-Standardwert für `PSDataDisk` lautet jetzt nicht mehr `None`, sondern `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="28f95-424">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="28f95-425">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="28f95-425">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="28f95-426">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="28f95-426">Az.Billing</span></span>
- <span data-ttu-id="28f95-427">Kombination von Billing-, Consumption- und UsageAggregates-Cmdlets. Ausführliche Informationen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="28f95-427">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="28f95-428">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="28f95-428">Az.CognitivServices</span></span>
- <span data-ttu-id="28f95-429">Vervollständigungen für SkuName und Typem für den Vorgang New-AzureRmCognitiveServicesAccount hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-429">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="28f95-430">GetSkusWithAccountParamSetName-Parametersatz aus Get-AzCognitiveServicesAccountSkus entfernt</span><span class="sxs-lookup"><span data-stu-id="28f95-430">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="28f95-431">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="28f95-431">Az.ContainerInstance</span></span>
- <span data-ttu-id="28f95-432">ManagedIdentity-Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-432">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="28f95-433">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="28f95-433">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="28f95-434">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="28f95-434">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="28f95-435">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="28f95-435">Az.DataLakeStore</span></span>
- <span data-ttu-id="28f95-436">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="28f95-436">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="28f95-437">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="28f95-437">Az.Monitor</span></span>
- <span data-ttu-id="28f95-438">Az.Insights in Az.Monitor umbenannt und weitere weniger wichtige grundlegende Änderungen durchgeführt. Informationen hierzu finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="28f95-438">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="28f95-439">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="28f95-439">Az.KeyVault</span></span>
- <span data-ttu-id="28f95-440">Veraltete PurgeDisabled-Eigenschaft aus Ausgabetypen entfernt</span><span class="sxs-lookup"><span data-stu-id="28f95-440">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="28f95-441">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="28f95-441">Az.MachineLearning</span></span>
- <span data-ttu-id="28f95-442">Cmdlets des Az.MachineLearningCompute-Moduls eingebunden</span><span class="sxs-lookup"><span data-stu-id="28f95-442">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="28f95-443">Az.Media</span><span class="sxs-lookup"><span data-stu-id="28f95-443">Az.Media</span></span>
- <span data-ttu-id="28f95-444">Veralteten -Tags-Alias aus New-AzMediaService entfernt</span><span class="sxs-lookup"><span data-stu-id="28f95-444">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="28f95-445">Az.Network</span><span class="sxs-lookup"><span data-stu-id="28f95-445">Az.Network</span></span>
<span data-ttu-id="28f95-446">Unterstützung für das Konfigurieren von RewriteRuleSets im Application Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-446">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="28f95-447">Neu hinzugefügte Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="28f95-447">New cmdlets added:</span></span>
        - <span data-ttu-id="28f95-448">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="28f95-448">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="28f95-449">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="28f95-449">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="28f95-450">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="28f95-450">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="28f95-451">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="28f95-451">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="28f95-452">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="28f95-452">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="28f95-453">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="28f95-453">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="28f95-454">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="28f95-454">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="28f95-455">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="28f95-455">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="28f95-456">Cmdlets mit optionalem Parameter -RewriteRuleSet aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-456">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="28f95-457">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="28f95-457">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="28f95-458">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="28f95-458">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="28f95-459">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="28f95-459">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="28f95-460">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="28f95-460">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="28f95-461">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="28f95-461">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="28f95-462">New-AzureRmApplicationGatewayUrlPathMapConfig: KeyVault-Unterstützung mithilfe von Identität zum Application Gateway hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="28f95-462">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="28f95-463">Cmdlets mit optionalem Parameter aktualisiert: -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="28f95-463">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="28f95-464">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="28f95-464">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="28f95-465">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="28f95-465">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="28f95-466">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="28f95-466">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="28f95-467">Cmdlet New-AzApplicationGateway mit optionalem Parameter -UserAssignedIdentity aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-467">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="28f95-468">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="28f95-468">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="28f95-469">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="28f95-469">Az.OperationalInsights</span></span>
- <span data-ttu-id="28f95-470">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="28f95-470">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="28f95-471">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="28f95-471">Az.Profile</span></span>
- <span data-ttu-id="28f95-472">Modulnamen in Az.Accounts geändert</span><span class="sxs-lookup"><span data-stu-id="28f95-472">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="28f95-473">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="28f95-473">Az.RecoveryServices</span></span>
- <span data-ttu-id="28f95-474">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="28f95-474">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="28f95-475">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="28f95-475">Az.Resources</span></span>
- <span data-ttu-id="28f95-476">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="28f95-476">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="28f95-477">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="28f95-477">Az.ServiceFabric</span></span>
- <span data-ttu-id="28f95-478">Unterstützung für das Angeben des Zertifikats anhand des allgemeinen Namens und Fingerabdrucks</span><span class="sxs-lookup"><span data-stu-id="28f95-478">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="28f95-479">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="28f95-479">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="28f95-480">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="28f95-480">Az.SIgnalR</span></span>
- <span data-ttu-id="28f95-481">Allgemeine Verfügbarkeit für PowerShell-Cmdlets für SIgnalR</span><span class="sxs-lookup"><span data-stu-id="28f95-481">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="28f95-482">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="28f95-482">Az.Sql</span></span>
- <span data-ttu-id="28f95-483">Neue Erkennungstypen Data_Exfiltration und Unsafe_Action zu Cmdlets für Bedrohungserkennung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-483">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="28f95-484">Dokumentationsbeispiele für Cmdlets für SQL-Überwachung aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-484">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="28f95-485">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="28f95-485">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="28f95-486">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="28f95-486">Az.Storage</span></span>
- <span data-ttu-id="28f95-487">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="28f95-487">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="28f95-488">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="28f95-488">Az.Websites</span></span>
- <span data-ttu-id="28f95-489">Informationen zu weniger wichtigen grundlegenden Änderungen finden Sie im [Migrationsleitfaden](https://aka.ms/azps-migration-guide).</span><span class="sxs-lookup"><span data-stu-id="28f95-489">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="28f95-490">0.7.0 – Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="28f95-490">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="28f95-491">Allgemein</span><span class="sxs-lookup"><span data-stu-id="28f95-491">General</span></span>

* <span data-ttu-id="28f95-492">Geringe Änderungen für anstehenden Übergang von AzureRM zu Az</span><span class="sxs-lookup"><span data-stu-id="28f95-492">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="28f95-493">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="28f95-493">Az.Compute</span></span>

* <span data-ttu-id="28f95-494">Unterstützung für UltraSSD und Katalogimages in einfachen Parametersätzen für `New-AzVm(ss)`-Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="28f95-494">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="28f95-495">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="28f95-495">Az.DataLakeStore</span></span>

* <span data-ttu-id="28f95-496">Nachgestellten Schrägstrich für die Domäne des ADLS-Kontos korrigiert</span><span class="sxs-lookup"><span data-stu-id="28f95-496">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="28f95-497">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="28f95-497">Az.FrontDoor</span></span>

* <span data-ttu-id="28f95-498">Einige fehlerhafte Links behoben</span><span class="sxs-lookup"><span data-stu-id="28f95-498">Fixed some broken links</span></span>
    - <span data-ttu-id="28f95-499">In den Artikeln zu New-AzureRmFrontDoor und Set-AzureRmFrontDoor den Artikel-Link zum Cmdlet „New-AzureRmFrontDoorHealthProbeSettingObject“ korrigiert.</span><span class="sxs-lookup"><span data-stu-id="28f95-499">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="28f95-500">Im Artikel zu New-AzureRmFrontDoorManagedRuleObject den Artikel-Link zum Cmdlet „New-AzureRmFrontDoorRuleGroupOverrideObject“ korrigiert.</span><span class="sxs-lookup"><span data-stu-id="28f95-500">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="28f95-501">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="28f95-501">Az.RecoveryServices</span></span>

* <span data-ttu-id="28f95-502">Clientseitige Validierungen für Wiederherstellungsvorgänge von Azure-Dateifreigaben hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="28f95-502">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="28f95-503">storageAccountName und storageAccountResourceGroupName für AFS-Wiederherstellung optional gemacht.</span><span class="sxs-lookup"><span data-stu-id="28f95-503">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="28f95-504">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="28f95-504">Az.Resources</span></span>

* <span data-ttu-id="28f95-505">Fehlerbehebung für https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="28f95-505">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="28f95-506">Get-AzureRmRoleAssignment für die Verwendung des Abonnementbereichs aktualisiert, wenn dieser beim Anfordern von klassischen Administratoren angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="28f95-506">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="28f95-507">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="28f95-507">Az.Sql</span></span>

* <span data-ttu-id="28f95-508">Geringe Änderungen für anstehenden Übergang von AzureRM zu Az</span><span class="sxs-lookup"><span data-stu-id="28f95-508">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="28f95-509">Problem mit der Verwendung von Get-AzureRmSqlDatabaseVulnerabilityAssessment mit .NET Core behoben</span><span class="sxs-lookup"><span data-stu-id="28f95-509">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="28f95-510">Dokumentation mit Hilfemeldungen zu Cmdlets für die SQL-Überwachung geändert.</span><span class="sxs-lookup"><span data-stu-id="28f95-510">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="28f95-511">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="28f95-511">Az.Storage</span></span>

* <span data-ttu-id="28f95-512">-EnableHierarchicalNamespace zu New-AzureRmStorageAccount hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-512">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="28f95-513">Problem behoben, bei dem für das Copy File-Cmdlet am Ziel kein Quellkontext wiederverwendet werden kann, wenn -DestContext nicht eingegeben wird</span><span class="sxs-lookup"><span data-stu-id="28f95-513">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="28f95-514">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="28f95-514">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="28f95-515">Unterstützung der Konfiguration von statischen Websites</span><span class="sxs-lookup"><span data-stu-id="28f95-515">Support Static Website configuration</span></span>
    - <span data-ttu-id="28f95-516">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="28f95-516">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="28f95-517">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="28f95-517">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="28f95-518">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="28f95-518">Az.Websites</span></span>

* <span data-ttu-id="28f95-519">Set-AzureRmWebApp und Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="28f95-519">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="28f95-520">Neuen Parameter (-AzureStoragePath) zum Angeben von Azure Storage-Pfaden hinzugefügt, die in Windows- und Linux-Container-Apps bereitgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="28f95-520">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="28f95-521">Verwenden Sie die Ausgabe des neuen Cmdlets New-AzureRmWebAppAzureStoragePath als Parameter zum Festlegen der Azure Storage-Pfade.</span><span class="sxs-lookup"><span data-stu-id="28f95-521">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="28f95-522">0.6.1 – November 2018</span><span class="sxs-lookup"><span data-stu-id="28f95-522">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="28f95-523">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="28f95-523">Az.ApiManagement</span></span>
* <span data-ttu-id="28f95-524">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-524">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="28f95-525">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="28f95-525">Az.Automation</span></span>
* <span data-ttu-id="28f95-526">Swagger-basierte Azure Automation-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="28f95-526">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="28f95-527">Cmdlets zur Updateverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-527">Added Update Management cmdlets</span></span>
* <span data-ttu-id="28f95-528">Cmdlets zur Quellcodeverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-528">Added Source Control cmdlets</span></span>
* <span data-ttu-id="28f95-529">Cmdlet „Remove-AzureRmAutomationHybridWorkerGroup“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-529">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="28f95-530">DSC-Befehl für die Knotenregistrierung korrigiert</span><span class="sxs-lookup"><span data-stu-id="28f95-530">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="28f95-531">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="28f95-531">Az.Compute</span></span>
* <span data-ttu-id="28f95-532">Identitätsproblem für SystemAssigned-Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="28f95-532">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="28f95-533">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-533">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="28f95-534">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="28f95-534">Az.ContainerInstance</span></span>
* <span data-ttu-id="28f95-535">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-535">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="28f95-536">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="28f95-536">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="28f95-537">Beschreibung der Beispiele für Marketplace-Cmdlets aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-537">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="28f95-538">Az.Network</span><span class="sxs-lookup"><span data-stu-id="28f95-538">Az.Network</span></span>
* <span data-ttu-id="28f95-539">Folgende Cmdlets hinzugefügt: New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="28f95-539">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="28f95-540">ICMP wieder unterstützten AzureFirewall-Netzwerkprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-540">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="28f95-541">Cmdlet „Test-AzureRmNetworkWatcherConnectivity“ aktualisiert und Überprüfung für Ziel-ID, Adresse und Port hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-541">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="28f95-542">Probleme mit Arbeitsspeicherauslastung in der VirtualNetwork-Zuordnung behoben</span><span class="sxs-lookup"><span data-stu-id="28f95-542">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="28f95-543">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="28f95-543">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="28f95-544">Problem beim Ändern der Richtlinie für eine geschützte Dateifreigabe behoben</span><span class="sxs-lookup"><span data-stu-id="28f95-544">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="28f95-545">Richtlinienzeitzone in Großschreibung geändert</span><span class="sxs-lookup"><span data-stu-id="28f95-545">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="28f95-546">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="28f95-546">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="28f95-547">Korrigiertes Beispiel in „New-AzureRmRecoveryServicesAsrProtectableItem“</span><span class="sxs-lookup"><span data-stu-id="28f95-547">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="28f95-548">Abhängigkeiten für Typzuordnungsproblem aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-548">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="28f95-549">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="28f95-549">Az.Relay</span></span>
* <span data-ttu-id="28f95-550">Optionaler Parameter „-KeyValue“ zu Cmdlet „New-AzureRmRelayKey“ hinzugefügt, der dem Benutzer das Angeben von „KeyValue“ ermöglicht</span><span class="sxs-lookup"><span data-stu-id="28f95-550">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="28f95-551">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="28f95-551">Az.Resources</span></span>
* <span data-ttu-id="28f95-552">Hilfedokumentation für ressourcenidentitätsbezogene Parameter in folgenden Elementen aktualisiert: `New-AzureRmPolicyAssignment` und</span><span class="sxs-lookup"><span data-stu-id="28f95-552">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and</span></span> `Set-AzureRmPolicyAssignment`
* <span data-ttu-id="28f95-553">Beispiel für „New-AzureRmPolicyDefinition“ hinzugefügt, das „-Metadata“ nutzt</span><span class="sxs-lookup"><span data-stu-id="28f95-553">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="28f95-554">Korrektur, um Beibehaltung von Groß-/Kleinschreibung in Tagschlüsseln in „NetStandard“ zu ermöglichen: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="28f95-554">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="28f95-555">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="28f95-555">Az.ServiceFabric</span></span>
* <span data-ttu-id="28f95-556">Benachrichtigung über veraltete Elemente für anstehende wichtige Änderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-556">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="28f95-557">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="28f95-557">Az.Sql</span></span>
* <span data-ttu-id="28f95-558">Neue Cmdlets für CRUD-Vorgänge in verwalteten Azure SQL-Datenbank-Instanzen und verwalteten Azure SQL-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-558">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="28f95-559">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="28f95-559">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="28f95-560">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="28f95-560">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="28f95-561">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="28f95-561">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="28f95-562">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="28f95-562">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="28f95-563">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="28f95-563">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="28f95-564">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="28f95-564">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="28f95-565">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="28f95-565">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="28f95-566">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="28f95-566">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="28f95-567">Erweiterte Verwaltung von Überwachungsrichtlinien auf einem Server oder in einer Datenbank aktiviert</span><span class="sxs-lookup"><span data-stu-id="28f95-567">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="28f95-568">Neuer Parameter (PredicateExpression) hinzugefügt, um die Filterung von Überwachungsprotokollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="28f95-568">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="28f95-569">Cmdlets wurden angepasst, sodass sie SQL-Clients anstelle von Legacyclients verwenden.</span><span class="sxs-lookup"><span data-stu-id="28f95-569">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="28f95-570">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="28f95-570">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="28f95-571">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="28f95-571">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="28f95-572">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="28f95-572">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="28f95-573">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="28f95-573">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="28f95-574">Problem bei Verwendung von „Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings“ mit festgelegtem Parameter für den Speicherkontonamen behoben</span><span class="sxs-lookup"><span data-stu-id="28f95-574">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="28f95-575">0.5.0 – November 2018</span><span class="sxs-lookup"><span data-stu-id="28f95-575">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="28f95-576">Allgemein</span><span class="sxs-lookup"><span data-stu-id="28f95-576">General</span></span>
* <span data-ttu-id="28f95-577">Ressourcenvervollständigungen für viele Kern-Cmdlets hinzugefügt (diese ermöglichen das Durchlaufen von vorhandenen Ressourcennamen per TAB-TASTE, wenn Cmdlets interaktiv aufgerufen werden)</span><span class="sxs-lookup"><span data-stu-id="28f95-577">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="28f95-578">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="28f95-578">Az.Profile</span></span>
* <span data-ttu-id="28f95-579">Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="28f95-579">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="28f95-580">Parameter „TenantId“ im Cmdlet „Connect-AzAccount“ in „Tenant“ umbenannt und Alias für „TenantId“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-580">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="28f95-581">Beschreibung von „TenantId“ für „Connect-AzAccount“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="28f95-581">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="28f95-582">Fehlermeldung für fehlgeschlagene Anmeldung bei Angabe der Mandantendomäne korrigiert</span><span class="sxs-lookup"><span data-stu-id="28f95-582">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="28f95-583">Problem in Bezug auf Kontextnamenskonflikt für Konten ohne Abonnements im Mandanten behoben</span><span class="sxs-lookup"><span data-stu-id="28f95-583">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="28f95-584">Problem mit DataLake-Endpunkten bei Verwendung von MSI behoben</span><span class="sxs-lookup"><span data-stu-id="28f95-584">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="28f95-585">Problem behoben, das zur Auslösung von „Disconnect-AzAccount“ führte, wenn keine Verbindung bestand</span><span class="sxs-lookup"><span data-stu-id="28f95-585">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="28f95-586">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="28f95-586">Az.CognitiveServices</span></span>
* <span data-ttu-id="28f95-587">Vorgang „Get-AzCognitiveServicesAccountSkus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-587">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="28f95-588">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="28f95-588">Az.Compute</span></span>
* <span data-ttu-id="28f95-589">Cmdlets Add-AzVmssVMDataDisk und Remove-AzVmssVMDataDisk hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-589">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="28f95-590">„Get-AzVMImage“ zeigt „AutomaticOSUpgradeProperties“ an</span><span class="sxs-lookup"><span data-stu-id="28f95-590">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="28f95-591">Problem behoben, aufgrund dessen die Optionswerte „SetAzVMChefExtension -BootstrapOptions“ und „-JsonAttribute“ nicht im JSON-Format festgelegt wurden</span><span class="sxs-lookup"><span data-stu-id="28f95-591">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="28f95-592">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="28f95-592">Az.DataLakeStore</span></span>
* <span data-ttu-id="28f95-593">Aktualisierung des DataLake-Pakets auf 1.1.10</span><span class="sxs-lookup"><span data-stu-id="28f95-593">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="28f95-594">Standardmäßige Parallelität zu Multithreadvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-594">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="28f95-595">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="28f95-595">Az.Insights</span></span>
* <span data-ttu-id="28f95-596">Problem Nr. 7267 behoben (Bereich für automatische Skalierung)</span><span class="sxs-lookup"><span data-stu-id="28f95-596">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="28f95-597">Probleme beim Erstellen einer neuen Regel für die automatische Skalierung, aufgrund derer die aufgelisteten Parameter nicht richtig festgelegt wurden (Es wurde stets der Standardwert festgelegt.)</span><span class="sxs-lookup"><span data-stu-id="28f95-597">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="28f95-598">Problem Nr. 7513 behoben [Insights] „Set-AzDiagnosticSetting“ erfordert die explizite Angabe von Kategorien während der Erstellung der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="28f95-598">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="28f95-599">Nun erfordert das Cmdlet nicht die explizite Angabe der Kategorien, die während der Erstellung aktiviert werden sollen. Das bedeutet, es funktioniert wie dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="28f95-599">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="28f95-600">Az.Network</span><span class="sxs-lookup"><span data-stu-id="28f95-600">Az.Network</span></span>
* <span data-ttu-id="28f95-601">„PeeringType“ wurde geändert und ist nun ein erforderlicher Parameter für die folgenden Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="28f95-601">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="28f95-602">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="28f95-602">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="28f95-603">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="28f95-603">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="28f95-604">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="28f95-604">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="28f95-605">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="28f95-605">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="28f95-606">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="28f95-606">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="28f95-607">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="28f95-607">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="28f95-608">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="28f95-608">Az.PolicyInsights</span></span>
* <span data-ttu-id="28f95-609">Cmdlets für Richtlinienwartung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-609">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="28f95-610">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="28f95-610">Az.Resources</span></span>
* <span data-ttu-id="28f95-611">Fehlerbehebung für https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="28f95-611">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="28f95-612">Zulassen der Auflistung von Ressourcen mithilfe des Parameters „-ResourceId“ für „Get-AzResource“</span><span class="sxs-lookup"><span data-stu-id="28f95-612">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="28f95-613">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="28f95-613">Az.ServiceBus</span></span>
* <span data-ttu-id="28f95-614">Schreibgeschützte Eigenschaft „MigrationState“ zu „PSServiceBusMigrationConfigurationAttributes“ hinzugefügt, was das Ermitteln des Migrationsstatus ermöglicht</span><span class="sxs-lookup"><span data-stu-id="28f95-614">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="28f95-615">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="28f95-615">Az.ServiceFabric</span></span>
* <span data-ttu-id="28f95-616">Hinzufügen des Zertifikats zu Linux VMSS korrigiert</span><span class="sxs-lookup"><span data-stu-id="28f95-616">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="28f95-617">„Add-AzServiceFabricClusterCertificate“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="28f95-617">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="28f95-618">Verwenden des richtigen Fingerabdrucks aus dem neuen Zertifikat (Azure/service-fabric-issues#932)</span><span class="sxs-lookup"><span data-stu-id="28f95-618">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="28f95-619">Richtige Anzeige von Ausnahmen (Azure/service-fabric-issues#1054)</span><span class="sxs-lookup"><span data-stu-id="28f95-619">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="28f95-620">„Update-AzServiceFabricDurability“ korrigiert, um die Clusterkonfiguration zu aktualisieren, bevor der VMSS-Vorgang „CreateOrUpdate“ gestartet wird</span><span class="sxs-lookup"><span data-stu-id="28f95-620">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="28f95-621">0.4.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="28f95-621">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="28f95-622">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="28f95-622">Az.Profile</span></span>
* <span data-ttu-id="28f95-623">Problem mit „Get-AzSubscription“ in Cloud Shell behoben</span><span class="sxs-lookup"><span data-stu-id="28f95-623">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="28f95-624">Allgemeiner Code aktualisiert, sodass die aktuelle Version von „ClientRuntime“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="28f95-624">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="28f95-625">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="28f95-625">Az.Compute</span></span>
* <span data-ttu-id="28f95-626">Neue Größen zur Whitelist von VM-Größen hinzugefügt, für die bei Verwendung des einfachen Parametersatzes für „New-AzVm“ der beschleunigte Netzwerkbetrieb aktiviert wird</span><span class="sxs-lookup"><span data-stu-id="28f95-626">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="28f95-627">ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="28f95-627">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="28f95-628">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="28f95-628">Az.DataLakeStore</span></span>
* <span data-ttu-id="28f95-629">Unterstützung für Regeln für virtuelle Netzwerke hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-629">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="28f95-630">Get-AzDataLakeStoreVirtualNetworkRule: Dient zum Abrufen oder Auflisten der Azure Data Lake Store-Regel für das virtuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="28f95-630">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="28f95-631">Add-AzDataLakeStoreVirtualNetworkRule: Fügt dem angegebenen Data Lake Store-Konto eine Regel für das virtuelle Netzwerk hinzu.</span><span class="sxs-lookup"><span data-stu-id="28f95-631">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="28f95-632">Set-AzDataLakeStoreVirtualNetworkRule: Ändert die angegebene Regel für das virtuelle Netzwerk in das angegebene Data Lake Store-Konto.</span><span class="sxs-lookup"><span data-stu-id="28f95-632">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="28f95-633">Remove-AzDataLakeStoreVirtualNetworkRule: Dient zum Löschen der Azure Data Lake Store-Regel für das virtuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="28f95-633">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="28f95-634">Az.Network</span><span class="sxs-lookup"><span data-stu-id="28f95-634">Az.Network</span></span>
* <span data-ttu-id="28f95-635">Cmdlet „Test-AzNetworkWatcherConnectivity“ aktualisiert, Protokollwert wird jetzt an Back-End übergeben.</span><span class="sxs-lookup"><span data-stu-id="28f95-635">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="28f95-636">ResourceName-Argumentvervollständigung zu allen Cmdlets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="28f95-636">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="28f95-637">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="28f95-637">Az.Resources</span></span>
* <span data-ttu-id="28f95-638">Problem behoben, aufgrund dessen „Get-AzRoleDefinition“ eine unverständliche Ausnahme auslöst (wenn das Standardprofil kein Abonnement enthält und kein Bereich festgelegt ist), indem im Szenario eine aussagekräftige Ausnahme hinzugefügt wurde.</span><span class="sxs-lookup"><span data-stu-id="28f95-638">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="28f95-639">Außerdem wurde der Standardparametersatz auf „RoleDefinitionNameParameterSet“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="28f95-639">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="28f95-640">0.3.0 – Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="28f95-640">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="28f95-641">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="28f95-641">Azure.Storage</span></span>
* <span data-ttu-id="28f95-642">Fehler beim Kopieren von Blobs/Dateien behoben, aufgrund dessen bei einem Metadatenproblem des Ziels keine Metadaten kopiert wurden</span><span class="sxs-lookup"><span data-stu-id="28f95-642">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="28f95-643">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="28f95-643">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="28f95-644">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="28f95-644">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="28f95-645">Der Abruf der Speicherressourcennutzung eines bestimmten Standorts wird jetzt unterstützt, und das Hinzufügen einer Warnmeldung für den Abruf der globalen Speicherressourcennutzung ist überflüssig.</span><span class="sxs-lookup"><span data-stu-id="28f95-645">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="28f95-646">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="28f95-646">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="28f95-647">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="28f95-647">Az.CognitiveServices</span></span>
* <span data-ttu-id="28f95-648">„Get-AzCognitiveServicesAccountSkus“ wird ohne vorhandenes Konto unterstützt.</span><span class="sxs-lookup"><span data-stu-id="28f95-648">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="28f95-649">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="28f95-649">Az.Compute</span></span>
* <span data-ttu-id="28f95-650">Korrektur von „Get-AzVM -ResourceGroupName <rg>“, sodass ggf. mehr als 50 Ergebnisse zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="28f95-650">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="28f95-651">Der Cmdlet-Hilfe zu „New-AzVmss“ wurde ein Beispiel für „SimpleParameterSet“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="28f95-651">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="28f95-652">Tippfehler in der Azure Disk Encryption-Statusmeldung behoben</span><span class="sxs-lookup"><span data-stu-id="28f95-652">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="28f95-653">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="28f95-653">Az.DataFactoryV2</span></span>
* <span data-ttu-id="28f95-654">Die Version des ADF .Net-SDK wurde auf 2.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="28f95-654">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="28f95-655">Az.Network</span><span class="sxs-lookup"><span data-stu-id="28f95-655">Az.Network</span></span>
* <span data-ttu-id="28f95-656">NetworkProfile-Funktionalität wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="28f95-656">Added NetworkProfile functionality.</span></span> <span data-ttu-id="28f95-657">Neue Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-657">new cmdlets added</span></span>
    - <span data-ttu-id="28f95-658">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="28f95-658">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="28f95-659">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="28f95-659">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="28f95-660">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="28f95-660">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="28f95-661">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="28f95-661">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="28f95-662">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="28f95-662">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="28f95-663">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="28f95-663">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="28f95-664">Dienstzuordnungslink in Subnetzmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-664">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="28f95-665">Cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-665">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="28f95-666">Cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-666">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="28f95-667">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="28f95-667">Az.RedisCache</span></span>
* <span data-ttu-id="28f95-668">Künftig sind beliebige Zeichenfolgen als Größenparameter zulässig.</span><span class="sxs-lookup"><span data-stu-id="28f95-668">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="28f95-669">P5 in Popup „PSArgumentCompleter“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-669">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="28f95-670">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="28f95-670">Az.Resources</span></span>
* <span data-ttu-id="28f95-671">Fehlender Parameter „-Mode“ zu „Set-AzPolicyDefinition“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="28f95-671">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="28f95-672">Cmdlet-Fehler bei „Get-AzProviderOperation“ für Vorgänge mit Ursprung behoben, der den Benutzer enthält</span><span class="sxs-lookup"><span data-stu-id="28f95-672">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="28f95-673">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="28f95-673">Az.Sql</span></span>
* <span data-ttu-id="28f95-674">Problem behoben, aufgrund dessen einige Sicherungs-Cmdlets das aktuelle Azure-Abonnements nicht erkannt haben</span><span class="sxs-lookup"><span data-stu-id="28f95-674">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="28f95-675">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="28f95-675">Az.Websites</span></span>
* <span data-ttu-id="28f95-676">Neues Cmdlet „Get-AzWebAppContainerContinuousDeploymentUrl“ zum Abrufen der Webhook-URL von Continuous Deployment für Container</span><span class="sxs-lookup"><span data-stu-id="28f95-676">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="28f95-677">Neue Cmdlets „New-AzWebAppContainerPSSession“ und „Enter-WebAppContainerPSSession“ zum Initiieren einer PowerShell-Remotesitzung in einer Windows-Container-App</span><span class="sxs-lookup"><span data-stu-id="28f95-677">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="28f95-678">0.2.0 – September 2018</span><span class="sxs-lookup"><span data-stu-id="28f95-678">0.2.0 - September 2018</span></span>
 <span data-ttu-id="28f95-679">Erste Version</span><span class="sxs-lookup"><span data-stu-id="28f95-679">Initial Release</span></span>