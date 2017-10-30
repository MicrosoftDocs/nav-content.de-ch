---
title: Deaktivieren des Artikelpreistracking
description: "Wenn ein Artikel im Lager nicht nachverfolgt wird, müssen die Artikelpreise nicht nachverfolgt werden, und es muss kein Lagerposten erstellt werden."
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
ms.openlocfilehash: c2043fe4506ba4baf1b76509f73d2ee99c7dba8c
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-deactivate-item-cost-tracking"></a><span data-ttu-id="59779-103">Gewusst wie: Deaktivieren des Artikelpreistracking</span><span class="sxs-lookup"><span data-stu-id="59779-103">How to: Deactivate Item Cost Tracking</span></span>
<span data-ttu-id="59779-104">Wenn ein Artikel im Lager nicht nachverfolgt wird, müssen die Artikelpreise nicht nachverfolgt werden, und es muss kein Lagerposten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="59779-104">When inventory is not tracked for an item, the item cost does not need to be tracked, and an item ledger entry does not need to be created.</span></span>  
  
 <span data-ttu-id="59779-105">Sie können das Artikelpreistracking für einen Artikel deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="59779-105">You can deactivate item cost tracking for an item.</span></span> <span data-ttu-id="59779-106">Im Allgemeinen sollte das Artikelpreistracking für Verbrauchsartikel (z. B. Altpapierprodukte) und Dienste, die als Produkte gelten (z. B. feste Parkgebühren), deaktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="59779-106">Generally, item cost tracking should be deactivated for consumable items, such as waste paper products and for services that are counted as items, such as flat rate parking fees.</span></span> <span data-ttu-id="59779-107">Das Artikelpreistracking sollte für Artikel deaktiviert werden, bei denen die Verfolgung zu falschen Rückschlüssen führen würde.</span><span class="sxs-lookup"><span data-stu-id="59779-107">Item cost tracking should be deactivated on items for which tracking could be misleading.</span></span> <span data-ttu-id="59779-108">Für Artikel, für die das Artikelpreistracking deaktiviert wurde, sind folgende Funktionen bzw. Systeme nicht verfügbar: Reservierung, Verfügbarkeitsprüfung, Artikelverfolgung und Materialplanungssysteme.</span><span class="sxs-lookup"><span data-stu-id="59779-108">Items for which item cost tracking has been deactivated are excluded from reservation, availability check, item tracking, and material planning systems.</span></span>  
  
### <a name="to-deactivate-item-cost-tracking"></a><span data-ttu-id="59779-109">So deaktivieren Sie das Artikelpreistracking</span><span class="sxs-lookup"><span data-stu-id="59779-109">To deactivate item cost tracking</span></span>  
  
1.  <span data-ttu-id="59779-110">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und öffnen Sie **Artikel**. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="59779-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="59779-111">Wählen Sie den erforderlichen Artikel aus. Wählen Sie auf der Registerkarte **Start** in der Gruppe **Verwalten** die Option **Bearbeiten** aus.</span><span class="sxs-lookup"><span data-stu-id="59779-111">Select the required item, and on the **Home** tab, in the **Manage** group, choose **Edit**.</span></span>  
  
3.  <span data-ttu-id="59779-112">Aktivieren Sie auf dem Inforegister **Allgemein** das Kontrollkästchen **Keine Lagerführung**.</span><span class="sxs-lookup"><span data-stu-id="59779-112">On the **General** FastTab, select the **No Stockkeeping** check box.</span></span>  
  
     <span data-ttu-id="59779-113">Wenn eine Transaktion für diesen Artikel gebucht wird, wird kein Lagerposten erstellt.</span><span class="sxs-lookup"><span data-stu-id="59779-113">An item ledger entry will not be created when you post a transaction for this item.</span></span> <span data-ttu-id="59779-114">Weitere Informationen erhalten Sie in der Tabelle "Lagerposten".</span><span class="sxs-lookup"><span data-stu-id="59779-114">For more information, see the Item Ledger Entry table.</span></span>  
  
    > [!NOTE]  
    >  <span data-ttu-id="59779-115">Das Kontrollkästchen **Keine Lagerführung** kann nicht für einen Artikel aktiviert werden, für den bereits Lagerposten gebucht wurden.</span><span class="sxs-lookup"><span data-stu-id="59779-115">You cannot select the **No Stockkeeping** check box on an item for which item ledger entries have already been posted.</span></span>  
  
4.  <span data-ttu-id="59779-116">Wählen Sie die Schaltfläche **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="59779-116">Choose the **OK** button.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="59779-117">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="59779-117">See Also</span></span>  
 <span data-ttu-id="59779-118">Option</span><span class="sxs-lookup"><span data-stu-id="59779-118">Item</span></span>   
 <span data-ttu-id="59779-119">Lagerposten</span><span class="sxs-lookup"><span data-stu-id="59779-119">Item Ledger Entry</span></span>   
 <span data-ttu-id="59779-120">[Lagerverwaltung (Schweiz)](swiss-inventory-management.md) </span><span class="sxs-lookup"><span data-stu-id="59779-120">[Swiss Inventory Management](swiss-inventory-management.md) </span></span>  
 [<span data-ttu-id="59779-121">Gewusst wie: Sperren von Lagerartikeln für Verkäufe oder Einkäufe</span><span class="sxs-lookup"><span data-stu-id="59779-121">How to: Block Inventory Items for Sales or Purchases</span></span>](how-to-block-inventory-items-for-sales-or-purchases.md)
