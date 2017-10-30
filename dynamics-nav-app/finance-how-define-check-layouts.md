---
title: Geben Sie das Layout eines Schecks an
description: "Sie können Ihre Checks entwerfen und srucken in unterschiedliche Formaten, um Standardwerten zu entsprechen."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, customize
ms.date: 06/15/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d99326be66bf16a4a756d9f78e11f9af37e11fbd
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-define-check-layouts"></a><span data-ttu-id="c2dee-103">Gewusst wie: Definieren von Scheck-Layouts</span><span class="sxs-lookup"><span data-stu-id="c2dee-103">How to: Define Check Layouts</span></span>
<span data-ttu-id="c2dee-104">Sie können Ihre Schecks entwerfen, um sie den Vorgaben anzupassen, die von den lokalen Behörden festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="c2dee-104">You can design your checks to conform with the standards set by the local authorities.</span></span> <span data-ttu-id="c2dee-105">Scheckbilder können in Englisch, Französisch oder Spanisch gedruckt werden.</span><span class="sxs-lookup"><span data-stu-id="c2dee-105">Check images can be printed in English, French, or Spanish.</span></span>

<span data-ttu-id="c2dee-106">Schecks können sowohl im USA- als auch im Kanada-Schecklayout, entweder im Scheck/Formular/Scheck-Format oder im Formular/Formular/Scheck-Format gedruckt werden.</span><span class="sxs-lookup"><span data-stu-id="c2dee-106">Checks are designed to print in both the United States and Canadian check image formats in either a check-stub-check format or a stub-stub-check format.</span></span>

## <a name="to-define-check-layouts"></a><span data-ttu-id="c2dee-107">So definieren Sie Schecklayouts</span><span class="sxs-lookup"><span data-stu-id="c2dee-107">To define check layouts</span></span>
1. <span data-ttu-id="c2dee-108">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "") Nach Seite oder Bericht suchen und geben **Berichtsauswahl Bankkonto** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="c2dee-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Report Selections Bank Account**, and then choose the related link.</span></span>
2. <span data-ttu-id="c2dee-109">Im Fenster **Berichts-Auswahl - Bankkonto** unter **Verwendung** wählen Sie **Scheck**.</span><span class="sxs-lookup"><span data-stu-id="c2dee-109">In the **Report Selection - Bank Acc.** window, in the **Usage** field, select **Check**.</span></span>
3. <span data-ttu-id="c2dee-110">Wählen Sie eine der folgenden Berichts-IDs:</span><span class="sxs-lookup"><span data-stu-id="c2dee-110">Select one of the following report IDs.</span></span>

| <span data-ttu-id="c2dee-111">Berichts-ID</span><span class="sxs-lookup"><span data-stu-id="c2dee-111">Report ID</span></span> | <span data-ttu-id="c2dee-112">Berichtsname</span><span class="sxs-lookup"><span data-stu-id="c2dee-112">Report Name</span></span> | <span data-ttu-id="c2dee-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c2dee-113">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="c2dee-114">1401</span><span class="sxs-lookup"><span data-stu-id="c2dee-114">1401</span></span> |<span data-ttu-id="c2dee-115">Aktivieren</span><span class="sxs-lookup"><span data-stu-id="c2dee-115">Check</span></span> |<span data-ttu-id="c2dee-116">Dieser Bericht wird standardmäßig verwendet.</span><span class="sxs-lookup"><span data-stu-id="c2dee-116">This is the default report.</span></span> |
| <span data-ttu-id="c2dee-117">10401</span><span class="sxs-lookup"><span data-stu-id="c2dee-117">10401</span></span> |<span data-ttu-id="c2dee-118">Scheck (Formular/Formular/Scheck)</span><span class="sxs-lookup"><span data-stu-id="c2dee-118">Check (Stub/Stub/Check)</span></span> |<span data-ttu-id="c2dee-119">Dieser Bericht dient dazu, Schecks im Formular/Formular/Scheck-Format zu drucken.</span><span class="sxs-lookup"><span data-stu-id="c2dee-119">This report is designed to print checks in a stub/stub/check format.</span></span> |
| <span data-ttu-id="c2dee-120">10411</span><span class="sxs-lookup"><span data-stu-id="c2dee-120">10411</span></span> |<span data-ttu-id="c2dee-121">Scheck (Formular/Scheck/Formular)</span><span class="sxs-lookup"><span data-stu-id="c2dee-121">Check (Stub/Check/Stub)</span></span> |<span data-ttu-id="c2dee-122">Dieser Bericht dient dazu, Schecks im Scheck/Formular/Scheck-Format zu drucken.</span><span class="sxs-lookup"><span data-stu-id="c2dee-122">This report is designed to print checks in a check/stub/check format.</span></span> |

<span data-ttu-id="c2dee-123">Wenn Sie Schecklayouts eingerichtet haben, können Sie Schecks aus dem Fenster **Zahlungsausgangs-Erfassungsjournal** drucken.</span><span class="sxs-lookup"><span data-stu-id="c2dee-123">When you have set up check layouts, you can print checks from the **Payment Journal** window.</span></span> <span data-ttu-id="c2dee-124">Weitere Informationen finden Sie unter [Vorgehensweise: Arbeiten mit Schecks](payables-how-work-checks.md).</span><span class="sxs-lookup"><span data-stu-id="c2dee-124">For more information, see [How to: Work with Checks](payables-how-work-checks.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="c2dee-125">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="c2dee-125">See Also</span></span>
[<span data-ttu-id="c2dee-126">Verwalten von Verbindlichkeiten|</span><span class="sxs-lookup"><span data-stu-id="c2dee-126">Managing Payables</span></span>](payables-manage-payables.md)  
<span data-ttu-id="c2dee-127">[Verwalten von Bankkonten](bank-manage-bank-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="c2dee-127">[Managing Bank Accounts](bank-manage-bank-accounts.md) </span></span>  
[<span data-ttu-id="c2dee-128">Abschließen von Periodenabschlüssen</span><span class="sxs-lookup"><span data-stu-id="c2dee-128">Completing Period-End Processes</span></span>](year-how-complete-period-end-processes.md)  
<span data-ttu-id="c2dee-129">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c2dee-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="c2dee-130">Allgemeine Geschäftsfunktionen</span><span class="sxs-lookup"><span data-stu-id="c2dee-130">General Business Functionality</span></span>](ui-across-business-areas.md)

