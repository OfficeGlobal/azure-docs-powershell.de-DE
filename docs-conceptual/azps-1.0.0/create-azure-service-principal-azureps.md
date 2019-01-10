---
title: Erstellen eines Azure-Dienstprinzipals mit Azure PowerShell
description: Hier erfahren Sie, wie Sie mit Azure PowerShell einen Dienstprinzipal für Ihre App oder Ihren Dienst erstellen.
keywords: Azure PowerShell, Azure Active Directory, Azure Active directory, AD, RBAC
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: 3e1c5ad280bdb29ce479dd0a478d0ed58237f969
ms.sourcegitcommit: 797c18f93aaa495ef005993b2e202d7378588dfa
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/19/2018
ms.locfileid: "53594781"
---
# <a name="create-an-azure-service-principal-with-azure-powershell"></a><span data-ttu-id="b8cdb-104">Erstellen eines Azure-Dienstprinzipals mit Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="b8cdb-104">Create an Azure service principal with Azure PowerShell</span></span>

<span data-ttu-id="b8cdb-105">Wenn Sie Ihre App oder Ihren Dienst mit Azure PowerShell verwalten möchten, sollten Sie sie bzw. ihn nicht unter Ihren eigenen Anmeldeinformationen, sondern unter einem AAD-Dienstprinzipal (Azure Active Directory) ausführen.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-105">If you plan to manage your app or service with Azure PowerShell, you should run it under an Azure Active Directory (AAD) service principal, rather than your own credentials.</span></span> <span data-ttu-id="b8cdb-106">In diesem Artikel wird Schritt für Schritt erläutert, wie Sie einen Sicherheitsprinzipal mit Azure PowerShell erstellen.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-106">This article steps you through creating a security principal with Azure PowerShell.</span></span>

## <a name="what-is-a-service-principal"></a><span data-ttu-id="b8cdb-107">Was ist ein Dienstprinzipal?</span><span class="sxs-lookup"><span data-stu-id="b8cdb-107">What is a service principal?</span></span>

<span data-ttu-id="b8cdb-108">Ein Azure-Dienstprinzipal ist eine Sicherheitsidentität, die durch von Benutzern erstellte Apps, Dienste und Automatisierungstools verwendet wird, um auf bestimmte Azure-Ressourcen zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-108">An Azure service principal is a security identity used by user-created apps, services, and automation tools to access specific Azure resources.</span></span> <span data-ttu-id="b8cdb-109">Dienstprinzipalen werden bestimmte Berechtigungen zugewiesen, die sich auf die zugehörigen Aufgaben beziehen, damit Sie die Sicherheit besser steuern können.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-109">Service principals are assigned specific permissions related to their tasks, giving you better security control.</span></span> <span data-ttu-id="b8cdb-110">Dies entspricht nicht einer allgemeinen Benutzeridentität, die normalerweise für das Vornehmen von Änderungen autorisiert ist.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-110">This is unlike a general user identity, which is usually authorized to make any changes.</span></span>

## <a name="verify-your-own-permission-level"></a><span data-ttu-id="b8cdb-111">Überprüfen der eigenen Berechtigungsstufe</span><span class="sxs-lookup"><span data-stu-id="b8cdb-111">Verify your own permission level</span></span>

<span data-ttu-id="b8cdb-112">Zunächst einmal müssen Sie sowohl in der Azure Active Directory-Instanz als auch im Azure-Abonnement über ausreichende Berechtigungen verfügen.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-112">First, you must have sufficient permissions in both your Azure Active Directory and your Azure subscription.</span></span> <span data-ttu-id="b8cdb-113">Sie müssen eine App in der Active Directory-Instanz erstellen und dem Dienstprinzipal eine Rolle zuweisen können.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-113">You must be able to create an app in the Active Directory and assign a role to the service principal.</span></span>

<span data-ttu-id="b8cdb-114">Die einfachste Möglichkeit zum Überprüfen, ob Ihr Konto über die richtigen Berechtigungen verfügt, ist die Vorgehensweise über das Portal.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-114">The easiest way to check whether your account has the right permissions is through the portal.</span></span> <span data-ttu-id="b8cdb-115">Siehe [Überprüfen der erforderlichen Berechtigung im Portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions).</span><span class="sxs-lookup"><span data-stu-id="b8cdb-115">See [Check required permission in portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions).</span></span>

## <a name="create-a-service-principal-for-your-app"></a><span data-ttu-id="b8cdb-116">Erstellen eines Dienstprinzipals für Ihre App</span><span class="sxs-lookup"><span data-stu-id="b8cdb-116">Create a service principal for your app</span></span>

