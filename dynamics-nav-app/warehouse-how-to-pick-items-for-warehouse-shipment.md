---
title: "Vorgehensweise: Kommissionieren von Artikeln für den Warenausgang"
description: Wenn Ihr Lagerort so eingerichtet wurde, dass die Bearbeitung der Kommissionierung und des Warenausgangs erforderlich ist, verwenden Sie die Kommissionierbelege, um Kommissionierinformationen vor dem Buchen des Warenausgangs zu erstellen und zu bearbeiten.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 256f7cfc0348b121a1302db49e57fa030b76f55c
ms.contentlocale: de-ch
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-pick-items-for-warehouse-shipment"></a>Vorgehensweise: Kommissionieren von Artikeln für den Warenausgang
Wenn Ihr Lagerort so eingerichtet wurde, dass die Bearbeitung der Kommissionierung und des Warenausgangs erforderlich ist, verwenden Sie die Kommissionierbelege, um Kommissionierinformationen vor dem Buchen des Warenausgangs zu erstellen und zu bearbeiten.  

Sie können einen Kommissionierungsbeleg nicht von Grund auf neu erstellen, da eine Kommissionierungsaktivität immer Teil eines Workflows ist, entweder in einem Abruf- oder Push-Szenario.  

Sie können Kommissionierungsbelege in einem Abrufverfahren erstellen, indem Sie einen leeren Warenausgangsbeleg öffnen, Herkunftsbelege ermitteln, die für die Lieferung freigegeben wurden, und dann für diese Lieferungen Kommissionierzeilen erstellen. Sie können die Funktionen **Herkunftsbelege holen** oder **Filter zum Holen von Herk.-Belegen verwenden** verwenden, um Herkunftsbelege zu ermitteln, die für den Warenausgang bereit sind.

Alternativ können Sie das Fenster **Kommissioniervorschlag** verwenden, um Kommissionierzeilen im Stapelbetrieb zu holen und zu erstellen. Weitere Informationen finden Sie unter [Vorgehensweise: Kommissionierungen im Vorschlag bearbeiten](warehouse-how-to-plan-picks-in-worksheets.md).  

Sie können Kommissionierungsbelege auch Push-artig im Fenster **Warenausgang** erstellen, indem Sie **Kommissionierung erstellen** auswählen.  

> [!NOTE]  
>  Die Kommissionierung für den Warenausgang von Artikeln, die mit dem betreffenden Verkaufsauftrag montiert werden, folgt denselben Schritten wie die reguläre Kommissionierung für den Warenausgang, die in diesem Thema beschrieben ist. Jedoch kann die Anzahl der Kommissionierzeilen pro zu liefernder Menge n:1 sein, da die Kommissionierung für die Komponenten, nicht für den Montageartikel erfolgt.  
>   
>  Die Kommissionierzeilen werden für den Wert im Feld **Restmenge** in den Zeilen des Montageauftrags erstellt, der mit der Verkaufsauftragszeile verknüpft ist, die geliefert wird. Dadurch ist sichergestellt, dass alle Komponenten in einer Aktion kommissioniert werden.  
>   
>  Weitere Informationen finden Sie im Abschnitt "Verwenden von Auftragsmontageartikeln in Warenausgängen".  
>   
>  Allgemeine Informationen über das Kommissionieren von Komponenten für Montageaufträge, einschließlich von Situationen, in denen der Montageartikel nicht mit einer Verkaufslieferung fällig ist, finden Sie unter [Vorgehensweise: Kommissionierung für die Produktion oder Montage](warehouse-how-to-pick-for-production.md).  

## <a name="to-pick-items-for-warehouse-shipment"></a>Um Artikel für den Warenausgang zu kommissionieren  
1.  Wählen Sie ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben Sie **Auswahl** ein und wählen dann den zugehörigen Link aus.  

    Wenn Sie an einer bestimmten Kommissionierung arbeiten möchten, wählen Sie die Kommissionierung in der Liste aus, oder filtern Sie die Liste, um die Kommissionierungen zu finden, die speziell Ihnen zugeordnet wurden. Öffnen Sie die Kommissionierungskarte.  
