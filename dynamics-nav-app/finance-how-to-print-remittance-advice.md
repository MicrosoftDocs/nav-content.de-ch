---
title: 'Vorgehensweise: Drucken von Zahlungsanzeigen'
description: "Sie können Ihren Kreditoren helfen, Abstimmungen auszuführen, indem Sie Zahlungsanzeige ausdrucken, bevor Sie ein Erf.-Journal buchen oder wenn Sie eine Zahlung buchen."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/26/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 71c84b4a7bad83e6008c0fa34f908e133b014a59
ms.contentlocale: de-ch
ms.lasthandoff: 10/26/2017

---

#<a name="how-to-print-remittance-advice"></a><span data-ttu-id="0ddca-103">Vorgehensweise: Drucken von Zahlungsanzeigen</span><span class="sxs-lookup"><span data-stu-id="0ddca-103">How to: Print Remittance Advice</span></span>
<span data-ttu-id="0ddca-104">Sie können Zahlungsanzeigen ausdrucken, bevor Sie ein Erf.-Journal buchen oder wenn Sie eine Zahlung gebucht haben.</span><span class="sxs-lookup"><span data-stu-id="0ddca-104">You can print remittance advice before posting a payment journal and after posting a payment.</span></span> <span data-ttu-id="0ddca-105">Diese Anzeige zeigt die Kreditors-Nummern an, was hilft, die Abstimmungen auszuführen.</span><span class="sxs-lookup"><span data-stu-id="0ddca-105">This advice displays vendor invoice numbers, which helps vendors to perform reconciliations.</span></span>

##<a name="to-print-remittance-advice"></a><span data-ttu-id="0ddca-106">Vorgehensweise: Drucken von Zahlungsanzeigen</span><span class="sxs-lookup"><span data-stu-id="0ddca-106">To print remittance advice</span></span>
1. <span data-ttu-id="0ddca-107">Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Zahlungs-Buchblatt** ein und wählen den zugehörenden Link aus.</span><span class="sxs-lookup"><span data-stu-id="0ddca-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="0ddca-108">Im Fenster **Zahlungsausgangs Erf.-Journal** wählen Sie die Zahlung aus, für die die Zahlungsanzeige gedruckt werden muss.</span><span class="sxs-lookup"><span data-stu-id="0ddca-108">In the **Payment Journal** window, select the payment for which remittance advice must be printed.</span></span>  
3. <span data-ttu-id="0ddca-109">Wählen Sie die **Zahlungsanzeige drucken** Aktion aus.</span><span class="sxs-lookup"><span data-stu-id="0ddca-109">Choose the **Print Remittance Advice** action.</span></span>  
4. <span data-ttu-id="0ddca-110">In der Stapelverarbeitung **Zahlungsanzeige - Erf.-Journal** im Inforegister **Fen. Erf.-Journalzeile**, wählen Sie die entsprechenden Filter aus.</span><span class="sxs-lookup"><span data-stu-id="0ddca-110">In the **Remittance Advice - Journal** batch job, on the **Fen. Journal Line** FastTab, choose the appropriate filters.</span></span>  
  
    >[!Note]
    > <span data-ttu-id="0ddca-111">Sie können anhand der externen Belegnummer des Kreditors filtern, um Zahlungen mit Rechnungen zu finden.</span><span class="sxs-lookup"><span data-stu-id="0ddca-111">You can filter using the vendor's external document number to match payments with invoices.</span></span>

5. <span data-ttu-id="0ddca-112">Wählen Sie im Inforegister **Verkäufer** die entsprechenden Filter aus.</span><span class="sxs-lookup"><span data-stu-id="0ddca-112">On the **Vendor** FastTab, choose the appropriate filters.</span></span>  
6. <span data-ttu-id="0ddca-113">Wählen Sie **Drucken**, um den Bericht zu drucken oder **Seitenansicht**, um den Bericht am Bildschirm anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="0ddca-113">Choose **Print** to print the report, or choose **Preview** to view it now.</span></span>  

## <a name="using-remittance-advice-reports"></a><span data-ttu-id="0ddca-114">Zahlungsanzeige-Berichte verwenden</span><span class="sxs-lookup"><span data-stu-id="0ddca-114">Using Remittance Advice Reports</span></span>
<span data-ttu-id="0ddca-115">Die folgende Tabelle beschreibt die Berichte, die Sie mit Zahlungsanzeigen verwenden können:</span><span class="sxs-lookup"><span data-stu-id="0ddca-115">The following table describes the reports that you can use with remittance advice:</span></span>

