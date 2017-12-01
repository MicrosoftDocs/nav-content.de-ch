---
title: Definieren der Beziehung zwischen Kostenarten und Sachkonten
description: Lernen, wie die beiden Felder definiert werden, die die Beziehung zwischen Kostenart und Fibukonto festlegen
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost types, general ledger
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: fcaeab6a164abf20011beec35ec004057098b360
ms.contentlocale: de-ch
ms.lasthandoff: 12/01/2017

---
# <a name="defining-the-relationship-between-cost-types-and-general-ledger-accounts"></a><span data-ttu-id="cd7e4-103">Definieren der Beziehung zwischen Kostenarten und Sachkonten</span><span class="sxs-lookup"><span data-stu-id="cd7e4-103">Defining the Relationship Between Cost Types and General Ledger Accounts</span></span>
<span data-ttu-id="cd7e4-104">Das Verbindung zwischen der Kostenart und dem Fibukonto wird in der Kostenart und im Fibukonto erstellt.</span><span class="sxs-lookup"><span data-stu-id="cd7e4-104">The relationship between the cost type and the general ledger account is created in the cost type and in the general ledger account.</span></span>  

* <span data-ttu-id="cd7e4-105">Das Feld **Fibukontenbereich** in der Tabelle **Kostenart** bestimmt, welche Fibukonten zu einer Kostenart gehören.</span><span class="sxs-lookup"><span data-stu-id="cd7e4-105">The **G/L Account Range** field in the **Cost Type** table establishes which general ledger accounts belong to a cost type.</span></span>  
* <span data-ttu-id="cd7e4-106">Das **Kostenartennummer**</span><span class="sxs-lookup"><span data-stu-id="cd7e4-106">The **Cost Type No.**</span></span> <span data-ttu-id="cd7e4-107">Feld im Kontenplan bestimmt, zu welcher Kostenart ein Fibukonto gehört.</span><span class="sxs-lookup"><span data-stu-id="cd7e4-107">field in the chart of accounts establishes which cost type a general ledger account belongs to.</span></span>  

<span data-ttu-id="cd7e4-108">Diese beiden Felder werden automatisch ausgefüllt, wenn Sie die **Kostenarten aus Kontenplan abrufen**-Funktion verwenden.</span><span class="sxs-lookup"><span data-stu-id="cd7e4-108">These two fields are filled automatically when you use the **Get Cost Types from Chart of Accounts** function.</span></span>  

## <a name="relationship-between-general-ledger-accounts-and-cost-types"></a><span data-ttu-id="cd7e4-109">Beziehung zwischen Fibukonten und Kostenarten</span><span class="sxs-lookup"><span data-stu-id="cd7e4-109">Relationship Between General Ledger Accounts and Cost Types</span></span>  
<span data-ttu-id="cd7e4-110">Zwischen Fibukonten und Kostenarten besteht eine n:1-Beziehung.</span><span class="sxs-lookup"><span data-stu-id="cd7e4-110">There is an n:1 relationship between general ledger accounts and cost types.</span></span> <span data-ttu-id="cd7e4-111">Mehrere Fibukonten können zu einer Kostenart gehören, aber jedes Fibukonto gehört nur zu einer Kostenart.</span><span class="sxs-lookup"><span data-stu-id="cd7e4-111">Several general ledger accounts can belong to one cost type, but each general ledger account belongs to only one cost type.</span></span> <span data-ttu-id="cd7e4-112">In der folgenden Tabelle werden die Details der Beziehung beschrieben.</span><span class="sxs-lookup"><span data-stu-id="cd7e4-112">The following table describes the details in the relationship.</span></span>  