<span data-ttu-id="b8cdb-117">Nachdem Sie sich an Ihrem Azure-Konto angemeldet haben, können Sie den Dienstprinzipal erstellen.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-117">Once signed in to your Azure account, you can create the service principal.</span></span> <span data-ttu-id="b8cdb-118">Ihre bereitgestellte App muss auf eine der folgenden Arten identifiziert werden:</span><span class="sxs-lookup"><span data-stu-id="b8cdb-118">You must have one of the following ways to identify your deployed app:</span></span>

* <span data-ttu-id="b8cdb-119">Mithilfe des eindeutigen Namens Ihrer bereitgestellten App („MyDemoWebApp“ in den folgenden Beispielen)</span><span class="sxs-lookup"><span data-stu-id="b8cdb-119">The unique name of your deployed app, such as "MyDemoWebApp" in the following examples</span></span>
* <span data-ttu-id="b8cdb-120">Mithilfe der Anwendungs-ID (GUID, die Ihrer bereitgestellten App, Ihrem bereitgestellten Dienst oder Ihrem bereitgestellten Objekt zugeordnet ist)</span><span class="sxs-lookup"><span data-stu-id="b8cdb-120">The Application ID, the unique GUID associated with your deployed app, service, or object</span></span>

### <a name="get-information-about-your-application"></a><span data-ttu-id="b8cdb-121">Abrufen von Informationen zu Ihrer Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8cdb-121">Get information about your application</span></span>

<span data-ttu-id="b8cdb-122">Mit dem Cmdlet `Get-AzADApplication` können Sie Informationen zu Ihrer Anwendung erhalten.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-122">The `Get-AzADApplication` cmdlet can be used to get information about your application.</span></span>

```azurepowershell-interactive
$app = Get-AzADApplication -DisplayNameStartWith MyDemoWebApp
$app
```

```output
DisplayName             : MyDemoWebApp
ObjectId                : 775f64cd-0ec8-4b9b-b69a-8b8946022d9f
IdentifierUris          : {http://MyDemoWebApp}
HomePage                : http://www.contoso.com
Type                    : Application
ApplicationId           : 00c01aaa-1603-49fc-b6df-b78c4e5138b4
AvailableToOtherTenants : False
AppPermissions          :
ReplyUrls               : {}
```

### <a name="create-a-service-principal-for-your-application"></a><span data-ttu-id="b8cdb-123">Erstellen eines Dienstprinzipals für Ihre Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8cdb-123">Create a service principal for your application</span></span>

<span data-ttu-id="b8cdb-124">Das Cmdlet `New-AzADServicePrincipal` dient zum Erstellen des Dienstprinzipals.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-124">The `New-AzADServicePrincipal` cmdlet is used to create the service principal.</span></span>

```azurepowershell-interactive
$servicePrincipal = New-AzADServicePrincipal -ApplicationId 00c01aaa-1603-49fc-b6df-b78c4e5138b4
```

```output
Secret                : System.Security.SecureString
ServicePrincipalNames : {00c01aaa-1603-49fc-b6df-b78c4e5138b4, http://MyDemoWebApp}
ApplicationId         : 00c01aaa-1603-49fc-b6df-b78c4e5138b4
DisplayName           : MyDemoWebApp
Id                    : 698138e7-d7b6-4738-a866-b4e3081a69e4
AdfsId                :
Type                  : ServicePrincipal
```

<span data-ttu-id="b8cdb-125">Von hier aus können Sie entweder direkt die `$servicePrincipal.Secret`-Eigenschaft als Argument für `Connect-AzAccount` verwenden (siehe „Anmelden mithilfe des Dienstprinzipals“) oder dieses `SecureString`-Element in eine Nur-Text-Zeichenfolge konvertieren:</span><span class="sxs-lookup"><span data-stu-id="b8cdb-125">From here, you can either directly use the `$servicePrincipal.Secret` property as an argument to `Connect-AzAccount` (see "Sign in using the service principal"), or you can convert this `SecureString` to a plain text string:</span></span>

```azurepowershell-interactive
$BSTR = [System.Runtime.InteropServices.Marshal]::SecureStringToBSTR($servicePrincipal.Secret)
$password = [System.Runtime.InteropServices.Marshal]::PtrToStringAuto($BSTR)
[Runtime.InteropServices.Marshal]::ZeroFreeBSTR($BSTR)
```

### <a name="sign-in-using-the-service-principal"></a><span data-ttu-id="b8cdb-126">Anmelden mithilfe des Dienstprinzipals</span><span class="sxs-lookup"><span data-stu-id="b8cdb-126">Sign in using the service principal</span></span>

