---
title: "Anlagen veräußern oder aus dem Verkehr ziehen"
description: "Sie müssen einen Verkaufswert buchen, wenn Sie eine Anlage verkaufen oder ausrangieren, die storniert werden sollten."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: scrap
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 38753282687aafa1d06542ba265225eb30720c20
ms.contentlocale: de-ch
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-dispose-of-or-retire-fixed-assets"></a><span data-ttu-id="6feb6-103">So geht's: Anlagen entsorgen oder außer Dienst stellen</span><span class="sxs-lookup"><span data-stu-id="6feb6-103">How to: Dispose of or Retire Fixed Assets</span></span>
<span data-ttu-id="6feb6-104">Wenn Sie eine Anlage verkaufen oder anderweitig entfernen, muss der Verkaufswert gebucht werden, um den Gewinn oder Verlust zu berechnen und zu erfassen.</span><span class="sxs-lookup"><span data-stu-id="6feb6-104">When you sell or otherwise dispose of a fixed asset, the disposal value must be posted to calculate and record the gain or loss.</span></span> <span data-ttu-id="6feb6-105">Ein Verkaufsposten muss der letzte gebuchte Posten einer Anlage sein.</span><span class="sxs-lookup"><span data-stu-id="6feb6-105">A disposal entry must be the last entry posted for a fixed asset.</span></span> <span data-ttu-id="6feb6-106">Für teilweise verkaufte Anlagen können Sie mehr als einen Verkaufsposten buchen.</span><span class="sxs-lookup"><span data-stu-id="6feb6-106">For partially disposed fixed assets, you can post more than one disposal entry.</span></span> <span data-ttu-id="6feb6-107">Die Summe aller gebuchten Verkaufsbeträge muss ein Habenposten sein.</span><span class="sxs-lookup"><span data-stu-id="6feb6-107">The total of all posted disposal amounts must be a credit amount.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="6feb6-108">Falls Sie für den Verkauf einer Anlage eine andere Anlage in Zahlung nehmen, müssen Sie sowohl den Verkauf der alten Anlage als auch die Anschaffung der neuen Anlage buchen.</span><span class="sxs-lookup"><span data-stu-id="6feb6-108">If you trade-in a fixed asset for another one, you must record both the sale of the old asset (disposal) and the purchase of the new one (acquisition).</span></span> <span data-ttu-id="6feb6-109">Weitere Informationen finden Sie unter [So geht's: Beschaffen von Anlagen](fa-how-acquire.md).</span><span class="sxs-lookup"><span data-stu-id="6feb6-109">For more information, see [How to: Acquire Fixed Assets](fa-how-acquire.md).</span></span>  

## <a name="to-post-a-disposal-from-the-fixed-asset-gl-journal"></a><span data-ttu-id="6feb6-110">So buchen Sie einen Verkauf aus dem Anlagen Fibu Erf.-Journal</span><span class="sxs-lookup"><span data-stu-id="6feb6-110">To post a disposal from the fixed asset G/L journal</span></span>
1. <span data-ttu-id="6feb6-111">Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Anlagen G/L-Buchblatt** ein und wählen den zugehörenden Link aus.</span><span class="sxs-lookup"><span data-stu-id="6feb6-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="6feb6-112">Erstellen Sie eine ursprüngliche Erf.-Journalzeile und füllen Sie die notwendigen Felder aus.</span><span class="sxs-lookup"><span data-stu-id="6feb6-112">Create an initial journal line and fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. <span data-ttu-id="6feb6-113">Wählen Sie im Feld **Anlagenbuchungsart** den **Verkauf**.</span><span class="sxs-lookup"><span data-stu-id="6feb6-113">In the **FA Posting Type** field, select **Disposal**.</span></span>  
4. <span data-ttu-id="6feb6-114">Wählen Sie die Aktion **Anlagengegenkonto einfügen**.</span><span class="sxs-lookup"><span data-stu-id="6feb6-114">Choose the **Insert FA Bal. Account** action.</span></span> <span data-ttu-id="6feb6-115">Eine zweite Erf.-Journalzeile wird für das Gegenkonto erstellt, das für die Buchung eines Verkaufs eingerichtet wird.</span><span class="sxs-lookup"><span data-stu-id="6feb6-115">A second journal line is created for the balancing account that is set up for disposal posting.</span></span>  

    > [!NOTE]  
>   <span data-ttu-id="6feb6-116">Schritt 4 funktioniert nur, wenn Sie Folgendes eingerichtet haben: Im Fenster **Anlagenbuchungsgruppenkarte** der Buchungsgruppe der Anlage enthält das Feld **Kto. Verkauf** das Sollkonto im Sachkonto und das Feld **Gegenkto Verkauf** enthält das Sachkonto, auf das die Gegenposten für Zuschreibungen gebucht werden sollen.</span><span class="sxs-lookup"><span data-stu-id="6feb6-116">Step 4 only works if you have set up the following: In the **FA Posting Group Card** window for the posting group of the fixed asset, the **Disposal Account** field contains the general ledger debit account and the **Disposal Bal. Account** field contains the general ledger account to which you want to post balancing entries for appreciation.</span></span> <span data-ttu-id="6feb6-117">Weitere Informationen finden Sie im Abschnitt "So richten Sie Anlagenbuchungsgruppen ein" in [So geht's: Allgemeine Anlageninformationen einrichten](fa-how-setup-general.md).</span><span class="sxs-lookup"><span data-stu-id="6feb6-117">For more information, see the "To set up fixed asset posting groups" section in [How to: Set Up General Fixed Asset Information](fa-how-setup-general.md).</span></span>  
5. <span data-ttu-id="6feb6-118">Wählen Sie die Aktion **Buchen** aus.</span><span class="sxs-lookup"><span data-stu-id="6feb6-118">Choose the **Post** action.</span></span>  

    <span data-ttu-id="6feb6-119">Wenn Sie eine Anlage zum Teil verkaufen, müssen Sie die Anlage aufteilen, bevor Sie die Verkaufstransaktion buchen können.</span><span class="sxs-lookup"><span data-stu-id="6feb6-119">If you sell or dispose of part of a fixed asset, you must split up the asset before you can record the disposal transaction.</span></span> <span data-ttu-id="6feb6-120">Weitere Informationen finden Sie unter [So geht's: Übertragen, Teilen oder Kombinieren von Anlagen.](fa-how-trans-split-combine.md).</span><span class="sxs-lookup"><span data-stu-id="6feb6-120">For more information, see [How to: Transfer, Split, or Combine Fixed Assets](fa-how-trans-split-combine.md).</span></span>  

## <a name="to-view-disposal-ledger-entries"></a><span data-ttu-id="6feb6-121">So zeigen Sie Verkaufsposten an</span><span class="sxs-lookup"><span data-stu-id="6feb6-121">To view disposal ledger entries</span></span>
<span data-ttu-id="6feb6-122">Wenn Sie eine Anlage verkaufen, wird der Verkaufswert in den Fibuposten gebucht, wo Sie die Ergebnisse anzeigen können.</span><span class="sxs-lookup"><span data-stu-id="6feb6-122">When you sell or dispose of a fixed asset, the disposal value is posted to the general ledger where you can view the result.</span></span>  

1. <span data-ttu-id="6feb6-123">Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Anlagen** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="6feb6-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Fixed Assets**, and then choose the related link.</span></span>  
2. <span data-ttu-id="6feb6-124">Wählen Sie die Anlage aus, für die Sie die Posten anzeigen möchten und wählen Sie dann die Aktion **AfA-Bücher** aus.</span><span class="sxs-lookup"><span data-stu-id="6feb6-124">Select the fixed asset that you want to view entries for, and then choose the **Depreciation Books** action.</span></span>  
3. <span data-ttu-id="6feb6-125">Wählen Sie das AfA-Buch aus, für das Sie die Posten anzeigen möchten und wählen Sie dann die Aktion **Posten** aus.</span><span class="sxs-lookup"><span data-stu-id="6feb6-125">Select the depreciation book that you want to view entries for, and then choose the **Ledger Entries** action.</span></span>  
4. <span data-ttu-id="6feb6-126">Wählen Sie im Feld **Anlagebuchungskategorie** die Zeile mit **Verkauf** aus, und klicken Sie auf die Aktion **Navigieren**.</span><span class="sxs-lookup"><span data-stu-id="6feb6-126">Select a line with **Disposal** in the **FA Posting Category** field, and then choose the **Navigate** action.</span></span>  
5. <span data-ttu-id="6feb6-127">Wählen Sie im Fenster **Navigieren** die Sachpostenzeile aus, und klicken Sie auf die Aktion **Anzeigen**.</span><span class="sxs-lookup"><span data-stu-id="6feb6-127">In the **Navigate** window, select the general ledger entry line, and then choose the **Show** action.</span></span>  

<span data-ttu-id="6feb6-128">Das Fenster **Sachposten** wird geöffnet, in dem Sie die Posten sehen können, die aus der Verkaufsbuchung resultieren.</span><span class="sxs-lookup"><span data-stu-id="6feb6-128">The **General Ledger Entries** window opens where you can see the entries that the disposal posting resulted in.</span></span>  

## <a name="see-also"></a><span data-ttu-id="6feb6-129">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="6feb6-129">See Also</span></span>
[<span data-ttu-id="6feb6-130">Anlagen</span><span class="sxs-lookup"><span data-stu-id="6feb6-130">Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="6feb6-131">Anlagen einrichten</span><span class="sxs-lookup"><span data-stu-id="6feb6-131">Setting Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="6feb6-132">Finanzen</span><span class="sxs-lookup"><span data-stu-id="6feb6-132">Finance</span></span>](finance.md)  
<span data-ttu-id="6feb6-133">[Willkommen bei [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="6feb6-133">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
<span data-ttu-id="6feb6-134">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6feb6-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
