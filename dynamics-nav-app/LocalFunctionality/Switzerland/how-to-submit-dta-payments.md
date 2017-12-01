---
title: "Gewusst wie: Übermitteln Sie DTA-Zahlungen"
description: "Um Datenträgeraustausch-Zahlungen (DTA) an Ihre Bank für Zahlung zu buchen, müssen Sie einige Aufgaben ausführen."
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
ms.openlocfilehash: 81e10c740ffe491338fc1d94fea6ef00ec930d3c
ms.contentlocale: de-ch
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-submit-dta-payments"></a><span data-ttu-id="0cd65-103">Gewusst wie: Senden von DTA-Zahlungen</span><span class="sxs-lookup"><span data-stu-id="0cd65-103">How to: Submit DTA Payments</span></span>
<span data-ttu-id="0cd65-104">Um Datenträgeraustausch-Zahlungen (DTA) an Ihre Bank für Zahlung zu buchen, müssen Sie Folgendes tun:</span><span class="sxs-lookup"><span data-stu-id="0cd65-104">To submit DatenTrägerAustausch (DTA) payments to your bank for payment, you must do the following:</span></span>  

- <span data-ttu-id="0cd65-105">Generieren einer DTA-Datei für elektronische Zahlung, nachdem Sie die Zahlungsavis gedruckt haben.</span><span class="sxs-lookup"><span data-stu-id="0cd65-105">Generate a DTA file for electronic payment after printing the payment advice.</span></span>  
- <span data-ttu-id="0cd65-106">DTA-Zahlungsauftrag drucken.</span><span class="sxs-lookup"><span data-stu-id="0cd65-106">Print the DTA payment order.</span></span>  

<span data-ttu-id="0cd65-107">Bevor Sie DTA-Zahlungen buchen, müssen Sie die Liste von Kreditoren für DTA-Zahlung prüfen.</span><span class="sxs-lookup"><span data-stu-id="0cd65-107">Before you submit DTA payments, you must verify the list of vendors for DTA payment.</span></span> <span data-ttu-id="0cd65-108">Weitere Informationen finden Sie unter [Gewusst wie: Überprüfen einer Liste von Kreditoren für DTA-Zahlungen](how-to-verify-a-list-of-vendors-for-dta-payments.md).</span><span class="sxs-lookup"><span data-stu-id="0cd65-108">For more information, see [How to: Verify a List of Vendors for DTA Payments](how-to-verify-a-list-of-vendors-for-dta-payments.md).</span></span>  

<span data-ttu-id="0cd65-109">Sie können das Erf.-Journal buchen, nachdem die Bankzahlungen vollständig sind.</span><span class="sxs-lookup"><span data-stu-id="0cd65-109">You can post the payment journal after the bank payments are complete.</span></span> <span data-ttu-id="0cd65-110">Sie können im Zahlungsausgangs-Erfassungsjournal DTA-Zahlungen auf Grundlage gebuchter Rechnungen vorschlagen lassen.</span><span class="sxs-lookup"><span data-stu-id="0cd65-110">In the payment journal, you can have the DTA payments suggested based on posted invoices.</span></span> <span data-ttu-id="0cd65-111">Die vorgeschlagenen Zahlungen enthalten Informationen zum Kreditor und zur externen Belegnummer und können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="0cd65-111">The suggested payments contain vendor and external document number information, and can be modified.</span></span> <span data-ttu-id="0cd65-112">Weitere Informationen finden Sie unter [Gewusst wie: Vorschlagen einer DTA-Zahlung für Kreditoren](how-to-suggest-dta-payment-for-vendors.md).</span><span class="sxs-lookup"><span data-stu-id="0cd65-112">For more information, see [How to: Suggest DTA Payment for Vendors](how-to-suggest-dta-payment-for-vendors.md).</span></span>  

## <a name="to-generate-a-dta-file"></a><span data-ttu-id="0cd65-113">So generieren Sie eine DTA-Datei</span><span class="sxs-lookup"><span data-stu-id="0cd65-113">To generate a DTA file</span></span>  

