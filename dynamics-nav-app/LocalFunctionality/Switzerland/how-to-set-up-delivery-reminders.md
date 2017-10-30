---
title: Einrichten von Lieferanmahnungen
description: "In [!INCLUDE[navnow](../../includes/navnow_md.md)] können Sie Einkaufslieferanmahnungen verwenden, um Kreditoren an überfällige Lieferungen zu erinnern. Zum Erstellen von Lieferanmahnungen für Kreditoren müssen Sie Basisdaten für die Erstellung von Lieferanmahnungen und Nummernserien für Lieferanmahnungen im Fenster **Kreditoren & Einkauf Einrichtung** einrichten."
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
ms.openlocfilehash: 6932a2004d4ac713fee87e9d4f5257d66c54db19
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-delivery-reminders"></a><span data-ttu-id="5ffe7-104">Gewusst wie: Einrichten von Lieferanmahnungen</span><span class="sxs-lookup"><span data-stu-id="5ffe7-104">How to: Set Up Delivery Reminders</span></span>
<span data-ttu-id="5ffe7-105">In [!INCLUDE[navnow](../../includes/navnow_md.md)] können Sie Einkaufslieferanmahnungen verwenden, um Kreditoren an überfällige Lieferungen zu erinnern.</span><span class="sxs-lookup"><span data-stu-id="5ffe7-105">In [!INCLUDE[navnow](../../includes/navnow_md.md)], you can use purchase delivery reminders to remind vendors about overdue deliveries.</span></span> <span data-ttu-id="5ffe7-106">Zum Erstellen von Lieferanmahnungen für Kreditoren müssen Sie Basisdaten für die Erstellung von Lieferanmahnungen und Nummernserien für Lieferanmahnungen im Fenster **Kreditoren & Einkauf Einrichtung** einrichten.</span><span class="sxs-lookup"><span data-stu-id="5ffe7-106">To create delivery reminders for vendors, you must set up base data for delivery reminder creation and number series for the delivery reminders in the **Purchases & Payables Setup** window.</span></span>  
  
### <a name="to-set-up-delivery-reminders"></a><span data-ttu-id="5ffe7-107">So richten Sie Lieferanmahnungen ein</span><span class="sxs-lookup"><span data-stu-id="5ffe7-107">To set up delivery reminders</span></span>  
  
1.  <span data-ttu-id="5ffe7-108">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen"), und öffnen Sie **Kreditoren- und Debitoren-Einrichtung**. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="5ffe7-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="5ffe7-109">Legen Sie im Inforegister **Allgemein** im Feld **Standard Lief.-Mahn. Datumsfeld** eine der folgenden Optionen gemäss der Beschreibung in der folgenden Tabelle fest.</span><span class="sxs-lookup"><span data-stu-id="5ffe7-109">On the **General** FastTab, in the **Default Del. Rem. Date Field** field, specify one of the following options as described in the following table.</span></span>  
  
    |<span data-ttu-id="5ffe7-110">ADD INCLUDE<!--[!INCLUDE[bp_tableoption](../../includes/bp_tabledescription_md.md)]--></span><span class="sxs-lookup"><span data-stu-id="5ffe7-110">ADD INCLUDE<!--[!INCLUDE[bp_tableoption](../../includes/bp_tabledescription_md.md)]--></span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="5ffe7-111">**Gewünschtes Wareneingangsdatum**</span><span class="sxs-lookup"><span data-stu-id="5ffe7-111">**Requested Receipt Date**</span></span>|<span data-ttu-id="5ffe7-112">So legen Sie fest, dass der Datumswert im Feld **Gewünschtes Wareneingangsdatum** auf der Bestellzeile als Standarddatum für das Erstellen von Lieferanmahnungen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="5ffe7-112">To specify that the date value in the **Requested Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  
    |<span data-ttu-id="5ffe7-113">**Zugesagtes Wareneingangsdatum**</span><span class="sxs-lookup"><span data-stu-id="5ffe7-113">**Promised Receipt Date**</span></span>|<span data-ttu-id="5ffe7-114">So legen Sie fest, dass der Datumswert im Feld **Zugesagtes Wareneingangsdatum** auf der Bestellzeile als Standarddatum für das Erstellen von Lieferanmahnungen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="5ffe7-114">To specify that the date value in the **Promised Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  
    |<span data-ttu-id="5ffe7-115">**Erwartetes Wareneingangsdatum**</span><span class="sxs-lookup"><span data-stu-id="5ffe7-115">**Expected Receipt Date**</span></span>|<span data-ttu-id="5ffe7-116">So legen Sie fest, dass der Datumswert im Feld **Erwartetes Wareneingangsdatum** auf der Bestellzeile als Standarddatum für das Erstellen von Lieferanmahnungen verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="5ffe7-116">To specify that the date value in the **Expected Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  
  
