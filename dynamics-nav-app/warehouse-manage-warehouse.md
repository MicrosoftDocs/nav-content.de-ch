---
title: "Lageraktivitäten"
description: "Nach dem Eingang und vor der Lieferung von Waren finden einige interne Lageraktivitäten statt, um einen effektiven Ablauf im Lager zu gewährleisten und um den Lagerbestand des Unternehmens zu organisieren und zu verwalten."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 77590a208843546459fef4528fad500f8969e846
ms.contentlocale: de-ch
ms.lasthandoff: 12/01/2017

---
# <a name="warehouse-management"></a><span data-ttu-id="08bd2-103">Logistik</span><span class="sxs-lookup"><span data-stu-id="08bd2-103">Warehouse Management</span></span>
<span data-ttu-id="08bd2-104">Nach dem Eingang und vor der Lieferung von Waren finden einige interne Lageraktivitäten statt, um einen effektiven Ablauf im Lager zu gewährleisten und um den Lagerbestand des Unternehmens zu organisieren und zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="08bd2-104">After goods are received and before goods are shipped, a series of internal warehouse activities take place to ensure an effective flow through the warehouse and to organize and maintain company inventories.</span></span>

<span data-ttu-id="08bd2-105">Zu den typischen Lageraktivitäten gehören das Einlagern von Artikeln, das Umlagern von Artikeln in Lagern oder zwischen Lagern und die Kommissionierung von Artikeln für die Montage, Produktion oder Lieferung.</span><span class="sxs-lookup"><span data-stu-id="08bd2-105">Typical warehouse activities include putting items away, moving items inside or between warehouses, and picking items for assembly, production, or shipment.</span></span> <span data-ttu-id="08bd2-106">Die Montage von Artikeln für Verkäufe oder Lager gilt auch als Lageraktivität, doch diese werden an anderer Stelle behandelt.</span><span class="sxs-lookup"><span data-stu-id="08bd2-106">Assembling items for sale or inventory may also be considered warehouse activities, but these are covered elsewhere.</span></span> <span data-ttu-id="08bd2-107">Weitere Informationen finden Sie unter [Montageverwaltung](assembly-assemble-items.md).</span><span class="sxs-lookup"><span data-stu-id="08bd2-107">For more information, see [Assembly Management](assembly-assemble-items.md).</span></span>  

<span data-ttu-id="08bd2-108">In großen Lagern können diese unterschiedlichen Aufgaben nach Abteilungen getrennt sein und die Integration kann durch einen gesteuerten Workflow verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="08bd2-108">In large warehouses, these different handling tasks can be separated by departments and the integration managed by a directed workflow.</span></span> <span data-ttu-id="08bd2-109">In einfacheren Installationen ist der Auftragsfluss weniger formalisiert und die Lageraktivitäten werden mit sogenannten Lagerbestandseinlagerungen und -kommissionierungen durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="08bd2-109">In simpler installations, the flow is less formalized and the warehouse activities are performed with so-called inventory put-aways and inventory picks.</span></span> <span data-ttu-id="08bd2-110">Weitere Informationen über grundlegende und erweiterte Lagerkonfigurationen finden Sie unter [Designdetails: Logistik Übersicht](design-details-warehouse-overview.md).</span><span class="sxs-lookup"><span data-stu-id="08bd2-110">For more information about basic versus advanced warehouse configurations, see [Design Details: Warehouse Overview](design-details-warehouse-overview.md).</span></span>

