---
title: Anmelden mit Azure PowerShell
description: Es wird beschrieben, wie Sie sich mit Azure PowerShell als Benutzer, per Dienstprinzipal oder mit verwalteten Identitäten für Azure-Ressourcen anmelden.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/29/2018
ms.openlocfilehash: 8b085720aeabe26c1293ece193e050b31f99a693
ms.sourcegitcommit: ae81b08a45d8729fc8d40156422e3eb2e94de8c7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/27/2018
ms.locfileid: "53786678"
---
# <a name="sign-in-with-azure-powershell"></a><span data-ttu-id="30b2e-103">Anmelden mit Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="30b2e-103">Sign in with Azure PowerShell</span></span>

<span data-ttu-id="30b2e-104">Azure PowerShell unterstützt mehrere Authentifizierungsmethoden.</span><span class="sxs-lookup"><span data-stu-id="30b2e-104">Azure PowerShell supports several authentication methods.</span></span> <span data-ttu-id="30b2e-105">Die einfachste Möglichkeit ist die interaktive Anmeldung über die Befehlszeile.</span><span class="sxs-lookup"><span data-stu-id="30b2e-105">The simplest way to get started is to sign in interactively at the command line.</span></span>

## <a name="sign-in-interactively"></a><span data-ttu-id="30b2e-106">Interaktives Anmelden</span><span class="sxs-lookup"><span data-stu-id="30b2e-106">Sign in interactively</span></span>

<span data-ttu-id="30b2e-107">Verwenden Sie für die interaktive Anmeldung das Cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).</span><span class="sxs-lookup"><span data-stu-id="30b2e-107">To sign in interactively, use the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>

```azurepowershell-interactive
Connect-AzAccount
```