2.  Wenn das Feld **Zugewiesene Benutzer-ID** leer ist, geben Sie gegebenenfalls Ihre ID ein, um sich zu identifizieren.  
3.  Führen Sie die tatsächliche Kommissionierung der Artikel aus.  

    Wenn das Lager für die Verwendung von Lagerplätzen eingerichtet wurde, werden die Vorgabelagerplätze der Artikel als Vorschlag für den Entnahmeort verwendet. Die Anweisungen erscheinen als zwei Zeilen, mindestens eine für jede Aktivitätenart, "Entnahme" und "Einlagerung".  

    Wenn das Lager mit gesteuerter Einlagerung und Kommissionierung eingerichtet wurde, wird die Lagerplatzpriorität verwendet, um die besten Lagerplätze für die Kommissionierung zu berechnen und in den Kommissionierzeilen vorzuschlagen. Die Anweisungen erscheinen als zwei Zeilen, mindestens eine für jede Aktivitätenart, "Entnahme" und "Einlagerung".  

4.  Wenn Sie die Kommissionierung ausgeführt und die Artikel in den Ausgangsbereich oder den Ausgangslagerplatz eingelagert haben, wählen Sie die Aktionen **Kommissionierung registrieren** aus.  

Die für Lieferung verantwortliche Person kann die Artikel in den Warenausgang bringen und den Warenausgang, einschließlich dem zugehörigen Herkunftsbeleg, im Fenster **Warenausgang** buchen. Weitere Informationen finden Sie unter [Vorgehensweise: Artikel liefern](warehouse-how-ship-items.md).   

Zusätzlich zur Kommissionierung für Herkunftsbelege, die in diesem Thema beschrieben wird, können Sie Artikel ohne Bezug zu Herkunftsbelegen an Lagerorten entnehmen und einlagern. Weitere Informationen finden Sie unter [Vorgehensweise: Kommissionieren und Einlagern ohne Herkunftsbeleg](warehouse-how-to-create-put-aways-from-internal-put-aways.md).  

## <a name="handling-assemble-to-order-items-in-warehouse-shipments"></a>Verwenden von Auftragsmontageartikeln in Warenausgängen
In den Auftragsmontageszenarien wird das Feld **Zu liefernde Menge** in Warenausgangszeilen verwendet, um zu erfassen, wie viele Einheiten montiert werden. Die angegebene Menge wird dann als Montageausstoss gebucht, wenn der Warenausgang gebucht wird.

Für andere Warenausgangszeilen ist der Wert im Feld **Zu liefernde Menge** von Anfang an Null.

Wenn Arbeiter für montagefertige Teile oder für die gesamte Auftragsmontagemenge zuständig sind, erfassen sie diese im Feld **Zu liefernde Menge** in der Warenausgangszeile und wählen dann die Aktion **Warenausgang buchen**. Das Ergebnis ist, dass der entsprechende Montageausstoss gebucht wird, einschliesslich des Komponentenverbrauchs. Eine Verkaufslieferung für die Menge wird für den Verkaufsauftrag gebucht.

Vom Montageauftrag aus können Sie **Warenausgangszeile für Programmfertigung** wählen, um auf die Warenausgangszeile zuzugreifen. Dies ist für Arbeiter hilfreich, die das Fenster **Warenausgang** üblicherweise nicht verwenden.

Nachdem der Warenausgang gebucht ist, werden verschiedene Felder in der Verkaufsauftragszeile aktualisiert, um den Status im Lager anzuzeigen. Die folgenden Felder werden auch aktualisiert, um anzuzeigen, wie viele Auftragsmontagemengen noch nicht montiert und geliefert wurden:

- **Auftragsmontage - Lagerrestbestellmenge**
- **Auftragsmontage - Lagerrestbestellmenge (Basis)**

> [!NOTE]
> In Kombinationsszenarien, in denen ein Teil der Menge zunächst montiert und ein anderer aus dem Lager geliefert werden muss, werden mindestens zwei Warenausgangszeilen erstellt. Eine für die Auftragsmontagemenge, und eine für die Lagermenge.

> In diesem Fall wird die Auftragsmontagemenge wie in diesem Thema beschrieben behandelt, und die Lagermenge wird wie jede andere reguläre Warenausgangszeile verarbeitet. Weitere Informationen finden Sie im Abschnitt "Kombinationsszenarien" in [Auftragsmontage und Lagermontage verstehen](assembly-assemble-to-order-or-assemble-to-stock.md).

## <a name="see-also"></a>Siehe auch  
[Logistik](warehouse-manage-warehouse.md)  
[Lagerbesttand](inventory-manage-inventory.md)  
[Lagerortverwaltung einrichten](warehouse-setup-warehouse.md)     
[Montageverwaltung](assembly-assemble-items.md)    
[Designdetails: Logistik](design-details-warehouse-management.md)  
[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