<span data-ttu-id="b8cdb-127">Nun können Sie sich als der neue Dienstprinzipal für die App anmelden, indem Sie die von Ihnen angegebene `appId` und das generierte `password`</span><span class="sxs-lookup"><span data-stu-id="b8cdb-127">You can now sign in as the new service principal for your app using the `appId` you provided and `password` that was</span></span>  
<span data-ttu-id="b8cdb-128">verwenden.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-128">generated.</span></span> <span data-ttu-id="b8cdb-129">Außerdem benötigen Sie die Mandanten-ID für den Dienstprinzipal.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-129">You also need the Tenant ID for the service principal.</span></span> <span data-ttu-id="b8cdb-130">Ihre Mandanten-ID wird angezeigt, wenn Sie sich mit Ihren persönlichen Anmeldeinformationen bei Azure anmelden.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-130">Your Tenant ID is displayed when you sign into Azure with your personal credentials.</span></span> <span data-ttu-id="b8cdb-131">Verwenden Sie die folgenden Befehle, um sich mit einem Dienstprinzipal anzumelden:</span><span class="sxs-lookup"><span data-stu-id="b8cdb-131">To sign in with a service principal, use the commands:</span></span>

```azurepowershell-interactive
$cred = New-Object System.Management.Automation.PSCredential ("00c01aaa-1603-49fc-b6df-b78c4e5138b4", $servicePrincipal.Secret)
Connect-AzAccount -Credential $cred -ServicePrincipal -TenantId XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```

<span data-ttu-id="b8cdb-132">Nach einer erfolgreichen Anmeldung wird die folgende Ausgabe angezeigt:</span><span class="sxs-lookup"><span data-stu-id="b8cdb-132">After a successful sign-in you see output like:</span></span>

```output
Environment           : AzureCloud
Account               : 00c01aaa-1603-49fc-b6df-b78c4e5138b4
TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
SubscriptionId        :
SubscriptionName      :
CurrentStorageAccount :
```

<span data-ttu-id="b8cdb-133">Glückwunsch!</span><span class="sxs-lookup"><span data-stu-id="b8cdb-133">Congratulations!</span></span> <span data-ttu-id="b8cdb-134">Die Anmeldeinformationen können zum Ausführen Ihrer App verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-134">You can use these credentials to run your app.</span></span> <span data-ttu-id="b8cdb-135">Als Nächstes müssen Sie die Berechtigungen des Dienstprinzipals anpassen.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-135">Next, you need to adjust the permissions of the service principal.</span></span>

## <a name="managing-roles"></a><span data-ttu-id="b8cdb-136">Verwalten von Rollen</span><span class="sxs-lookup"><span data-stu-id="b8cdb-136">Managing roles</span></span>