<span data-ttu-id="08bd2-111">Bevor Sie Lageraktivitäten ausführen können, müssen Sie das System für die relevante Komplexität der Lagerverarbeitung einrichten.</span><span class="sxs-lookup"><span data-stu-id="08bd2-111">Before you can perform warehouse activities, you must set the system up for the relevant complexity of warehouse processing.</span></span> <span data-ttu-id="08bd2-112">Weitere Informationen finden Sie unter [Lagerortverwaltung einrichten](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="08bd2-112">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>

 <span data-ttu-id="08bd2-113">In der folgenden Tabelle wird eine Reihe von Aufgaben mit Verknüpfungen zu den beschriebenen Themen erläutert.</span><span class="sxs-lookup"><span data-stu-id="08bd2-113">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="08bd2-114">**Bis**</span><span class="sxs-lookup"><span data-stu-id="08bd2-114">**To**</span></span>|<span data-ttu-id="08bd2-115">**Siehe**</span><span class="sxs-lookup"><span data-stu-id="08bd2-115">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="08bd2-116">Erfassen Sie den Eingang von Artikeln an Lagerorten, entweder mit nur einer Einkaufsbestellung, in einfachen Lagerorteinrichtungen oder mit einem Wareneingang, im Falle von halb- oder vollautomatisierter Lagerverarbeitung am Lagerort.</span><span class="sxs-lookup"><span data-stu-id="08bd2-116">Record the receipt of items at warehouse locations, either with a purchase order only, in simple location setups, or with a warehouse receipt, in case of semi or fully automated warehouse processing at the location.</span></span>|[<span data-ttu-id="08bd2-117">Vorgehensweise: Wareneingang von Artikeln</span><span class="sxs-lookup"><span data-stu-id="08bd2-117">How to: Receive Items</span></span>](warehouse-how-receive-items.md)|
|<span data-ttu-id="08bd2-118">Umgehen Sie die Einlagerungs- und Kommissionierungsvorgänge, um einen Artikel direkt vom Wareneingang oder der Fertigung zum Versenden zu beschleunigen.</span><span class="sxs-lookup"><span data-stu-id="08bd2-118">Bypass the put-away and pick processes to expedite an item straight from receiving or production to shipping.</span></span>|[<span data-ttu-id="08bd2-119">Vorgehensweise: Crossdocking von Artikeln</span><span class="sxs-lookup"><span data-stu-id="08bd2-119">How to: Cross-Dock Items</span></span>](warehouse-how-to-cross-dock-items.md)|    
|<span data-ttu-id="08bd2-120">Lagern Sie Artikel ein, die bei Einkäufen, Verkaufsrücksendungen, Umlagerungen oder Fertigerzeugnissen eingehen, gemäß dem konfigurierten Lageraktivitätsvorgang ein.</span><span class="sxs-lookup"><span data-stu-id="08bd2-120">Put away items received from purchases, sales returns, transfers, or production output according to the configured warehouse process.</span></span>|[<span data-ttu-id="08bd2-121">Einlagerung von Artikeln</span><span class="sxs-lookup"><span data-stu-id="08bd2-121">Putting Items Away</span></span>](warehouse-put-away-items.md)|
|<span data-ttu-id="08bd2-122">Lagern Sie Artikel zwischen Lagerplätzen in dem Lager um.</span><span class="sxs-lookup"><span data-stu-id="08bd2-122">Move items between bins in the warehouse.</span></span>|[<span data-ttu-id="08bd2-123">Umlagern von Artikeln</span><span class="sxs-lookup"><span data-stu-id="08bd2-123">Moving Items</span></span>](warehouse-move-items.md)|
|<span data-ttu-id="08bd2-124">Kommissionieren Sie Artikel, die geliefert, umgelagert oder bei der Montage bzw. Produktion verbraucht werden, gemäß dem konfigurierten Lageraktivitätsvorgang.</span><span class="sxs-lookup"><span data-stu-id="08bd2-124">Pick items to be shipped, transferred, or consumed in assembly or production, according to the configured warehouse process.</span></span>|[<span data-ttu-id="08bd2-125">Kommissionieren von Artikeln</span><span class="sxs-lookup"><span data-stu-id="08bd2-125">Picking Items</span></span>](warehouse-pick-items.md)|
|<span data-ttu-id="08bd2-126">Erfassen Sie die Lieferung von Artikeln aus Lagerorten, entweder mit nur einem Verkaufsauftrag, in einfachen Lagerorteinrichtungen oder mit einem Warenausgang, im Falle von halb- oder vollautomatisierter Lagerverarbeitung am Lagerort.</span><span class="sxs-lookup"><span data-stu-id="08bd2-126">Record the shipment of items from warehouse locations, either with a sales order only, in simple location setups, or with a warehouse shipment, in case of semi or fully automated warehouse processes at the location.</span></span>|[<span data-ttu-id="08bd2-127">So gehts: Artikel versenden</span><span class="sxs-lookup"><span data-stu-id="08bd2-127">How to: Ship Items</span></span>](warehouse-how-ship-items.md)|  

## <a name="see-also"></a><span data-ttu-id="08bd2-128">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="08bd2-128">See Also</span></span>  
 [<span data-ttu-id="08bd2-129">Lagerbesttand</span><span class="sxs-lookup"><span data-stu-id="08bd2-129">Inventory</span></span>](inventory-manage-inventory.md)  
 <span data-ttu-id="08bd2-130">[Lagerortverwaltung einrichten](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="08bd2-130">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
 <span data-ttu-id="08bd2-131">[Montageverwaltung](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="08bd2-131">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="08bd2-132">Designdetails: Logistik</span><span class="sxs-lookup"><span data-stu-id="08bd2-132">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
 <span data-ttu-id="08bd2-133">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="08bd2-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
