---
title: Vorgehensweise beim Arbeiten mit Lagerbuchungsperioden
description: "Sie können den Zeitrahmen steuern, auf den Mitarbeiter Beitragsänderungen des Lagerbestandes buchen können, indem Sie Lagerbuchungsperioden definieren."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: inventory, periods
ms.date: 08/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 289b12d39c9f67913d862cb3500cccae0b3823d2
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-work-with-inventory-periods"></a>Vorgehensweise: Arbeiten mit Lagerbuchungsperioden
Eine Lagerbuchungsperiode definiert eine Zeitspanne, in der Sie Änderungen des Lagerbestandes buchen können. Eine Lagerbuchungsperiode ist durch das Datum definiert, an dem sie endet (wird auch als Enddatum bezeichnet). Wenn Sie eine Lagerbuchungsperiode schliessen, können Sie vor diesem Enddatum keine Änderungen des erwarteten oder in Rechnung gestellten Lagerbestandes buchen. Vor diesem Enddatum können Sie keine neuen Werte im Lager buchen. Wenn Sie in der geschlossenen Periode offene Artikelposten haben, es also positive Mengen gibt, die noch nicht für ausgehende Transaktion ausgeglichen wurden, können Sie weiterhin ausgehende Mengen mit diesen Posten verknüpfen, auch wenn die Periode geschlossen ist.  

In den folgenden Abschnitten werden diese Schritte beschrieben:  

* Lagerbuchungsperioden erstellen.  
* Lagerbuchungsperioden schliessen.  
* Lagerbuchungsperioden erneut öffnen.  

## <a name="to-create-an-inventory-period"></a>Eine Lagerbuchungsperiode erstellen  
1. Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol Nach Seite oder Bericht suchen"), geben **Lagerbuchungsperioden** ein und wählen dann den zugehörigen Link aus.  
2. Erstellen Sie eine neue Zeile.  
3. Geben Sie in das Feld **Enddatum** das letzte Datum der Lagerbuchungsperiode ein, die Sie definieren möchten. Wenn die Periode geschlossen ist, können Sie vor diesem Datum keine Lagerbestandsänderungen buchen.  
4. Geben Sie im Feld **Name** einen beschreibenden Namen ein. Wählen Sie die Schaltfläche **OK** aus.  

## <a name="closing-inventory-periods"></a>Lagerbuchungsperioden schliessen  
Das Feld **Abgeschlossen** gibt an, ob die Lagerbuchungsperiode hinsichtlich Änderungen der Lagerbestandswerte geschlossen ist. Sie können dieses Feld nicht bearbeiten.  

Sofern die folgenden Aussagen zutreffen, können Sie jede Lagerbuchungsperiode schliessen:  

* In dieser Periode gibt es keine offenen ausgehenden Lagerposten (d. h., es gibt keinen negativen Lagerbestand).  
* Die Preise aller Artikel wurden mit der Stapelverarbeitung **Lagerreg. fakt. Einst. Preise** reguliert.  

Das heisst, dass alle ausgehenden Transaktionsmengen (z. B. von Verkaufsaufträgen, ausgehenden Umlagerungen, Verkaufsrechnungen, Einkaufsreklamationen oder Einkaufsgutschriften) mit der im Lagerbestand vorhandenen Menge ausgeglichen werden müssen.  

### <a name="to-close-an-inventory-period"></a>Eine Lagerbuchungsperiode schliessen  
1. Bevor Sie eine Lagerbuchungsperiode schliessen, sollten Sie den Batchauftrag **Lagerreg. fakt. Einst. Preise** ausführen, um sich zu vergewissern, dass alle Kostenregulierungen gebucht sind. Wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Funktionen** die Option **Kosten anpassen - Artikel** aus.  

     Führen Sie den Bericht **Lagerbuchungsperiode schliessen - Test** aus, um zu ermitteln, ob es in der Lagerbuchungsperiode offene ausgehende Artikelposten oder Artikel gibt, deren Preise noch nicht reguliert wurden.  
2. Wählen Sie die Aktion **Lagerbuchungsperiode schließen - Test**.  

     Führen Sie den Batchauftrag **Lagerregulierung buchen** aus, damit sichergestellt ist, dass alle Preise in der Finanzbuchhaltung gebucht werden.  
3. Wählen Sie die Aktion **Lager auf Sachkonten buchen** aus.  
4. Wählen Sie im Fenster  **Lagerbuchungsperioden** die Lagerbuchungsperiode aus, die geschlossen werden soll.  
5. Wählen Sie die Aktion **Periode schließen**. Nachdem die Lagerbuchungsperiode geschlossen wurde, können Sie vor dem Enddatum keine Lagerbestandsänderungen mehr buchen. Die Preise aller Artikel müssen mit der Stapelverarbeitung **Lagerreg. fakt. Einst. Preise** reguliert sein, bevor Sie die Lagerbuchungsperiode schliessen.  
6. Wählen Sie die Schaltfläche **Ja**, wenn Sie bestätigen möchten, dass die Periode geschlossen werden soll, oder wählen Sie die Schaltfläche **Nein**, wenn Sie das Schliessen abbrechen möchten.  
7. Die Lagerbuchungsperiode wird geschlossen und nach Beendigung dieses Vorgangs wird eine Bestätigungsmeldung angezeigt.  

## <a name="reopening-inventory-periods"></a>Lagerbuchungsperioden erneut öffnen  
Nachdem Sie eine Lagerbuchungsperiode geschlossen haben, können Sie diese Periode nicht mehr löschen. Sie können sie aber erneut öffnen, wenn Sie Buchungen vor dem Enddatum der Lagerbuchungsperiode zulassen möchten. Ein erneutes Öffnen einer Periode bewirkt, dass auch jede Lagerbuchungsperiode geöffnet wird, deren Enddatum hinter dem Enddatum der Periode liegt, die Sie erneut öffnen.  

### <a name="to-reopen-an-inventory-period"></a>So öffnen Sie eine Lagerbuchungsperiode erneut  
1. Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol Nach Seite oder Bericht suchen"), geben **Lagerbuchungsperioden** ein und wählen dann den zugehörigen Link aus.  
2. Wählen Sie die Lagerbuchungsperiode aus, die erneut geöffnet werden soll.  
3. Wählen Sie die Aktion **Periode erneut öffnen**. Bestätigen Sie, dass Sie die Periode erneut öffnen möchten.  
4. Alle Lagerbuchungsperioden, deren Enddatum nach der von Ihnen ausgewählten Periode liegt, werden erneut geöffnet.  

## <a name="see-also"></a>Siehe auch  
[Designdetails: Bestandsperioden](design-details-inventory-periods.md)  
[Finanzen](finance.md)  
[Lagerbesttand](inventory-manage-inventory.md)  
[Arbeiten mit Dynamics NAV](ui-work-product.md)

