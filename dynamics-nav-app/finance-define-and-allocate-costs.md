---
title: Definieren und Zuweisen von Kosten
description: "Kostenumlagen verschieben Kosten und Einnahmen zwischen Kostenarten, Kostenstellen und Kostenträgern. Sie können so viele Zuteilungen wie notwendig definieren."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: b42f7e0c832bccabb29f62e4589ba3e178778e5f
ms.contentlocale: de-ch
ms.lasthandoff: 12/01/2017

---
# <a name="defining-and-allocating-costs"></a><span data-ttu-id="9e1c5-104">Definieren und Zuweisen von Kosten</span><span class="sxs-lookup"><span data-stu-id="9e1c5-104">Defining and Allocating Costs</span></span>
<span data-ttu-id="9e1c5-105">Kostenumlagen verschieben Kosten und Einnahmen zwischen Kostenarten, Kostenstellen und Kostenträgern.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-105">Cost allocations move costs and revenues between cost types, cost centers, and cost objects.</span></span> <span data-ttu-id="9e1c5-106">Sie können so viele Zuteilungen wie notwendig definieren.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-106">You can define as many allocations as you need.</span></span> <span data-ttu-id="9e1c5-107">Jede Zuteilung besteht aus:</span><span class="sxs-lookup"><span data-stu-id="9e1c5-107">Each allocation consists of:</span></span>  

-   <span data-ttu-id="9e1c5-108">Eine Verteilungsquelle.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-108">An allocation source.</span></span>  
-   <span data-ttu-id="9e1c5-109">Mindestens einem Zuteilungsziel.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-109">One or more allocation targets.</span></span>  

<span data-ttu-id="9e1c5-110">Die Zuteilungsquelle gibt an, welche Kosten zugeordnet werden müssen, und die Zuteilungsziele bestimmen, wo die Kosten zugeordnet werden müssen.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-110">The allocation source establishes which costs must be allocated, and the allocation targets determine where the costs must be allocated.</span></span> <span data-ttu-id="9e1c5-111">Beispielsweise kann eine Zuteilungsquelle die Kosten für die Kostenart "Strom und Heizung" sein.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-111">For example, an allocation source can be the costs for the Electricity and Heating cost type.</span></span> <span data-ttu-id="9e1c5-112">Sie ordnen alle Strom- und Heizkosten drei Kostenstellen zu: Werkstatt, Produktion und Verkauf.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-112">You allocate all electricity and heating costs to three cost centers: Workshop, Production, and Sales.</span></span> <span data-ttu-id="9e1c5-113">Diese Kostenstellen sind Ihre Zuteilungsziele.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-113">These cost centers are your allocation targets.</span></span>  

<span data-ttu-id="9e1c5-114">Für jede Zuteilungsquelle legen Sie eine Zuteilungsebene, eine Gültigkeitsdauer und eine Variante als Gruppen-ID fest.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-114">For each allocation source, you define an allocation level, a validity period, and a variant as grouping identifier.</span></span> <span data-ttu-id="9e1c5-115">Sie können einen Batchauftrag verwenden, um Filter festzulegen und Zuteilungsdefinitionen auszuwählen und dann automatisch Kostenumlagen auszuführen.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-115">You can use a batch job to set filters to select allocation definitions and then run cost allocations automatically.</span></span>  

<span data-ttu-id="9e1c5-116">Für jedes Zuteilungsziel definieren Sie eine Zuteilungsgrundlage.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-116">For each allocation target, you define an allocation base.</span></span> <span data-ttu-id="9e1c5-117">Die Zuteilungsgrundlage kann entweder statisch oder dynamisch sein.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-117">The allocation base can be either static or dynamic.</span></span>  

