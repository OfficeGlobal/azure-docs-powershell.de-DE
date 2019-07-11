---
title: Anmelden mit Azure PowerShell
description: Es wird beschrieben, wie Sie sich mit Azure PowerShell als Benutzer, per Dienstprinzipal oder mit verwalteten Identitäten für Azure-Ressourcen anmelden.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 02/20/2019
ms.openlocfilehash: 1e25d4650cc20d7b6613e0efb12ec60d424608c4
ms.sourcegitcommit: 5bdedc77b27b66998387486761ec67ed9326f169
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/24/2019
ms.locfileid: "67345343"
---
# <a name="sign-in-with-azure-powershell"></a><span data-ttu-id="ba63f-103">Anmelden mit Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="ba63f-103">Sign in with Azure PowerShell </span></span>

<span data-ttu-id="ba63f-104">Azure PowerShell unterstützt mehrere Authentifizierungsmethoden.</span><span class="sxs-lookup"><span data-stu-id="ba63f-104">Azure PowerShell supports several authentication methods.</span></span> <span data-ttu-id="ba63f-105">Den einfachsten Einstieg ermöglicht der [Azure Cloud Shell](/azure/cloud-shell/overview)-Dienst, der Sie automatisch anmeldet.</span><span class="sxs-lookup"><span data-stu-id="ba63f-105">The easiest way to get started is with [Azure Cloud Shell](/azure/cloud-shell/overview), which automatically logs you in.</span></span> <span data-ttu-id="ba63f-106">Bei einer lokalen Installation können Sie sich interaktiv über Ihren Browser anmelden.</span><span class="sxs-lookup"><span data-stu-id="ba63f-106">With a local install, you can sign in interactively through your browser.</span></span> <span data-ttu-id="ba63f-107">Beim Schreiben von Skripts für die Automatisierung besteht der empfohlene Ansatz darin, einen [Dienstprinzipal](create-azure-service-principal-azureps.md) mit den erforderlichen Berechtigungen zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="ba63f-107">When writing scripts for automation, the recommended approach is to use a [service principal](create-azure-service-principal-azureps.md) with the necessary permissions.</span></span> <span data-ttu-id="ba63f-108">Indem Sie die Anmeldeberechtigungen für Ihren Anwendungsfall so weit wie möglich einschränken, tragen Sie zur Sicherheit Ihrer Azure-Ressourcen bei.</span><span class="sxs-lookup"><span data-stu-id="ba63f-108">When you restrict sign-in permissions as much as possible for your use case, you help keep your Azure resources secure.</span></span>

<span data-ttu-id="ba63f-109">Nach der Anmeldung werden Befehle für Ihr Standardabonnement ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="ba63f-109">After signing in, commands are run against your default subscription.</span></span> <span data-ttu-id="ba63f-110">Verwenden Sie das Cmdlet [Set-AzContext](/powershell/module/az.accounts/set-azcontext), um Ihr aktives Abonnement für eine Sitzung zu ändern.</span><span class="sxs-lookup"><span data-stu-id="ba63f-110">To change your active subscription for a session, use the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span> <span data-ttu-id="ba63f-111">Verwenden Sie [Set-AzDefault](/powershell/module/az.accounts/set-azdefault), um das Standardabonnement zu ändern, das beim Anmelden mit Azure PowerShell verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="ba63f-111">To change the default subscription used when logging in with Azure PowerShell, use [Set-AzDefault](/powershell/module/az.accounts/set-azdefault).</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="ba63f-112">Ihre Anmeldeinformationen werden in mehreren PowerShell-Sitzungen gemeinsam verwendet, solange Sie angemeldet bleiben.</span><span class="sxs-lookup"><span data-stu-id="ba63f-112">Your credentials are shared among multiple PowerShell sessions as long as you remain signed in.</span></span>
> <span data-ttu-id="ba63f-113">Weitere Informationen finden Sie im Artikel zu [beständigen Anmeldeinformationen](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="ba63f-113">For more information, see the article on [Persistent Credentials](context-persistence.md).</span></span>

## <a name="sign-in-interactively"></a><span data-ttu-id="ba63f-114">Interaktives Anmelden</span><span class="sxs-lookup"><span data-stu-id="ba63f-114">Sign in interactively</span></span>

<span data-ttu-id="ba63f-115">Verwenden Sie für die interaktive Anmeldung das Cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).</span><span class="sxs-lookup"><span data-stu-id="ba63f-115">To sign in interactively, use the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>

