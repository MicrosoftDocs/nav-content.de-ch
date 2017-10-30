---
title: Abschliessen eines LSV-Einzugs
description: "LSV+ (Lastschrift Verfahren)-Einzüge müssen abgeschlossen werden, um LSV-Dateien zu schreiben, die zum Zahlungseinzug an die Bank gesendet werden können. Wenn Sie einen Einzug abschliessen, ist dieser beendet, und die Buchungen im LSV-Journal werden kombiniert."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 1d63f24a50024f4561b5827f2b6b1328c207a873
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-close-an-lsv-collection"></a><span data-ttu-id="796ce-104">Gewusst wie: Abschliessen eines LSV-Einzugs</span><span class="sxs-lookup"><span data-stu-id="796ce-104">How to: Close an LSV Collection</span></span>
<span data-ttu-id="796ce-105">LSV+ (Lastschrift Verfahren)-Einzüge müssen abgeschlossen werden, um LSV-Dateien zu schreiben, die zum Zahlungseinzug an die Bank gesendet werden können.</span><span class="sxs-lookup"><span data-stu-id="796ce-105">You must close Lastschrift Verfahren (LSV+) collections to write LSV files that can be sent to the bank for payment collection.</span></span> <span data-ttu-id="796ce-106">Wenn Sie einen Einzug abschliessen, ist dieser beendet, und die Buchungen im LSV-Journal werden kombiniert.</span><span class="sxs-lookup"><span data-stu-id="796ce-106">When you close a collection, the collection is complete, and the postings in the LSV journal are combined.</span></span>  
  
 <span data-ttu-id="796ce-107">Wenn der Einzug abgeschlossen ist, wird die aktuelle Einzugsnummer im LSV-Journal auf Grundlage des letzten Einzugs zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="796ce-107">When the collection is complete, the current collection number is assigned in the LSV journal, based on the last collection.</span></span> <span data-ttu-id="796ce-108">Diese LSV-Nummer wird für alle ausstehenden Rechnungen an die Debitorenposten übertragen.</span><span class="sxs-lookup"><span data-stu-id="796ce-108">This LSV number is transferred to the customer entries for all outstanding invoices.</span></span> <span data-ttu-id="796ce-109">Anhand der LSV-Nummer kann die Einzugsdatei jederzeit rekonstruiert werden.</span><span class="sxs-lookup"><span data-stu-id="796ce-109">The collection file can be reconstructed at any time using the LSV number.</span></span> <span data-ttu-id="796ce-110">Das Feld **Abwarten** wird auch mit **LSV** in den Debitorenposten ausgefüllt, um die Duplizierung von offenen Posten zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="796ce-110">The **On Hold** field is also populated with **LSV** in the customer entries to avoid the duplication of open entries.</span></span> <span data-ttu-id="796ce-111">Weitere Informationen finden Sie in den Tabellen **LSV Journal** und **Debitorenposten**.</span><span class="sxs-lookup"><span data-stu-id="796ce-111">For more information, see the **LSV Journal** table and the **Cust. Ledger Entry** table.</span></span> <span data-ttu-id="796ce-112">Ausserdem kann ein abgeschlossener Einzug auch erneut geöffnet werden.</span><span class="sxs-lookup"><span data-stu-id="796ce-112">You can also reopen a closed collection.</span></span>  
  
### <a name="to-close-an-lsv-collection"></a><span data-ttu-id="796ce-113">So schliessen Sie einen LSV-Einzug</span><span class="sxs-lookup"><span data-stu-id="796ce-113">To close an LSV collection</span></span>  
  
1.  <span data-ttu-id="796ce-114">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite ober Bericht suchen"), und öffnen Sie **LSV-Journal Liste**. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="796ce-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **LSV Journal List**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="796ce-115">Wählen Sie die erforderliche Erf.-Journalzeile aus, und wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Funktionen** die Option **Buchungsdatum korrigieren** aus.</span><span class="sxs-lookup"><span data-stu-id="796ce-115">Select the required journal line, on the **Actions** tab, in the **Functions** group, select **Modify Posting Date**.</span></span> <span data-ttu-id="796ce-116">Dadurch wird der Wert im Feld **Valutadatum** geändert, indem der während des LSV-Einzugs vorgeschlagene Wert verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="796ce-116">This will modify the value in the **Credit Date** field by using the value suggested during the LSV collection.</span></span>  
  
3.  <span data-ttu-id="796ce-117">Geben Sie im Feld **Neues Datum** das neue Datum ein.</span><span class="sxs-lookup"><span data-stu-id="796ce-117">In the **New Date** field, enter the new date.</span></span>  
  