> [!NOTE]
> <span data-ttu-id="b8cdb-137">Bei der rollenbasierten Zugriffssteuerung (Role-Based Access Control, RBAC) in Azure handelt es sich um ein Modell zum Definieren und Verwalten von Rollen für Benutzer- und Dienstprinzipale.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-137">Azure Role-Based Access Control (RBAC) is a model for defining and managing roles for user and service principals.</span></span> <span data-ttu-id="b8cdb-138">Rollen sind bestimmte Berechtigungen zugeordnet, die bestimmen, welche Ressourcen ein Prinzipal lesen, aufrufen, schreiben oder verwalten kann.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-138">Roles have sets of permissions associated with them, which determine the resources a principal can read, access, write, or manage.</span></span> <span data-ttu-id="b8cdb-139">Weitere Informationen zu RBAC und Rollen finden Sie unter [ Integrierte Rollen für die rollenbasierte Zugriffssteuerung in Azure](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="b8cdb-139">For more information on RBAC and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="b8cdb-140">Für die Verwaltung von Rollenzuweisungen stehen in Azure PowerShell folgende Cmdlets zur Verfügung:</span><span class="sxs-lookup"><span data-stu-id="b8cdb-140">Azure PowerShell provides the following cmdlets to manage role assignments:</span></span>

* [<span data-ttu-id="b8cdb-141">Get-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b8cdb-141">Get-AzRoleAssignment</span></span>](/powershell/module/az.resources/get-azroleassignment)
* [<span data-ttu-id="b8cdb-142">New-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b8cdb-142">New-AzRoleAssignment</span></span>](/powershell/module/az.resources/new-azroleassignment)
* [<span data-ttu-id="b8cdb-143">Remove-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b8cdb-143">Remove-AzRoleAssignment</span></span>](/powershell/module/az.resources/remove-azroleassignment)

<span data-ttu-id="b8cdb-144">Standardmäßig hat ein Dienstprinzipal die Rolle **Mitwirkender**.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-144">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="b8cdb-145">Je nachdem, in welchem Maß Ihrer App mit Azure Services interagiert, ist das unter Umständen nicht die beste Wahl, da diese Rolle über umfassende Berechtigungen verfügt.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-145">It may not be the best choice depending on the scope of your app's interactions with Azure services, given its broad permissions.</span></span>
<span data-ttu-id="b8cdb-146">Die Rolle **Leser** ist stärker eingeschränkt und bietet sich für Apps ohne Schreibzugriff an.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-146">The **Reader** role is more restrictive and can be a good choice for read-only apps.</span></span> <span data-ttu-id="b8cdb-147">Über das Azure-Portal können Sie Details zu rollenspezifischen Berechtigungen anzeigen oder benutzerdefinierte Berechtigungen erstellen.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-147">You can view details on role-specific permissions or create custom ones through the Azure portal.</span></span>

<span data-ttu-id="b8cdb-148">Im folgenden Beispiel fügen wir unserem vorherigen Beispiel die Rolle **Leser** hinzu und löschen die Rolle **Mitwirkender**:</span><span class="sxs-lookup"><span data-stu-id="b8cdb-148">In this example, we add the **Reader** role to our prior example, and delete the **Contributor** one:</span></span>

```azurepowershell-interactive
New-AzRoleAssignment -ResourceGroupName myRG -ObjectId 698138e7-d7b6-4738-a866-b4e3081a69e4 -RoleDefinitionName Reader
```

```output
RoleAssignmentId   : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myRG/providers/Microsoft.Authorization/roleAssignments/818892f2-d075-46a1-a3a2-3a4e1a12fcd5
Scope              : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myRG
DisplayName        : MyDemoWebApp
SignInName         :
RoleDefinitionName : Reader
RoleDefinitionId   : b24988ac-6180-42a0-ab88-20f7382dd24c
ObjectId           : 698138e7-d7b6-4738-a866-b4e3081a69e4
ObjectType         : ServicePrincipal
```

```azurepowershell-interactive
Remove-AzRoleAssignment -ResourceGroupName myRG -ObjectId 698138e7-d7b6-4738-a866-b4e3081a69e4 -RoleDefinitionName Contributor
```

<span data-ttu-id="b8cdb-149">So zeigen Sie die derzeit zugewiesenen Rollen an:</span><span class="sxs-lookup"><span data-stu-id="b8cdb-149">To view the current roles assigned:</span></span>

```azurepowershell-interactive
Get-AzRoleAssignment -ResourceGroupName myRG -ObjectId 698138e7-d7b6-4738-a866-b4e3081a69e4
```

```output
RoleAssignmentId   : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myRG/providers/Microsoft.Authorization/roleAssignments/0906bbd8-9982-4c03-8dae-aeaae8b13f9e
Scope              : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myRG
DisplayName        : MyDemoWebApp
SignInName         :
RoleDefinitionName : Reader
RoleDefinitionId   : acdd72a7-3385-48ef-bd42-f606fba81ae7
ObjectId           : 698138e7-d7b6-4738-a866-b4e3081a69e4
ObjectType         : ServicePrincipal
```

<span data-ttu-id="b8cdb-150">Weitere Azure PowerShell-Cmdlets für die Rollenverwaltung:</span><span class="sxs-lookup"><span data-stu-id="b8cdb-150">Other Azure PowerShell cmdlets for role management:</span></span>

* [<span data-ttu-id="b8cdb-151">Get-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="b8cdb-151">Get-AzRoleDefinition</span></span>](/powershell/module/az.resources/Get-azRoleDefinition)
* [<span data-ttu-id="b8cdb-152">New-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="b8cdb-152">New-AzRoleDefinition</span></span>](/powershell/module/az.resources/New-azRoleDefinition)
* [<span data-ttu-id="b8cdb-153">Remove-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="b8cdb-153">Remove-AzRoleDefinition</span></span>](/powershell/module/az.resources/Remove-azRoleDefinition)
* [<span data-ttu-id="b8cdb-154">Set-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="b8cdb-154">Set-AzRoleDefinition</span></span>](/powershell/module/az.resources/Set-azRoleDefinition)

## <a name="change-the-credentials-of-the-security-principal"></a><span data-ttu-id="b8cdb-155">Ändern der Anmeldeinformationen des Sicherheitsprinzipals</span><span class="sxs-lookup"><span data-stu-id="b8cdb-155">Change the credentials of the security principal</span></span>

<span data-ttu-id="b8cdb-156">Aus Sicherheitsgründen empfiehlt es sich, regelmäßig die Berechtigungen zu überprüfen und das Kennwort zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-156">It's a good security practice to review the permissions and update the password regularly.</span></span> <span data-ttu-id="b8cdb-157">Darüber hinaus sollten Sie auch die Sicherheitsanmeldeinformationen verwalten und ändern, wenn sich Ihre App verändert.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-157">You may also want to manage and modify the security credentials as your app changes.</span></span> <span data-ttu-id="b8cdb-158">Zum Ändern des Dienstprinzipalkennworts können wir beispielsweise ein neues Kennwort erstellen und das alte entfernen.</span><span class="sxs-lookup"><span data-stu-id="b8cdb-158">For example, we can change the password of the service principal by creating a new password and removing the old one.</span></span>

### <a name="add-a-new-password-for-the-service-principal"></a><span data-ttu-id="b8cdb-159">Hinzufügen eines neuen Kennworts für den Dienstprinzipal</span><span class="sxs-lookup"><span data-stu-id="b8cdb-159">Add a new password for the service principal</span></span>

```azurepowershell-interactive
New-AzADSpCredential -ServicePrincipalName http://MyDemoWebApp
```

```output
Secret    : System.Security.SecureString
StartDate : 11/16/2018 12:38:23 AM
EndDate   : 11/16/2019 12:38:23 AM
KeyId     : 6f801c3e-6fcd-42b9-be8e-320b17ba1d36
Type      : Password
```

### <a name="get-a-list-of-credentials-for-the-service-principal"></a><span data-ttu-id="b8cdb-160">Abrufen einer Liste mit Anmeldeinformationen für den Dienstprinzipal</span><span class="sxs-lookup"><span data-stu-id="b8cdb-160">Get a list of credentials for the service principal</span></span>

```azurepowershell-interactive
Get-AzADSpCredential -ServicePrincipalName http://MyDemoWebApp
```

```output
StartDate           EndDate             KeyId                                Type
---------           -------             -----                                ----
3/8/2017 5:58:24 PM 3/8/2018 5:58:24 PM 6f801c3e-6fcd-42b9-be8e-320b17ba1d36 Password
5/5/2016 4:55:27 PM 5/5/2017 4:55:27 PM ca9d4846-4972-4c70-b6f5-a4effa60b9bc Password
```

### <a name="remove-the-old-password-from-the-service-principal"></a><span data-ttu-id="b8cdb-161">Entfernen des alten Kennworts für den Dienstprinzipal</span><span class="sxs-lookup"><span data-stu-id="b8cdb-161">Remove the old password from the service principal</span></span>

```azurepowershell-interactive
Remove-AzADSpCredential -ServicePrincipalName http://MyDemoWebApp -KeyId ca9d4846-4972-4c70-b6f5-a4effa60b9bc
```

```output
Confirm
Are you sure you want to remove credential with keyId '6f801c3e-6fcd-42b9-be8e-320b17ba1d36' for
service principal objectId '698138e7-d7b6-4738-a866-b4e3081a69e4'.
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

### <a name="verify-the-list-of-credentials-for-the-service-principal"></a><span data-ttu-id="b8cdb-162">Überprüfen der Liste mit Anmeldeinformationen für den Dienstprinzipal</span><span class="sxs-lookup"><span data-stu-id="b8cdb-162">Verify the list of credentials for the service principal</span></span>

```azurepowershell-interactive
Get-AzADSpCredential -ServicePrincipalName http://MyDemoWebApp
```

```output
StartDate           EndDate             KeyId                                Type
---------           -------             -----                                ----
3/8/2017 5:58:24 PM 3/8/2018 5:58:24 PM 6f801c3e-6fcd-42b9-be8e-320b17ba1d36 Password
```

### <a name="get-information-about-the-service-principal"></a><span data-ttu-id="b8cdb-163">Abrufen von Informationen zum Dienstprinzipal</span><span class="sxs-lookup"><span data-stu-id="b8cdb-163">Get information about the service principal</span></span>

```azurepowershell-interactive
$svcprincipal = Get-AzADServicePrincipal -ObjectId 698138e7-d7b6-4738-a866-b4e3081a69e4
$svcprincipal | Select-Object *
```

```output
ServicePrincipalNames : {http://MyDemoWebApp, 00c01aaa-1603-49fc-b6df-b78c4e5138b4}
ApplicationId         : 00c01aaa-1603-49fc-b6df-b78c4e5138b4
DisplayName           : MyDemoWebApp
Id                    : 698138e7-d7b6-4738-a866-b4e3081a69e4
Type                  : ServicePrincipal
```
