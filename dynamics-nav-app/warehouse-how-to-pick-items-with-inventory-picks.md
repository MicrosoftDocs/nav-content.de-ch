---
title: 'So wird''s gemacht: Artikel mit der Lagerkommissionierung kommissionieren'
description: "Wenn ein Lagerort so eingerichtet wurde, dass Kommissionierung erforderlich ist, jedoch Warenausgang nicht erforderlich ist, verwenden Sie Lagerkommissionierbelege, um Kommissionier- und Warenausgangsinformationen für Ihre Herkunftsbelege zu erfassen und zu buchen."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 3bb2df6d727b52b3fc579cbcc3bd13539b75e6b1
ms.contentlocale: de-ch
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-pick-items-with-inventory-picks"></a><span data-ttu-id="d4885-103">So wird's gemacht: Artikel mit der Lagerkommissionierung kommissionieren</span><span class="sxs-lookup"><span data-stu-id="d4885-103">How to: Pick Items with Inventory Picks</span></span>
<span data-ttu-id="d4885-104">Wenn Ihr Lagerort so eingerichtet wurde, dass Kommissionierung erforderlich ist, jedoch Warenausgang nicht erforderlich ist, verwenden Sie das Fenster **Lagerkommissionierung**, um Kommissionier- und Warenausgangsinformationen für Ihre Herkunftsbelege zu erfassen und zu buchen.</span><span class="sxs-lookup"><span data-stu-id="d4885-104">When your location is set up to require pick processing but not shipment processing, you use the **Inventory Pick** window to record and post picking and shipping information for your source documents.</span></span> <span data-ttu-id="d4885-105">Der ausgehende Herkunftsbeleg kann ein Verkaufsauftrag, eine Einkaufsreklamation, ein ausgehender Umlagerungsauftrag oder ein Fertigungsauftrag sein, dessen Komponenten zum Kommissionieren bereitstehen.</span><span class="sxs-lookup"><span data-stu-id="d4885-105">The outbound source document can be a sales order, a purchase return order, an outbound transfer order, or a production order whose components are ready to be picked.</span></span>

> [!NOTE]  
> <span data-ttu-id="d4885-106">Komponenten für Montageaufträge können nicht mit Lagerkommissionierungen kommissioniert oder gebucht werden.</span><span class="sxs-lookup"><span data-stu-id="d4885-106">Components for assembly orders cannot be picked or posted with inventory picks.</span></span> <span data-ttu-id="d4885-107">Verwenden Sie stattdessen das Fenster **Lagerbestandsumlagerung**.</span><span class="sxs-lookup"><span data-stu-id="d4885-107">Instead, use the **Inventory Movement** window.</span></span> <span data-ttu-id="d4885-108">Weitere Informationen finden Sie in[Vorgehensweise: Umlagern von Komponenten in einen Arbeitsgangbereich in den grundlegenden Lagerfunktionen](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)</span><span class="sxs-lookup"><span data-stu-id="d4885-108">For more information, see [How to: Move Components to an Operation Area in Basic Warehousing](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md).</span></span>

>  <span data-ttu-id="d4885-109">Bei der Kommissionierung und Lieferung von Verkaufszeilenmengen, die auftragsbezogen montiert werden, müssen Sie bestimmte Regeln einhalten, wenn sie die Lagerkommissionierzeilen erstellen.</span><span class="sxs-lookup"><span data-stu-id="d4885-109">When picking and shipping sales line quantities that are assembled to the order, you must follow certain rules when creating the inventory pick lines.</span></span> <span data-ttu-id="d4885-110">Weitere Informationen finden Sie im Abschnitt "Verwenden von Auftragsmontageartikeln in Lagerkommissionierungen".</span><span class="sxs-lookup"><span data-stu-id="d4885-110">For more information, see the “Handling Assemble-to-Order Items in Inventory Picks” section.</span></span>  

<span data-ttu-id="d4885-111">Sie können eine Lagerkommissionierung auf drei Arten erstellen:</span><span class="sxs-lookup"><span data-stu-id="d4885-111">You can create an inventory pick in three ways:</span></span>  

