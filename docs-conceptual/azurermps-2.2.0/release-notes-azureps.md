---
title: Azure PowerShell-Änderungsprotokoll | Microsoft-Dokumentation
description: Hierbei handelt es sich um einen Verlauf der Änderungen, die in der neuesten Version an Azure PowerShell vorgenommen wurden.
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: a00bc2f13117f1b07f0dcc5808eddbabe1df940f
ms.sourcegitcommit: 2eea03b7ac19ad6d7c8097743d33c7ddb9c4df77
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/06/2018
ms.locfileid: "34821665"
---
# <a name="release-notes"></a><span data-ttu-id="a700f-103">Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="a700f-103">Release notes</span></span>

<span data-ttu-id="a700f-104">Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="a700f-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-220"></a><span data-ttu-id="a700f-105">Version 2.2.0</span><span class="sxs-lookup"><span data-stu-id="a700f-105">Version 2.2.0</span></span>
* <span data-ttu-id="a700f-106">Compute</span><span class="sxs-lookup"><span data-stu-id="a700f-106">Compute</span></span>
  - <span data-ttu-id="a700f-107">Unterstützung zum Abfragen des Verschlüsselungsstatus aus der AzureDiskEncryptionForLinux-Erweiterung wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="a700f-107">Add support for querying encryption status from the AzureDiskEncryptionForLinux extension</span></span>
* <span data-ttu-id="a700f-108">DataFactory</span><span class="sxs-lookup"><span data-stu-id="a700f-108">DataFactory</span></span>
  - <span data-ttu-id="a700f-109">Ein neues Cmdlet zum Auflisten der Aktivitätsfenster wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="a700f-109">Added new cmdlet for listing activity windows</span></span>
    + <span data-ttu-id="a700f-110">Get-AzureRmDataFactoryActivityWindow</span><span class="sxs-lookup"><span data-stu-id="a700f-110">Get-AzureRmDataFactoryActivityWindow</span></span>
* <span data-ttu-id="a700f-111">DataLake</span><span class="sxs-lookup"><span data-stu-id="a700f-111">DataLake</span></span>
  - <span data-ttu-id="a700f-112">Der Parameter `Host` wurde in `DatabaseHost` geändert. Außerdem wurde `Host` ein Alias hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="a700f-112">Changed parameter `Host` to `DatabaseHost` and added alias to `Host`</span></span>
    + <span data-ttu-id="a700f-113">New-AzureRmDataLakeAnalyticsCatalogSecret</span><span class="sxs-lookup"><span data-stu-id="a700f-113">New-AzureRmDataLakeAnalyticsCatalogSecret</span></span>
    + <span data-ttu-id="a700f-114">Set-AzureRmDataLakeAnalyticsCatalogSecret</span><span class="sxs-lookup"><span data-stu-id="a700f-114">Set-AzureRmDataLakeAnalyticsCatalogSecret</span></span>
  - <span data-ttu-id="a700f-115">Hinzufügen von Unterstützung für die Entfernung der ACL und Standard-ACL</span><span class="sxs-lookup"><span data-stu-id="a700f-115">Add support for ACL and Default ACL removal</span></span>
  - <span data-ttu-id="a700f-116">Unterstützung für das Abrufen und Festlegen unbenannter Berechtigungen für Dateien und Ordner wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="a700f-116">Add support for getting and setting unnamed permissions on files and folders</span></span>
* <span data-ttu-id="a700f-117">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a700f-117">KeyVault</span></span>
  - <span data-ttu-id="a700f-118">Unterstützung für Zertifikate wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="a700f-118">Add support for certificates</span></span>
    + <span data-ttu-id="a700f-119">Add-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="a700f-119">Add-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="a700f-120">Add-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="a700f-120">Add-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="a700f-121">Get-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="a700f-121">Get-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="a700f-122">Get-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="a700f-122">Get-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="a700f-123">Get-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="a700f-123">Get-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="a700f-124">Get-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="a700f-124">Get-AzureKeyVaultCertificateOperation</span></span>
    + <span data-ttu-id="a700f-125">Get-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="a700f-125">Get-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="a700f-126">Import-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="a700f-126">Import-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="a700f-127">New-AzureKeyVaultCertificateAdministratorDetails</span><span class="sxs-lookup"><span data-stu-id="a700f-127">New-AzureKeyVaultCertificateAdministratorDetails</span></span>
    + <span data-ttu-id="a700f-128">New-AzureKeyVaultCertificateOrganizationDetails</span><span class="sxs-lookup"><span data-stu-id="a700f-128">New-AzureKeyVaultCertificateOrganizationDetails</span></span>
    + <span data-ttu-id="a700f-129">New-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="a700f-129">New-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="a700f-130">Remove-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="a700f-130">Remove-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="a700f-131">Remove-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="a700f-131">Remove-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="a700f-132">Remove-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="a700f-132">Remove-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="a700f-133">Remove-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="a700f-133">Remove-AzureKeyVaultCertificateOperation</span></span>
    + <span data-ttu-id="a700f-134">Set-AzureKeyVaultCertificateAttribute</span><span class="sxs-lookup"><span data-stu-id="a700f-134">Set-AzureKeyVaultCertificateAttribute</span></span>
    + <span data-ttu-id="a700f-135">Set-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="a700f-135">Set-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="a700f-136">Set-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="a700f-136">Set-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="a700f-137">Stop-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="a700f-137">Stop-AzureKeyVaultCertificateOperation</span></span>
