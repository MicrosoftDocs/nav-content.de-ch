---
title: "Designdetails – Lagerkostenberechnung"
description: Diese Dokumentation stellt einen detaillierten technischen Einblick in die Konzepte und Prinzipien bereit, die in den Lagerkostenfunktionen in [!INCLUDE[d365fin](includes/d365fin_md.md)] verwendet werden.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, inventory, costing
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 8403486a897a3031ad0f488b4eb7e415daa1b8a0
ms.contentlocale: de-ch
ms.lasthandoff: 12/01/2017

---
# <a name="design-details-inventory-costing"></a><span data-ttu-id="3fad1-103">Designdetails: Lagerkostenberechnung</span><span class="sxs-lookup"><span data-stu-id="3fad1-103">Design Details: Inventory Costing</span></span>
<span data-ttu-id="3fad1-104">Diese Dokumentation stellt einen detaillierten technischen Einblick in die Konzepte und Prinzipien bereit, die in den Lagerkostenfunktionen in [!INCLUDE[d365fin](includes/d365fin_md.md)] verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="3fad1-104">This documentation provides detailed technical insight to the concepts and principles that are used within the Inventory Costing features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="3fad1-105">Die Kostenverwaltung, die auch als "Lagerabgang" bezeichnet wird, dient zum Erfassen und Melden der Betriebskosten eines Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="3fad1-105">Inventory costing, also referred to as cost management, is concerned with recording and reporting business operating costs.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="3fad1-106">In diesem Abschnitt</span><span class="sxs-lookup"><span data-stu-id="3fad1-106">In This Section</span></span>  
[<span data-ttu-id="3fad1-107">Designdetails: Kostenberechnungsmethoden</span><span class="sxs-lookup"><span data-stu-id="3fad1-107">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)  
[<span data-ttu-id="3fad1-108">Designdetails: Artikelausgleich</span><span class="sxs-lookup"><span data-stu-id="3fad1-108">Design Details: Item Application</span></span>](design-details-item-application.md)  
[<span data-ttu-id="3fad1-109">Designdetails: Kostenregulierung</span><span class="sxs-lookup"><span data-stu-id="3fad1-109">Design Details: Cost Adjustment</span></span>](design-details-cost-adjustment.md)  
[<span data-ttu-id="3fad1-110">Designdetails: Soll-Kosten-Buchen</span><span class="sxs-lookup"><span data-stu-id="3fad1-110">Design Details: Expected Cost Posting</span></span>](design-details-expected-cost-posting.md)  
[<span data-ttu-id="3fad1-111">Designdetails: Durchschnittskosten</span><span class="sxs-lookup"><span data-stu-id="3fad1-111">Design Details: Average Cost</span></span>](design-details-average-cost.md)  
[<span data-ttu-id="3fad1-112">Designdetails: Abweichung</span><span class="sxs-lookup"><span data-stu-id="3fad1-112">Design Details: Variance</span></span>](design-details-variance.md)  
[<span data-ttu-id="3fad1-113">Designdetails: Rundung</span><span class="sxs-lookup"><span data-stu-id="3fad1-113">Design Details: Rounding</span></span>](design-details-rounding.md)  
[<span data-ttu-id="3fad1-114">Designdetails: Kostenkomponenten</span><span class="sxs-lookup"><span data-stu-id="3fad1-114">Design Details: Cost Components</span></span>](design-details-cost-components.md)  
[<span data-ttu-id="3fad1-115">Designdetails: Bestandsperioden</span><span class="sxs-lookup"><span data-stu-id="3fad1-115">Design Details: Inventory Periods</span></span>](design-details-inventory-periods.md)  
[<span data-ttu-id="3fad1-116">Designdetails: Bestandsbuchung</span><span class="sxs-lookup"><span data-stu-id="3fad1-116">Design Details: Inventory Posting</span></span>](design-details-inventory-posting.md)  
[<span data-ttu-id="3fad1-117">Designdetails: Fertigungsauftragsbuchung</span><span class="sxs-lookup"><span data-stu-id="3fad1-117">Design Details: Production Order Posting</span></span>](design-details-production-order-posting.md)  
[<span data-ttu-id="3fad1-118">Designdetails: Montageauftragsbuchung</span><span class="sxs-lookup"><span data-stu-id="3fad1-118">Design Details: Assembly Order Posting</span></span>](design-details-assembly-order-posting.md)  
[<span data-ttu-id="3fad1-119">Designdetails: Abgleich mit der Finanzbuchhaltung</span><span class="sxs-lookup"><span data-stu-id="3fad1-119">Design Details: Reconciliation with the General Ledger</span></span>](design-details-reconciliation-with-the-general-ledger.md)  
[<span data-ttu-id="3fad1-120">Designdetails: Konten in der Finanzbuchhaltung</span><span class="sxs-lookup"><span data-stu-id="3fad1-120">Design Details: Accounts in the General Ledger</span></span>](design-details-accounts-in-the-general-ledger.md)  
[<span data-ttu-id="3fad1-121">Designdetails: Neubewertung</span><span class="sxs-lookup"><span data-stu-id="3fad1-121">Design Details: Revaluation</span></span>](design-details-revaluation.md)