```azurepowershell-interactive
Connect-AzAccount
```

<span data-ttu-id="ba63f-116">Bei der Ausführung wird von diesem Cmdlet eine Tokenzeichenfolge bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="ba63f-116">When run, this cmdlet will present a token string.</span></span> <span data-ttu-id="ba63f-117">Kopieren Sie diese Zeichenfolge, und fügen Sie sie in einem Browser unter https://microsoft.com/devicelogin ein, um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="ba63f-117">To sign in, copy this string and paste it into https://microsoft.com/devicelogin in a browser.</span></span> <span data-ttu-id="ba63f-118">Ihre PowerShell-Sitzung wird für die Verbindungsherstellung mit Azure authentifiziert.</span><span class="sxs-lookup"><span data-stu-id="ba63f-118">Your PowerShell session will be authenticated to connect to Azure.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="ba63f-119">Die Autorisierung mit Anmeldeinformationen (Benutzername/Kennwort) wurde in Azure PowerShell aufgrund von Änderungen in Active Directory-Autorisierungsimplementierungen und Sicherheitsbedenken entfernt.</span><span class="sxs-lookup"><span data-stu-id="ba63f-119">Username/password credential authorization has been removed in Azure PowerShell due to changes in Active Directory authorization implementations and security concerns.</span></span>
> <span data-ttu-id="ba63f-120">Wenn Sie die Autorisierung mit Anmeldeinformationen zu Automatisierungszwecken verwenden, [erstellen Sie stattdessen einen Dienstprinzipal](create-azure-service-principal-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="ba63f-120">If you use credential authorization for automation purposes, instead [create a service principal](create-azure-service-principal-azureps.md).</span></span>

## <a name="sign-in-with-a-service-principal-a-namesp-signin"></a><span data-ttu-id="ba63f-121">Anmelden mit einem Dienstprinzipal<a name="sp-signin"/></span><span class="sxs-lookup"><span data-stu-id="ba63f-121">Sign in with a service principal <a name="sp-signin"/></span></span>

<span data-ttu-id="ba63f-122">Dienstprinzipale sind nicht interaktive Azure-Konten.</span><span class="sxs-lookup"><span data-stu-id="ba63f-122">Service principals are non-interactive Azure accounts.</span></span> <span data-ttu-id="ba63f-123">Wie bei anderen Benutzerkonten auch, werden die Berechtigungen mit Azure Active Directory verwaltet.</span><span class="sxs-lookup"><span data-stu-id="ba63f-123">Like other user accounts, their permissions are managed with Azure Active Directory.</span></span> <span data-ttu-id="ba63f-124">Indem für einen Dienstprinzipal nur die benötigten Berechtigungen gewährt werden, bleibt die Sicherheit Ihrer Automatisierungsskripts gewahrt.</span><span class="sxs-lookup"><span data-stu-id="ba63f-124">By granting a service principal only the permissions it needs, your automation scripts stay secure.</span></span>

<span data-ttu-id="ba63f-125">Informationen zur Erstellung eines Dienstprinzipals für die Verwendung mit PowerShell finden Sie unter [Erstellen eines Azure-Dienstprinzipals mit Azure PowerShell](create-azure-service-principal-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="ba63f-125">To learn how to create a service principal for use with Azure PowerShell, see [Create an Azure service principal with Azure PowerShell](create-azure-service-principal-azureps.md).</span></span>

<span data-ttu-id="ba63f-126">Verwenden Sie für die Anmeldung mit einem Dienstprinzipal das Cmdlet `Connect-AzAccount` mit dem Argument `-ServicePrincipal`.</span><span class="sxs-lookup"><span data-stu-id="ba63f-126">To sign in with a service principal, use the `-ServicePrincipal` argument with the `Connect-AzAccount` cmdlet.</span></span> <span data-ttu-id="ba63f-127">Sie benötigen auch die Anwendungs-ID und die Anmeldeinformationen des Dienstprinzipals sowie die dem Dienstprinzipal zugeordnete Mandanten-ID.</span><span class="sxs-lookup"><span data-stu-id="ba63f-127">You'll also need the service principal's application ID, sign-in credentials, and the tenant ID associate with the service principal.</span></span> <span data-ttu-id="ba63f-128">Wie Sie sich mit einem Dienstprinzipal anmelden, hängt davon ab, ob er für die kennwortbasierte oder die zertifikatbasierte Authentifizierung konfiguriert wurde.</span><span class="sxs-lookup"><span data-stu-id="ba63f-128">How you sign in with a service principal will depend on whether it's configured for password-based or certificate-based authentication.</span></span>

### <a name="password-based-authentication"></a><span data-ttu-id="ba63f-129">Kennwortbasierte Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="ba63f-129">Password-based authentication</span></span>

<span data-ttu-id="ba63f-130">Verwenden Sie das Cmdlet [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential), um die Anmeldeinformationen des Dienstprinzipals als entsprechendes Objekt abzurufen.</span><span class="sxs-lookup"><span data-stu-id="ba63f-130">To get the service principal's credentials as the appropriate object, use the [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) cmdlet.</span></span> <span data-ttu-id="ba63f-131">Mit diesem Cmdlet wird eine Eingabeaufforderung für Benutzername und Kennwort angezeigt.</span><span class="sxs-lookup"><span data-stu-id="ba63f-131">This cmdlet will present a prompt for a username and password.</span></span> <span data-ttu-id="ba63f-132">Verwenden Sie die Dienstprinzipal-ID als Benutzernamen.</span><span class="sxs-lookup"><span data-stu-id="ba63f-132">Use the service principal ID for the username.</span></span>

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzAccount -ServicePrincipal -Credential $pscredential -TenantId $tenantId
```

<span data-ttu-id="ba63f-133">Für Automatisierungsszenarien müssen Sie Anmeldeinformationen aus einem Benutzernamen und einer sicheren Zeichenfolge erstellen:</span><span class="sxs-lookup"><span data-stu-id="ba63f-133">For automation scenarios, you need to create credentials from a user name and secure string:</span></span>

```azurepowershell-interactive
$passwd = ConvertTo-SecureString <use a secure password here> -AsPlainText -Force
$pscredential = New-Object System.Management.Automation.PSCredential('service principal name/id', $passwd)
Connect-AzAccount -ServicePrincipal -Credential $pscredential -TenantId $tenantId
```

<span data-ttu-id="ba63f-134">Achten Sie darauf, gute Methoden für die Kennwortspeicherung zu verwenden, wenn Sie Dienstprinzipalverbindungen automatisieren.</span><span class="sxs-lookup"><span data-stu-id="ba63f-134">Make sure that you use good password storage practices when automating service principal connections.</span></span>

### <a name="certificate-based-authentication"></a><span data-ttu-id="ba63f-135">Zertifikatbasierte Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="ba63f-135">Certificate-based authentication</span></span>

<span data-ttu-id="ba63f-136">Zertifikatbasierte Authentifizierung erfordert, dass Azure PowerShell Informationen von einem lokalen Zertifikatsspeicher basierend auf einem Fingerabdruck des Zertifikats abrufen kann.</span><span class="sxs-lookup"><span data-stu-id="ba63f-136">Certificate-based authentication requires that Azure PowerShell can retrieve information from a local certificate store based on a certificate thumbprint.</span></span>
```azurepowershell-interactive
Connect-AzAccount -ServicePrincipal -TenantId $tenantId -CertificateThumbprint <thumbprint>
```

<span data-ttu-id="ba63f-137">In PowerShell 5.1 kann der Zertifikatspeicher mit den [PKI](/powershell/module/pkiclient)-Modul verwaltet und überprüft werden.</span><span class="sxs-lookup"><span data-stu-id="ba63f-137">In PowerShell 5.1, the certificate store can be managed and inspected with the [PKI](/powershell/module/pkiclient) module.</span></span> <span data-ttu-id="ba63f-138">Für PowerShell Core 6.x und höher ist der Prozess komplizierter.</span><span class="sxs-lookup"><span data-stu-id="ba63f-138">For PowerShell Core 6.x and later, the process is more complicated.</span></span> <span data-ttu-id="ba63f-139">Die folgenden Skripts zeigen, wie ein vorhandenes Zertifikat in den für PowerShell zugänglichen Zertifikatspeicher importiert wird.</span><span class="sxs-lookup"><span data-stu-id="ba63f-139">The following scripts show you how to import an existing certificate into the certificate store accessible by PowerShell.</span></span>

#### <a name="import-a-certificate-in-powershell-51"></a><span data-ttu-id="ba63f-140">Importieren eines Zertifikats in PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="ba63f-140">Import a certificate in PowerShell 5.1</span></span>

```azurepowershell-interactive
# Import a PFX
$credentials = Get-Credential -Message "Provide PFX private key password"
Import-PfxCertificate -FilePath <path to certificate> -Password $credentials.Password -CertStoreLocation cert:\CurrentUser\My
```

#### <a name="import-a-certificate-in-powershell-core-6x-and-later"></a><span data-ttu-id="ba63f-141">Importieren eines Zertifikats in PowerShell Core 6.x und höher</span><span class="sxs-lookup"><span data-stu-id="ba63f-141">Import a certificate in PowerShell Core 6.x and later</span></span>

```azurepowershell-interactive
# Import a PFX
$storeName = [System.Security.Cryptography.X509Certificates.StoreName]::My 
$storeLocation = [System.Security.Cryptography.X509Certificates.StoreLocation]::CurrentUser 
$store = [System.Security.Cryptography.X509Certificates.X509Store]::new($storeName, $storeLocation) 
$certPath = <path to certificate>
$credentials = Get-Credential -Message "Provide PFX private key password"
$flag = [System.Security.Cryptography.X509Certificates.X509KeyStorageFlags]::Exportable 
$certificate = [System.Security.Cryptography.X509Certificates.X509Certificate2]::new($certPath, $credentials.Password, $flag) 
$store.Open([System.Security.Cryptography.X509Certificates.OpenFlags]::ReadWrite) 
$store.Add($Certificate) 
$store.Close()
```

## <a name="sign-in-using-a-managed-identity"></a><span data-ttu-id="ba63f-142">Anmelden mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="ba63f-142">Sign in using a managed identity</span></span> 

<span data-ttu-id="ba63f-143">Verwaltete Identitäten sind ein Feature von Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ba63f-143">Managed identities are a feature of Azure Active Directory.</span></span> <span data-ttu-id="ba63f-144">Bei verwalteten Identitäten handelt es sich um Dienstprinzipale, die den in Azure ausgeführten Ressourcen zugewiesen sind.</span><span class="sxs-lookup"><span data-stu-id="ba63f-144">Managed identities are service principals assigned to resources that run in Azure.</span></span> <span data-ttu-id="ba63f-145">Sie können den Dienstprinzipal einer verwalteten Identität für die Anmeldung verwenden und ein App-exklusives Zugriffstoken für den Zugriff auf andere Ressourcen beziehen.</span><span class="sxs-lookup"><span data-stu-id="ba63f-145">You can use a managed identity service principal for sign-in, and acquire an app-only access token to access other resources.</span></span> <span data-ttu-id="ba63f-146">Verwaltete Identitäten stehen nur für Ressourcen zur Verfügung, die in einer Azure-Cloud ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="ba63f-146">Managed identities are only available on resources running in an Azure cloud.</span></span>

<span data-ttu-id="ba63f-147">Weitere Informationen zu verwalteten Identitäten für Azure-Ressourcen finden Sie unter [Verwenden von verwalteten Identitäten für Azure-Ressourcen auf einem virtuellen Azure-Computer zum Abrufen eines Zugriffstokens](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span><span class="sxs-lookup"><span data-stu-id="ba63f-147">To learn more about managed identities for Azure resources, see [How to use managed identities for Azure resources on an Azure VM to acquire an access token](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span></span>

## <a name="sign-in-with-a-non-default-tenant-or-as-a-cloud-solution-provider-csp"></a><span data-ttu-id="ba63f-148">Anmelden mit einem anderen Mandanten als dem Standardmandanten oder als Cloudlösungsanbieter (Cloud Solution Provider, CSP)</span><span class="sxs-lookup"><span data-stu-id="ba63f-148">Sign in with a non-default tenant or as a Cloud Solution Provider (CSP)</span></span>

<span data-ttu-id="ba63f-149">Wenn Ihr Konto mehr als einem Mandanten zugeordnet ist, muss bei der Verbindungsherstellung für die Anmeldung der Parameter `-TenantId` verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="ba63f-149">If your account is associated with more than one tenant, sign-in requires the use of the `-TenantId` parameter when connecting.</span></span> <span data-ttu-id="ba63f-150">Dieser Parameter funktioniert auch mit jedem anderen Anmeldeverfahren.</span><span class="sxs-lookup"><span data-stu-id="ba63f-150">This parameter will work with any other sign-in method.</span></span> <span data-ttu-id="ba63f-151">Beim Anmelden kann dieser Parameterwert entweder die Azure-Objekt-ID des Mandanten (Mandanten-ID) oder der vollqualifizierte Domänenname des Mandanten sein.</span><span class="sxs-lookup"><span data-stu-id="ba63f-151">When logging in, this parameter value can either be the Azure object ID of the tenant (Tenant ID) or the fully qualified domain name of the tenant.</span></span>

<span data-ttu-id="ba63f-152">Wenn Sie ein [Cloudlösungsanbieter (Cloud Solution Provider, CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/) sind, **muss** der Wert `-TenantId` eine Mandanten-ID sein.</span><span class="sxs-lookup"><span data-stu-id="ba63f-152">If you're a [Cloud Solution Provider (CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/), the `-TenantId` value **must** be a tenant ID.</span></span>

```azurepowershell-interactive
Connect-AzAccount -TenantId 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a><span data-ttu-id="ba63f-153">Anmelden bei einer anderen Cloud</span><span class="sxs-lookup"><span data-stu-id="ba63f-153">Sign in to another Cloud</span></span>

<span data-ttu-id="ba63f-154">Azure-Clouddienste verfügen über Umgebungen, die jeweils mit den regionalen Gesetzen zum Umgang mit Daten konform sind.</span><span class="sxs-lookup"><span data-stu-id="ba63f-154">Azure cloud services offer environments compliant with regional data-handling laws.</span></span>
<span data-ttu-id="ba63f-155">Legen Sie die Umgebung für Konten in einer regionalen Cloud fest, wenn Sie sich mit dem Argument `-Environment` anmelden.</span><span class="sxs-lookup"><span data-stu-id="ba63f-155">For accounts in a regional cloud, set the environment when you sign in with the `-Environment` argument.</span></span>
<span data-ttu-id="ba63f-156">Beispiel für den Fall, dass sich Ihr Konto in der Cloud in China befindet:</span><span class="sxs-lookup"><span data-stu-id="ba63f-156">For example, if your account is in the China cloud:</span></span>

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

<span data-ttu-id="ba63f-157">Mit dem folgenden Befehl wird eine Liste mit den verfügbaren Umgebungen abgerufen:</span><span class="sxs-lookup"><span data-stu-id="ba63f-157">The following command gets a list of available environments:</span></span>

```azurepowershell-interactive
Get-AzEnvironment | Select-Object Name
```