- <span data-ttu-id="d4885-112">Erstellen Sie die Kommissionierung in zwei Schritten, indem Sie zuerst eine Lagerkommissionierung anfordern, indem Sie den Herkunftsbeleg freigeben.</span><span class="sxs-lookup"><span data-stu-id="d4885-112">Create the pick in two steps by first requesting an inventory pick by releasing the source document.</span></span> <span data-ttu-id="d4885-113">Dies signalisiert dem Lager, dass der Herkunftsbeleg für die Kommissionierung bereit ist.</span><span class="sxs-lookup"><span data-stu-id="d4885-113">This signals to the warehouse that the source document is ready for picking.</span></span> <span data-ttu-id="d4885-114">Die Lagereinkommissionierung kann dann im Fenster **Lagereinlagerung** erstellt werden, die auf dem Herkunftsbeleg basiert.</span><span class="sxs-lookup"><span data-stu-id="d4885-114">The inventory pick can then be created in the **Inventory Pick** window based on the source document.</span></span>  
- <span data-ttu-id="d4885-115">Erstellen Sie die Lagerkommissionierung direkt vom Herkunftsbeleg aus.</span><span class="sxs-lookup"><span data-stu-id="d4885-115">Create the inventory pick directly from the source document itself.</span></span>  
- <span data-ttu-id="d4885-116">Sie können für mehrere Herkunftsbelege gleichzeitig Lagerkommissionierungen erstellen, indem Sie einen Batchauftrag verwenden.</span><span class="sxs-lookup"><span data-stu-id="d4885-116">You can create inventory picks for several source documents at the same time by using the batch job.</span></span>  

## <a name="to-request-an-inventory-pick-by-releasing-the-source-document"></a><span data-ttu-id="d4885-117">So fordern Sie eine Lagerkommissionierung durch Freigabe des Herkunftsbelegs an</span><span class="sxs-lookup"><span data-stu-id="d4885-117">To request an inventory pick by releasing the source document</span></span>  
<span data-ttu-id="d4885-118">Bei Verkaufsaufträgen, Einkaufsreklamationen und ausgehenden Umlagerungsaufträgen erstellen Sie die erwartete Lagerbewegung, indem Sie den Auftrag freigeben.</span><span class="sxs-lookup"><span data-stu-id="d4885-118">For sales orders, purchase return orders, and outbound transfer orders, you create the warehouse request by releasing the order.</span></span> <span data-ttu-id="d4885-119">Nachfolgend wird erläutert, wie dies mit einem Verkaufsauftrag erreicht wird.</span><span class="sxs-lookup"><span data-stu-id="d4885-119">The following describes how to do this from a sales order.</span></span>

1.  <span data-ttu-id="d4885-120">Alternativ wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Verkaufsauftrag** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="d4885-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="d4885-121">Wählen Sie den Verkaufsauftrag, den Sie freigeben möchten, und wählen Sie die **Freigeben** Aktion aus.</span><span class="sxs-lookup"><span data-stu-id="d4885-121">Select the sales order that you want to release, and then choose the **Release** action.</span></span>

<span data-ttu-id="d4885-122">Bei Fertigungsaufträgen erzeugen Sie die erwartete Lagerbewegung für das Kommissionieren der Komponenten automatisch (dies wird *Vorwärtsbuchen* genannt), wenn der Status des Fertigungsauftrags in **Freigegeben** geändert wird oder wenn der freigegebene Fertigungsauftrag erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="d4885-122">For production orders, you automatically create the warehouse request for the picking of components, called *flushing*, when the production order status is changed to **Released** or when the released production order is created.</span></span> <span data-ttu-id="d4885-123">Weitere Informationen finden Sie unter [Vorgehensweise: Kommissionierung für die Produktion oder Montage](warehouse-how-to-pick-for-production.md).</span><span class="sxs-lookup"><span data-stu-id="d4885-123">For more information, see [How to: Pick for Production or Assembly](warehouse-how-to-pick-for-production.md).</span></span>

