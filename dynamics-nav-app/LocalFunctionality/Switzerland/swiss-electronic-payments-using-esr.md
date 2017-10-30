---
title: Elektronischer Zahlungsverkehr (Schweiz) mit ESR
description: "Die elektronische Zahlungsform \"Einzahlungsschein mit Referenznummer\" (ESR) ist ein elektronischer Debitorendienst, mit dem der Debitor offene Rechnungen in Schweizer Franken (CHF) und Euro (EUR) fakturieren und eingehende Zahlungen effizient buchen kann. Die Referenznummer oder Codezeile enthält alle relevanten Buchhaltungsdaten."
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
ms.openlocfilehash: 9063443b4efc8275aa487406c8c34f00d6b52782
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="swiss-electronic-payments-using-esr"></a><span data-ttu-id="74ced-104">Elektronischer Zahlungsverkehr (Schweiz) mit ESR</span><span class="sxs-lookup"><span data-stu-id="74ced-104">Swiss Electronic Payments Using ESR</span></span>
<span data-ttu-id="74ced-105">Die elektronische Zahlungsform "Einzahlungsschein mit Referenznummer" (ESR) ist ein elektronischer Debitorendienst, mit dem der Debitor offene Rechnungen in Schweizer Franken (CHF) und Euro (EUR) fakturieren und eingehende Zahlungen effizient buchen kann.</span><span class="sxs-lookup"><span data-stu-id="74ced-105">The Einzahlungsschein mit Referenznummer (ESR) electronic payment method is an electronic debtor service that allows the customer to bill open invoices in Swiss Francs (CHF) and Euros (EUR), and to post incoming payments efficiently.</span></span> <span data-ttu-id="74ced-106">Die Referenznummer oder Codezeile enthält alle relevanten Buchhaltungsdaten.</span><span class="sxs-lookup"><span data-stu-id="74ced-106">The reference number, or code line, contains all relevant bookkeeping data.</span></span>  
  
 <span data-ttu-id="74ced-107">Elektronische Zahlungen mittels ESR bieten folgende Möglichkeiten:</span><span class="sxs-lookup"><span data-stu-id="74ced-107">With ESR electronic payments, you can do the following:</span></span>  
  
-   <span data-ttu-id="74ced-108">Senden Sie ESR-Einzahlungsscheine mit eindeutigen Referenznummern auf den Rechnungen.</span><span class="sxs-lookup"><span data-stu-id="74ced-108">Send ESR payment slips with unique reference numbers on the invoices.</span></span> <span data-ttu-id="74ced-109">Durch die eindeutigen ESR-Referenznummern werden mit den Ausgleichszahlungen automatisch die zugehörigen Rechnungen ausgeglichen.</span><span class="sxs-lookup"><span data-stu-id="74ced-109">Because of the unique ESR reference numbers, the payments for settlement are automatically applied to the related invoices.</span></span> <span data-ttu-id="74ced-110">Weitere Informationen finden Sie unter [Gewusst wie: Drucken von ESR-Rechnungen](how-to-print-esr-invoices.md).</span><span class="sxs-lookup"><span data-stu-id="74ced-110">For more information, see [How to: Print ESR Invoices](how-to-print-esr-invoices.md).</span></span>  
  
-   <span data-ttu-id="74ced-111">Laden Sie die ESR-Dateien täglich von der Bank herunter.</span><span class="sxs-lookup"><span data-stu-id="74ced-111">Download the ESR files from the bank daily.</span></span> <span data-ttu-id="74ced-112">Die Dateien enthalten Informationen zu allen bezahlten Rechnungen.</span><span class="sxs-lookup"><span data-stu-id="74ced-112">The files contain information about all paid invoices.</span></span>  
  
