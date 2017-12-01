---
title: Einrichten von Lieferbenachrichtigungen
description: "In [!INCLUDE[navnow](../../includes/navnow_md.md)] können Sie EinkaufsLieferbenachrichtigungen verwenden, um Kreditoren an überfällige Lieferungen zu erinnern."
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
ms.openlocfilehash: 8895148c8e969f1d4cf95c21924940668fdd6bf3
ms.contentlocale: de-ch
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-set-up-delivery-reminders"></a><span data-ttu-id="feb80-103">Gewusst wie: Einrichten von Lieferbenachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="feb80-103">How to: Set Up Delivery Reminders</span></span>
<span data-ttu-id="feb80-104">In [!INCLUDE[navnow](../../includes/navnow_md.md)] können Sie EinkaufsLieferbenachrichtigungen verwenden, um Kreditoren an überfällige Lieferungen zu erinnern.</span><span class="sxs-lookup"><span data-stu-id="feb80-104">In [!INCLUDE[navnow](../../includes/navnow_md.md)], you can use purchase delivery reminders to remind vendors about overdue deliveries.</span></span> <span data-ttu-id="feb80-105">Zum Erstellen von Lieferbenachrichtigungen für Kreditoren müssen Sie Basisdaten für die Erstellung von Lieferbenachrichtigungen und Nummernserien für Lieferbenachrichtigungen im Fenster **Kreditoren & Einkauf Einrichtung** einrichten.</span><span class="sxs-lookup"><span data-stu-id="feb80-105">To create delivery reminders for vendors, you must set up base data for delivery reminder creation and number series for the delivery reminders in the **Purchases & Payables Setup** window.</span></span>  

## <a name="to-set-up-delivery-reminders"></a><span data-ttu-id="feb80-106">So richten Sie Lieferbenachrichtigungen ein</span><span class="sxs-lookup"><span data-stu-id="feb80-106">To set up delivery reminders</span></span>  

1.  <span data-ttu-id="feb80-107">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen"), und öffnen Sie **Kreditoren- und Debitoren-Einrichtung**. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="feb80-107">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="feb80-108">Legen Sie im Inforegister **Allgemein** im Feld **Standard Lief.-Mahn. Datumsfeld** eine der folgenden Optionen gemäss der Beschreibung in der folgenden Tabelle fest.</span><span class="sxs-lookup"><span data-stu-id="feb80-108">On the **General** FastTab, in the **Default Del. Rem. Date Field** field, specify one of the following options as described in the following table.</span></span>  

    |<span data-ttu-id="feb80-109">Option</span><span class="sxs-lookup"><span data-stu-id="feb80-109">Option</span></span>|<span data-ttu-id="feb80-110">Description</span><span class="sxs-lookup"><span data-stu-id="feb80-110">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="feb80-111">**Gewünschtes Wareneingangsdatum**</span><span class="sxs-lookup"><span data-stu-id="feb80-111">**Requested Receipt Date**</span></span>|<span data-ttu-id="feb80-112">So legen Sie fest, dass der Datumswert im Feld **Gewünschtes Wareneingangsdatum** auf der Bestellzeile als Standarddatum für das Erstellen von Lieferbenachrichtigungen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="feb80-112">To specify that the date value in the **Requested Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  
    |<span data-ttu-id="feb80-113">**Zugesagtes Wareneingangsdatum**</span><span class="sxs-lookup"><span data-stu-id="feb80-113">**Promised Receipt Date**</span></span>|<span data-ttu-id="feb80-114">So legen Sie fest, dass der Datumswert im Feld **Zugesagtes Wareneingangsdatum** auf der Bestellzeile als Standarddatum für das Erstellen von Lieferbenachrichtigungen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="feb80-114">To specify that the date value in the **Promised Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  
    |<span data-ttu-id="feb80-115">**Erwartetes Wareneingangsdatum**</span><span class="sxs-lookup"><span data-stu-id="feb80-115">**Expected Receipt Date**</span></span>|<span data-ttu-id="feb80-116">So legen Sie fest, dass der Datumswert im Feld **Erwartetes Wareneingangsdatum** auf der Bestellzeile als Standarddatum für das Erstellen von Lieferbenachrichtigungen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="feb80-116">To specify that the date value in the **Expected Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  

3.  <span data-ttu-id="feb80-117">Füllen Sie im Inforegister **Nummerierung** die Felder gemäss der Beschreibung in der folgenden Tabelle aus.</span><span class="sxs-lookup"><span data-stu-id="feb80-117">On the **Numbering** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="feb80-118">Feld</span><span class="sxs-lookup"><span data-stu-id="feb80-118">Field</span></span>|<span data-ttu-id="feb80-119">Description</span><span class="sxs-lookup"><span data-stu-id="feb80-119">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="feb80-120">**Lieferbenachrichtigungsnummern**</span><span class="sxs-lookup"><span data-stu-id="feb80-120">**Delivery Reminder Nos.**</span></span>|<span data-ttu-id="feb80-121">Der Nummernseriencode für Lieferbenachrichtigungen.</span><span class="sxs-lookup"><span data-stu-id="feb80-121">The number series code for delivery reminders.</span></span>|  
    |<span data-ttu-id="feb80-122">**Reg. Lieferbenachrichtigungsnummern**</span><span class="sxs-lookup"><span data-stu-id="feb80-122">**Issued Delivery Reminder Nos.**</span></span>|<span data-ttu-id="feb80-123">Der Nummernseriencode für ausgestellte Lieferbenachrichtigungen.</span><span class="sxs-lookup"><span data-stu-id="feb80-123">The number series code for issued delivery reminders.</span></span>|  

4.  <span data-ttu-id="feb80-124">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="feb80-124">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="feb80-125">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="feb80-125">See Also</span></span>  
 <span data-ttu-id="feb80-126">[Lieferbenachrichtigungen](delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="feb80-126">[Delivery Reminders](delivery-reminders.md) </span></span>  
 <span data-ttu-id="feb80-127">[Gewusst wie: Einrichten von Lieferbenachrichtigungsmethoden, Ebenen und Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md) </span><span class="sxs-lookup"><span data-stu-id="feb80-127">[How to: Set Up Delivery Reminder Terms, Levels, and Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md) </span></span>  
 <span data-ttu-id="feb80-128">[Gewusst wie: Zuweisen von Lieferbenachrichtigungscodes zu Kreditoren](how-to-assign-delivery-reminder-codes-to-vendors.md) </span><span class="sxs-lookup"><span data-stu-id="feb80-128">[How to: Assign Delivery Reminder Codes to Vendors](how-to-assign-delivery-reminder-codes-to-vendors.md) </span></span>  
 [<span data-ttu-id="feb80-129">Gewusst wie: Manuelles Erstellen von Lieferbenachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="feb80-129">How to: Create Delivery Reminders Manually</span></span>](how-to-create-delivery-reminders-manually.md)