<span data-ttu-id="30b2e-108">Bei der Ausführung wird von diesem Cmdlet eine Tokenzeichenfolge bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="30b2e-108">When run, this cmdlet will present a token string.</span></span> <span data-ttu-id="30b2e-109">Kopieren Sie diese Zeichenfolge, und fügen Sie sie in einem Browser unter https://microsoft.com/devicelogin ein.</span><span class="sxs-lookup"><span data-stu-id="30b2e-109">To log in, copy this string and paste it into https://microsoft.com/devicelogin in a browser.</span></span> <span data-ttu-id="30b2e-110">Ihre PowerShell-Sitzung wird dann für die Verbindungsherstellung mit Azure authentifiziert.</span><span class="sxs-lookup"><span data-stu-id="30b2e-110">Your PowerShell session will then be authenticated to connect to Azure.</span></span> <span data-ttu-id="30b2e-111">Diese Authentifizierung gilt jeweils für die aktuelle PowerShell-Sitzung.</span><span class="sxs-lookup"><span data-stu-id="30b2e-111">This authentication lasts for the current PowerShell session.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="30b2e-112">Ihre Anmeldeinformationen werden in mehreren PowerShell-Sitzungen gemeinsam verwendet, solange Sie angemeldet bleiben.</span><span class="sxs-lookup"><span data-stu-id="30b2e-112">Your credentials are shared among multiple PowerShell sessions as long as you remain signed in.</span></span>
> <span data-ttu-id="30b2e-113">Weitere Informationen finden Sie im Artikel zu [beständigen Anmeldeinformationen](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="30b2e-113">For more information, see the article on [Persistent Credentials](context-persistence.md).</span></span>

## <a name="sign-in-with-a-service-principal"></a><span data-ttu-id="30b2e-114">Anmelden mit einem Dienstprinzipal</span><span class="sxs-lookup"><span data-stu-id="30b2e-114">Sign in with a service principal</span></span>

<span data-ttu-id="30b2e-115">Dienstprinzipale sind nicht interaktive Azure-Konten.</span><span class="sxs-lookup"><span data-stu-id="30b2e-115">Service principals are non-interactive Azure accounts.</span></span> <span data-ttu-id="30b2e-116">Wie bei anderen Benutzerkonten auch, werden die Berechtigungen mit Azure Active Directory verwaltet.</span><span class="sxs-lookup"><span data-stu-id="30b2e-116">Like other user accounts, their permissions are managed with Azure Active Directory.</span></span> <span data-ttu-id="30b2e-117">Indem für einen Dienstprinzipal nur die benötigten Berechtigungen gewährt werden, bleibt die Sicherheit Ihrer Automatisierungsskripts gewahrt.</span><span class="sxs-lookup"><span data-stu-id="30b2e-117">By granting a service principal only the permissions it needs, your automation scripts stay secure.</span></span>

<span data-ttu-id="30b2e-118">Informationen zur Erstellung eines Dienstprinzipals für die Verwendung mit PowerShell finden Sie unter [Erstellen eines Azure-Dienstprinzipals mit Azure PowerShell](create-azure-service-principal-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="30b2e-118">To learn how to create a service principal for use with Azure PowerShell, see [Create an Azure service principal with Azure PowerShell](create-azure-service-principal-azureps.md).</span></span>

<span data-ttu-id="30b2e-119">Verwenden Sie für die Anmeldung mit einem Dienstprinzipal das Cmdlet `Connect-AzAccount` mit dem Argument `-ServicePrincipal`.</span><span class="sxs-lookup"><span data-stu-id="30b2e-119">To sign in with a service principal, use the `-ServicePrincipal` argument with the `Connect-AzAccount` cmdlet.</span></span> <span data-ttu-id="30b2e-120">Sie benötigen auch die Anwendungs-ID und die Anmeldeinformationen des Dienstprinzipals sowie die dem Dienstprinzipal zugeordnete Mandanten-ID.</span><span class="sxs-lookup"><span data-stu-id="30b2e-120">You'll also need the service principal's application ID, sign-in credentials, and the tenant ID associate with the service principal.</span></span> <span data-ttu-id="30b2e-121">Verwenden Sie das Cmdlet [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential), um die Anmeldeinformationen des Dienstprinzipals als entsprechendes Objekt abzurufen.</span><span class="sxs-lookup"><span data-stu-id="30b2e-121">To get the service principal's credentials as the appropriate object, use the [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) cmdlet.</span></span> <span data-ttu-id="30b2e-122">Bei diesem Cmdlet wird eine Eingabeaufforderung für die Benutzer-ID und das Kennwort des Dienstprinzipals angezeigt.</span><span class="sxs-lookup"><span data-stu-id="30b2e-122">This cmdlet will present a prompt for the service principal user ID and password.</span></span>

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-an-azure-managed-service-identity"></a><span data-ttu-id="30b2e-123">Anmelden mit einer verwalteten Azure-Dienstidentität</span><span class="sxs-lookup"><span data-stu-id="30b2e-123">Sign in using an Azure Managed Service Identity</span></span>

<span data-ttu-id="30b2e-124">Verwaltete Identitäten für Azure-Ressourcen ist eine Funktion von Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="30b2e-124">Managed identities for Azure resources is a feature of Azure Active Directory.</span></span> <span data-ttu-id="30b2e-125">Sie können den Dienstprinzipal einer verwalteten Identität für die Anmeldung verwenden und ein App-exklusives Zugriffstoken für den Zugriff auf andere Ressourcen beziehen.</span><span class="sxs-lookup"><span data-stu-id="30b2e-125">You can use a managed identity service principal for sign-in, and acquire an app-only access token to access other resources.</span></span> <span data-ttu-id="30b2e-126">Verwaltete Identitäten stehen nur für virtuelle Computer zur Verfügung, die in einer Azure-Cloud ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="30b2e-126">Managed identities are only available on virtual machines running in an Azure cloud.</span></span>

<span data-ttu-id="30b2e-127">Weitere Informationen zu verwalteten Identitäten für Azure-Ressourcen finden Sie unter [Verwenden von verwalteten Identitäten für Azure-Ressourcen auf einem virtuellen Azure-Computer zum Abrufen eines Zugriffstokens](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span><span class="sxs-lookup"><span data-stu-id="30b2e-127">For more information about managed identities for Azure resources, see [How to use managed identities for Azure resources on an Azure VM to acquire an access token](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span></span>

## <a name="sign-in-as-a-cloud-solution-provider-csp"></a><span data-ttu-id="30b2e-128">Anmelden als Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="30b2e-128">Sign in as a Cloud Solution Provider (CSP)</span></span>

<span data-ttu-id="30b2e-129">Eine Anmeldung als [(Cloud Solution Provider, CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/) erfordert die Verwendung von `-TenantId`.</span><span class="sxs-lookup"><span data-stu-id="30b2e-129">A [Cloud Solution Provider (CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/) sign-in requires the use of `-TenantId`.</span></span> <span data-ttu-id="30b2e-130">In der Regel kann dieser Parameter entweder als Mandanten-ID oder als Domänenname angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="30b2e-130">Normally, this parameter can be provided as either a tenant ID or a domain name.</span></span> <span data-ttu-id="30b2e-131">Für die CSP-Anmeldung muss jedoch eine **Mandanten-ID** bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="30b2e-131">However, for CSP sign-in, it must be provided a **tenant ID**.</span></span>

```azurepowershell-interactive
Connect-AzAccount -TenantId 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a><span data-ttu-id="30b2e-132">Anmelden bei einer anderen Cloud</span><span class="sxs-lookup"><span data-stu-id="30b2e-132">Sign in to another Cloud</span></span>

<span data-ttu-id="30b2e-133">Azure-Clouddienste verfügen über Umgebungen, die jeweils mit den regionalen Bestimmungen zum Umgang mit Daten konform sind.</span><span class="sxs-lookup"><span data-stu-id="30b2e-133">Azure cloud services offer environments compliant with regional data-handling regulations.</span></span>
<span data-ttu-id="30b2e-134">Legen Sie die Umgebung für Konten in einer regionalen Cloud fest, wenn Sie sich mit dem Argument `-Environment` anmelden.</span><span class="sxs-lookup"><span data-stu-id="30b2e-134">For accounts in a regional cloud, set the environment when you sign in with the `-Environment` argument.</span></span>
<span data-ttu-id="30b2e-135">Beispiel für den Fall, dass sich Ihr Konto in der Cloud in China befindet:</span><span class="sxs-lookup"><span data-stu-id="30b2e-135">For example, if your account is in the China cloud:</span></span>

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

<span data-ttu-id="30b2e-136">Mit dem folgenden Befehl wird eine Liste mit den verfügbaren Umgebungen abgerufen:</span><span class="sxs-lookup"><span data-stu-id="30b2e-136">The following command gets a list of available environments:</span></span>

```azurepowershell-interactive
Get-AzEnvironment | Select-Object Name
```

## <a name="learn-more-about-managing-azure-role-based-access"></a><span data-ttu-id="30b2e-137">Weitere Informationen zum Verwalten des rollenbasierten Zugriffs in Azure</span><span class="sxs-lookup"><span data-stu-id="30b2e-137">Learn more about managing Azure role-based access</span></span>

<span data-ttu-id="30b2e-138">Weitere Informationen zur Authentifizierung und Abonnementverwaltung in Azure finden Sie unter [Verwalten von Konten, Abonnements und Administratorrollen](/azure/active-directory/role-based-access-control-configure).</span><span class="sxs-lookup"><span data-stu-id="30b2e-138">For more information about authentication and subscription management in Azure, see [Manage Accounts, Subscriptions, and Administrative Roles](/azure/active-directory/role-based-access-control-configure).</span></span>

<span data-ttu-id="30b2e-139">Azure PowerShell-Cmdlets für die Rollenverwaltung:</span><span class="sxs-lookup"><span data-stu-id="30b2e-139">Azure PowerShell cmdlets for role management:</span></span>

* [<span data-ttu-id="30b2e-140">Get-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="30b2e-140">Get-AzRoleAssignment</span></span>](/powershell/module/az.Resources/Get-azRoleAssignment)
* [<span data-ttu-id="30b2e-141">Get-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="30b2e-141">Get-AzRoleDefinition</span></span>](/powershell/module/az.Resources/Get-azRoleDefinition)
* [<span data-ttu-id="30b2e-142">New-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="30b2e-142">New-AzRoleAssignment</span></span>](/powershell/module/az.Resources/New-azRoleAssignment)
* [<span data-ttu-id="30b2e-143">New-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="30b2e-143">New-AzRoleDefinition</span></span>](/powershell/module/az.Resources/New-azRoleDefinition)
* [<span data-ttu-id="30b2e-144">Remove-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="30b2e-144">Remove-AzRoleAssignment</span></span>](/powershell/module/az.Resources/Remove-azRoleAssignment)
* [<span data-ttu-id="30b2e-145">Remove-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="30b2e-145">Remove-AzRoleDefinition</span></span>](/powershell/module/az.Resources/Remove-azRoleDefinition)
* [<span data-ttu-id="30b2e-146">Set-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="30b2e-146">Set-AzRoleDefinition</span></span>](/powershell/module/az.Resources/Set-azRoleDefinition)