-   <span data-ttu-id="74ced-113">Importieren Sie die ESR-Dateien, und erstellen Sie automatisch für jede Zahlung Zahlungszeilen.</span><span class="sxs-lookup"><span data-stu-id="74ced-113">Import the ESR files and create payment lines automatically for each payment.</span></span> <span data-ttu-id="74ced-114">Weitere Informationen finden Sie unter [Gewusst wie: Importieren von ESR-Zahlungen](how-to-import-esr-payments.md).</span><span class="sxs-lookup"><span data-stu-id="74ced-114">For more information, see [How to: Import ESR Payments](how-to-import-esr-payments.md).</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="74ced-115">Vor der Verwendung des ESR-Moduls müssen die Bank, das Bankkonto und der Dateiname eingerichtet werden.</span><span class="sxs-lookup"><span data-stu-id="74ced-115">Before you can use the ESR module, you must set up the bank, bank account, and file name.</span></span> <span data-ttu-id="74ced-116">Sie müssen auch festlegen, ob ESR oder ESR+ verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="74ced-116">You must also specify whether ESR or ESR+ should be used.</span></span> <span data-ttu-id="74ced-117">Weitere Informationen finden Sie in der Tabelle "ESR Einrichtung".</span><span class="sxs-lookup"><span data-stu-id="74ced-117">For more information, see the ESR Setup table.</span></span>  
  
 <span data-ttu-id="74ced-118">Nachdem Sie die Einrichtungsinformationen überprüft haben, können Sie das Rechnungsformular anpassen und eine Testserie erstellen, die von der Bank oder dem Postdienst überprüft werden kann.</span><span class="sxs-lookup"><span data-stu-id="74ced-118">When you have evaluated the setup information, you can adjust the invoice form, and you can create a test series that you can ask your bank or postal service to validate.</span></span>  
  
 <span data-ttu-id="74ced-119">Beachten Sie beim Einrichten von Nummernserien für Rechnungen die folgenden Richtlinien:</span><span class="sxs-lookup"><span data-stu-id="74ced-119">When you set up number series for invoices, you must follow these guidelines:</span></span>  
  
-   <span data-ttu-id="74ced-120">Verwenden Sie maximal acht Ziffern.</span><span class="sxs-lookup"><span data-stu-id="74ced-120">Use a maximum of eight digits.</span></span>  
  
-   <span data-ttu-id="74ced-121">Verwenden Sie nur numerische Zeichen.</span><span class="sxs-lookup"><span data-stu-id="74ced-121">Use only numeric characters.</span></span>  
  
-   <span data-ttu-id="74ced-122">Stellen Sie den Nummern keine Nullen voran.</span><span class="sxs-lookup"><span data-stu-id="74ced-122">Do not precede numbers with zeros.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="74ced-123">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="74ced-123">See Also</span></span>  
 <span data-ttu-id="74ced-124">[Elektronische Zahlungen (Schweiz)](swiss-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="74ced-124">[Swiss Electronic Payments](swiss-electronic-payments.md) </span></span>  
 <span data-ttu-id="74ced-125">[Gewusst wie: Drucken von ESR-Rechnungen](how-to-print-esr-invoices.md) </span><span class="sxs-lookup"><span data-stu-id="74ced-125">[How to: Print ESR Invoices](how-to-print-esr-invoices.md) </span></span>  
 <span data-ttu-id="74ced-126">[Gewusst wie: Importieren von ESR-Zahlungen](how-to-import-esr-payments.md) </span><span class="sxs-lookup"><span data-stu-id="74ced-126">[How to: Import ESR Payments](how-to-import-esr-payments.md) </span></span>  
 <span data-ttu-id="74ced-127">[Elektronische Zahlungen mit DTA (Schweiz)](swiss-electronic-payments-using-dta.md) </span><span class="sxs-lookup"><span data-stu-id="74ced-127">[Swiss Electronic Payments Using DTA](swiss-electronic-payments-using-dta.md) </span></span>  
 <span data-ttu-id="74ced-128">[Elektronische Zahlungen mit LSV+ (Schweiz)](swiss-electronic-payments-using-lsv-.md) </span><span class="sxs-lookup"><span data-stu-id="74ced-128">[Swiss Electronic Payments Using LSV+](swiss-electronic-payments-using-lsv-.md) </span></span>  
 <span data-ttu-id="74ced-129">ESR Einrichtung</span><span class="sxs-lookup"><span data-stu-id="74ced-129">ESR Setup</span></span>   
 <span data-ttu-id="74ced-130">Nr.</span><span class="sxs-lookup"><span data-stu-id="74ced-130">No.</span></span> <span data-ttu-id="74ced-131">Serien</span><span class="sxs-lookup"><span data-stu-id="74ced-131">Series</span></span>
