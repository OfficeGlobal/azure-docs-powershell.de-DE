---
title: Anmelden mit Azure PowerShell
description: Es wird beschrieben, wie Sie sich mit Azure PowerShell als Benutzer, per Dienstprinzipal oder mit verwalteten Identitäten für Azure-Ressourcen anmelden.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/29/2018
ms.openlocfilehash: 80c59a10666c6e3a01e6c33716fce40094fb14be
ms.sourcegitcommit: c6fd0e490fa0e33b8b768b679682a47d8faae1cf
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/16/2019
ms.locfileid: "54342063"
---
# <a name="sign-in-with-azure-powershell"></a><span data-ttu-id="d1680-103">Anmelden mit Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="d1680-103">Sign in with Azure PowerShell</span></span>

<span data-ttu-id="d1680-104">Azure PowerShell unterstützt mehrere Authentifizierungsmethoden.</span><span class="sxs-lookup"><span data-stu-id="d1680-104">Azure PowerShell supports several authentication methods.</span></span> <span data-ttu-id="d1680-105">Den einfachsten Einstieg ermöglicht der [Azure Cloud Shell](/azure/cloud-shell/overview)-Dienst, der Sie automatisch anmeldet.</span><span class="sxs-lookup"><span data-stu-id="d1680-105">The easiest way to get started is with [Azure Cloud Shell](/azure/cloud-shell/overview), which automatically logs you in.</span></span> <span data-ttu-id="d1680-106">Bei einer lokalen Installation können Sie sich interaktiv über Ihren Browser anmelden.</span><span class="sxs-lookup"><span data-stu-id="d1680-106">With a local install, you can sign in interactively through your browser.</span></span> <span data-ttu-id="d1680-107">Beim Schreiben von Skripts für die Automatisierung besteht der empfohlene Ansatz darin, einen [Dienstprinzipal](create-azure-service-principal-azureps.md) mit den erforderlichen Berechtigungen zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="d1680-107">When writing scripts for automation, the recommended approach is to use a [service principal](create-azure-service-principal-azureps.md) with the necessary permissions.</span></span> <span data-ttu-id="d1680-108">Indem Sie die Anmeldeberechtigungen für Ihren Anwendungsfall so weit wie möglich einschränken, tragen Sie zur Sicherheit Ihrer Azure-Ressourcen bei.</span><span class="sxs-lookup"><span data-stu-id="d1680-108">When you restrict sign-in permissions as much as possible for your use case, you help keep your Azure resources secure.</span></span>

<span data-ttu-id="d1680-109">Nach der Anmeldung werden Befehle für Ihr Standardabonnement ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="d1680-109">After signing in, commands are run against your default subscription.</span></span> <span data-ttu-id="d1680-110">Verwenden Sie das Cmdlet [Set-AzContext](/powershell/module/az.accounts/set-azcontext), um Ihr aktives Abonnement für eine Sitzung zu ändern.</span><span class="sxs-lookup"><span data-stu-id="d1680-110">To change your active subscription for a session, use the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span> <span data-ttu-id="d1680-111">Verwenden Sie [Set-AzDefault](/powershell/module/az.accounts/set-azdefault), um das Standardabonnement zu ändern, das beim Anmelden mit Azure PowerShell verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="d1680-111">To change the default subscription used when logging in with Azure PowerShell, use [Set-AzDefault](/powershell/module/az.accounts/set-azdefault).</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="d1680-112">Ihre Anmeldeinformationen werden in mehreren PowerShell-Sitzungen gemeinsam verwendet, solange Sie angemeldet bleiben.</span><span class="sxs-lookup"><span data-stu-id="d1680-112">Your credentials are shared among multiple PowerShell sessions as long as you remain signed in.</span></span>
> <span data-ttu-id="d1680-113">Weitere Informationen finden Sie im Artikel zu [beständigen Anmeldeinformationen](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="d1680-113">For more information, see the article on [Persistent Credentials](context-persistence.md).</span></span>

## <a name="sign-in-interactively"></a><span data-ttu-id="d1680-114">Interaktives Anmelden</span><span class="sxs-lookup"><span data-stu-id="d1680-114">Sign in interactively</span></span>

<span data-ttu-id="d1680-115">Verwenden Sie für die interaktive Anmeldung das Cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).</span><span class="sxs-lookup"><span data-stu-id="d1680-115">To sign in interactively, use the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>

```azurepowershell-interactive
Connect-AzAccount
```

<span data-ttu-id="d1680-116">Bei der Ausführung wird von diesem Cmdlet eine Tokenzeichenfolge bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="d1680-116">When run, this cmdlet will present a token string.</span></span> <span data-ttu-id="d1680-117">Kopieren Sie diese Zeichenfolge, und fügen Sie sie in einem Browser unter https://microsoft.com/devicelogin ein, um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="d1680-117">To sign in, copy this string and paste it into https://microsoft.com/devicelogin in a browser.</span></span> <span data-ttu-id="d1680-118">Ihre PowerShell-Sitzung wird für die Verbindungsherstellung mit Azure authentifiziert.</span><span class="sxs-lookup"><span data-stu-id="d1680-118">Your PowerShell session will be authenticated to connect to Azure.</span></span>

