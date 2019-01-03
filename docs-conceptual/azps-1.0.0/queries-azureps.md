---
title: Abfragen der Ausgabe von Azure PowerShell-Cmdlets
description: Hier erfahren Sie, wie Sie in Azure Ressourcenabfragen ausführen und die Ergebnisse formatieren.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: fd0135f981452a2425f4dc8b9c9708d4907eff2a
ms.sourcegitcommit: 797c18f93aaa495ef005993b2e202d7378588dfa
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/19/2018
ms.locfileid: "53594789"
---
# <a name="query-output-of-azure-powershell-cmdlets"></a><span data-ttu-id="5efab-103">Abfragen der Ausgabe von Azure PowerShell-Cmdlets</span><span class="sxs-lookup"><span data-stu-id="5efab-103">Query output of Azure PowerShell cmdlets</span></span>

<span data-ttu-id="5efab-104">Abfragen können in PowerShell mithilfe integrierter Cmdlets ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="5efab-104">Querying in PowerShell can be completed by using built-in cmdlets.</span></span> <span data-ttu-id="5efab-105">Cmdlet-Namen haben in PowerShell das Format **_Verb-Nomen_**.</span><span class="sxs-lookup"><span data-stu-id="5efab-105">In PowerShell, cmdlet names take the form of **_Verb-Noun_**.</span></span> <span data-ttu-id="5efab-106">Die Abfrage-Cmdlets sind am Verb **_Get_** zu erkennen.</span><span class="sxs-lookup"><span data-stu-id="5efab-106">The cmdlets using the verb **_Get_** are the query cmdlets.</span></span> <span data-ttu-id="5efab-107">Bei den Cmdlet-Nomen handelt es sich um die Arten von Azure-Ressourcen, für die eine dem Cmdlet-Verb entsprechende Aktion ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="5efab-107">The cmdlet nouns are the types of Azure resources that are acted upon by the cmdlet verbs.</span></span>

## <a name="select-simple-properties"></a><span data-ttu-id="5efab-108">Auswählen einfacher Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5efab-108">Select simple properties</span></span>

<span data-ttu-id="5efab-109">In Azure PowerShell ist für jedes Cmdlet eine Standardformatierung definiert.</span><span class="sxs-lookup"><span data-stu-id="5efab-109">Azure PowerShell has default formatting defined for each cmdlet.</span></span> <span data-ttu-id="5efab-110">Die am häufigsten verwendeten Eigenschaften für die einzelnen Ressourcentypen werden automatisch in einer Tabelle oder Liste angezeigt.</span><span class="sxs-lookup"><span data-stu-id="5efab-110">The most common properties for each resource type are displayed in a table or list format automatically.</span></span> <span data-ttu-id="5efab-111">Weitere Informationen zum Formatieren der Ausgabe finden Sie unter [Formatieren von Abfrageergebnissen](formatting-output.md).</span><span class="sxs-lookup"><span data-stu-id="5efab-111">For more information about formatting output, see [Formatting query results](formatting-output.md).</span></span>

<span data-ttu-id="5efab-112">Fragen Sie mithilfe des Cmdlets `Get-AzVM` eine Liste mit virtuellen Computern in Ihrem Konto ab.</span><span class="sxs-lookup"><span data-stu-id="5efab-112">Use the `Get-AzVM` cmdlet to query for a list of VMs in your account.</span></span>

```azurepowershell-interactive
Get-AzVM
```

<span data-ttu-id="5efab-113">Die Standardausgabe wird automatisch als Tabelle formatiert.</span><span class="sxs-lookup"><span data-stu-id="5efab-113">The default output is automatically formatted as a table.</span></span>

```output
ResourceGroupName          Name   Location          VmSize  OsType              NIC ProvisioningState
-----------------          ----   --------          ------  ------              --- -----------------
MYWESTEURG        MyUnbuntu1610 westeurope Standard_DS1_v2   Linux myunbuntu1610980         Succeeded
MYWESTEURG          MyWin2016VM westeurope Standard_DS1_v2 Windows   mywin2016vm880         Succeeded
```