1.  <span data-ttu-id="0cd65-114">Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Zahlungs-Buchblatt** ein und wählen den zugehörenden Link aus.</span><span class="sxs-lookup"><span data-stu-id="0cd65-114">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="0cd65-115">Wählen Sie im Feld **Erf.-Journalname** den erforderlichen Erf.-Journalnamen aus.</span><span class="sxs-lookup"><span data-stu-id="0cd65-115">In the **Batch Name** field, select the required journal batch.</span></span>  
3.  <span data-ttu-id="0cd65-116">Wählen Sie die Art aus, den Sie erstellen möchten beispielsweise eine DTA-Datei und dann die Aktion **DTA-Datei generieren** auswählen.</span><span class="sxs-lookup"><span data-stu-id="0cd65-116">Select the payment entry that you want to generate as a DTA file, and then choose the **Generate DTA File** action.</span></span>  
4.  <span data-ttu-id="0cd65-117">Füllen Sie im Stapelverarbeitungsauftrag **DTA Datei** die Felder wie in der folgenden Tabelle beschrieben aus.</span><span class="sxs-lookup"><span data-stu-id="0cd65-117">In the **DTA File** batch job, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="0cd65-118">Feld</span><span class="sxs-lookup"><span data-stu-id="0cd65-118">Field</span></span>|<span data-ttu-id="0cd65-119">Description</span><span class="sxs-lookup"><span data-stu-id="0cd65-119">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="0cd65-120">**DTA Bank für Datei**</span><span class="sxs-lookup"><span data-stu-id="0cd65-120">**DTA Bank for File**</span></span>|<span data-ttu-id="0cd65-121">Wählen Sie die DTA-Bankleitzahl, aus der die Daten für den gewünschten Namen und die Sicherungskopie übertragen werden müssen.</span><span class="sxs-lookup"><span data-stu-id="0cd65-121">Select the DTA bank code from which the information for the file name and backup copy is to be transferred.</span></span> <span data-ttu-id="0cd65-122">Dieses Feld nutzt die Hauptbankadresse als Vorgabe, Sie können diese Informationen ändern, wenn Sie möchten.</span><span class="sxs-lookup"><span data-stu-id="0cd65-122">This field uses the main bank name as the default, but you can modify this information if you want.</span></span>|  
    |<span data-ttu-id="0cd65-123">**Sammelzahlung pro Kreditor**</span><span class="sxs-lookup"><span data-stu-id="0cd65-123">**Combined payment for vendor**</span></span>|<span data-ttu-id="0cd65-124">Geben Sie an, ob die Zahlungszeilen, die denselben Kreditor haben, Währung, Bank und gutzuschreibende Bank in der erzeugten DTA-Datei zusammenfassen soll.</span><span class="sxs-lookup"><span data-stu-id="0cd65-124">Specify if the payment lines that have the same vendor, currency, bank, and debit bank will be combined in the generated DTA file.</span></span>|  

5.  <span data-ttu-id="0cd65-125">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="0cd65-125">Choose the **OK** button.</span></span> <span data-ttu-id="0cd65-126">Die DTA-Datei wird im angegebenen Ordner erstellt.</span><span class="sxs-lookup"><span data-stu-id="0cd65-126">The DTA file is generated in the predetermined folder.</span></span>  

<span data-ttu-id="0cd65-127">Nachdem Sie die DTA-Datei generiert haben, können Sie den DTA-Vergütungsauftrag ausdrucken und sowohl die Datei als auch den Vergütungsauftrag an die Bank übertragen.</span><span class="sxs-lookup"><span data-stu-id="0cd65-127">After you have generated the DTA file, you can print the DTA payment order and transfer both the file and the payment order to your bank.</span></span> <span data-ttu-id="0cd65-128">Im DTA-Vergütungsauftrag sind alle vorgeschlagenen Kreditorenzahlungen in einem Fenster **Zahlungsausgangs Erf.-Journal** basierend auf dem Währungscode aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="0cd65-128">The DTA payment order lists all suggested vendor payments in a **Payment Journal** window based on currency code.</span></span> <span data-ttu-id="0cd65-129">Dieser Auftrag wird an die Bank gesendet, um die DTA-Datei zur Zahlung freizugeben.</span><span class="sxs-lookup"><span data-stu-id="0cd65-129">This order is sent to the bank to release the DTA file for payment.</span></span>  

