---
title: "WIP-Methoden für die Berechnung und die Aufzeichnung des Projektstatus"
description: "Beschreibt die unterschiedlichen Umlaufbestand (WIP)-Methoden, die verwendet werden können, um Finanzdaten für Projekte zu senden und zu überwachen, die im Umlaufbestand sind."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: work in process, work in progress, calculate project WIP
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: e9595d17f00d257f96bc1c31f48e97b3c4a2a3d2
ms.contentlocale: de-ch
ms.lasthandoff: 12/01/2017

---
# <a name="understanding-wip-methods"></a><span data-ttu-id="9e376-103">Verständnis - WIP-Methoden</span><span class="sxs-lookup"><span data-stu-id="9e376-103">Understanding WIP Methods</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="9e376-104">unterstützt die folgenden Methoden zum Berechnen der Inventur und der Wert der unfertigen Arbeit.</span><span class="sxs-lookup"><span data-stu-id="9e376-104"> supports the following methods of calculating and recording the value of work in process.</span></span>

| <span data-ttu-id="9e376-105">WIP-Methode</span><span class="sxs-lookup"><span data-stu-id="9e376-105">WIP Method</span></span> | <span data-ttu-id="9e376-106">Formel</span><span class="sxs-lookup"><span data-stu-id="9e376-106">Calculation Formula</span></span> | <span data-ttu-id="9e376-107">Berechnungsbeschreibung</span><span class="sxs-lookup"><span data-stu-id="9e376-107">Calculation Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="9e376-108">Einstandswert</span><span class="sxs-lookup"><span data-stu-id="9e376-108">Cost Value</span></span> |<span data-ttu-id="9e376-109">Realisierte Einnahmen = Fakturierbarer, verrechneter Preis</span><span class="sxs-lookup"><span data-stu-id="9e376-109">Recognized Revenue = Billable Invoiced Price</span></span><br /><br /> <span data-ttu-id="9e376-110">Erwarteter Einstandsbetrag = Fakturierbarer Gesamtbetrag * geplanter Einstandspreisanteil</span><span class="sxs-lookup"><span data-stu-id="9e376-110">Estimated Total Costs = Billable Total Price x Budget Cost Ratio</span></span><br /><br /> <span data-ttu-id="9e376-111">WIP-Kosten = (Prozentsatz der Fertigung -In Rechnung gestellt %) x Erwarteter Einstandsbetrag</span><span class="sxs-lookup"><span data-stu-id="9e376-111">WIP Costs = (Percentage of Completion - Invoiced %) x Estimated Total Costs</span></span><br /><br /> <span data-ttu-id="9e376-112">Prozentsatz der Fertigung = Gesamtverbrauchskosten / Geplante Gesamtkosten</span><span class="sxs-lookup"><span data-stu-id="9e376-112">Percentage of Completion = Usage Total Costs / Budget Total Costs</span></span><br /> <span data-ttu-id="9e376-113">Fakturiert % = Fakturierbarer verrechneter Preis</span><span class="sxs-lookup"><span data-stu-id="9e376-113">Invoiced % = Billable Invoiced Price</span></span><br /><br /> <span data-ttu-id="9e376-114">Verrechenbarer Gesamtpreis der deklarierten Kosten = Verbrauch Gesamtkosten - WIP</span><span class="sxs-lookup"><span data-stu-id="9e376-114">Billable Total Price Recognized Costs = Usage Total Costs - WIP</span></span> |<span data-ttu-id="9e376-115">Berechnungen vom Typ "Einstandswert" beginnen mit der Berechnung des Werts dessen, was bereitgestellt wurde. Zu diesem Zweck wird ein Anteil des erwarteten Einstandsbetrags (basierend auf dem Prozentsatz der Fertigstellung) herangezogen.</span><span class="sxs-lookup"><span data-stu-id="9e376-115">Cost value calculations start by calculating the value of what has been provided by taking a proportion of the estimated total costs based on percentage of completion.</span></span> <span data-ttu-id="9e376-116">Fakturierte Einstandsbeträge werden abgezogen, indem ein Anteil des erwarteten Einstandsbetrags (basierend auf dem fakturierten Prozentsatz) herangezogen wird.</span><span class="sxs-lookup"><span data-stu-id="9e376-116">Invoiced costs are subtracted by taking a proportion of the estimated total costs based on the invoiced percentage.</span></span><br /><br /> <span data-ttu-id="9e376-117">Damit korrekte Ergebnisse erzielt werden können, müssen für das gesamte Projekt Werte für "Fakturierbarer Gesamtbetrag", "Plan Gesamtpreis" und "Plan Gesamtkosten" eingegeben werden.</span><span class="sxs-lookup"><span data-stu-id="9e376-117">This calculation requires that the billable total price, budget total price, and budget total costs be correctly entered for the whole job.</span></span> |
| <span data-ttu-id="9e376-118">Vertriebskosten</span><span class="sxs-lookup"><span data-stu-id="9e376-118">Cost of Sales</span></span> |<span data-ttu-id="9e376-119">Realisierte Einnahmen = Fakturierbarer, verrechneter Preis</span><span class="sxs-lookup"><span data-stu-id="9e376-119">Recognized Revenue = Billable Invoiced Price</span></span><br /><br /> <span data-ttu-id="9e376-120">Deklarierte Kosten = Plan Gesamtkosten x Fakturierter Prozentbetrag</span><span class="sxs-lookup"><span data-stu-id="9e376-120">Recognized Costs = Budget Total Cost x Invoiced Percentage</span></span><br /><br /> <span data-ttu-id="9e376-121">Fakturiert % = Fakturierbarer Rechnungsbetrag / Fakturierbarer Gesamtpreis</span><span class="sxs-lookup"><span data-stu-id="9e376-121">Invoiced % = Billable Invoiced Price / Billable Total Price</span></span><br /><br /> <span data-ttu-id="9e376-122">(Fakturiert % ist als Spalte in Projektaufgabenzeilen vorhanden)</span><span class="sxs-lookup"><span data-stu-id="9e376-122">(Invoiced % exists as column on job task lines)</span></span><br /><br /> <span data-ttu-id="9e376-123">WIP-Kosten = Verbrauch (Einstandsbetrag) - deaktivierte Kosten</span><span class="sxs-lookup"><span data-stu-id="9e376-123">WIP Costs = Usage Total Costs – Recognized Costs</span></span> |<span data-ttu-id="9e376-124">Berechnungen vom Typ "Vertriebskosten" beginnen mit der Berechnung der deklarierten Kosten.</span><span class="sxs-lookup"><span data-stu-id="9e376-124">Cost of sales calculations begin by calculating the recognized costs.</span></span> <span data-ttu-id="9e376-125">Kosten werden proportional auf der Basis von "Plan Gesamtkosten" realisiert.</span><span class="sxs-lookup"><span data-stu-id="9e376-125">Costs are recognized proportionally based on budget total costs.</span></span><br /><br /> <span data-ttu-id="9e376-126">Damit korrekte Ergebnisse erzielt werden können, müssen für das gesamte Projekt Werte für "Fakturierbarer Gesamtbetrag" und "Plan Gesamtkosten" eingegeben werden.</span><span class="sxs-lookup"><span data-stu-id="9e376-126">This calculation requires that the billable total price and budget total costs be correctly entered for the whole job.</span></span> |
| <span data-ttu-id="9e376-127">Verkaufswert</span><span class="sxs-lookup"><span data-stu-id="9e376-127">Sales Value</span></span> |<span data-ttu-id="9e376-128">Deaktivierte Kosten = Verbrauch (Einstandsbetrag)</span><span class="sxs-lookup"><span data-stu-id="9e376-128">Recognized Costs = Usage Total Costs</span></span><br /><br /> <span data-ttu-id="9e376-129">Realisierte Einnahmen = Verbrauch (Verkaufspreis) x geplanter Rechnungsanteil</span><span class="sxs-lookup"><span data-stu-id="9e376-129">Recognized Revenue = Usage Total Price x Expected invoicing ratio</span></span><br /><br /> <span data-ttu-id="9e376-130">Kosten Zu-/Abschlag % = Fakturierbarer Gesamtbetrag / Plan Gesamtkosten</span><span class="sxs-lookup"><span data-stu-id="9e376-130">Cost Recovery % = Billable Total Price / Budget Total Price</span></span><br /><br /> <span data-ttu-id="9e376-131">WIP Verkäufe = deklarierte Verkäufe - Fakturierbarer Rechnungspreis</span><span class="sxs-lookup"><span data-stu-id="9e376-131">WIP Sales = Recognized Sales - Billable Invoiced Price</span></span> |<span data-ttu-id="9e376-132">Bei Berechnungen vom Typ "Verkaufswert" werden die Einnahmen proportional basierend auf "Verbrauch Gesamtkosten" und dem erwarteten Kostenzu-/-abschlagsanteil realisiert.</span><span class="sxs-lookup"><span data-stu-id="9e376-132">Sales value calculations recognize revenue proportionally based on usage total costs and the expected cost recovery ratio.</span></span><br /><br /> <span data-ttu-id="9e376-133">Damit korrekte Ergebnisse erzielt werden können, müssen für das gesamte Projekt Werte für "Fakturierbarer Gesamtbetrag" und "Plan Gesamtkosten" eingegeben werden.</span><span class="sxs-lookup"><span data-stu-id="9e376-133">This calculation requires that the billable total price and budget total price be correctly entered for the whole job.</span></span> |
| <span data-ttu-id="9e376-134">Prozentsatz der Fertigung</span><span class="sxs-lookup"><span data-stu-id="9e376-134">Percentage of Completion</span></span> |<span data-ttu-id="9e376-135">Deaktivierte Kosten = Verbrauch (Einstandsbetrag)</span><span class="sxs-lookup"><span data-stu-id="9e376-135">Recognized Costs = Usage Total Costs</span></span><br /><br /> <span data-ttu-id="9e376-136">Realisierte Einnahmen = Fakturierbarer Gesamtbetrag x Prozentsatz der Fertigung</span><span class="sxs-lookup"><span data-stu-id="9e376-136">Recognized Revenue = Billable Total Price x Percentage of Completion</span></span><br /><br /> <span data-ttu-id="9e376-137">Prozentsatz der Fertigung = Gesamtverbrauchskosten / Geplante Gesamtkosten</span><span class="sxs-lookup"><span data-stu-id="9e376-137">Percentage of Completion = Usage Total Costs / Budget Total Costs</span></span><br /> <span data-ttu-id="9e376-138">(Wird in Projektplanungszeilen als "Kosten Abschluss %" angegeben)</span><span class="sxs-lookup"><span data-stu-id="9e376-138">(Referred to as "Cost Completion %" on job task lines)</span></span><br /><br /> <span data-ttu-id="9e376-139">WIP Verkäufe = deklarierte Verkäufe - Fakturierbarer Rechnungspreis</span><span class="sxs-lookup"><span data-stu-id="9e376-139">WIP Sales = Recognized Sales - Billable Invoiced Price</span></span> |<span data-ttu-id="9e376-140">Bei Berechnungen vom Typ "Prozentsatz der Fertigung" werden Einnahmen proportional – auf der Basis des Prozentsatzes der Fertigstellung, also "Verbrauch" contra "Einstandspreis" – realisiert.</span><span class="sxs-lookup"><span data-stu-id="9e376-140">Percentage of completion calculations recognize revenue proportionally based on the percentage of completion, that is, usage total costs vs. budget costs.</span></span><br /><br /> <span data-ttu-id="9e376-141">Damit korrekte Ergebnisse erzielt werden können, müssen für das gesamte Projekt Werte für "Fakturierbarer Gesamtbetrag" und "Plan Gesamtkosten" eingegeben werden.</span><span class="sxs-lookup"><span data-stu-id="9e376-141">This calculation requires that the billable total price and budget total costs be correctly entered for the whole job.</span></span> |
| <span data-ttu-id="9e376-142">Abgeschl. Vertrag</span><span class="sxs-lookup"><span data-stu-id="9e376-142">Completed Contract</span></span> |<span data-ttu-id="9e376-143">WIP-Betrag = WIP-Einstandsbetrag = Verbrauch (Einstandsbetrag)</span><span class="sxs-lookup"><span data-stu-id="9e376-143">WIP Amount = WIP Cost Amount = Usage (Total Cost)</span></span><br /><br /> <span data-ttu-id="9e376-144">WIP-Verkaufsbetrag = Fakturierbarer (Rechnungsbetrag)</span><span class="sxs-lookup"><span data-stu-id="9e376-144">WIP Sales Amount = Billable (Invoiced Price)</span></span> |<span data-ttu-id="9e376-145">Bei der Option "Abgeschl. Vertrag" werden Einnahmen und Kosten erst nach Abschluss des Projekts realisiert.</span><span class="sxs-lookup"><span data-stu-id="9e376-145">Completed contract does not recognize revenue and costs until the job is complete.</span></span> <span data-ttu-id="9e376-146">Dies kann nützlich sein, wenn die Schätzungen der Kosten und Einnahmen für das Projekt äusserst unsicher sind.</span><span class="sxs-lookup"><span data-stu-id="9e376-146">You may want to do this when there is high uncertainty around the estimates of costs and revenue for the job.</span></span><br /><br /> <span data-ttu-id="9e376-147">Der gesamte Verbrauch wird auf das Konto für Kosten nicht abgeschlossener Arbeiten (Aktiva) gebucht, und alle fakturierten Verkäufe werden auf das Konto für fakturierte Verkäufe nicht abgeschlossener Arbeiten (Passiva) gebucht, bis das Projekt abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="9e376-147">All usage is posted to the WIP Costs account (asset) and all invoiced sales are posted to the WIP Invoiced Sales account (liability) until the job is complete.</span></span> |

## <a name="see-also"></a><span data-ttu-id="9e376-148">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="9e376-148">See Also</span></span>
[<span data-ttu-id="9e376-149">Projektmanagement</span><span class="sxs-lookup"><span data-stu-id="9e376-149">Project Management</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="9e376-150">Finanzen</span><span class="sxs-lookup"><span data-stu-id="9e376-150">Finance</span></span>](finance.md)  
<span data-ttu-id="9e376-151">[Einkauf](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="9e376-151">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="9e376-152">[Verkauf](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="9e376-152">[Sales](sales-manage-sales.md)    </span></span>  
<span data-ttu-id="9e376-153">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9e376-153">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