-   <span data-ttu-id="9e1c5-118">Die statische Zuteilungsgrundlagen basieren auf einem definierten Wert, zum Beispiel Quadratmeter oder ein eingerichtetes Verteilungsverhältnis, wie 5:2:4.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-118">Static allocation bases are based on a definite value, such as square footage or an established allocation ratio, such as 5:2:4.</span></span>  
-   <span data-ttu-id="9e1c5-119">Die dynamische Zuteilung basiert auf veränderbaren Werten, wie z. B. die Anzahl der Mitarbeiter in einer Kostenstelle oder die Verkaufseinnahmen eines Kostenträgers in einem bestimmten Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-119">Dynamic allocation bases depend on changeable values, such as the number of employees in a cost center or sales revenue of a cost object throughout a certain time period.</span></span>  

<span data-ttu-id="9e1c5-120">In der folgenden Tabelle wird eine Reihe von Aufgaben mit Verknüpfungen zu den beschriebenen Themen erläutert.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-120">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="9e1c5-121">An</span><span class="sxs-lookup"><span data-stu-id="9e1c5-121">To</span></span>|<span data-ttu-id="9e1c5-122">Informationen</span><span class="sxs-lookup"><span data-stu-id="9e1c5-122">See</span></span>|  
|--------|---------|  
|<span data-ttu-id="9e1c5-123">Richten Sie die Zuteilungsquelle und ihre Ziele ein.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-123">Set up allocation source and its targets.</span></span>|[<span data-ttu-id="9e1c5-124">Vorgehensweise: Einrichten von Zuteilungsquellen und -zielen</span><span class="sxs-lookup"><span data-stu-id="9e1c5-124">How to: Set Up Allocation Source and Targets</span></span>](finance-how-to-set-up-allocation-source-and-targets.md)|  
|<span data-ttu-id="9e1c5-125">Richten Sie verschiedene Filter für dynamische Zuteilungsgrundlagen ein.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-125">Set up various filters for dynamic allocation bases.</span></span>|[<span data-ttu-id="9e1c5-126">Setzen von Filtern für dynamische Zuteilungsgrundlagen</span><span class="sxs-lookup"><span data-stu-id="9e1c5-126">Setting Filters for Dynamic Allocation Bases</span></span>](finance-setting-filters-for-dynamic-allocation-bases.md)|  
|<span data-ttu-id="9e1c5-127">Sehen Sie sich ein Beispiel für das Definieren einer statischen Umlage an.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-127">See an example of how to define a static allocation.</span></span>|[<span data-ttu-id="9e1c5-128">Szenario-Beispiel: Definieren von statischen Umlagen basierend auf dem Verteilungsverhältnis</span><span class="sxs-lookup"><span data-stu-id="9e1c5-128">Scenario Example: Defining Static Allocations Based on Allocation Ratio</span></span>](finance-scenario-example-defining-static-allocations-based-on-allocation-ratio.md)|  
|<span data-ttu-id="9e1c5-129">Sehen Sie sich ein Beispiel für das Definieren einer dynamischen Zuteilung an.</span><span class="sxs-lookup"><span data-stu-id="9e1c5-129">See an example of how to define a dynamic allocation.</span></span>|[<span data-ttu-id="9e1c5-130">Szenario-Beispiel: Definieren von dynamischen Zuteilungen auf der Basis der verkauften Artikel</span><span class="sxs-lookup"><span data-stu-id="9e1c5-130">Scenario Example: Defining Dynamic Allocations Based on Items Sold</span></span>](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md)|  

## <a name="see-also"></a><span data-ttu-id="9e1c5-131">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="9e1c5-131">See Also</span></span>  
 <span data-ttu-id="9e1c5-132">[Einrichten der Kostenrechnung](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="9e1c5-132">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
 <span data-ttu-id="9e1c5-133">[Übertragung und Buchung von Kostenzuteilungen](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="9e1c5-133">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
 <span data-ttu-id="9e1c5-134">[Kostenrechnung](finance-manage-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="9e1c5-134">[Accounting for Costs](finance-manage-cost-accounting.md) </span></span>  
 <span data-ttu-id="9e1c5-135">[Terminologie der Kostenrechnung](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="9e1c5-135">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
 [<span data-ttu-id="9e1c5-136">Informationen zur Kostenrechnung</span><span class="sxs-lookup"><span data-stu-id="9e1c5-136">About Cost Accounting</span></span>](finance-about-cost-accounting.md)
