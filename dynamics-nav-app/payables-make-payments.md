---
title: Zahlungen vornehmen
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 67d948dab76ca7533604025fb53b37aff84bbc11
ms.contentlocale: de-ch
ms.lasthandoff: 07/19/2017

---

# <a name="make-payments"></a><span data-ttu-id="45805-102">Zahlungen vornehmen</span><span class="sxs-lookup"><span data-stu-id="45805-102">Make Payments</span></span>
<span data-ttu-id="45805-103">Wenn Sie Zahlungen an Kreditoren leisten, buchen Sie die jeweiligen Zahlungszeilen im **Zahlungsausgangs-Erfassungsjournal**-Fenster.</span><span class="sxs-lookup"><span data-stu-id="45805-103">When you make payments to vendors, you post the related payment lines in the **Payment Journal** window.</span></span> <span data-ttu-id="45805-104">Verwenden Sie zum Suchen fälliger Zahlungen im Zahlungsausgangs Buch.-Blatt die Funktion **Zahlungsvorschlag**.</span><span class="sxs-lookup"><span data-stu-id="45805-104">You can use the **Suggest Vendor Payments** function to find payments that are due.</span></span> <span data-ttu-id="45805-105">Darüber hinaus können Sie sich mithilfe des Berichts **Kreditor - Saldo nach Perioden** einen Überblick über die fälligen Zahlungen verschaffen.</span><span class="sxs-lookup"><span data-stu-id="45805-105">You can also use the **Vendor - Summary Aging** report to get an overview of due payments.</span></span>

<span data-ttu-id="45805-106">Im Zahlungsausgangs-Erfassungsjournal können Sie Computerschecks drucken sowie ausgestellte Schecks erfassen.</span><span class="sxs-lookup"><span data-stu-id="45805-106">From the payment journal, you can print computer checks or record when checks are written.</span></span> <span data-ttu-id="45805-107">Wenn Sie **Computer Scheck** im Feld **Bankkontozahlungsart** wählen, dann müssen alle Posten für Schecks gedruckt werden, damit die Erfassungsjournalzeilen gebucht werden können.</span><span class="sxs-lookup"><span data-stu-id="45805-107">If you select **Computer Check** in the **Bank Payment Type** field, then any lines representing checks must be printed before the payment journal can be posted.</span></span>

<span data-ttu-id="45805-108">Wenn Zahlungen gebucht werden, exportieren Sie sie in eine Bankdatei für den Upload zu Ihrer Bank zur Verarbeitung.</span><span class="sxs-lookup"><span data-stu-id="45805-108">When the payments are posted, you can export them to a bank file for upload to your bank for processing.</span></span>

<span data-ttu-id="45805-109">Nachdem die Zahlungen in Ihrer Bank getätigt wurden, müssen Sie diese in ihre entsprechenden offenen Kreditorenposten ausgleichen.</span><span class="sxs-lookup"><span data-stu-id="45805-109">After the payments are made at your bank, you must apply them to their related open vendor ledger entries.</span></span> <span data-ttu-id="45805-110">Sie können dies manuell oder über den Import in eine Bankkontoauszugsdatei und das Automatische Ausgleichen der Zahlungen durchführen.</span><span class="sxs-lookup"><span data-stu-id="45805-110">You can do this manually or by importing a bank statement file and applying the payments automatically.</span></span> <span data-ttu-id="45805-111">Weitere Informationen finden Sie beispielsweise unter [Zahlungen automatisch vornehmen und Bankkonten abstimmen](receivables-apply-payments-auto-reconcile-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="45805-111">For more information, see, for example, [Apply Payments Automatically and Reconcile Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md).</span></span>

<span data-ttu-id="45805-112">In der folgenden Tabelle wird eine Reihe von Aufgaben mit Verknüpfungen zu den beschriebenen Themen erläutert.</span><span class="sxs-lookup"><span data-stu-id="45805-112">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="45805-113">Aktion</span><span class="sxs-lookup"><span data-stu-id="45805-113">To</span></span> |<span data-ttu-id="45805-114">Informationen</span><span class="sxs-lookup"><span data-stu-id="45805-114">See</span></span> |
|---|----|
|<span data-ttu-id="45805-115">Verwenden Sie die Funktion, um Kreditorenzahlungen entsprechend gewählten Kriterien, wie Fälligkeitsdatum, Skontoeignung und Ihrer Liquidität vorzuschlagen.</span><span class="sxs-lookup"><span data-stu-id="45805-115">Use a function to suggest vendor payments according to selected criteria, such as due date, discount eligibility, and your liquidity.</span></span>|[<span data-ttu-id="45805-116">Vorgehensweise: Erstellen von Zahlungsvorschlägen für Kreditoren</span><span class="sxs-lookup"><span data-stu-id="45805-116">How to: Suggest Vendor Payments</span></span>](payables-how-suggest-vendor-payments.md)|
|<span data-ttu-id="45805-117">Stellen Sie Schecks für Zahlungen entweder als Ausdruck oder als Computer Schecks aus.</span><span class="sxs-lookup"><span data-stu-id="45805-117">Issue checks for payments, either as print-outs or as computer checks.</span></span> <span data-ttu-id="45805-118">Annullieren Sie Schecks vor oder nach dem Buchen.</span><span class="sxs-lookup"><span data-stu-id="45805-118">Void checks before or after posting.</span></span>|[<span data-ttu-id="45805-119">So gehts: Arbeiten mit Schecks</span><span class="sxs-lookup"><span data-stu-id="45805-119">How to: Work With Checks</span></span>](payables-how-work-checks.md)|
|<span data-ttu-id="45805-120">Exportierten Sie Zahlungen aus dem Fenster **Zahlungsausgangs-Erfassungsjournal** in eine Bankdatei, die Sie auf Ihr elektronisches Bankkonto zur Verarbeitung hochladen.</span><span class="sxs-lookup"><span data-stu-id="45805-120">Export payments from the **Payment Journal** window to a bank file that you upload to your bank for processing.</span></span>|[<span data-ttu-id="45805-121">Vorgehensweise: Zahlungen in eine Bankdatei exportieren</span><span class="sxs-lookup"><span data-stu-id="45805-121">How to: Export Payments to a Bank File</span></span>](payables-how-export-payments-bank-file.md)|

## <a name="see-also"></a><span data-ttu-id="45805-122">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="45805-122">See Also</span></span>
[<span data-ttu-id="45805-123">Verwalten von Verbindlichkeiten</span><span class="sxs-lookup"><span data-stu-id="45805-123">Manage Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="45805-124">Einkauf verwalten</span><span class="sxs-lookup"><span data-stu-id="45805-124">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="45805-125">Verwalten von Forderungen</span><span class="sxs-lookup"><span data-stu-id="45805-125">Manage Receivables</span></span>](receivables-manage-receivables.md)