## <a name="sign-in-with-credentials"></a><span data-ttu-id="d1680-119">Anmelden mit Anmeldeinformationen</span><span class="sxs-lookup"><span data-stu-id="d1680-119">Sign in with credentials</span></span>

<span data-ttu-id="d1680-120">Sie können sich auch mit einem `PSCredential`-Objekt anmelden, das für die Verbindungsherstellung mit Azure autorisiert ist.</span><span class="sxs-lookup"><span data-stu-id="d1680-120">You can also sign in with a `PSCredential` object authorized to connect to Azure.</span></span>
<span data-ttu-id="d1680-121">Die einfachste Möglichkeit zum Abrufen eines Objekts mit Anmeldeinformationen ist die Verwendung des Cmdlets [Get-Credential](/powershell/module/Microsoft.PowerShell.Security/Get-Credential).</span><span class="sxs-lookup"><span data-stu-id="d1680-121">The easiest way to get a credential object is with the [Get-Credential](/powershell/module/Microsoft.PowerShell.Security/Get-Credential) cmdlet.</span></span> <span data-ttu-id="d1680-122">Beim Ausführen werden Sie bei diesem Cmdlet zum Eingeben eines Benutzername/Kennwort-Paars als Anmeldeinformationen aufgefordert.</span><span class="sxs-lookup"><span data-stu-id="d1680-122">When run, this cmdlet will prompt you for a username/password credential pair.</span></span>

> [!Note]
> <span data-ttu-id="d1680-123">Dieser Ansatz funktioniert nicht für Microsoft-Konten oder Konten, für die die Authentifizierung in zwei Schritten aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="d1680-123">This approach doesn't work with Microsoft accounts or accounts that have two-factor authentication enabled.</span></span>

```azurepowershell-interactive
$creds = Get-Credential
Connect-AzAccount -Credential $creds
```

## <a name="sign-in-with-a-service-principal"></a><span data-ttu-id="d1680-124">Anmelden mit einem Dienstprinzipal</span><span class="sxs-lookup"><span data-stu-id="d1680-124">Sign in with a service principal</span></span>

<span data-ttu-id="d1680-125">Dienstprinzipale sind nicht interaktive Azure-Konten.</span><span class="sxs-lookup"><span data-stu-id="d1680-125">Service principals are non-interactive Azure accounts.</span></span> <span data-ttu-id="d1680-126">Wie bei anderen Benutzerkonten auch, werden die Berechtigungen mit Azure Active Directory verwaltet.</span><span class="sxs-lookup"><span data-stu-id="d1680-126">Like other user accounts, their permissions are managed with Azure Active Directory.</span></span> <span data-ttu-id="d1680-127">Indem für einen Dienstprinzipal nur die benötigten Berechtigungen gewährt werden, bleibt die Sicherheit Ihrer Automatisierungsskripts gewahrt.</span><span class="sxs-lookup"><span data-stu-id="d1680-127">By granting a service principal only the permissions it needs, your automation scripts stay secure.</span></span>