|<span data-ttu-id="cd7e4-113">Verbindungen</span><span class="sxs-lookup"><span data-stu-id="cd7e4-113">Relationship</span></span>|<span data-ttu-id="cd7e4-114">**Fibukontobereich**</span><span class="sxs-lookup"><span data-stu-id="cd7e4-114">**G/L Account Range**</span></span>|<span data-ttu-id="cd7e4-115">**Kostenartnr.**</span><span class="sxs-lookup"><span data-stu-id="cd7e4-115">**Cost Type No.**</span></span>|  
|------------------|------------------------------------------------|-------------------------------------------|  
|<span data-ttu-id="cd7e4-116">Ein Fibukonto für jede Kostenart</span><span class="sxs-lookup"><span data-stu-id="cd7e4-116">One general ledger account for each cost type</span></span>|<span data-ttu-id="cd7e4-117">Ein Fibukonto</span><span class="sxs-lookup"><span data-stu-id="cd7e4-117">One general ledger account</span></span>|<span data-ttu-id="cd7e4-118">Eine Kostenart</span><span class="sxs-lookup"><span data-stu-id="cd7e4-118">One cost type</span></span>|  
|<span data-ttu-id="cd7e4-119">Mehrere Fibukonten für eine Kostenart</span><span class="sxs-lookup"><span data-stu-id="cd7e4-119">Several general ledger accounts for one cost type</span></span>|<span data-ttu-id="cd7e4-120">Fibukontobereich, z. B. 7110 ... 7193 für jedes Fibukonto</span><span class="sxs-lookup"><span data-stu-id="cd7e4-120">General ledger account range, for example, 7110..7193 for each general ledger account</span></span>|<span data-ttu-id="cd7e4-121">Für jedes Fibukonto im Bereich gibt es nur eine Kostenart</span><span class="sxs-lookup"><span data-stu-id="cd7e4-121">For each general ledger account in the range, there is only one cost type</span></span>|  
|<span data-ttu-id="cd7e4-122">Kostenarten ohne entsprechende Fibukonten</span><span class="sxs-lookup"><span data-stu-id="cd7e4-122">Cost types without corresponding general ledger accounts</span></span>|<Empty>||  
|<span data-ttu-id="cd7e4-123">Fibukonten, deren Posten nicht übertragen werden</span><span class="sxs-lookup"><span data-stu-id="cd7e4-123">General ledger accounts whose entries will not be transferred</span></span>||<Empty>|  

## <a name="cost-types-without-a-relationship-to-the-general-ledger"></a><span data-ttu-id="cd7e4-124">Kostenarten ohne Beziehung zum Fibukonto</span><span class="sxs-lookup"><span data-stu-id="cd7e4-124">Cost Types Without a Relationship to the General Ledger</span></span>  
<span data-ttu-id="cd7e4-125">Eine Kostenart hat möglicherweise keine Beziehung zu Fibukonten, wenn eine der folgenden Bedingungen zutrifft:</span><span class="sxs-lookup"><span data-stu-id="cd7e4-125">A cost type may not have a relationship to general ledger accounts if one of the following conditions is true:</span></span>  

* <span data-ttu-id="cd7e4-126">Konten für die betriebliche Buchhaltung, wie Berech. Zinsen und Abschreibungen, entnehmen nur Kosten aus der betrieblichen Buchhaltung.</span><span class="sxs-lookup"><span data-stu-id="cd7e4-126">Accounts for operational accounting, such as Calc. Interest and Depreciation, only take costs from the operational accounting.</span></span>  
* <span data-ttu-id="cd7e4-127">Helfende Kostenarten, wie Kostenarten 9901, 9902 und 9903 in der [!INCLUDE[d365fin](includes/d365fin_md.md)]-Datenbank, werden als Haben- und Sollbeträge für Zuordnungen verwendet.</span><span class="sxs-lookup"><span data-stu-id="cd7e4-127">Helping cost types, such as cost types 9901, 9902, and 9903 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, are used as credit and debit accounts for allocations.</span></span>  
* <span data-ttu-id="cd7e4-128">Das helfende Konto, 9920 in der [!INCLUDE[d365fin](includes/d365fin_md.md)]-Datenbank, enthält tatsächliche Zugänge, die die Differenz zwischen Kosten und Ausgaben des Fibukontos anzeigen.</span><span class="sxs-lookup"><span data-stu-id="cd7e4-128">The helping account, 9920 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, contains actual accruals that show the difference between costs and the expense from the general ledger.</span></span>  

## <a name="see-also"></a><span data-ttu-id="cd7e4-129">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="cd7e4-129">See Also</span></span>  
[<span data-ttu-id="cd7e4-130">Kostenrechnung</span><span class="sxs-lookup"><span data-stu-id="cd7e4-130">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="cd7e4-131">[Einrichten der Kostenrechnung](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="cd7e4-131">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
[<span data-ttu-id="cd7e4-132">Informationen zur Kostenrechnung</span><span class="sxs-lookup"><span data-stu-id="cd7e4-132">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
<span data-ttu-id="cd7e4-133">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="cd7e4-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

