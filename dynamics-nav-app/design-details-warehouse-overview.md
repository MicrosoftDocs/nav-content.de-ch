---
title: "Designdetails – Lagerübersicht"
description: "Um die physische Bewegung der Artikel auf dieser Zonen- und Lagerplatzebene zu unterstützen, müssen alle Informationen für jede Transaktion oder Umlagerung im Lager nachverfolgt werden. Dies wird in der Tabelle **Lagerplatzposten** verwaltet. Jede Transaktion wird in einem Lagerplatzjournal gespeichert."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 6e93b63fe6faefc601444a4179833818f384e364
ms.contentlocale: de-ch
ms.lasthandoff: 12/01/2017

---
# <a name="design-details-warehouse-overview"></a><span data-ttu-id="c75d0-105">Designdetails: Lagerübersicht</span><span class="sxs-lookup"><span data-stu-id="c75d0-105">Design Details: Warehouse Overview</span></span>
<span data-ttu-id="c75d0-106">Um die physische Bewegung der Artikel auf dieser Zonen- und Lagerplatzebene zu unterstützen, müssen alle Informationen für jede Transaktion oder Umlagerung im Lager nachverfolgt werden.</span><span class="sxs-lookup"><span data-stu-id="c75d0-106">To support the physical handling of items on the zone and bin level, all information must be traced for each transaction or movement in the warehouse.</span></span> <span data-ttu-id="c75d0-107">Dies wird in der Tabelle **Lagerplatzposten** verwaltet.</span><span class="sxs-lookup"><span data-stu-id="c75d0-107">This is managed in the **Warehouse Entry** table.</span></span> <span data-ttu-id="c75d0-108">Jede Transaktion wird in einem Lagerplatzjournal gespeichert.</span><span class="sxs-lookup"><span data-stu-id="c75d0-108">Each transaction is stored in a warehouse register.</span></span>  

<span data-ttu-id="c75d0-109">Logistikbelege und ein Logistik Erf.-Journal werden verwendet, um Artikelumlagerungen im Lager zu erfassen.</span><span class="sxs-lookup"><span data-stu-id="c75d0-109">Warehouse documents and a warehouse journal are used to register item movements in the warehouse.</span></span> <span data-ttu-id="c75d0-110">Immer wenn ein Artikel im Lager umgelagert, erhalten, eingelagert, kommissioniert, geliefert oder angepasst wird, werden Lagerposten registriert, um die physischen Informationen zu Zone, Lagerplatz und Menge zu speichern.</span><span class="sxs-lookup"><span data-stu-id="c75d0-110">Every time that an item in the warehouse is moved, received, put away, picked, shipped, or adjusted, warehouse entries are registered to store the physical information about zone, bin, and quantity.</span></span> <span data-ttu-id="c75d0-111">Weitere Informationen finden Sie unter [Designdetails: Eingehender Lagerfluss](design-details-outbound-warehouse-flow.md).</span><span class="sxs-lookup"><span data-stu-id="c75d0-111">For more information, see [Design Details: Inbound Warehouse Flow](design-details-outbound-warehouse-flow.md).</span></span>  

