---
title: "Suche nach Belegen ohne Dateianhänge"
Description: "Sie können nach Fibuposten für gebuchte Einkaufs- und Verkaufsbelege suchen, die keine eingehenden  elektronische Belege haben, wie importierte Rechnungen."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 515026b4da842afeda1759f50313dc26bcfd3350
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-find-posted-documents-without-incoming-document-records"></a><span data-ttu-id="14a38-103">So wird's gemacht: Gebuchte Belege ohne Eingangsbelege finden</span><span class="sxs-lookup"><span data-stu-id="14a38-103">How to: Find Posted Documents without Incoming Document Records</span></span>
<span data-ttu-id="14a38-104">In den Fenstern **Kontenplan** und **Sachposten** können Sie eine Suchfunktion verwenden, um Sachposten für gebuchte Einkaufs- und Verkaufsbelege zu finden, für die keine eingehende Belegdatensätze vorhanden sind, und dann zentral eine Verknüpfung zu vorhandenen Datensätzen herstellen oder neue mit angefügten Belegdateien erstellen.</span><span class="sxs-lookup"><span data-stu-id="14a38-104">From the **Chart of Accounts** and **General Ledger Entries** windows, you can use a search function to find general ledger entries for posted purchase and sales documents that do not have incoming document records and then centrally link to existing records or create new ones with attached document files.</span></span>

## <a name="to-find-posted-documents-without-incoming-document-records"></a><span data-ttu-id="14a38-105">So finden Sie gebuchte Belege ohne zugehörige Eingangsbelege</span><span class="sxs-lookup"><span data-stu-id="14a38-105">To find posted documents without incoming document records</span></span>
1. <span data-ttu-id="14a38-106">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben **Kontenplan** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="14a38-106">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="14a38-107">Wählen Sie eine Zeile für ein Fibukonto aus, für dessen Fibuposten Sie gebuchte Einkaufs- und Verkaufsbelege abrufen möchten, zu denen keine Eingangsbelege vorhanden sind, und wählen Sie dann die Aktion **Gebuchte Belege ohne Eingangsbeleg**.</span><span class="sxs-lookup"><span data-stu-id="14a38-107">Select a line for a G/L account for whose general ledger entries you want to see posted purchase and sales documents without incoming document records, and then choose the **Posted Documents without Incoming Document** action.</span></span>
3. <span data-ttu-id="14a38-108">Alternativ wählen Sie die Aktion **Ledger Entries** aus.</span><span class="sxs-lookup"><span data-stu-id="14a38-108">Alternatively, choose the **Ledger Entries** action.</span></span>
4. <span data-ttu-id="14a38-109">Wählen Sie im Fenster **Sachposten** die Aktion **Gebuchte Belege ohne Eingangsbelege** aus.</span><span class="sxs-lookup"><span data-stu-id="14a38-109">In the **General Ledger Entries** window, choose the **Posted Documents without Incoming Documents** action.</span></span>

<span data-ttu-id="14a38-110">Daraufhin wird das Fenster **Gebuchte Belege ohne Eingangsbeleg** geöffnet, dass die gebuchten Einkaufs- und Verkaufsbelege ohne zugehörige Eingangsbelege enthält, die von Fibuposten auf dem Fibukonto dargestellt werden, für das Sie das Fenster geöffnet haben.</span><span class="sxs-lookup"><span data-stu-id="14a38-110">The **Posted Documents without Incoming Document** window opens showing posted purchase and sales documents without incoming document records represented by general ledger entries on the G/L account that you opened the window for.</span></span> <span data-ttu-id="14a38-111">Das Fenster kann maximal 1000 Zeilen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="14a38-111">The window can show a maximum of 1000 lines.</span></span> <span data-ttu-id="14a38-112">Standardmäßig enthält das Feld **Datumsfilter** daher einen Filter, der die Anzeige auf Einträge beschränkt, deren Buchungsdatum zwischen dem Beginn der Buchhaltungsperiode und dem Arbeitsdatum liegt.</span><span class="sxs-lookup"><span data-stu-id="14a38-112">By default, the **Date Filter** field therefore contains a filter that limits the lines to entries with posting dates from the beginning of the accounting period to the work date.</span></span>

## <a name="to-connect-found-documents-to-existing-incoming-document-records"></a><span data-ttu-id="14a38-113">So verknüpfen Sie gefundene Belege mit vorhandenen Eingangsbelegen</span><span class="sxs-lookup"><span data-stu-id="14a38-113">To connect found documents to existing incoming document records</span></span>
1. <span data-ttu-id="14a38-114">Wählen Sie im Fenster **Gebuchte Belege ohne Eingangsbeleg** die Zeile für einen gebuchten Beleg aus, den Sie mit einem vorhandenen Eingangsbeleg verknüpfen möchten, und wählen Sie dann die Aktion **Eingehenden Beleg auswählen** aus.</span><span class="sxs-lookup"><span data-stu-id="14a38-114">In the **Posted Documents without Incoming Document** window, select the line for a posted document that you want to connect to an existing incoming document record, and then choose the **Select Incoming Document** action.</span></span>
2. <span data-ttu-id="14a38-115">Wählen Sie im Fenster **Eingehende Belege** den Eingangsbeleg aus, den Sie der gefundenen Buchung zuordnen möchten, und klicken Sie anschließend auf die Schaltfläche **OK**.</span><span class="sxs-lookup"><span data-stu-id="14a38-115">In the **Incoming Documents** window, select the incoming document record that you want to connect to posted document found, and then choose the **OK** button.</span></span>
3. <span data-ttu-id="14a38-116">Im Fenster **Gebuchte Belege ohne Eingangsbeleg** wird der gewählte Eingangsbeleg nun mit dem gebuchten Beleg verknüpft und in der InfoBox **Eingehende Belegdateien** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="14a38-116">In the **Posted Documents without Incoming Document** window, the selected incoming document record is now connected to the posted document, as you can see in the **Incoming Document Files** FactBox.</span></span>

<span data-ttu-id="14a38-117">Wenn das Fenster **Eingehende Belege** keinen relevanten Eingangsbeleg-Datensatz enthält, können Sie einen erstellen.</span><span class="sxs-lookup"><span data-stu-id="14a38-117">If a relevant incoming document record does not exist in the **Incoming Documents** window, then you can create it.</span></span> <span data-ttu-id="14a38-118">Weitere Informationen finden Sie unter [So gehts: Eingehende Belege erstellen](across-how-create-income-document-records.md).</span><span class="sxs-lookup"><span data-stu-id="14a38-118">For more information, see [How to: Create Incoming Document Records](across-how-create-income-document-records.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="14a38-119">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="14a38-119">See Also</span></span>
[<span data-ttu-id="14a38-120">Eingehende Dokumente verarbeiten</span><span class="sxs-lookup"><span data-stu-id="14a38-120">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="14a38-121">Eingehende Belege</span><span class="sxs-lookup"><span data-stu-id="14a38-121">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="14a38-122">Einkauf</span><span class="sxs-lookup"><span data-stu-id="14a38-122">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="14a38-123">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="14a38-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