<span data-ttu-id="d4885-124">Nachdem die erwartete Lagerbewegung erzeugt wurde, kann ein Lagermitarbeiter, der der Kommissionierung von Artikeln zugewiesen wurde, sehen, dass der Herkunftsbeleg zur Kommissionierung bereitsteht, und einen neuen Kommissionierbeleg auf Grundlage der erwarteten Lagerbewegung aus erstellen.</span><span class="sxs-lookup"><span data-stu-id="d4885-124">After the warehouse request has been created, a warehouse employee assigned to picking items can see that the source document is ready to be picked and can create a new pick document based on the warehouse request.</span></span>  

## <a name="to-create-an-inventory-pick-based-on-the-source-document"></a><span data-ttu-id="d4885-125">So erstellen Sie eine Lagerkommissionierung auf Grundlage des Herkunftsbelegs</span><span class="sxs-lookup"><span data-stu-id="d4885-125">To create an inventory pick based on the source document</span></span>
<span data-ttu-id="d4885-126">Nachdem die Anforderung erstellt wurde, kann der Lagermitarbeiter eine neue Lagerkommissionierung auf Grundlage des freigegebenen Herkunftsbelegs erstellen.</span><span class="sxs-lookup"><span data-stu-id="d4885-126">Now that the request is created, the warehouse employee can create a new inventory pick based on the released source document.</span></span>
1.  <span data-ttu-id="d4885-127">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben Sie **Lagerkommissionierung** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="d4885-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Inventory Picks**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="d4885-128">Wählen Sie die Aktion **Neu** aus.</span><span class="sxs-lookup"><span data-stu-id="d4885-128">Choose the **New** action.</span></span>  
3. <span data-ttu-id="d4885-129">Wählen Sie im Feld **Herkunftsbeleg** die Art des Herkunftsbelegs aus, auf dem die Kommissionierung basiert.</span><span class="sxs-lookup"><span data-stu-id="d4885-129">In the **Source Document** field, select the type of source document you are picking for.</span></span>  
4. <span data-ttu-id="d4885-130">Wählen Sie im Feld **Herkunftsnr.** den Herkunftsbeleg aus.</span><span class="sxs-lookup"><span data-stu-id="d4885-130">In the **Source No.** field, select the source document.</span></span>  
5. <span data-ttu-id="d4885-131">Oder wählen Sie die Aktion **Herkunftsbeleg holen** aus, um den Beleg aus einer Liste von ausgehenden Herkunftsbelegen auszuwählen, die zur Kommissionierung am Lagerort bereit sind.</span><span class="sxs-lookup"><span data-stu-id="d4885-131">Alternatively, choose the **Get Source Document** action to select the document from a list of outbound source documents that are ready for picking at the location.</span></span>  
6. <span data-ttu-id="d4885-132">Wählen Sie die Schaltfläche **OK**, um die Kommissionierungszeilen gemäß dem ausgewählten Herkunftsbeleg auszufüllen.</span><span class="sxs-lookup"><span data-stu-id="d4885-132">Choose the **OK** button to fill the pick lines according to the selected source document.</span></span>  

## <a name="to-create-an-inventory-pick-from-the-source-document"></a><span data-ttu-id="d4885-133">Eine Lagerkommissionierung vom Herkunftsbeleg aus erstellen</span><span class="sxs-lookup"><span data-stu-id="d4885-133">To create an inventory pick from the source document</span></span>  
1.  <span data-ttu-id="d4885-134">Im Herkunftsbeleg, der ein Auftrag, eine Einkaufsreklamation, ein ausgehender Umlagerungsauftrag oder ein Fertigungsauftrag sein kann, klicken Sie auf die Aktion **Lagerbelege erstellen**.</span><span class="sxs-lookup"><span data-stu-id="d4885-134">In the source document, which can be a sales order, purchase return order, outbound transfer order, or production order, choose the **Create Inventory Put-away/Pick** action.</span></span>
2.  <span data-ttu-id="d4885-135">Aktivieren Sie das Kontrollkästchen **Lagerkomm. erst.**</span><span class="sxs-lookup"><span data-stu-id="d4885-135">Select the **Create Invt. Pick** check box.</span></span>  
3.  <span data-ttu-id="d4885-136">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="d4885-136">Choose the **OK** button.</span></span> <span data-ttu-id="d4885-137">Eine neue Lagerkommissionierung wird erstellt.</span><span class="sxs-lookup"><span data-stu-id="d4885-137">A new inventory pick will be created.</span></span>