<span data-ttu-id="c75d0-112">Die Tabelle **Lagerplatzinhalt** wird verwendet, um alle verschiedenen Dimensionen des Inhalts eines Lagerplatzes pro Artikel zu bearbeiten, wie etwa Mengeneinheit, Höchstmenge oder Mindestmenge.</span><span class="sxs-lookup"><span data-stu-id="c75d0-112">The **Bin Content** table is used to handle all the different dimensions of the contents of a bin per item, such as unit of measure, maximum quantity, and minimum quantity.</span></span> <span data-ttu-id="c75d0-113">Die Tabelle **Lagerplatzinhalt** enthält auch Flussfelder zu den Lagerplatzposten, Lageranweisungen und Logistik-Buch.-Blattzeilen, wodurch sichergestellt wird, dass die Verfügbarkeit eines Artikels pro Lagerplatz und eines Lagerplatzes für einen Artikel schnell berechnet werden kann.</span><span class="sxs-lookup"><span data-stu-id="c75d0-113">The **Bin Content** table also contains flow fields to the warehouse entries, warehouse instructions, and warehouse journal lines, which ensures that the availability of an item per bin and a bin for an item can be calculated quickly.</span></span> <span data-ttu-id="c75d0-114">Weitere Informationen finden Sie unter [Designdetails: Verfügbarkeit im Lager](design-details-availability-in-the-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="c75d0-114">For more information, see [Design Details: Availability in the Warehouse](design-details-availability-in-the-warehouse.md).</span></span>  

<span data-ttu-id="c75d0-115">Wenn Artikelbuchungen außerhalb des Lagermoduls auftreten, wird ein Standard-Ausgleichslagerplatz pro Lagerort verwendet, um Lagerplatzposten mit Inventurposten zu synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="c75d0-115">When item postings occur outside the warehouse module, a default adjustment bin per location is used to synchronize warehouse entries with inventory entries.</span></span> <span data-ttu-id="c75d0-116">Während der Inventur des Lagers werden jegliche Abweichungen zwischen berechneten und gezählten Mengen am Regulierungslagerplatz erfasst und dann als korrigierende Lagerposten gebucht.</span><span class="sxs-lookup"><span data-stu-id="c75d0-116">During physical inventory of the warehouse, any differences between the calculated and counted quantities are recorded in the adjustment bin and then posted as correcting item ledger entries.</span></span> <span data-ttu-id="c75d0-117">Weitere Informationen finden Sie unter [Designdetails: Bestandintegration](design-details-integration-with-inventory.md).</span><span class="sxs-lookup"><span data-stu-id="c75d0-117">For more information, see [Design Details: Integration with Inventory](design-details-integration-with-inventory.md).</span></span>  

<span data-ttu-id="c75d0-118">Die folgenden Abbildung zeigt typische Warenflüsse.</span><span class="sxs-lookup"><span data-stu-id="c75d0-118">The following illustration outlines typical warehouse flows.</span></span>  

<span data-ttu-id="c75d0-119">![Übersicht Lagerprozesse](media/design_details_warehouse_management_overview.png "design_details_warehouse_management_overview")</span><span class="sxs-lookup"><span data-stu-id="c75d0-119">![Overview of warehouse processes](media/design_details_warehouse_management_overview.png "design_details_warehouse_management_overview")</span></span>  

## <a name="basic-or-advanced-warehousing"></a><span data-ttu-id="c75d0-120">Grundlegende oder erweiterte Lagerhaltung</span><span class="sxs-lookup"><span data-stu-id="c75d0-120">Basic or Advanced Warehousing</span></span>  
<span data-ttu-id="c75d0-121">Lagerfunktionen in [!INCLUDE[d365fin](includes/d365fin_md.md)] können in unterschiedlichen Komplexitätsebenen implementiert werden, abhängig von den Prozessen eines Unternehmens und dem Auftragsvolumen.</span><span class="sxs-lookup"><span data-stu-id="c75d0-121">Warehouse functionality in [!INCLUDE[d365fin](includes/d365fin_md.md)] can be implemented in different complexity levels, depending on a company’s processes and order volume.</span></span> <span data-ttu-id="c75d0-122">Der wichtigste Unterschied besteht darin, dass Aktivitäten in der einfachen Logistik Auftrag für Auftrag durchgeführt werden, während sie in der erweiterten Logistik für mehrere Aufträge konsolidiert werden.</span><span class="sxs-lookup"><span data-stu-id="c75d0-122">The main difference is that activities are performed order-by-order in basic warehousing when they are consolidated for multiple orders in advanced warehousing.</span></span>  

 <span data-ttu-id="c75d0-123">Um zwischen den verschiedenen Komplexitätsebenen zu unterscheiden, verwendet diese Dokumentation zwei allgemeine Bezeichnungen, grundlegende und erweiterte Lagerhaltung.</span><span class="sxs-lookup"><span data-stu-id="c75d0-123">To differentiate between the different complexity levels, this documentation refers to two general denominations, Basic and Advanced Warehousing.</span></span> <span data-ttu-id="c75d0-124">Diese einfache Unterscheidung umfasst mehrere verschiedene Komplexitätsebenen, die durch definierte Produktdetails und Lagerorteinrichtung definiert sind, wobei jede durch unterschiedliche UI-Dokumente unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="c75d0-124">This simple differentiation covers several different complexity levels as defined by product granules and location setup, each supported by different UI documents.</span></span> <span data-ttu-id="c75d0-125">Weitere Informationen finden Sie unter [Designdetails: Lagerhaus einrichten](design-details-warehouse-setup.md).</span><span class="sxs-lookup"><span data-stu-id="c75d0-125">For more information, see [Design Details: Warehouse Setup](design-details-warehouse-setup.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="c75d0-126">Die höchstentwickelte Ebene der Logistik wird in dieser Dokumentation als „WMS-Installationen“ bezeichnet, da diese Methode die höchstentwickelten Elemente und Logistiksysteme erfordert.</span><span class="sxs-lookup"><span data-stu-id="c75d0-126">The most advanced level of warehousing is referred to as “WMS installations” in this documentation, since this level requires the most advanced granule, Warehouse Management Systems.</span></span>  

 <span data-ttu-id="c75d0-127">Die folgenden verschiedenen UI-Dokumente werden in der einfachen und der erweiterten Logistik verwendet.</span><span class="sxs-lookup"><span data-stu-id="c75d0-127">The following different UI documents are used in basic and advanced warehousing.</span></span>  

## <a name="basic-ui-documents"></a><span data-ttu-id="c75d0-128">Grundlegende UI-Dokumente</span><span class="sxs-lookup"><span data-stu-id="c75d0-128">Basic UI Documents</span></span>  

-   <span data-ttu-id="c75d0-129">**Lagereinlagerung**</span><span class="sxs-lookup"><span data-stu-id="c75d0-129">**Inventory Put-away**</span></span>  
-   <span data-ttu-id="c75d0-130">**Lagerkommissionierung**</span><span class="sxs-lookup"><span data-stu-id="c75d0-130">**Inventory Pick**</span></span>  
-   <span data-ttu-id="c75d0-131">**Lagerbestandsumlagerung**</span><span class="sxs-lookup"><span data-stu-id="c75d0-131">**Inventory Movement**</span></span>  
-   <span data-ttu-id="c75d0-132">**Artikel Erf.-Journal**</span><span class="sxs-lookup"><span data-stu-id="c75d0-132">**Item Journal**</span></span>  
-   <span data-ttu-id="c75d0-133">**Artikel Umlag. Erf.-Journal**</span><span class="sxs-lookup"><span data-stu-id="c75d0-133">**Item Reclassification Journal**</span></span>  
-   <span data-ttu-id="c75d0-134">(Verschiedene Berichte)</span><span class="sxs-lookup"><span data-stu-id="c75d0-134">(Various reports)</span></span>  

## <a name="advanced-ui-documents"></a><span data-ttu-id="c75d0-135">Erweiterte UI-Dokumente</span><span class="sxs-lookup"><span data-stu-id="c75d0-135">Advanced UI Documents</span></span>  

-   <span data-ttu-id="c75d0-136">**Wareneingang**</span><span class="sxs-lookup"><span data-stu-id="c75d0-136">**Warehouse Receipt**</span></span>  
-   <span data-ttu-id="c75d0-137">**Einlagerungsvorschlag**</span><span class="sxs-lookup"><span data-stu-id="c75d0-137">**Put-away Worksheet**</span></span>  
-   <span data-ttu-id="c75d0-138">**Einlagerung**</span><span class="sxs-lookup"><span data-stu-id="c75d0-138">**Warehouse Put-away**</span></span>  
-   <span data-ttu-id="c75d0-139">**Kommissioniervorschlag**</span><span class="sxs-lookup"><span data-stu-id="c75d0-139">**Pick Worksheet**</span></span>  
-   <span data-ttu-id="c75d0-140">**Kommissionierung**</span><span class="sxs-lookup"><span data-stu-id="c75d0-140">**Warehouse Pick**</span></span>  
-   <span data-ttu-id="c75d0-141">**Lagerplatzumlagerungsvorschlag**</span><span class="sxs-lookup"><span data-stu-id="c75d0-141">**Movement Worksheet**</span></span>  
-   <span data-ttu-id="c75d0-142">**Lagerplatzumlagerung**</span><span class="sxs-lookup"><span data-stu-id="c75d0-142">**Warehouse Movement**</span></span>  
-   <span data-ttu-id="c75d0-143">**Interne Kommissionierung**</span><span class="sxs-lookup"><span data-stu-id="c75d0-143">**Internal Whse. Pick**</span></span>  
-   <span data-ttu-id="c75d0-144">**Interne Einlag.-Anforderung**</span><span class="sxs-lookup"><span data-stu-id="c75d0-144">**Internal Whse. Put-away**</span></span>  
-   <span data-ttu-id="c75d0-145">**Lagerplatz Erst.-Vorschlag**</span><span class="sxs-lookup"><span data-stu-id="c75d0-145">**Bin Creation Worksheet**</span></span>  
-   <span data-ttu-id="c75d0-146">**Lagerplatzinh. Erst.-Vorschlag**</span><span class="sxs-lookup"><span data-stu-id="c75d0-146">**Bin Content Creation Worksheet**</span></span>  
-   <span data-ttu-id="c75d0-147">**Logistik Artikel Erf.-Journal**</span><span class="sxs-lookup"><span data-stu-id="c75d0-147">**Whse. Item Journal**</span></span>  
-   <span data-ttu-id="c75d0-148">**Umlagerung Logistik Artikel Erf.-Journal**</span><span class="sxs-lookup"><span data-stu-id="c75d0-148">**Whse. Item Reclass. Journal**</span></span>  
-   <span data-ttu-id="c75d0-149">(Verschiedene Berichte)</span><span class="sxs-lookup"><span data-stu-id="c75d0-149">(Various reports)</span></span>  

<span data-ttu-id="c75d0-150">Weitere Informationen über jeden Beleg finden Sie den entsprechenden Fensterthemen.</span><span class="sxs-lookup"><span data-stu-id="c75d0-150">For more information about each document, see the respective window topics.</span></span>  

### <a name="terminology"></a><span data-ttu-id="c75d0-151">Terminologie</span><span class="sxs-lookup"><span data-stu-id="c75d0-151">Terminology</span></span>  
<span data-ttu-id="c75d0-152">Um mit den Finanzbegriffen Einkauf und von Verkauf zu entsprechen, verwendet [!INCLUDE[d365fin](includes/d365fin_md.md)] Lagerdokumentation die folgenden Begriffe für Warenfluss im Lager.</span><span class="sxs-lookup"><span data-stu-id="c75d0-152">To align with the financial concepts of purchases and sales, [!INCLUDE[d365fin](includes/d365fin_md.md)] warehouse documentation refers to the following terms for item flow in the warehouse.</span></span>  

|<span data-ttu-id="c75d0-153">Begriff</span><span class="sxs-lookup"><span data-stu-id="c75d0-153">Term</span></span>|<span data-ttu-id="c75d0-154">Description</span><span class="sxs-lookup"><span data-stu-id="c75d0-154">Description</span></span>|  
|----------|---------------------------------------|  
|<span data-ttu-id="c75d0-155">Eingehender Fluss</span><span class="sxs-lookup"><span data-stu-id="c75d0-155">Inbound flow</span></span>|<span data-ttu-id="c75d0-156">Artikel, die in den Lagerort eingehen, z.B. Einkäufe und eingehende Umlagerungen.</span><span class="sxs-lookup"><span data-stu-id="c75d0-156">Items moving into the warehouse location, such as purchases and inbound transfers.</span></span>|  
|<span data-ttu-id="c75d0-157">Interne Flüsse</span><span class="sxs-lookup"><span data-stu-id="c75d0-157">Internal flow</span></span>|<span data-ttu-id="c75d0-158">Artikel, die innerhalb des Lagerorts verschoben werden, wie z.B. Produktionskomponenten und fertiggestellte Artikel.</span><span class="sxs-lookup"><span data-stu-id="c75d0-158">Items moving inside the warehouse location, such as production components and output.</span></span>|  
|<span data-ttu-id="c75d0-159">Ausgehender Warenfluss</span><span class="sxs-lookup"><span data-stu-id="c75d0-159">Outbound flow</span></span>|<span data-ttu-id="c75d0-160">Artikel, die aus dem Lagerort ausgehen, z.B. Verkäufe und ausgehende Umlagerungen.</span><span class="sxs-lookup"><span data-stu-id="c75d0-160">Items moving out of the warehouse location, such as sales and outbound transfers.</span></span>|  

## <a name="see-also"></a><span data-ttu-id="c75d0-161">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="c75d0-161">See Also</span></span>  
 [<span data-ttu-id="c75d0-162">Designdetails: Logistik</span><span class="sxs-lookup"><span data-stu-id="c75d0-162">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)