## <a name="to-print-a-dta-payment-order"></a><span data-ttu-id="0cd65-130">So drucken Sie einen DTA-Vergütungsauftrag</span><span class="sxs-lookup"><span data-stu-id="0cd65-130">To print a DTA payment order</span></span>  

1.  <span data-ttu-id="0cd65-131">Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Zahlungs-Buchblatt** ein und wählen den zugehörenden Link aus.</span><span class="sxs-lookup"><span data-stu-id="0cd65-131">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="0cd65-132">Wählen Sie im Feld **Erf.-Journalname** den erforderlichen Erf.-Journalnamen aus.</span><span class="sxs-lookup"><span data-stu-id="0cd65-132">In the **Batch Name** field, select the required journal batch.</span></span>  
3.  <span data-ttu-id="0cd65-133">Wählen Sie die erforderliche vorgeschlagene Zahlungszeilen aus, und wählen Sie die Aktion **Vorgeschlagener DTA-Zahlungsauftrag** aus.</span><span class="sxs-lookup"><span data-stu-id="0cd65-133">Select the required payment entry, and then choose the **DTA Payment Order** action.</span></span>  
4.  <span data-ttu-id="0cd65-134">Geben Sie im Feld **Nachricht** eine Nachricht an die Bank ein, die unten auf dem Vergütungsauftrag ausgedruckt wird.</span><span class="sxs-lookup"><span data-stu-id="0cd65-134">In the **Message** field, enter a message for the bank, to be printed at the bottom of the payment order.</span></span>  
5.  <span data-ttu-id="0cd65-135">Wählen Sie die Schaltfläche **Drucken** aus, um den DTA-Zahlungsbericht zu drucken, oder die Schaltfläche **Vorschau**, um den Bericht auf dem Bildschirm anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="0cd65-135">Choose the **Print** button to print the DTA payment order or choose the **Preview** button to view it on the screen.</span></span>  

    <span data-ttu-id="0cd65-136">Sie müssen den DTA-Zahlungsauftrag und die DTA-Datei für die Bank buchen, in der Zahlungen an Kreditoren in mehrere Stunden freigegeben werden.</span><span class="sxs-lookup"><span data-stu-id="0cd65-136">You must submit the DTA payment order and the DTA file to the bank, where payments to the vendors are released in a few hours.</span></span> <span data-ttu-id="0cd65-137">Nachdem die Zahlungen von der Bank verarbeitet wurden, können Sie das Zahlungsjournal buchen.</span><span class="sxs-lookup"><span data-stu-id="0cd65-137">After the payments have been processed by the bank, you can post the payment journal.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0cd65-138">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="0cd65-138">See Also</span></span>  
 <span data-ttu-id="0cd65-139">[Elektronische Zahlungen mit DTA (Schweiz)](swiss-electronic-payments-using-dta.md) </span><span class="sxs-lookup"><span data-stu-id="0cd65-139">[Swiss Electronic Payments Using DTA](swiss-electronic-payments-using-dta.md) </span></span>  
 <span data-ttu-id="0cd65-140">[Gewusst wie: Vorschlagen einer DTA-Zahlung für Kreditoren](how-to-suggest-dta-payment-for-vendors.md) </span><span class="sxs-lookup"><span data-stu-id="0cd65-140">[How to: Suggest DTA Payment for Vendors](how-to-suggest-dta-payment-for-vendors.md) </span></span>  
 <span data-ttu-id="0cd65-141">[Gewusst wie: Überprüfen einer Liste von Kreditoren für DTA-Zahlungen](how-to-verify-a-list-of-vendors-for-dta-payments.md) </span><span class="sxs-lookup"><span data-stu-id="0cd65-141">[How to: Verify a List of Vendors for DTA Payments](how-to-verify-a-list-of-vendors-for-dta-payments.md) </span></span>  
 [<span data-ttu-id="0cd65-142">Gewusst wie: Exportieren von Zahlungen mit EZAG</span><span class="sxs-lookup"><span data-stu-id="0cd65-142">How to: Export Payments Using EZAG</span></span>](how-to-export-payments-using-ezag.md)

