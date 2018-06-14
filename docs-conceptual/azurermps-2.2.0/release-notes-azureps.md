---
title: Azure PowerShell-Änderungsprotokoll | Microsoft-Dokumentation
description: Hierbei handelt es sich um einen Verlauf der Änderungen, die in der neuesten Version an Azure PowerShell vorgenommen wurden.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: ca25f3c66f8e8f4c64fc04275da2bd28e32d2f6c
ms.sourcegitcommit: c98e3a21037ebd82936828bcb544eed902b24212
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/08/2018
ms.locfileid: "34854612"
---
# <a name="release-notes"></a><span data-ttu-id="34c16-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="34c16-103">Release notes</span></span>

<span data-ttu-id="34c16-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="34c16-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-220"></a><span data-ttu-id="34c16-105">Version 2.2.0</span><span class="sxs-lookup"><span data-stu-id="34c16-105">Version 2.2.0</span></span>
* <span data-ttu-id="34c16-106">Compute</span><span class="sxs-lookup"><span data-stu-id="34c16-106">Compute</span></span>
  - <span data-ttu-id="34c16-107">Unterstützung zum Abfragen des Verschlüsselungsstatus aus der AzureDiskEncryptionForLinux-Erweiterung wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="34c16-107">Add support for querying encryption status from the AzureDiskEncryptionForLinux extension</span></span>
* <span data-ttu-id="34c16-108">DataFactory</span><span class="sxs-lookup"><span data-stu-id="34c16-108">DataFactory</span></span>
  - <span data-ttu-id="34c16-109">Ein neues Cmdlet zum Auflisten der Aktivitätsfenster wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="34c16-109">Added new cmdlet for listing activity windows</span></span>
    + <span data-ttu-id="34c16-110">Get-AzureRmDataFactoryActivityWindow</span><span class="sxs-lookup"><span data-stu-id="34c16-110">Get-AzureRmDataFactoryActivityWindow</span></span>
* <span data-ttu-id="34c16-111">DataLake</span><span class="sxs-lookup"><span data-stu-id="34c16-111">DataLake</span></span>
  - <span data-ttu-id="34c16-112">Der Parameter `Host` wurde in `DatabaseHost` geändert. Außerdem wurde `Host` ein Alias hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="34c16-112">Changed parameter `Host` to `DatabaseHost` and added alias to `Host`</span></span>
    + <span data-ttu-id="34c16-113">New-AzureRmDataLakeAnalyticsCatalogSecret</span><span class="sxs-lookup"><span data-stu-id="34c16-113">New-AzureRmDataLakeAnalyticsCatalogSecret</span></span>
    + <span data-ttu-id="34c16-114">Set-AzureRmDataLakeAnalyticsCatalogSecret</span><span class="sxs-lookup"><span data-stu-id="34c16-114">Set-AzureRmDataLakeAnalyticsCatalogSecret</span></span>
  - <span data-ttu-id="34c16-115">Hinzufügen von Unterstützung für die Entfernung der ACL und Standard-ACL</span><span class="sxs-lookup"><span data-stu-id="34c16-115">Add support for ACL and Default ACL removal</span></span>
  - <span data-ttu-id="34c16-116">Unterstützung für das Abrufen und Festlegen unbenannter Berechtigungen für Dateien und Ordner wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="34c16-116">Add support for getting and setting unnamed permissions on files and folders</span></span>