## <a name="to-create-multiple-inventory-picks-with-a-batch-job"></a><span data-ttu-id="d4885-138">Mehrere Lagerkommissionierungen mit einem Batchauftrag erstellen</span><span class="sxs-lookup"><span data-stu-id="d4885-138">To create multiple inventory picks with a batch job</span></span>  
1.  <span data-ttu-id="d4885-139">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben Sie **Lagerbelege erstellen** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="d4885-139">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Create Invt. Put-away / Pick**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="d4885-140">Verwenden Sie im Inforegister **Erwartete Lagerbewegung** die Felder **Herkunftsbeleg** und **Herkunftsnr.**, um Filter auf bestimmte Arten von Belegen oder Bereiche von Belegnummern zu setzen.</span><span class="sxs-lookup"><span data-stu-id="d4885-140">On the **Warehouse Request** FastTab, use the **Source Document** and **Source No.** fields to filter on certain types of documents  or ranges of document numbers.</span></span> <span data-ttu-id="d4885-141">Beispielsweise können Sie Kommissionierungen nur für Verkaufsaufträge erstellen.</span><span class="sxs-lookup"><span data-stu-id="d4885-141">For example, you can create picks only for sales orders.</span></span>  
3. <span data-ttu-id="d4885-142">Aktivieren Sie im Inforegister **Optionen** das Kontrollkästchen **Lagerkomm. erst.** aus.</span><span class="sxs-lookup"><span data-stu-id="d4885-142">On the **Options** FastTab, select the **Create Invt. Pick** check box.</span></span>
4. <span data-ttu-id="d4885-143">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="d4885-143">Choose the **OK** button.</span></span> <span data-ttu-id="d4885-144">Die angegebenen Lagerkommissionierungen werden erstellt.</span><span class="sxs-lookup"><span data-stu-id="d4885-144">The specified inventory picks are created.</span></span>

> [!NOTE]  
>  <span data-ttu-id="d4885-145">Bei der Kommissionierung und Lieferung von Verkaufszeilenmengen, die auftragsbezogen montiert werden, sollten Sie bestimmte Regeln einhalten, wenn sie die Lagerkommissionierzeilen erstellen.</span><span class="sxs-lookup"><span data-stu-id="d4885-145">If picking and shipping sales line quantities that are assembled to the order you should follow certain rules when creating the inventory pick lines.</span></span> <span data-ttu-id="d4885-146">Weitere Informationen finden Sie im Abschnitt "Verwenden von Auftragsmontageartikeln in Lagerkommissionierungen".</span><span class="sxs-lookup"><span data-stu-id="d4885-146">For more information, see the “Handling Assemble-to-Order Items in Inventory Picks” section.</span></span>  
>   
>  <span data-ttu-id="d4885-147">In den Basis-Lagerkonfigurationen werden Artikel, die nach Verkaufsauftrag montiert werden, aus dem entsprechenden Verkaufsauftrag kommissioniert, wie in diesem Thema erläutert.</span><span class="sxs-lookup"><span data-stu-id="d4885-147">In basic warehouse configurations, items that are assembled to sales orders are picked from the related sales order, as explained in this topic.</span></span> <span data-ttu-id="d4885-148">Weitere Informationen finden Sie im Abschnitt "Verwenden von Auftragsmontageartikeln in Lagerkommissionierungen" in der Lagerkommissionierung.</span><span class="sxs-lookup"><span data-stu-id="d4885-148">For more information, see “Handling Assemble-to-Order Items in Inventory Picks” in Inventory Pick.</span></span>  

