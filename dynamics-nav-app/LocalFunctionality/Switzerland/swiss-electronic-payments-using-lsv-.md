---
title: Elektronischer Zahlungsverkehr (Schweiz) mit LSV+
description: "Die elektronische Zahlungsmethode Lastschrift Verfahren (LSV+) oder Einzug, eine optimierte Version von LSV, ermöglicht Firmen das direkte Abrufen von Zahlungen von Debitorenbankkonten. Zum Abrufen von Debitorenzahlungen muss eine LSV-Datei an die Bank gesendet werden, die dann die Abbuchung der in der Datei angeforderten Zahlungen abwickelt."
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
ms.openlocfilehash: bde56909ab329a08cb29ae5a372eab2c81d4a2e9
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="swiss-electronic-payments-using-lsv"></a><span data-ttu-id="89d1c-104">Elektronischer Zahlungsverkehr (Schweiz) mit LSV+</span><span class="sxs-lookup"><span data-stu-id="89d1c-104">Swiss Electronic Payments Using LSV+</span></span>
<span data-ttu-id="89d1c-105">Die elektronische Zahlungsmethode Lastschrift Verfahren (LSV+) oder Einzug, eine optimierte Version von LSV, ermöglicht Firmen das direkte Abrufen von Zahlungen von Debitorenbankkonten.</span><span class="sxs-lookup"><span data-stu-id="89d1c-105">The Lastschrift Verfahren (LSV+)—or direct debit—electronic payment method, an improved version of LSV, allows companies to retrieve payments directly from its customers’ bank accounts.</span></span> <span data-ttu-id="89d1c-106">Zum Abrufen von Debitorenzahlungen muss eine LSV-Datei an die Bank gesendet werden, die dann die Abbuchung der in der Datei angeforderten Zahlungen abwickelt.</span><span class="sxs-lookup"><span data-stu-id="89d1c-106">To retrieve customer payments, you must send an LSV file to the bank, and the bank will collect the payments requested in the file.</span></span>  
  
 <span data-ttu-id="89d1c-107">Die LSV+-Methode ist ein Einzugsverfahren mit Recht auf Widerspruch.</span><span class="sxs-lookup"><span data-stu-id="89d1c-107">The LSV+ method is a direct debit principle with right of objection.</span></span> <span data-ttu-id="89d1c-108">BDD (Business Direct Debit) ist ein Einzugsverfahren ohne Recht auf Widerspruch.</span><span class="sxs-lookup"><span data-stu-id="89d1c-108">Business Direct Debit (BDD) is a direct debit system without right of objection.</span></span> <span data-ttu-id="89d1c-109">Die Formate der an die Bank gesendeten Dateien sind für LSV+ und BDD identisch.</span><span class="sxs-lookup"><span data-stu-id="89d1c-109">The file format to be sent to the bank is the same for LSV+ and BDD.</span></span>  
  
 <span data-ttu-id="89d1c-110">Bevor Sie das LSV-Modul verwenden, müssen die Einstellungen im Fenster **LSV Einrichtung** festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="89d1c-110">Before using the LSV module, you must define the settings in the **LSV Setup** window.</span></span> <span data-ttu-id="89d1c-111">Weitere Informationen finden Sie in der Tabelle "LSV Einrichtung".</span><span class="sxs-lookup"><span data-stu-id="89d1c-111">For more information, see the LSV Setup table.</span></span>  
  
## <a name="automatic-esr-processing"></a><span data-ttu-id="89d1c-112">Automatische ESR-Verarbeitung</span><span class="sxs-lookup"><span data-stu-id="89d1c-112">Automatic ESR Processing</span></span>  
 <span data-ttu-id="89d1c-113">Sie können Zahlungsgutschrifttransaktionen im Einzahlungsschein mit Referenznummer (ESR)-Dateiformat von der Bank herunterladen.</span><span class="sxs-lookup"><span data-stu-id="89d1c-113">You can download payment credit transactions in Einzahlungsschein mit Referenznummer (ESR) file format from the bank.</span></span> <span data-ttu-id="89d1c-114">Wenn die ESR-Referenznummer in das LSV+-System integriert ist, können Sie verarbeitete LSV-Zahlungen in der ESR-Datei erhalten.</span><span class="sxs-lookup"><span data-stu-id="89d1c-114">You can receive processed LSV payments in the ESR file if the ESR reference number is integrated with the LSV+ system.</span></span> <span data-ttu-id="89d1c-115">Wenn LSV+-Zahlungen in Ihren importierten LSV-Dateien enthalten sind, werden die entsprechenden LSV-Journalzeilen automatisch geschlossen.</span><span class="sxs-lookup"><span data-stu-id="89d1c-115">If LSV+ payments are included in your imported LSV files, the related LSV journal lines are closed automatically.</span></span> <span data-ttu-id="89d1c-116">Die automatische ESR-Verarbeitung wird nur bei Zahlungen in Schweizer Franken (CHF) durchgeführt. Hierzu müssen Sie folgende Schritte durchführen:</span><span class="sxs-lookup"><span data-stu-id="89d1c-116">Automatic ESR processing is performed only for payments that use Swiss Francs (CHF), and requires that you do the following:</span></span>  
  
