---
title: "Ergebnisse der Übertragung"
description: "Dieses Thema beschreibt, welche passiert, nachdem Sie Fibuposten in Kostenposten übertragen."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: general ledger, transfer, cost entries
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 476830c732e8c48a131a1429dc05f41b25f33f46
ms.contentlocale: de-ch
ms.lasthandoff: 12/01/2017

---
# <a name="results-of-transferring-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="095c9-103">Kriterien für die Übertragung von Fibuposten in Kostenposten</span><span class="sxs-lookup"><span data-stu-id="095c9-103">Results of Transferring General Ledger Entries to Cost Entries</span></span>
<span data-ttu-id="095c9-104">Während der Übertragung der Fibuposten zu den Kostenposten erstellt [!INCLUDE[d365fin](includes/d365fin_md.md)] Verknüpfungen in den Posten in der Tabelle **Fibuposten**, der Tabelle **Kostenposten** und der Tabelle **Kostenjournal**, damit es möglich ist, Verbindungen zwischen Kostenposten und Fibuposten zu verfolgen.</span><span class="sxs-lookup"><span data-stu-id="095c9-104">During the transfer of general ledger entries to cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] creates connections in the entries in the **G/L Entry** table, the **Cost Entry** table, and the **Cost Register** table to make it possible to trace the connections between cost entries and general ledger entries.</span></span>  

## <a name="general-ledger-entries"></a><span data-ttu-id="095c9-105">Sachposten</span><span class="sxs-lookup"><span data-stu-id="095c9-105">General Ledger Entries</span></span>  
<span data-ttu-id="095c9-106">Für jeden Fibuposten, der zur Kostenrechnung übertragen wird, füllt [!INCLUDE[d365fin](includes/d365fin_md.md)] das Kostenfeld **Laufnr.** aus.</span><span class="sxs-lookup"><span data-stu-id="095c9-106">For each general ledger entry that is transferred to cost accounting, [!INCLUDE[d365fin](includes/d365fin_md.md)] fills the cost **Entry No.** field.</span></span>  

## <a name="cost-entries"></a><span data-ttu-id="095c9-107">Kostenposten</span><span class="sxs-lookup"><span data-stu-id="095c9-107">Cost Entries</span></span>  
<span data-ttu-id="095c9-108">Für jeden Kostenposten speichert [!INCLUDE[d365fin](includes/d365fin_md.md)] die Laufnummer des entsprechenden Fibupostens im Feld **Fibuposten Laufnr.** in der Tabelle **Kostenposten**.</span><span class="sxs-lookup"><span data-stu-id="095c9-108">For each cost entry, [!INCLUDE[d365fin](includes/d365fin_md.md)] saves the entry number of the corresponding general ledger entry in the **G/L Entry No.** field in the **Cost Entry** table.</span></span>  

<span data-ttu-id="095c9-109">Für kombinierte Kostenposten speichert [!INCLUDE[d365fin](includes/d365fin_md.md)] die laufende Nummer des letzten Fibupostens, der dem Posten mit der höchsten laufenden Nummer entspricht.</span><span class="sxs-lookup"><span data-stu-id="095c9-109">For combined cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] saves the entry number of the last general ledger entry, which is the entry with the highest entry number.</span></span>  

<span data-ttu-id="095c9-110">Das Feld **Fibukonto** in der Tabelle **Kostenposten** enthält die Nummer des Fibukontos, von dem der Kostenposten stammt.</span><span class="sxs-lookup"><span data-stu-id="095c9-110">The **G/L Account** field in the **Cost Entry** table contains the number of the general ledger account that the cost entry came from.</span></span>  

<span data-ttu-id="095c9-111">Für einzelne Kostenposten überträgt [!INCLUDE[d365fin](includes/d365fin_md.md)] den Buchungstext aus dem Fibuposten in das Textfeld **Beschreibung**.</span><span class="sxs-lookup"><span data-stu-id="095c9-111">For single cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] transfers the posting text from the general ledger entry to the **Description** text field.</span></span> <span data-ttu-id="095c9-112">Für kombinierte Posten zeigt das Textfeld, dass diese Posten als kombinierte Posten übertragen werden.</span><span class="sxs-lookup"><span data-stu-id="095c9-112">For combined entries, the text field shows these entries are transferred as combined entries.</span></span> <span data-ttu-id="095c9-113">Zum Beispiel kann für einen kombinierten Posten für den Monat Oktober 2013 der Text lauten: **Kombinierte Posten, Oktober 2013**.</span><span class="sxs-lookup"><span data-stu-id="095c9-113">For example, for a combined entry for the month of October in 2013, the text can be **Combined Entries, October 2013**.</span></span>  

## <a name="cost-register"></a><span data-ttu-id="095c9-114">Kostenjournal</span><span class="sxs-lookup"><span data-stu-id="095c9-114">Cost Register</span></span>  
<span data-ttu-id="095c9-115">In der Tabelle **Kostenregister** erstellt [!INCLUDE[d365fin](includes/d365fin_md.md)] einen Posten mit der Quellenübertragung aus dem Fibukonto.</span><span class="sxs-lookup"><span data-stu-id="095c9-115">In the **Cost Register** table, [!INCLUDE[d365fin](includes/d365fin_md.md)] creates an entry with the source transfer from general ledger.</span></span> <span data-ttu-id="095c9-116">Der Posten erfasst die erste und letzte Postennummer der übertragenen Sachposten sowie die erste und letzte Nummer der erstellten Kostenposten.</span><span class="sxs-lookup"><span data-stu-id="095c9-116">The entry records the first and last entry numbers of the general ledger entries that are transferred, in addition to the first and last entry numbers of the cost entries that are created.</span></span>  

## <a name="see-also"></a><span data-ttu-id="095c9-117">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="095c9-117">See Also</span></span>  
<span data-ttu-id="095c9-118">[Vorgehensweise: Übertragen von Sachposten in Kostenposten](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="095c9-118">[How to: Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span></span>  
<span data-ttu-id="095c9-119">[Kriterien für die Übertragung von Sachposten in Kostenposten](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="095c9-119">[Criteria for Transferring General Ledger Entries to Cost Entries](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span></span>  
<span data-ttu-id="095c9-120">[Automatische Übertragung und kombinierte Posten](finance-automatic-transfer-combined-entries.md) </span><span class="sxs-lookup"><span data-stu-id="095c9-120">[Automatic Transfer and Combined Entries](finance-automatic-transfer-combined-entries.md) </span></span>  
[<span data-ttu-id="095c9-121">Übertragung und Buchung von Kostenzuteilungen</span><span class="sxs-lookup"><span data-stu-id="095c9-121">Transferring and Posting Cost Entries</span></span>](finance-transfer-and-post-cost-entries.md)  