<span data-ttu-id="5efab-114">Mit dem Cmdlet `Select-Object` können Sie spezifische Eigenschaften auswählen, die für Sie von Interesse sind.</span><span class="sxs-lookup"><span data-stu-id="5efab-114">The `Select-Object` cmdlet can be used to select the specific properties that are interesting to you.</span></span>

```azurepowershell-interactive
Get-AzVM | Select Name,ResourceGroupName,Location
```

```output
Name          ResourceGroupName Location
----          ----------------- --------
MyUnbuntu1610 MYWESTEURG        westeurope
MyWin2016VM   MYWESTEURG        westeurope
```

## <a name="select-complex-nested-properties"></a><span data-ttu-id="5efab-115">Auswählen komplexer geschachtelter Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5efab-115">Select complex nested properties</span></span>

<span data-ttu-id="5efab-116">Wenn die gewünschte Eigenschaft in der JSON-Ausgabe verschachtelt ist, müssen Sie den vollständigen Pfad zur Eigenschaft angeben.</span><span class="sxs-lookup"><span data-stu-id="5efab-116">If the property you want is nested in the JSON output, you need to supply the full path to the property.</span></span> <span data-ttu-id="5efab-117">Das folgende Beispiel zeigt, wie Sie den VM-Namen und den Betriebssystemtyp auf der Grundlage des Cmdlets `Get-AzVM` auswählen.</span><span class="sxs-lookup"><span data-stu-id="5efab-117">The following example shows how to select the VM Name and the OS type from the `Get-AzVM` cmdlet.</span></span>

```azurepowershell-interactive
Get-AzVM | Select Name,@{Name='OSType'; Expression={$_.StorageProfile.OSDisk.OSType}}
```

```output
Name           OSType
----           ------
MyUnbuntu1610   Linux
MyWin2016VM   Windows
```

## <a name="filter-results-with-the-where-object-cmdlet"></a><span data-ttu-id="5efab-118">Filtern von Ergebnissen mithilfe des Cmdlets „Where-Object“</span><span class="sxs-lookup"><span data-stu-id="5efab-118">Filter results with the Where-Object cmdlet</span></span>

<span data-ttu-id="5efab-119">Mit dem Cmdlet `Where-Object` können Sie das Ergebnis auf der Grundlage eines beliebigen Eigenschaftswerts filtern.</span><span class="sxs-lookup"><span data-stu-id="5efab-119">The `Where-Object` cmdlet allows you to filter the result based on any property value.</span></span> <span data-ttu-id="5efab-120">Im folgenden Beispiel wählt der Filter nur virtuelle Computer aus, deren Name „RGD“ enthält.</span><span class="sxs-lookup"><span data-stu-id="5efab-120">In the following example, the filter selects only VMs that have the text "RGD" in their name.</span></span>

```azurepowershell-interactive
Get-AzVM | Where ResourceGroupName -like RGD* | Select ResourceGroupName,Name
```

```output
ResourceGroupName  Name
-----------------  ----
RGDEMO001          KBDemo001VM
RGDEMO001          KBDemo020
```

<span data-ttu-id="5efab-121">Im nächsten Beispiel werden die virtuellen Computer zurückgegeben, bei denen „vmSize“ den Wert „Standard_DS1_V2“ besitzt.</span><span class="sxs-lookup"><span data-stu-id="5efab-121">With the next example, the results will return the VMs that have the vmSize 'Standard_DS1_V2'.</span></span>

```azurepowershell-interactive
Get-AzVM | Where vmSize -eq Standard_DS1_V2
```

```output
ResourceGroupName          Name     Location          VmSize  OsType              NIC ProvisioningState
-----------------          ----     --------          ------  ------              --- -----------------
MYWESTEURG        MyUnbuntu1610   westeurope Standard_DS1_v2   Linux myunbuntu1610980         Succeeded
MYWESTEURG          MyWin2016VM   westeurope Standard_DS1_v2 Windows   mywin2016vm880         Succeeded
```