* <span data-ttu-id="a700f-138">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="a700f-138">Network</span></span>

  - <span data-ttu-id="a700f-139">Ein neuer Switch-Parameter wurde für die Netzwerkschnittstelle hinzugefügt, um beschleunigte Netzwerke zu aktivieren/deaktivieren. +New-AzureRmNetworkInterface -EnableAcceleratedNetworking</span><span class="sxs-lookup"><span data-stu-id="a700f-139">New switch parameter added for network interface to enable/disable accelerated networking +New-AzureRmNetworkInterface -EnableAcceleratedNetworking</span></span>
  - <span data-ttu-id="a700f-140">Die Funktion für Aktiv/Aktiv-Gateways für PowerShell-Cmdlets wurde aktiviert.</span><span class="sxs-lookup"><span data-stu-id="a700f-140">Enable Active-Active gateway feature PowerShell cmdlets</span></span>
    + <span data-ttu-id="a700f-141">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="a700f-141">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
    + <span data-ttu-id="a700f-142">Remove-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="a700f-142">Remove-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="a700f-143">Ein neues Cmdlet wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="a700f-143">Added new cmdlet</span></span>
    + <span data-ttu-id="a700f-144">Test-AzureRmPrivateIpAddressAvailability</span><span class="sxs-lookup"><span data-stu-id="a700f-144">Test-AzureRmPrivateIpAddressAvailability</span></span>
* <span data-ttu-id="a700f-145">angeben</span><span class="sxs-lookup"><span data-stu-id="a700f-145">Resources</span></span>
  - <span data-ttu-id="a700f-146">Zonen in Anbieter- und Ressourcen-Cmdlets werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a700f-146">Support zones in provider and resource cmdlets</span></span>
    + <span data-ttu-id="a700f-147">Get-AzureRmProvider</span><span class="sxs-lookup"><span data-stu-id="a700f-147">Get-AzureRmProvider</span></span>
    + <span data-ttu-id="a700f-148">New-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="a700f-148">New-AzureRmResource</span></span>
    + <span data-ttu-id="a700f-149">Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="a700f-149">Set-AzureRmResource</span></span>
* <span data-ttu-id="a700f-150">Sql</span><span class="sxs-lookup"><span data-stu-id="a700f-150">Sql</span></span>
  - <span data-ttu-id="a700f-151">Neue Cmdlets für die Richtlinienverwaltung der Azure SQL-Bedrohungserkennung auf Serverebene wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="a700f-151">Added new cmdlets for Azure SQL threat detection policy management at server level</span></span>
    + <span data-ttu-id="a700f-152">Get-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a700f-152">Get-AzureRmSqlServerThreatDetectionPolicy</span></span>
    + <span data-ttu-id="a700f-153">Remove-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a700f-153">Remove-AzureRmSqlServerThreatDetectionPolicy</span></span>
    + <span data-ttu-id="a700f-154">Set-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a700f-154">Set-AzureRmSqlServerThreatDetectionPolicy</span></span>
  - <span data-ttu-id="a700f-155">Neue Cmdlets wurden hinzugefügt, um die Aktivierung/Deaktivierung von „GeoBackupPolicy“ für SQL Azure Data Warehouses zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="a700f-155">Added new cmdlets to support enabling/disabling GeoBackupPolicy for Sql Azure DataWarehouses</span></span>
    + <span data-ttu-id="a700f-156">Get-AzureRmSqlDatabaseGeoBackupPolicy</span><span class="sxs-lookup"><span data-stu-id="a700f-156">Get-AzureRmSqlDatabaseGeoBackupPolicy</span></span>
    + <span data-ttu-id="a700f-157">Set-AzureRmSqlDatabaseGeoBackupPolicy</span><span class="sxs-lookup"><span data-stu-id="a700f-157">Set-AzureRmSqlDatabaseGeoBackupPolicy</span></span>
  - <span data-ttu-id="a700f-158">Neue Cmdlets für Azure SQL Advisor und empfohlene Aktions-APIs wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="a700f-158">Added new cmdlets for Azure Sql Advisors and Recommended Actions APIs</span></span>
    + <span data-ttu-id="a700f-159">Get-AzureRmSqlDatabaseAdvisor</span><span class="sxs-lookup"><span data-stu-id="a700f-159">Get-AzureRmSqlDatabaseAdvisor</span></span>
    + <span data-ttu-id="a700f-160">Get-AzureRmSqlElasticPoolAdvisor</span><span class="sxs-lookup"><span data-stu-id="a700f-160">Get-AzureRmSqlElasticPoolAdvisor</span></span>
    + <span data-ttu-id="a700f-161">Get-AzureRmSqlServerAdvisor</span><span class="sxs-lookup"><span data-stu-id="a700f-161">Get-AzureRmSqlServerAdvisor</span></span>
    + <span data-ttu-id="a700f-162">Get-AzureRmSqlDatabaseRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="a700f-162">Get-AzureRmSqlDatabaseRecommendedActions</span></span>
    + <span data-ttu-id="a700f-163">Get-AzureRmSqlElasticPoolRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="a700f-163">Get-AzureRmSqlElasticPoolRecommendedActions</span></span>
    + <span data-ttu-id="a700f-164">Get-AzureRmSqlServerRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="a700f-164">Get-AzureRmSqlServerRecommendedActions</span></span>
    + <span data-ttu-id="a700f-165">Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="a700f-165">Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="a700f-166">Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="a700f-166">Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="a700f-167">Set-AzureRmSqlServerAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="a700f-167">Set-AzureRmSqlServerAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="a700f-168">Set-AzureRmSqlDatabaseRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="a700f-168">Set-AzureRmSqlDatabaseRecommendedActionState</span></span>
    + <span data-ttu-id="a700f-169">Set-AzureRmSqlElasticPoolRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="a700f-169">Set-AzureRmSqlElasticPoolRecommendedActionState</span></span>
    + <span data-ttu-id="a700f-170">Set-AzureRmSqlServerRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="a700f-170">Set-AzureRmSqlServerRecommendedActionState</span></span>