* <span data-ttu-id="34c16-117">KeyVault</span><span class="sxs-lookup"><span data-stu-id="34c16-117">KeyVault</span></span>
  - <span data-ttu-id="34c16-118">Unterstützung für Zertifikate wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="34c16-118">Add support for certificates</span></span>
    + <span data-ttu-id="34c16-119">Add-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="34c16-119">Add-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="34c16-120">Add-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="34c16-120">Add-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="34c16-121">Get-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="34c16-121">Get-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="34c16-122">Get-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="34c16-122">Get-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="34c16-123">Get-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="34c16-123">Get-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="34c16-124">Get-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="34c16-124">Get-AzureKeyVaultCertificateOperation</span></span>
    + <span data-ttu-id="34c16-125">Get-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="34c16-125">Get-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="34c16-126">Import-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="34c16-126">Import-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="34c16-127">New-AzureKeyVaultCertificateAdministratorDetails</span><span class="sxs-lookup"><span data-stu-id="34c16-127">New-AzureKeyVaultCertificateAdministratorDetails</span></span>
    + <span data-ttu-id="34c16-128">New-AzureKeyVaultCertificateOrganizationDetails</span><span class="sxs-lookup"><span data-stu-id="34c16-128">New-AzureKeyVaultCertificateOrganizationDetails</span></span>
    + <span data-ttu-id="34c16-129">New-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="34c16-129">New-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="34c16-130">Remove-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="34c16-130">Remove-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="34c16-131">Remove-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="34c16-131">Remove-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="34c16-132">Remove-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="34c16-132">Remove-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="34c16-133">Remove-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="34c16-133">Remove-AzureKeyVaultCertificateOperation</span></span>
    + <span data-ttu-id="34c16-134">Set-AzureKeyVaultCertificateAttribute</span><span class="sxs-lookup"><span data-stu-id="34c16-134">Set-AzureKeyVaultCertificateAttribute</span></span>
    + <span data-ttu-id="34c16-135">Set-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="34c16-135">Set-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="34c16-136">Set-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="34c16-136">Set-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="34c16-137">Stop-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="34c16-137">Stop-AzureKeyVaultCertificateOperation</span></span>
* <span data-ttu-id="34c16-138">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="34c16-138">Network</span></span>

  - <span data-ttu-id="34c16-139">Ein neuer Switch-Parameter wurde für die Netzwerkschnittstelle hinzugefügt, um beschleunigte Netzwerke zu aktivieren/deaktivieren. +New-AzureRmNetworkInterface -EnableAcceleratedNetworking</span><span class="sxs-lookup"><span data-stu-id="34c16-139">New switch parameter added for network interface to enable/disable accelerated networking +New-AzureRmNetworkInterface -EnableAcceleratedNetworking</span></span>
  - <span data-ttu-id="34c16-140">Die Funktion für Aktiv/Aktiv-Gateways für PowerShell-Cmdlets wurde aktiviert.</span><span class="sxs-lookup"><span data-stu-id="34c16-140">Enable Active-Active gateway feature PowerShell cmdlets</span></span>
    + <span data-ttu-id="34c16-141">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="34c16-141">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
    + <span data-ttu-id="34c16-142">Remove-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="34c16-142">Remove-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="34c16-143">Ein neues Cmdlet wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="34c16-143">Added new cmdlet</span></span>
    + <span data-ttu-id="34c16-144">Test-AzureRmPrivateIpAddressAvailability</span><span class="sxs-lookup"><span data-stu-id="34c16-144">Test-AzureRmPrivateIpAddressAvailability</span></span>
* <span data-ttu-id="34c16-145">angeben</span><span class="sxs-lookup"><span data-stu-id="34c16-145">Resources</span></span>
  - <span data-ttu-id="34c16-146">Zonen in Anbieter- und Ressourcen-Cmdlets werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34c16-146">Support zones in provider and resource cmdlets</span></span>
    + <span data-ttu-id="34c16-147">Get-AzureRmProvider</span><span class="sxs-lookup"><span data-stu-id="34c16-147">Get-AzureRmProvider</span></span>
    + <span data-ttu-id="34c16-148">New-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="34c16-148">New-AzureRmResource</span></span>
    + <span data-ttu-id="34c16-149">Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="34c16-149">Set-AzureRmResource</span></span>