-   <span data-ttu-id="89d1c-117">Nachdem Sie die LSV+-Datei an die Bank gesendet haben, übermitteln Sie innerhalb von drei Tagen nach dem angeforderten LSV-Verarbeitungsdatum einen Zahlungsbericht.</span><span class="sxs-lookup"><span data-stu-id="89d1c-117">After you have sent the LSV+ file to the bank, submit a payments report within three business days following the requested LSV processing date.</span></span>  
  
-   <span data-ttu-id="89d1c-118">Importieren Sie die ESR-Dateien, und buchen Sie die ESR-Journale.</span><span class="sxs-lookup"><span data-stu-id="89d1c-118">Import the ESR files, and post the ESR journals.</span></span> <span data-ttu-id="89d1c-119">Falls eine importierte ESR-Transaktion mit einer offenen LSV+-Zahlungszeile verknüpft ist, wird die entsprechende LSV-Journalzeile automatisch von ESR geschlossen.</span><span class="sxs-lookup"><span data-stu-id="89d1c-119">If an imported ESR transaction is related to an open LSV+ payment line, then the appropriate LSV journal line is automatically closed by ESR.</span></span>  
  
    > [!NOTE]  
    >  <span data-ttu-id="89d1c-120">Beim Importieren einer ESR-Datei wird die LSV-Journalzeile unabhängig vom ESR-Transaktionstyp von ESR geschlossen, falls das entsprechende LSV-Journal gefunden wird.</span><span class="sxs-lookup"><span data-stu-id="89d1c-120">When importing an ESR file, the LSV journal line is closed by ESR if the appropriate LSV journal is found, regardless of the ESR transaction type.</span></span>  
  
-   <span data-ttu-id="89d1c-121">Nach dem LSV-Verarbeitungsdatum können Sie die LSV-Journalzeilen überprüfen.</span><span class="sxs-lookup"><span data-stu-id="89d1c-121">After the LSV processing date, you can check the LSV journal lines.</span></span> <span data-ttu-id="89d1c-122">Wenn alle LSV-Journalzeilen geschlossen sind, wird der **LSV-Status** zu **Beendet** aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="89d1c-122">If all of the LSV journal lines are closed, then the status of the **LSV Status** field is updated to  **Finished**.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="89d1c-123">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="89d1c-123">See Also</span></span>  
 <span data-ttu-id="89d1c-124">[Gewusst wie: Verarbeiten eines LSV-Einzugs](how-to-process-an-lsv-collection.md) </span><span class="sxs-lookup"><span data-stu-id="89d1c-124">[How to: Process an LSV Collection](how-to-process-an-lsv-collection.md) </span></span>  
 <span data-ttu-id="89d1c-125">[Gewusst wie: Abschliessen eines LSV-Einzugs](how-to-close-an-lsv-collection.md) </span><span class="sxs-lookup"><span data-stu-id="89d1c-125">[How to: Close an LSV Collection](how-to-close-an-lsv-collection.md) </span></span>  
 <span data-ttu-id="89d1c-126">[Gewusst wie: Buchen von LSV+-Zahlungen](how-to-post-lsv-payments.md) </span><span class="sxs-lookup"><span data-stu-id="89d1c-126">[How to: Post LSV+ Payments](how-to-post-lsv-payments.md) </span></span>  
 <span data-ttu-id="89d1c-127">[Gewusst wie: Exportieren von Zahlungen mit LSV](how-to-export-payments-using-lsv.md) </span><span class="sxs-lookup"><span data-stu-id="89d1c-127">[How to: Export Payments Using LSV](how-to-export-payments-using-lsv.md) </span></span>  
 <span data-ttu-id="89d1c-128">[Elektronische Zahlungen (Schweiz)](swiss-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="89d1c-128">[Swiss Electronic Payments](swiss-electronic-payments.md) </span></span>  
 <span data-ttu-id="89d1c-129">[Elektronische Zahlungen mit DTA (Schweiz)](swiss-electronic-payments-using-dta.md) </span><span class="sxs-lookup"><span data-stu-id="89d1c-129">[Swiss Electronic Payments Using DTA](swiss-electronic-payments-using-dta.md) </span></span>  
 <span data-ttu-id="89d1c-130">[Elektronische Zahlungen mit ESR (Schweiz)](swiss-electronic-payments-using-esr.md) </span><span class="sxs-lookup"><span data-stu-id="89d1c-130">[Swiss Electronic Payments Using ESR](swiss-electronic-payments-using-esr.md) </span></span>  
 <span data-ttu-id="89d1c-131">LSV Einrichtung</span><span class="sxs-lookup"><span data-stu-id="89d1c-131">LSV Setup</span></span>