|<span data-ttu-id="0ddca-116">Bericht</span><span class="sxs-lookup"><span data-stu-id="0ddca-116">Report</span></span>|<span data-ttu-id="0ddca-117">Description</span><span class="sxs-lookup"><span data-stu-id="0ddca-117">Description</span></span>|
|----|----|
|<span data-ttu-id="0ddca-118">Rimessenavis – Erf.-Journal-Bericht</span><span class="sxs-lookup"><span data-stu-id="0ddca-118">Remittance Advice - Journal Report</span></span>|<span data-ttu-id="0ddca-119">Dieser Bericht zeigt, welche Belege in der Zahlung erfasst werden.</span><span class="sxs-lookup"><span data-stu-id="0ddca-119">This report indicates which documents are included in the payment.</span></span> <span data-ttu-id="0ddca-120">Für Fibu Erf.-Journalzeilen können Sie die Erf.-Journalvorlage und den Erf.-Journalnamen definieren, aus denen die Zahlungsanzeigen gedruckt werden, das Datum der ersten Aktivität, die gedruckt wird und den Filter auf einer Belegnummer.</span><span class="sxs-lookup"><span data-stu-id="0ddca-120">For general journal lines, you can specify the journal template and journal batch from which the remittance advices will be printed, the date of the first activity to print, and filter on a document number.</span></span> <span data-ttu-id="0ddca-121">Sie können die Anzahl der Kreditoren festlegen, die in den Bericht aufgenommen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="0ddca-121">For vendors, you can enter the vendor numbers to include in the report.</span></span> |
|<span data-ttu-id="0ddca-122">Rimessenavis – Eintragsbericht</span><span class="sxs-lookup"><span data-stu-id="0ddca-122">Remittance Advice - Entries Report</span></span>| <span data-ttu-id="0ddca-123">Dieser Bericht zeigt, welche Belege in der Zahlung erfasst werden.</span><span class="sxs-lookup"><span data-stu-id="0ddca-123">This report indicates which documents are included in the payment.</span></span> <span data-ttu-id="0ddca-124">Sie definieren die Berichtsinhalte, indem Sie Filter setzen.</span><span class="sxs-lookup"><span data-stu-id="0ddca-124">You define the report contents by setting filters.</span></span> <span data-ttu-id="0ddca-125">Sie können weitere Felder im Register einrichten, indem Sie das Feld **Feld** auswählen.</span><span class="sxs-lookup"><span data-stu-id="0ddca-125">You can set additional fields on the tab by choosing the **Field** field.</span></span> <span data-ttu-id="0ddca-126">Für Kreditorenposten können Sie die Kreditoren angeben, die im Bericht, in Datum der ersten zu druckenden Aktivität, in der Währung und der zu berücksichtigen Postennummer zu berücksichtigen sind.</span><span class="sxs-lookup"><span data-stu-id="0ddca-126">For vendor ledger entries, you can specify the vendors to include in the report, the date of the first activity to print, the currency, and the entry number to include.</span></span> |

> [!Note]
> <span data-ttu-id="0ddca-127">Die Zahlungsanzeige - Erf.-Journal-Bericht unterstützt keine Querwährungs-Anwendungsszenarien oder -Zahlungstoleranzen.</span><span class="sxs-lookup"><span data-stu-id="0ddca-127">The Remittance Advice - Journal Report does not support cross currency application scenarios or payment tolerances.</span></span> <span data-ttu-id="0ddca-128">Weitere Informationen finden Sie unter [So geht's: Anwendung von Kreditorenposten in unterschiedlichen Währungen aktivieren](finance-how-enable-application-ledger-entries-different-currencies.md)</span><span class="sxs-lookup"><span data-stu-id="0ddca-128">For more information, see [How to: Enable Application of Ledger Entries in Different Currencies](finance-how-enable-application-ledger-entries-different-currencies.md).</span></span>

> [!Tip]
> <span data-ttu-id="0ddca-129">Weitere Informationen darüber, wie Sie mit Berichten arbeiten, finden Sie unter [Anzeigen von Testberichten vor dem Buchen](ui-how-view-test-reports-posting.md) [Arbeiten mit Berichten](ui-work-report.md) und [Ermitteln, Filtern und Sortieren von Daten](ui-enter-criteria-filters.md).</span><span class="sxs-lookup"><span data-stu-id="0ddca-129">For more information about how to work with reports, see [Viewing Test Reports before Posting](ui-how-view-test-reports-posting.md), [Work with Reports](ui-work-report.md), and [Searching, Filtering, and Sorting Data](ui-enter-criteria-filters.md).</span></span>

##<a name="see-also"></a><span data-ttu-id="0ddca-130">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="0ddca-130">See Also</span></span>  
[<span data-ttu-id="0ddca-131">Willkommen bei Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="0ddca-131">Welcome to Dynamics NAV</span></span>](across-get-started.md)