* <span data-ttu-id="34c16-150">Sql</span><span class="sxs-lookup"><span data-stu-id="34c16-150">Sql</span></span>
  - <span data-ttu-id="34c16-151">Neue Cmdlets für die Richtlinienverwaltung der Azure SQL-Bedrohungserkennung auf Serverebene wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="34c16-151">Added new cmdlets for Azure SQL threat detection policy management at server level</span></span>
    + <span data-ttu-id="34c16-152">Get-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="34c16-152">Get-AzureRmSqlServerThreatDetectionPolicy</span></span>
    + <span data-ttu-id="34c16-153">Remove-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="34c16-153">Remove-AzureRmSqlServerThreatDetectionPolicy</span></span>
    + <span data-ttu-id="34c16-154">Set-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="34c16-154">Set-AzureRmSqlServerThreatDetectionPolicy</span></span>
  - <span data-ttu-id="34c16-155">Neue Cmdlets wurden hinzugefügt, um die Aktivierung/Deaktivierung von „GeoBackupPolicy“ für SQL Azure Data Warehouses zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="34c16-155">Added new cmdlets to support enabling/disabling GeoBackupPolicy for Sql Azure DataWarehouses</span></span>
    + <span data-ttu-id="34c16-156">Get-AzureRmSqlDatabaseGeoBackupPolicy</span><span class="sxs-lookup"><span data-stu-id="34c16-156">Get-AzureRmSqlDatabaseGeoBackupPolicy</span></span>
    + <span data-ttu-id="34c16-157">Set-AzureRmSqlDatabaseGeoBackupPolicy</span><span class="sxs-lookup"><span data-stu-id="34c16-157">Set-AzureRmSqlDatabaseGeoBackupPolicy</span></span>
  - <span data-ttu-id="34c16-158">Neue Cmdlets für Azure SQL Advisor und empfohlene Aktions-APIs wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="34c16-158">Added new cmdlets for Azure Sql Advisors and Recommended Actions APIs</span></span>
    + <span data-ttu-id="34c16-159">Get-AzureRmSqlDatabaseAdvisor</span><span class="sxs-lookup"><span data-stu-id="34c16-159">Get-AzureRmSqlDatabaseAdvisor</span></span>
    + <span data-ttu-id="34c16-160">Get-AzureRmSqlElasticPoolAdvisor</span><span class="sxs-lookup"><span data-stu-id="34c16-160">Get-AzureRmSqlElasticPoolAdvisor</span></span>
    + <span data-ttu-id="34c16-161">Get-AzureRmSqlServerAdvisor</span><span class="sxs-lookup"><span data-stu-id="34c16-161">Get-AzureRmSqlServerAdvisor</span></span>
    + <span data-ttu-id="34c16-162">Get-AzureRmSqlDatabaseRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="34c16-162">Get-AzureRmSqlDatabaseRecommendedActions</span></span>
    + <span data-ttu-id="34c16-163">Get-AzureRmSqlElasticPoolRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="34c16-163">Get-AzureRmSqlElasticPoolRecommendedActions</span></span>
    + <span data-ttu-id="34c16-164">Get-AzureRmSqlServerRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="34c16-164">Get-AzureRmSqlServerRecommendedActions</span></span>
    + <span data-ttu-id="34c16-165">Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="34c16-165">Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="34c16-166">Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="34c16-166">Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="34c16-167">Set-AzureRmSqlServerAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="34c16-167">Set-AzureRmSqlServerAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="34c16-168">Set-AzureRmSqlDatabaseRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="34c16-168">Set-AzureRmSqlDatabaseRecommendedActionState</span></span>
    + <span data-ttu-id="34c16-169">Set-AzureRmSqlElasticPoolRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="34c16-169">Set-AzureRmSqlElasticPoolRecommendedActionState</span></span>
    + <span data-ttu-id="34c16-170">Set-AzureRmSqlServerRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="34c16-170">Set-AzureRmSqlServerRecommendedActionState</span></span>