## <a name="to-record-the-inventory-picks"></a><span data-ttu-id="d4885-149">So erfassen Sie die Lagerkommissionierungen</span><span class="sxs-lookup"><span data-stu-id="d4885-149">To record the inventory picks</span></span>  
1.  <span data-ttu-id="d4885-150">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben Sie **Lagerkommissionierung** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="d4885-150">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Inventory Pick**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d4885-151">Geben Sie im Feld **Lagerplatzcode** auf den Kommissionierungszeilen wird der Lagerplatz der Kommissionierung entsprechend des Standardlagerplatzes des Artikels vorgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="d4885-151">In the **Bin Code** field on the pick lines, the bin that the items must be picked from is suggesting per the item's default bin.</span></span> <span data-ttu-id="d4885-152">Sie können – falls erforderlich – in diesem Fenster den Lagerplatz ändern.</span><span class="sxs-lookup"><span data-stu-id="d4885-152">You can change the bin in this window if necessary.</span></span>  
3. <span data-ttu-id="d4885-153">Führen Sie die Kommissionierung durch und geben Sie die Informationen über die tatsächlich eingelagerte Menge in das Feld **Bewegungsmenge** ein.</span><span class="sxs-lookup"><span data-stu-id="d4885-153">Perform the pick and enter the information for the actual quantity put away in the **Qty. to Handle** field.</span></span>

    <span data-ttu-id="d4885-154">Wenn es erforderlich ist, die Artikel einer Zeile aus mehr als einem Lagerplatz zu kommissionieren, beispielsweise, da sie im designierte Lagerplatz nicht verfügbar sind, verwenden Sie die Funktion **Zeile aufteilen** im Inforegister **Zeilen**.</span><span class="sxs-lookup"><span data-stu-id="d4885-154">If it is necessary to pick the items for one line from more than one bin, for example because they are not available in the designated bin, then use the **Split Line** function on the **Lines** FastTab.</span></span> <span data-ttu-id="d4885-155">Weitere Informationen über das Aufteilen von Zeilen finden Sie unter [Vorgehensweise: Aufteilen von Lageraktivitätszeilen](warehouse-how-to-split-warehouse-activity-lines.md).</span><span class="sxs-lookup"><span data-stu-id="d4885-155">For more information about splitting lines, see [How to: Split Warehouse Activity Lines](warehouse-how-to-split-warehouse-activity-lines.md).</span></span>  
4. <span data-ttu-id="d4885-156">Wenn Sie die Kommissionierung durchgeführt haben, wählen Sie die **Buchen** Aktion aus.</span><span class="sxs-lookup"><span data-stu-id="d4885-156">When you have performed the pick, choose the **Post** action.</span></span>    

<span data-ttu-id="d4885-157">Der Buchungsvorgang bucht die Lieferung der Herkunftsbelegzeilen, die kommissioniert wurden. Bei Fertigungsaufträgen wird durch den Buchungsvorgang der Verbrauch gebucht.</span><span class="sxs-lookup"><span data-stu-id="d4885-157">The posting process will post the shipment of the source document lines that have been picked, or in the case of production orders, the posting process will post the consumption.</span></span> <span data-ttu-id="d4885-158">Wenn der Lagerort Lagerplätze verwendet, erzeugt der Buchungsvorgang darüber hinaus Lagerplatzposten, um die Mengenänderungen in den Lagerplätzen zu buchen.</span><span class="sxs-lookup"><span data-stu-id="d4885-158">If the location uses bins, the posting will also create warehouse entries to post the bin quantity changes.</span></span>  

## <a name="to-delete-inventory-pick-lines"></a><span data-ttu-id="d4885-159">Lagerkommissionierzeilen löschen</span><span class="sxs-lookup"><span data-stu-id="d4885-159">To delete inventory pick lines</span></span>  
<span data-ttu-id="d4885-160">Wenn Artikel in der Lagerkommissionierung nicht verfügbar sind, können Sie die Lagerkommissionierzeilen normalerweise löschen, nachdem Sie sie gebucht haben, und dann den Lagerkommissionierungsbeleg löschen.</span><span class="sxs-lookup"><span data-stu-id="d4885-160">If items on the inventory pick are not available, then you can delete those inventory pick lines after posting and then delete the inventory pick document.</span></span> <span data-ttu-id="d4885-161">Der Herkunftsbeleg, beispielsweise ein Verkaufsauftrag oder ein Fertigungsauftrag, enthält dann restliche Artikel zum Kommissionieren, die später durch eine neue Lagerkommissionierung erhalten werden können, wenn die Artikel verfügbar werden.</span><span class="sxs-lookup"><span data-stu-id="d4885-161">The source document, such as a sales order or a production order, will have remaining items to be picked, which can be obtained through a new inventory pick later when the items become available.</span></span>  

