---
title: Importieren von ESR-Zahlungen
description: "Nach Eingang einer Zahlung eines Debitors erhalten Sie eine Datei mit Informationen zu bezahlten Rechnungen. Sie können diese Datei elektronisch von der Bank oder per E-Mail empfangen."
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: c69d1f8574a4d890904f2c5ee00983186d070d17
ms.contentlocale: de-ch
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-import-esr-payments"></a><span data-ttu-id="fc9fa-104">Gewusst wie: Importieren von ESR-Zahlungen</span><span class="sxs-lookup"><span data-stu-id="fc9fa-104">How to: Import ESR Payments</span></span>
<span data-ttu-id="fc9fa-105">Nach Eingang einer Zahlung eines Debitors erhalten Sie eine Datei mit Informationen zu bezahlten Rechnungen.</span><span class="sxs-lookup"><span data-stu-id="fc9fa-105">After you receive payment from a customer, you receive a file that contains information about paid invoices.</span></span> <span data-ttu-id="fc9fa-106">Sie können diese Datei elektronisch von der Bank oder per E-Mail empfangen.</span><span class="sxs-lookup"><span data-stu-id="fc9fa-106">You can receive this file from your bank electronically, or by mail.</span></span>  

<span data-ttu-id="fc9fa-107">Sie können die ESR (Einzahlungsschein mit Referenznummer)-Rechnungsdaten aus der Datei importieren, die Daten mithilfe des ESR-Berichts für Verkaufsrechnungen oder des ESR-Abschnittberichts drucken und diese vor der Buchung überprüfen.</span><span class="sxs-lookup"><span data-stu-id="fc9fa-107">You can import the Einzahlungsschein mit Referenznummer (ESR) invoice data from the file, print the data by using the sales invoice ESR report or the sales ESR coupon report, and verify before posting.</span></span> <span data-ttu-id="fc9fa-108">Weitere Informationen finden Sie unter [Gewusst wie: Drucken von ESR-Rechnungen](how-to-print-esr-invoices.md).</span><span class="sxs-lookup"><span data-stu-id="fc9fa-108">For more information, see [How to: Print ESR Invoices](how-to-print-esr-invoices.md).</span></span>  

## <a name="to-import-esr-payments"></a><span data-ttu-id="fc9fa-109">So importieren Sie ESR-Zahlungen</span><span class="sxs-lookup"><span data-stu-id="fc9fa-109">To import ESR payments</span></span>  

1.  <span data-ttu-id="fc9fa-110">Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und öffnen **Zlg.-Eing. Erfassungsjournale**. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="fc9fa-110">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cash Receipt Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="fc9fa-111">Wählen Sie im Feld **Erf.-Journalname** den erforderlichen Erf.-Journalnamen aus.</span><span class="sxs-lookup"><span data-stu-id="fc9fa-111">In the **Batch Name** field, select the required journal batch.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="fc9fa-112">Das Erfassungsjournal muss leer sein, bevor die ESR-Datei importiert werden kann.</span><span class="sxs-lookup"><span data-stu-id="fc9fa-112">The journal must be empty before you import the ESR file.</span></span> <span data-ttu-id="fc9fa-113">Sie können jeweils nur eine ESR-Datei in ein Zahlungseingangs Erf.-Journal importieren.</span><span class="sxs-lookup"><span data-stu-id="fc9fa-113">You cannot import more than one ESR file into the same cash receipt journal.</span></span>  

3.  <span data-ttu-id="fc9fa-114">Wählen Sie die Aktion **ESR-Datei lesen** aus.</span><span class="sxs-lookup"><span data-stu-id="fc9fa-114">Choose the **Read ESR File** action.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="fc9fa-115">Falls Sie mehr als eine ESR-Bank definiert haben, werden Sie in einer Warnmeldung zur Auswahl der entsprechenden Bank aufgefordert.</span><span class="sxs-lookup"><span data-stu-id="fc9fa-115">If you have defined more than one ESR bank, a warning message displays instructing you to choose the relevant bank.</span></span> <span data-ttu-id="fc9fa-116">Weitere Informationen finden Sie in der Tabelle "ESR Einrichtung".</span><span class="sxs-lookup"><span data-stu-id="fc9fa-116">For more information, see the ESR Setup table.</span></span>  

4.  <span data-ttu-id="fc9fa-117">Wählen Sie die Schaltfläche **Ja**, und wählen Sie dann die Schaltfläche **OK**.</span><span class="sxs-lookup"><span data-stu-id="fc9fa-117">Choose the **Yes** button, and then choose the **OK** button.</span></span>  

<span data-ttu-id="fc9fa-118">Die Zahlungsinformationen werden in die Journalzeilen importiert.</span><span class="sxs-lookup"><span data-stu-id="fc9fa-118">The payments information is imported to the journal lines.</span></span> <span data-ttu-id="fc9fa-119">Die Zahlungen werden automatisch für die jeweiligen Rechnungen entsprechend den eindeutigen ESR-Referenznummern übernommen.</span><span class="sxs-lookup"><span data-stu-id="fc9fa-119">The payments are automatically applied to the respective invoices according to unique ESR reference numbers.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fc9fa-120">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="fc9fa-120">See Also</span></span>  
 <span data-ttu-id="fc9fa-121">[Elektronische Zahlungen mit ESR (Schweiz)](swiss-electronic-payments-using-esr.md) </span><span class="sxs-lookup"><span data-stu-id="fc9fa-121">[Swiss Electronic Payments Using ESR](swiss-electronic-payments-using-esr.md) </span></span>  
 [<span data-ttu-id="fc9fa-122">Gewusst wie: Drucken von ESR-Rechnungen</span><span class="sxs-lookup"><span data-stu-id="fc9fa-122">How to: Print ESR Invoices</span></span>](how-to-print-esr-invoices.md)