<span data-ttu-id="d1680-128">Informationen zur Erstellung eines Dienstprinzipals für die Verwendung mit PowerShell finden Sie unter [Erstellen eines Azure-Dienstprinzipals mit Azure PowerShell](create-azure-service-principal-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="d1680-128">To learn how to create a service principal for use with Azure PowerShell, see [Create an Azure service principal with Azure PowerShell](create-azure-service-principal-azureps.md).</span></span>

<span data-ttu-id="d1680-129">Verwenden Sie für die Anmeldung mit einem Dienstprinzipal das Cmdlet `Connect-AzAccount` mit dem Argument `-ServicePrincipal`.</span><span class="sxs-lookup"><span data-stu-id="d1680-129">To sign in with a service principal, use the `-ServicePrincipal` argument with the `Connect-AzAccount` cmdlet.</span></span> <span data-ttu-id="d1680-130">Sie benötigen auch die Anwendungs-ID und die Anmeldeinformationen des Dienstprinzipals sowie die dem Dienstprinzipal zugeordnete Mandanten-ID.</span><span class="sxs-lookup"><span data-stu-id="d1680-130">You'll also need the service principal's application ID, sign-in credentials, and the tenant ID associate with the service principal.</span></span> <span data-ttu-id="d1680-131">Verwenden Sie das Cmdlet [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential), um die Anmeldeinformationen des Dienstprinzipals als entsprechendes Objekt abzurufen.</span><span class="sxs-lookup"><span data-stu-id="d1680-131">To get the service principal's credentials as the appropriate object, use the [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) cmdlet.</span></span> <span data-ttu-id="d1680-132">Bei diesem Cmdlet wird eine Eingabeaufforderung für die Benutzer-ID und das Kennwort des Dienstprinzipals angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d1680-132">This cmdlet will present a prompt for the service principal user ID and password.</span></span>

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-a-managed-identity"></a><span data-ttu-id="d1680-133">Anmelden mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="d1680-133">Sign in using a managed identity</span></span> 

<span data-ttu-id="d1680-134">Verwaltete Identitäten sind ein Feature von Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d1680-134">Managed identities are a feature of Azure Active Directory.</span></span> <span data-ttu-id="d1680-135">Bei verwalteten Identitäten handelt es sich um Dienstprinzipale, die den in Azure ausgeführten Ressourcen zugewiesen sind.</span><span class="sxs-lookup"><span data-stu-id="d1680-135">Managed identities are service principals assigned to resources that run in Azure.</span></span> <span data-ttu-id="d1680-136">Sie können den Dienstprinzipal einer verwalteten Identität für die Anmeldung verwenden und ein App-exklusives Zugriffstoken für den Zugriff auf andere Ressourcen beziehen.</span><span class="sxs-lookup"><span data-stu-id="d1680-136">You can use a managed identity service principal for sign-in, and acquire an app-only access token to access other resources.</span></span> <span data-ttu-id="d1680-137">Verwaltete Identitäten stehen nur für Ressourcen zur Verfügung, die in einer Azure-Cloud ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="d1680-137">Managed identities are only available on resources running in an Azure cloud.</span></span>

<span data-ttu-id="d1680-138">Weitere Informationen zu verwalteten Identitäten für Azure-Ressourcen finden Sie unter [Verwenden von verwalteten Identitäten für Azure-Ressourcen auf einem virtuellen Azure-Computer zum Abrufen eines Zugriffstokens](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span><span class="sxs-lookup"><span data-stu-id="d1680-138">To learn more about managed identities for Azure resources, see [How to use managed identities for Azure resources on an Azure VM to acquire an access token](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span></span>

## <a name="sign-in-with-a-non-default-tenant-or-as-a-cloud-solution-provider-csp"></a><span data-ttu-id="d1680-139">Anmelden mit einem anderen Mandanten als dem Standardmandanten oder als Cloudlösungsanbieter (Cloud Solution Provider, CSP)</span><span class="sxs-lookup"><span data-stu-id="d1680-139">Sign in with a non-default tenant or as a Cloud Solution Provider (CSP)</span></span>

<span data-ttu-id="d1680-140">Wenn Ihr Konto mehr als einem Mandanten zugeordnet ist, muss bei der Verbindungsherstellung für die Anmeldung der Parameter `-TenantId` verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="d1680-140">If your account is associated with more than one tenant, sign-in requires the use of the `-TenantId` parameter when connecting.</span></span> <span data-ttu-id="d1680-141">Dieser Parameter funktioniert auch mit jedem anderen Anmeldeverfahren.</span><span class="sxs-lookup"><span data-stu-id="d1680-141">This parameter will work with any other sign-in method.</span></span> <span data-ttu-id="d1680-142">Beim Anmelden kann dieser Parameterwert entweder die Azure-Objekt-ID des Mandanten (Mandanten-ID) oder der vollqualifizierte Domänenname des Mandanten sein.</span><span class="sxs-lookup"><span data-stu-id="d1680-142">When logging in, this parameter value can either be the Azure object ID of the tenant (Tenant ID) or the fully qualified domain name of the tenant.</span></span>

<span data-ttu-id="d1680-143">Wenn Sie ein [Cloudlösungsanbieter (Cloud Solution Provider, CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/) sind, **muss** der Wert `-TenantId` eine Mandanten-ID sein.</span><span class="sxs-lookup"><span data-stu-id="d1680-143">If you're a [Cloud Solution Provider (CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/), the `-TenantId` value **must** be a tenant ID.</span></span>

```azurepowershell-interactive
Connect-AzAccount -TenantId 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a><span data-ttu-id="d1680-144">Anmelden bei einer anderen Cloud</span><span class="sxs-lookup"><span data-stu-id="d1680-144">Sign in to another Cloud</span></span>

<span data-ttu-id="d1680-145">Azure-Clouddienste verfügen über Umgebungen, die jeweils mit den regionalen Gesetzen zum Umgang mit Daten konform sind.</span><span class="sxs-lookup"><span data-stu-id="d1680-145">Azure cloud services offer environments compliant with regional data-handling laws.</span></span>
<span data-ttu-id="d1680-146">Legen Sie die Umgebung für Konten in einer regionalen Cloud fest, wenn Sie sich mit dem Argument `-Environment` anmelden.</span><span class="sxs-lookup"><span data-stu-id="d1680-146">For accounts in a regional cloud, set the environment when you sign in with the `-Environment` argument.</span></span>
<span data-ttu-id="d1680-147">Beispiel für den Fall, dass sich Ihr Konto in der Cloud in China befindet:</span><span class="sxs-lookup"><span data-stu-id="d1680-147">For example, if your account is in the China cloud:</span></span>

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

<span data-ttu-id="d1680-148">Mit dem folgenden Befehl wird eine Liste mit den verfügbaren Umgebungen abgerufen:</span><span class="sxs-lookup"><span data-stu-id="d1680-148">The following command gets a list of available environments:</span></span>

```azurepowershell-interactive
Get-AzEnvironment | Select-Object Name
```