> [!WARNING]  
>  <span data-ttu-id="d4885-162">Dieser Prozess ist nicht möglich, wenn Serien-/Chargennummern im Herkunftsbeleg angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="d4885-162">This process is not possible if serial/lot numbers are specified on the source document.</span></span> <span data-ttu-id="d4885-163">Wenn beispielsweise eine Verkaufsauftragszeile eine Serien-/Chargennummer enthält, wird diese Artikeltrackingpezifikationen gelöscht, wenn eine Lagerkommissionierungszeile für die Serien-/Chargennummer gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="d4885-163">For example, if a sales order line contains a serial/lot number, then that item tracking specification will be deleted if an inventory pick line for the serial/lot number is deleted.</span></span>  
>   
>  <span data-ttu-id="d4885-164">Wenn Lagerkommissionierzeilen Serien-/Chargennummern haben, die nicht verfügbar sind, dürfen Sie die entsprechenden Zeilen nicht löschen.</span><span class="sxs-lookup"><span data-stu-id="d4885-164">If inventory pick lines have serial/lot numbers that are not available, you must not delete the lines in question.</span></span> <span data-ttu-id="d4885-165">Stattdessen müssen Sie das Feld **Qualitätshandhabung** in null ändern, die tatsächlichen Kommissionierungen buchen und den Lagerkommissionierungsbeleg dann löschen.</span><span class="sxs-lookup"><span data-stu-id="d4885-165">Instead, you must change the **Qty. to Handle** field to zero, post the actual picks, and then delete the inventory pick document.</span></span> <span data-ttu-id="d4885-166">Dadurch ist sichergestellt, dass die Lagerkommissionierzeilen für diese Serien-/Chargennummern später aus dem Verkaufsauftrag wiederhergestellt werden können.</span><span class="sxs-lookup"><span data-stu-id="d4885-166">This ensures that the inventory pick lines for those serial/lot numbers can be recreated from the sales order later.</span></span>  

