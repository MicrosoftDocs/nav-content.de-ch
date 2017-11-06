---
title: Exportieren von Zahlungen mit EZAG
description: "Sie können eine Datei für elektronische Zahlung mithilfe der EZAG (Elektronischer Zahlungsauftrag)-Methode generieren und sie exportieren, damit sie von der Bank für Zahlungen verwendet werden."
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
ms.openlocfilehash: 856a98e6c4d0f8820fa993deac3d44898f9420b3
ms.contentlocale: de-ch
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-export-payments-using-ezag"></a><span data-ttu-id="5068a-103">Gewusst wie: Exportieren von Zahlungen mit EZAG</span><span class="sxs-lookup"><span data-stu-id="5068a-103">How to: Export Payments Using EZAG</span></span>
<span data-ttu-id="5068a-104">Sie können eine Datei für elektronische Zahlung mithilfe der EZAG (Elektronischer Zahlungsauftrag)-Methode generieren und sie exportieren, damit sie von der Bank für Zahlungen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="5068a-104">You can generate a file for electronic payment using the Elektronischer Zahlungsauftrag (EZAG) method, and export it for the bank to use for the payments.</span></span>  

## <a name="to-export-payments-using-ezag"></a><span data-ttu-id="5068a-105">So exportieren Sie Zahlungen mit EZAG</span><span class="sxs-lookup"><span data-stu-id="5068a-105">To export payments using EZAG</span></span>  

1.  <span data-ttu-id="5068a-106">Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Zahlungs-Buchblatt** ein und wählen den zugehörenden Link aus.</span><span class="sxs-lookup"><span data-stu-id="5068a-106">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="5068a-107">Wählen Sie im Feld **Erf.-Journalname** den Erf.-Journalnamen aus.</span><span class="sxs-lookup"><span data-stu-id="5068a-107">In the **Batch Name** field, select the journal batch name.</span></span>  
3.  <span data-ttu-id="5068a-108">Wählen Sie die Aktion **EZAG-Datei erstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="5068a-108">Choose the **Generate EZAG File** action.</span></span>  
4.  <span data-ttu-id="5068a-109">Füllen Sie im Stapelverarbeitungsauftrag **EZAG Datei** die Felder auf dem Inforegister **Optionen** wie in der folgenden Tabelle beschrieben aus.</span><span class="sxs-lookup"><span data-stu-id="5068a-109">In the **EZAG File** batch job, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="5068a-110">Feld</span><span class="sxs-lookup"><span data-stu-id="5068a-110">Field</span></span>|<span data-ttu-id="5068a-111">Description</span><span class="sxs-lookup"><span data-stu-id="5068a-111">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="5068a-112">**Belastung auf Bank**</span><span class="sxs-lookup"><span data-stu-id="5068a-112">**Debit to bank**</span></span>|<span data-ttu-id="5068a-113">Geben Sie den Code der zu belastenden Bank an.</span><span class="sxs-lookup"><span data-stu-id="5068a-113">Specify the code of the bank to be charged.</span></span>|  
    |<span data-ttu-id="5068a-114">**Sammelzahlung pro Kreditor**</span><span class="sxs-lookup"><span data-stu-id="5068a-114">**Combined payment for vendor**</span></span>|<span data-ttu-id="5068a-115">Geben Sie an, ob die Zahlungszeilen in der generierten EZAG-Datei, die den gleichen Kreditor, die gleiche Währung, die gleiche Bank und die gleiche Belastungsbank besitzen, kombiniert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="5068a-115">Specify if the payment lines that have the same vendor, currency, bank, and debit bank in the generated EZAG file will be combined.</span></span>|  
    |<span data-ttu-id="5068a-116">**Versand per Diskette**</span><span class="sxs-lookup"><span data-stu-id="5068a-116">**Shipment with disk**</span></span>|<span data-ttu-id="5068a-117">Geben Sie an, ob die EZAG-Datei auf einem Datenträger gespeichert werden soll, damit Sie sie der Bank zukommen lassen können.</span><span class="sxs-lookup"><span data-stu-id="5068a-117">Specify if the EZAG file will be saved to a disk so that you can deliver it to the bank.</span></span>|  

5.  <span data-ttu-id="5068a-118">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="5068a-118">Choose the **OK** button.</span></span> <span data-ttu-id="5068a-119">Die EZAG-Datei wird generiert.</span><span class="sxs-lookup"><span data-stu-id="5068a-119">The EZAG file is generated.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5068a-120">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="5068a-120">See Also</span></span>  
 <span data-ttu-id="5068a-121">[Elektronische Zahlungen mit DTA (Schweiz)](swiss-electronic-payments-using-dta.md) </span><span class="sxs-lookup"><span data-stu-id="5068a-121">[Swiss Electronic Payments Using DTA](swiss-electronic-payments-using-dta.md) </span></span>  
 <span data-ttu-id="5068a-122">[Gewusst wie: Vorschlagen einer DTA-Zahlung für Kreditoren](how-to-suggest-dta-payment-for-vendors.md) </span><span class="sxs-lookup"><span data-stu-id="5068a-122">[How to: Suggest DTA Payment for Vendors](how-to-suggest-dta-payment-for-vendors.md) </span></span>  
 <span data-ttu-id="5068a-123">[Gewusst wie: Überprüfen einer Liste von Kreditoren für DTA-Zahlungen](how-to-verify-a-list-of-vendors-for-dta-payments.md) </span><span class="sxs-lookup"><span data-stu-id="5068a-123">[How to: Verify a List of Vendors for DTA Payments](how-to-verify-a-list-of-vendors-for-dta-payments.md) </span></span>  
 [<span data-ttu-id="5068a-124">Gewusst wie: Senden von DTA-Zahlungen</span><span class="sxs-lookup"><span data-stu-id="5068a-124">How to: Submit DTA Payments</span></span>](how-to-submit-dta-payments.md) 