3.  <span data-ttu-id="5ffe7-117">Füllen Sie im Inforegister **Nummerierung** die Felder gemäss der Beschreibung in der folgenden Tabelle aus.</span><span class="sxs-lookup"><span data-stu-id="5ffe7-117">On the **Numbering** FastTab, fill in the fields as described in the following table.</span></span>  
  
    |<span data-ttu-id="5ffe7-118">Feld</span><span class="sxs-lookup"><span data-stu-id="5ffe7-118">Field</span></span>|<span data-ttu-id="5ffe7-119">Description</span><span class="sxs-lookup"><span data-stu-id="5ffe7-119">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="5ffe7-120">**Lieferanmahnungsnummern**</span><span class="sxs-lookup"><span data-stu-id="5ffe7-120">**Delivery Reminder Nos.**</span></span>|<span data-ttu-id="5ffe7-121">Der Nummernseriencode für Lieferanmahnungen.</span><span class="sxs-lookup"><span data-stu-id="5ffe7-121">The number series code for delivery reminders.</span></span>|  
    |<span data-ttu-id="5ffe7-122">**Reg. Lieferanmahnungsnummern**</span><span class="sxs-lookup"><span data-stu-id="5ffe7-122">**Issued Delivery Reminder Nos.**</span></span>|<span data-ttu-id="5ffe7-123">Der Nummernseriencode für ausgestellte Lieferanmahnungen.</span><span class="sxs-lookup"><span data-stu-id="5ffe7-123">The number series code for issued delivery reminders.</span></span>|  
  
4.  <span data-ttu-id="5ffe7-124">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="5ffe7-124">Choose the **OK** button.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="5ffe7-125">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="5ffe7-125">See Also</span></span>  
 <span data-ttu-id="5ffe7-126">Kreditoren & Einkauf Einrichtung</span><span class="sxs-lookup"><span data-stu-id="5ffe7-126">Purchases & Payables Setup</span></span>   
 <span data-ttu-id="5ffe7-127">[Lieferanmahnungen](delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="5ffe7-127">[Delivery Reminders](delivery-reminders.md) </span></span>  
 <span data-ttu-id="5ffe7-128">[Gewusst wie: Einrichten von Lieferanmahnungsmethoden, Ebenen und Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md) </span><span class="sxs-lookup"><span data-stu-id="5ffe7-128">[How to: Set Up Delivery Reminder Terms, Levels, and Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md) </span></span>  
 <span data-ttu-id="5ffe7-129">[Gewusst wie: Zuweisen von Lieferanmahnungscodes zu Kreditoren](how-to-assign-delivery-reminder-codes-to-vendors.md) </span><span class="sxs-lookup"><span data-stu-id="5ffe7-129">[How to: Assign Delivery Reminder Codes to Vendors](how-to-assign-delivery-reminder-codes-to-vendors.md) </span></span>  
 [<span data-ttu-id="5ffe7-130">Gewusst wie: Manuelles Erstellen von Lieferanmahnungen</span><span class="sxs-lookup"><span data-stu-id="5ffe7-130">How to: Create Delivery Reminders Manually</span></span>](how-to-create-delivery-reminders-manually.md)