## <a name="handling-assemble-to-order-items-with-inventory-picks"></a><span data-ttu-id="d4885-167">Verarbeiten von Auftragsmontageartikel mit Lagerkommissionierungen</span><span class="sxs-lookup"><span data-stu-id="d4885-167">Handling Assemble-to-Order Items with Inventory Picks</span></span>
<span data-ttu-id="d4885-168">Das Fenster **Lagerkommissionierung** wird auch verwendet, um für Verkäufe zu kommissionieren und zu liefern, in denen Artikel montiert werden müssen, bevor sie geliefert werden können.</span><span class="sxs-lookup"><span data-stu-id="d4885-168">The **Inventory Pick** window is also used to pick and ship for sales where items must be assembled before they can be shipped.</span></span> <span data-ttu-id="d4885-169">Weitere Informationen finden Sie unter [Vorgehensweise: Verkaufen von Auftragsmontageartikeln](assembly-how-to-sell-items-assembled-to-order.md).</span><span class="sxs-lookup"><span data-stu-id="d4885-169">For more information, see [How to: Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span></span>

<span data-ttu-id="d4885-170">Die zu liefernden Artikel sind an einem Lagerplatz erst dann tatsächlich vorhanden, wenn sie zusammengestellt und als Ausstoss für einen Lagerplatz im Montagebereich gebucht wurden.</span><span class="sxs-lookup"><span data-stu-id="d4885-170">Items to be shipped are not physically present in a bin until they are assembled and posted as output to a bin in the assembly area.</span></span> <span data-ttu-id="d4885-171">Das bedeutet, dass das Kommissionieren von Auftragsmontageartikeln zur Lieferung einem speziellen Ablauf folgt.</span><span class="sxs-lookup"><span data-stu-id="d4885-171">This means that picking assemble-to-order items for shipment follows a special flow.</span></span> <span data-ttu-id="d4885-172">Von einem Lagerplatz bringen Lagermitarbeiter die Montageartikel zur Versandstelle und buchen dann die Lagerkommissionierung.</span><span class="sxs-lookup"><span data-stu-id="d4885-172">From a bin, warehouse workers take the assembly items to the shipping dock and then post the inventory pick.</span></span> <span data-ttu-id="d4885-173">Die gebuchte Lagerkommissionierung bucht dann den Montageausstoss, den Komponentenverbrauch und die Verkaufslieferung.</span><span class="sxs-lookup"><span data-stu-id="d4885-173">The posted inventory pick then posts the assembly output, the component consumption, and the sales shipment.</span></span>

<span data-ttu-id="d4885-174">Sie können [!INCLUDE[d365fin](includes/d365fin_md.md)] einrichten, um eine automatische Lagerbestandsumlagerung zu erstellen, wenn die Lagerkommissionierung für die Montageartikel erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="d4885-174">You can set up [!INCLUDE[d365fin](includes/d365fin_md.md)] to automatically create an inventory movement when the inventory pick for the assembly item is created.</span></span> <span data-ttu-id="d4885-175">Um dies zu aktivieren, müssen Sie das Feld **Umlagerungen automatisch erstellen** im Fenster **Montageeinrichtung** auswählen.</span><span class="sxs-lookup"><span data-stu-id="d4885-175">To enable this, you must select the **Create Movements Automatically** field in the **Assembly Setup** window.</span></span> <span data-ttu-id="d4885-176">Weitere Informationen finden Sie in[Vorgehensweise: Umlagern von Komponenten in einen Arbeitsgangbereich in den grundlegenden Lagerfunktionen](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)</span><span class="sxs-lookup"><span data-stu-id="d4885-176">For more information, see [How to: Move Components to an Operation Area in Basic Warehousing](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md).</span></span>

<span data-ttu-id="d4885-177">Lagerkommissionierzeilen für Verkaufsartikel werden je nachdem, ob keine, einige oder alle Verkaufspositionsmengen auf Bestellung gefertigt werden, auf unterschiedliche Weise erstellt.</span><span class="sxs-lookup"><span data-stu-id="d4885-177">Inventory pick lines for sales items are created in different ways depending on whether none, some, or all of the sales line quantities are assembled to order.</span></span>

<span data-ttu-id="d4885-178">Bei regulären Verkäufen, wo Sie Lagerkommissionierungen verwenden, um Liefer- und Lagermengen zu buchen, wird eine Verkaufsauftragszeile, oder mehre, wenn der Artikel in verschiedenen Lagerplätzen platziert ist, erstellt für jede Verkaufszeile.</span><span class="sxs-lookup"><span data-stu-id="d4885-178">In regular sales where you use inventory picks to post shipment of inventory quantities, one inventory pick line, or several if the item is placed in different bins, is created for each sales order line.</span></span> <span data-ttu-id="d4885-179">Diese Kommissionierzeile basiert auf der Menge im Feld **Zu liefernde Menge**.</span><span class="sxs-lookup"><span data-stu-id="d4885-179">This pick line is based on the quantity in the **Qty. to Ship** field.</span></span>

<span data-ttu-id="d4885-180">In Auftragsmontageverkäufen, bei denen die gesamte Menge aus der Verkaufsauftragszeile montiert wird, wird eine Lagerkommissionierzeile für diese Menge erstellt.</span><span class="sxs-lookup"><span data-stu-id="d4885-180">In assemble-to-order sales where the full quantity on the sales order line is assembled to order, one inventory pick line is created for that quantity.</span></span> <span data-ttu-id="d4885-181">Das bedeutet, dass der Wert im Feld "Menge für Montage" dem Wert im Feld **Zu liefernde Menge** entspricht.</span><span class="sxs-lookup"><span data-stu-id="d4885-181">This means that the value in the Quantity to Assemble field is the same as the value in the **Qty. to Ship** field.</span></span> <span data-ttu-id="d4885-182">Das Feld **Auftragsmontage** wird in der Zeile ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="d4885-182">The **Assemble to Order** field is selected on the line.</span></span>

<span data-ttu-id="d4885-183">Wenn ein Montageausgabefluss für den Lagerort eingerichtet wird, wird der Wert im Feld **LP-Code f. Prog.fert.lief.** oder der Wert im Feld **Montage-Ausgangslagerplatzcode** in dieser Reihenfolge in das Feld **Lagerplatzcode** in der Lagerkommissionierzeile eingefügt.</span><span class="sxs-lookup"><span data-stu-id="d4885-183">If an assembly output flow is set up for the location, then the value in the **Asm.-to-Order Shpt. Bin Code** field or the value in the **From-Assembly Bin Code** field, in that order, is inserted in the **Bin Code** field on the inventory pick line.</span></span>

<span data-ttu-id="d4885-184">Wenn kein Lagerplatzcode in der Verkaufsauftragszeile angegeben wird und kein Montageausgabefluss für den Lagerort eingerichtet wird, bleibt das Feld **Lagerplatzcode** in der Lagerkommissionierzeile leer.</span><span class="sxs-lookup"><span data-stu-id="d4885-184">If no bin code is specified on the sales order line, and no assembly output flow is set up for the location, then the **Bin Code** field on the inventory pick line is empty.</span></span> <span data-ttu-id="d4885-185">Der Lagermitarbeiter muss das Fenster **Lagerplatzinhalte** öffnen und den Lagerort auswählen, in dem die Montageartikel montiert werden.</span><span class="sxs-lookup"><span data-stu-id="d4885-185">The warehouse worker must open the **Bin Contents** window and select the bin where the assembly items are assembled.</span></span>

<span data-ttu-id="d4885-186">In Kombinationsszenarien in denen ein Teil der Menge zunächst montiert werden muss und andere aus dem Lager kommissioniert werden müssen, werden mindestens zwei Lagerkommissionierzeilen erstellt.</span><span class="sxs-lookup"><span data-stu-id="d4885-186">In combination scenarios, where a part of the quantity must first be assembled and another must be picked from inventory, a minimum of two inventory pick lines are created.</span></span> <span data-ttu-id="d4885-187">Eine Kommissionierzeile ist für die Programmfertigungsmenge.</span><span class="sxs-lookup"><span data-stu-id="d4885-187">One pick line is for the assemble-to-order quantity.</span></span> <span data-ttu-id="d4885-188">Die andere Kommissionierzeile hängt davon ab, welche Lagerplätze die Restmenge aus dem Lagerbestand erfüllen können.</span><span class="sxs-lookup"><span data-stu-id="d4885-188">The other pick line depends on which bins can fulfill the remaining quantity from inventory.</span></span> <span data-ttu-id="d4885-189">Lagerplatzcodes in den beiden Zeilen werden auf verschiedene Weise ausgefüllt, wie für die beiden verschiedenen Verkaufsarten beschrieben.</span><span class="sxs-lookup"><span data-stu-id="d4885-189">Bin codes on the two lines are filled in different ways as described for the two different sales types respectively.</span></span> <span data-ttu-id="d4885-190">Weitere Informationen finden Sie im Abschnitt "Kombinationsszenarien" in [Auftragsmontage und Lagermontage verstehen](assembly-assemble-to-order-or-assemble-to-stock.md).</span><span class="sxs-lookup"><span data-stu-id="d4885-190">For more information, see the “Combination Scenarios” section in [Understanding Assemble to Order and Assemble to Stock](assembly-assemble-to-order-or-assemble-to-stock.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="d4885-191">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="d4885-191">See Also</span></span>  
[<span data-ttu-id="d4885-192">Logistik</span><span class="sxs-lookup"><span data-stu-id="d4885-192">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="d4885-193">Lagerbesttand</span><span class="sxs-lookup"><span data-stu-id="d4885-193">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="d4885-194">[Lagerortverwaltung einrichten](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="d4885-194">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="d4885-195">[Montageverwaltung](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="d4885-195">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="d4885-196">Designdetails: Logistik</span><span class="sxs-lookup"><span data-stu-id="d4885-196">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="d4885-197">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d4885-197">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