4.  <span data-ttu-id="796ce-118">Wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Funktionen** **Einzug abschliessen** aus.</span><span class="sxs-lookup"><span data-stu-id="796ce-118">On the **Actions** tab, in the **Functions** group, select **Close Collection**.</span></span>  
  
    > [!NOTE]  
    >  <span data-ttu-id="796ce-119">Die Felder auf dem Inforegister **Optionen** für die Stapelverarbeitung **LSV Einzug abschliessen** können nicht geändert werden und entsprechen der ausgewählten Erf.-Journalzeile.</span><span class="sxs-lookup"><span data-stu-id="796ce-119">The fields on the **Options** FastTab for the **LSV Close Collection** batch job cannot be modified, and correspond to the selected journal line.</span></span>  
  
5.  <span data-ttu-id="796ce-120">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="796ce-120">Choose the **OK** button.</span></span>  
  
     <span data-ttu-id="796ce-121">Im Fenster **LSV-Journal Liste** wird der Wert im Feld **LSV-Status** von **Bearbeiten** in **Freigegeben** geändert.</span><span class="sxs-lookup"><span data-stu-id="796ce-121">In the **LSV Journal List** window, the value in the **LSV Status** field is changed from **Edit** to **Released**.</span></span> <span data-ttu-id="796ce-122">Die Erf.-Journalzeilen können nicht mehr geändert werden.</span><span class="sxs-lookup"><span data-stu-id="796ce-122">The journal lines can no longer be modified.</span></span>  
  
### <a name="to-reopen-an-lsv-collection"></a><span data-ttu-id="796ce-123">So öffnen Sie einen LSV-Einzug erneut</span><span class="sxs-lookup"><span data-stu-id="796ce-123">To reopen an LSV collection</span></span>  
  
1.  <span data-ttu-id="796ce-124">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite ober Bericht suchen"), und öffnen Sie **LSV-Journal Liste**. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="796ce-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **LSV Journal List**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="796ce-125">Wählen Sie die erforderliche Erf.-Journalzeile aus, für die Sie den Einzug erneut öffnen möchten, wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Funktion** **Einzug erneut öffnen** aus.</span><span class="sxs-lookup"><span data-stu-id="796ce-125">Select the required journal line for which you want to reopen the collection, on the **Actions** tab, in the **Functions** group, select **Reopen Collection**.</span></span>  
  
    > [!NOTE]  
    >  <span data-ttu-id="796ce-126">Der Einzug kann nur erneut geöffnet werden, wenn die LSV+-Datei noch nicht an die Bank übermittelt wurde.</span><span class="sxs-lookup"><span data-stu-id="796ce-126">You can only reopen the collection if you have not yet submitted the LSV+ file to the bank.</span></span>  
  
3.  <span data-ttu-id="796ce-127">Wählen Sie die Schaltfläche **Ja**, um das erneute Öffnen des Einzugs zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="796ce-127">Choose the **Yes** button to confirm the reopening of the collection.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="796ce-128">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="796ce-128">See Also</span></span>  
 <span data-ttu-id="796ce-129">[Elektronische Zahlungen mit LSV+ (Schweiz)](swiss-electronic-payments-using-lsv-.md) </span><span class="sxs-lookup"><span data-stu-id="796ce-129">[Swiss Electronic Payments Using LSV+](swiss-electronic-payments-using-lsv-.md) </span></span>  
 <span data-ttu-id="796ce-130">[Gewusst wie: Verarbeiten eines LSV-Einzugs](how-to-process-an-lsv-collection.md) </span><span class="sxs-lookup"><span data-stu-id="796ce-130">[How to: Process an LSV Collection](how-to-process-an-lsv-collection.md) </span></span>  
 <span data-ttu-id="796ce-131">[Gewusst wie: Buchen von LSV+-Zahlungen](how-to-post-lsv-payments.md) </span><span class="sxs-lookup"><span data-stu-id="796ce-131">[How to: Post LSV+ Payments](how-to-post-lsv-payments.md) </span></span>  
 <span data-ttu-id="796ce-132">[Gewusst wie: Exportieren von Zahlungen mit LSV](how-to-export-payments-using-lsv.md) </span><span class="sxs-lookup"><span data-stu-id="796ce-132">[How to: Export Payments Using LSV](how-to-export-payments-using-lsv.md) </span></span>  
 <span data-ttu-id="796ce-133">LSV Journal</span><span class="sxs-lookup"><span data-stu-id="796ce-133">LSV Journal</span></span>   
 <span data-ttu-id="796ce-134">LSV-Journalzeile</span><span class="sxs-lookup"><span data-stu-id="796ce-134">LSV Journal Line</span></span>   
 <span data-ttu-id="796ce-135">Debitorenposten</span><span class="sxs-lookup"><span data-stu-id="796ce-135">Cust. Ledger Entry</span></span>
