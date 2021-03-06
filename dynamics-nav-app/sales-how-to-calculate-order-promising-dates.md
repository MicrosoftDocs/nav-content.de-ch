---
title: 'So wird''s gemacht: Lieferterminzusagen berechnen'
description: "Die Funktion \"Lieferterminzusagen\" ist ein Werkzeug zur Berechnung des frühestmöglichen Datums, an dem ein Artikel zum Versand oder zur Lieferung verfügbar ist. Sie erstellt ausserdem Bestellvorschlagszeilen für das Datum, welches Sie akzeptiert haben."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/10/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 5c2167397d95d04c937ddf1820e6e9edff906b2f
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-calculate-order-promising-dates"></a>So wird's gemacht: Lieferterminzusagen berechnen
Ein Mandant muss in der Lage sein, seine Debitoren über Auftragslieferdaten zu informieren. Das Fenster **Lieferzusagenzeilen** ermöglicht Ihnen, dies von einer Verkaufsauftragszeile aus zu tun.  

Auf Grundlage der bekannten und erwarteten Verfügbarkeitstermine eines Artikels berechnet [!INCLUDE[d365fin](includes/d365fin_md.md)] sofort die Lieferdaten, die dann dem Debitor zugesagt werden können.  

Wenn Sie in einer Verkaufszeile ein gewünschtes Lieferdatum eingeben, wird dieses Datum als Ausgangspunkt für die folgenden Berechnungen verwendet:  

- Gewünschtes Lieferdatum - Transportzeit = Geplantes Warenausgangsdatum  
- Geplantes Warenausgangsdatum - Ausgeh. Lagerdurchlaufzeit = Warenausgangsdatum  

Falls die Artikel am Lieferdatum zur Kommissionierung zur Verfügung stehen, kann der Verkaufsvorgang fortgesetzt werden. Falls die Artikel am Lieferdatum nicht zur Kommissionierung zur Verfügung stehen, erscheint eine Warnmeldung die auf diesen Umstand hinweist.  

Wenn Sie kein angefordertes Lieferdatum auf der Verkaufsauftragszeile angeben oder das angeforderte Lieferdatum nicht eingehalten werden kann, wird das früheste Datum, an dem die Artikel verfügbar sind, berechnet. Dieses Datum wird dann im Feld **Versanddatum** auf der Zeile eingegeben, und das Datum, an dem Sie planen, die Artikel zu liefern, sowie das Datum, an dem Sie an den Kunden ausgeliefert werden, werden anhand der nachfolgenden Formeln berechnet.  

- Warenausgangsdatum + Ausgeh. Lagerdurchlaufzeit = Geplantes Warenausgangsdatum  
- Geplantes Warenausgangsdatum + Transportzeit = Geplantes Lieferdatum  

## <a name="about-order-promising"></a>Über Lieferterminzusagen
Die Funktion Lieferzusagen ermöglicht Ihnen, den Versand oder die Lieferung eines Auftrags zu einem bestimmten Datum zuzusagen. Das Datum, zu dem der Artikel verfügbar oder geeignet für eine Zusage ist, wird berechnet und Auftragszeilen für das Datum, welches Sie akzeptiert haben, erstellt. Die Funktion "Lieferterminzusagen" ist ein Werkzeug zur Berechnung des frühestmöglichen Datums, an dem ein Artikel zum Versand oder zur Lieferung verfügbar ist. Sie erstellt außerdem Bestellvorschlagszeilen, falls die Artikel zuerst gekauft werden müssen, für das Datum, welches Sie akzeptiert haben.

[!INCLUDE[d365fin](includes/d365fin_md.md)] verwendet zwei grundlegende Konzepte:  

- Lieferzusage (Available to promise, ATP)  
- Beschaffungszusage (Capable to promise, CTP)  

### <a name="available-to-promise"></a>Lieferzusage  
"Lieferzusage (Available to promise, ATP)" berechnet die Daten auf der Grundlage des Reservierungssystems. Dabei wird eine Verfügbarkeitsprüfung der nicht reservierten Mengen im Lagerbestand im Hinblick auf die geplante Produktion, Einkäufe, Umlagerungen und Verkaufsreklamationen durchgeführt. Auf Grundlage dieser Informationen berechnet  [!INCLUDE[d365fin](includes/d365fin_md.md)] automatisch das Auslieferungsdatum des Kundenauftrags, weil die Artikel, entweder im Lagerbestand oder im Rahmen geplanter Wareneingänge, verfügbar sind.  

### <a name="capable-to-promise"></a>Beschaffungszusage  
"Beschaffungszusage (Capable to promise, CTP)" geht von einem "Was wäre-wenn"-Szenario aus, bei dem der Artikel nicht im Lagerbestand vorhanden ist und keine Aufträge geplant sind. Auf Grundlage dieses Szenarios berechnet [!INCLUDE[d365fin](includes/d365fin_md.md)] das früheste Datum, zu dem der Artikel verfügbar sein kann, wenn er gefertigt werden, bezogen werden oder umgelagert werden muss.  


### <a name="calculations"></a>Berechnungen  
Wenn [!INCLUDE[d365fin](includes/d365fin_md.md)] das Auslieferungsdatum des Debitors berechnet, werden zwei Aufgaben ausgeführt:  

- Berechnung des frühesten Lieferdatums, wenn der Debitor kein bestimmtes Lieferdatum angefragt hat.  
- Prüfung, ob das vom Debitor angefragte oder ihm zugesagte Lieferdatum realistisch ist.  

Wenn der Debitor kein bestimmtes Lieferdatum anfragt, wird das Lieferdatum auf das Arbeitsdatum festgelegt, und die Verfügbarkeit basiert dann auf diesem Datum. Wenn der Artikel im Lagerbestand vorhanden ist, berechnet [!INCLUDE[d365fin](includes/d365fin_md.md)] den Termin, zu dem der Auftrag geliefert werden kann. Dazu dienen die folgenden Formeln:  

- Warenausg.-Datum + Ausgehende Lagerdurchlaufzeit + Geplanter Warenausgang + Lagerdurchlaufzeit = Datum  
- Geplantes Warenausgangsdatum + Transportzeit = Geplantes Lieferdatum  

[!INCLUDE[d365fin](includes/d365fin_md.md)] überprüft dann, ob das berechnete Lieferdatum realistisch ist; dazu wird zeitlich rückwärts berechnet, wann der Artikel verfügbar sein muss, um den zugesagten Termin einhalten zu können. Dazu dienen die folgenden Formeln:  

- Geplantes Lieferdatum - Transportzeit = Geplantes Warenausgangsdatum  
- Geplantes Warenausgangsdatum - Ausgehende Lagerdurchlaufzeit + Warenausg.-Datum  

Das Lieferdatum wird für die Verfügbarkeitsprüfung verwendet. Wenn der Artikel an diesem Datum verfügbar ist, bestätigt [!INCLUDE[d365fin](includes/d365fin_md.md)], dass die angeforderte/zugesagte Lieferung eingehalten werden kann, indem das geplante Lieferdatum auf das angefragte/zugesagte Lieferdatum gesetzt wird. Wenn der Artikel nicht verfügbar ist, wird ein leeres Datum zurückgegeben, und der Auftragsbearbeiter kann die CTP-Funktion verwenden.  

Auf Grundlage neuer Daten und Uhrzeiten werden alle damit verbundenen Daten gemäss den oben aufgeführten Formeln berechnet. Die CTP-Berechnung dauert, gibt jedoch ein präzises Datum an, zu dem der Debitor die Lieferung des Artikels erwarten kann. Die Daten, die per CTP berechnet werden, werden den Fenstern **Geplantes Lieferdatum** und **Frühestmög. Warenausgangsdatum** im Fenster **Lieferterminzusagenzeilen** angegeben.  

Der Auftragsverarbeiter beendet den CTP-Prozess, indem er die Datumsangaben akzeptiert. Dies bedeutet, dass eine Planungszeile und ein Reservierungsposten für diesen Artikels vor den berechneten Daten erstellt werden, damit sichergestellt ist, dass der Auftrag erfüllt wird.  

Zusätzlich zu den externen Lieferterminzusagen, die Sie im Fenster **Lieferterminzusagenzeilen** durchführen können, können Sie interne oder externe Lieferdaten für Stücklistenrtikel zusagen. Weitere Informationen finden Sie unter [Vorgehensweise: Die Verfügbarkeit von Artikeln anzeigen](inventory-how-availability-overview.md)

## <a name="to-set-up-order-promising"></a>Lieferterminzusagen einrichten  
1. Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png " Nach Seite oder Bericht suchen")und geben **Lieferterminzusagen Einrichtung** ein. Wählen Sie dann den zugehörigen Link aus.  
2. Geben Sie eine Zahl und einen Zeiteinheitencode in das Feld **Verschiebung (Zeit)** ein. Wählen Sie einen der folgenden Codes aus.  

    |Code|Beschreibung|  
    |----------|-----------------|  
    |**T**|Kalendertag|  
    |**a**|Woche|  
    |**M**|Monat|  
    |**Q**|Quartal|  
    |**J**|Jahr|  

    "3w" bedeutet zum Beispiel, dass die Verschiebung drei Wochen beträgt. Stellen Sie ein "l" vor einen dieser Codes, um die jeweils laufende Zeiteinheit anzugeben. Wenn Sie zum Beispiel als Basis für die Verschiebung den aktuellen Monat verwenden möchten, geben Sie **lm** ein.  
3. Geben Sie in das Feld **Lieferterminzusagennummern** eine Nummernserie ein, indem Sie eine Zeile aus der Liste im Fenster **Nummernserien** wählen.  
4. Geben Sie eine Lieferterminzusagenvorlage im Feld **Lieferterminzusagenvorlage** ein, indem Sie eine Zeile im Fenster **Bestellvorschlag Vorl.-Übers.** wählen.  
5. Geben Sie im Feld **Lieferterminzusagenvorschlag** einen Vorschlag ein, indem Sie eine Zeile im Fenster **Bestellvorschlagsnamen** wählen.

### <a name="to-enter-inbound-warehouse-handling-time-in-the-inventory-setup-window"></a>Eingehende Lagerdurchlaufzeit im Einrichtungsfenster des Bestands eingeben  
Wenn Sie die Lagerdurchlaufzeit bei der Berechnung der Lieferterminzusage in der Einkaufszeile berücksichtigen wollen, können Sie sie als Vorgabewert für das Lager und für Ihren Lagerort einrichten.    
1. Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben Sie **Lagereinrichtung** ein. Wählen Sie dann den zugehörigen Link aus.  
2. Im Inforegister **Allgemein** im Feld **Eingeh. Lagerdurchlaufzeit** geben Sie die Anzahl Tage ein, die die Anwendung bei der Berechnung der Lieferterminzusage berücksichtigen soll.  

> [!NOTE]  
>  Wenn Sie das Feld **Eingeh. Lagerdurchlaufzeit** auf der **Lagerortkarte** für Ihren Lagerort ausgefüllt haben, verwendet die Anwendung den Inhalt dieses Feldes als eingehende Vorgabelagerdurchlaufzeit.  

### <a name="to-enter-inbound-warehouse-handling-time-on-location-cards"></a>Eingehende Lagerdurchlaufzeit in Lagerortkarten eingeben  
1. Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben Sie **Lagerplätze** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Öffnen Sie die relevante Lagerortkarte.  
3.  Im Inforegister **Lager** im Feld **Eingeh. Lagerdurchlaufzeit** geben Sie die Anzahl Tage ein, die bei der Berechnung der Lieferterminzusage berücksichtigt werden soll.  

> [!NOTE]  
>  Wenn Sie das Feld **Eingeh. Lagerdurchlaufzeit** leer lassen, verwendet die Berechnung den Wert im Fenster **Lager Einrichtung**.

### <a name="to-enter-outbound-warehouse-handling-time-in-the-inventory-setup-window"></a>Ausgehende Lagerdurchlaufzeit im Einrichtungsfenster des Bestands eingeben  
Wenn Sie eine ausgehende Lagerdurchlaufzeit bei der Berechnung der Lieferterminzusage in der Verkaufszeile berücksichtigen möchten, können Sie diese als Vorgabewert für das Lager eingeben.

1. Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben Sie **Lagereinrichtung** ein. Wählen Sie dann den zugehörigen Link aus.  
2. Im Inforegister **Allgemein** im Feld **Ausgeh. Lagerdurchlaufzeit** geben Sie die Anzahl Tage ein, die die Anwendung bei der Berechnung der Lieferterminzusage berücksichtigen soll.  

> [!NOTE]  
>  Wenn Sie das Feld **Ausgeh. Lagerdurchlaufzeit** auf der Standortkarte für Ihren Standort ausgefüllt haben, wird der Inhalt dieses Feldes als ausgehende Vorgabelagerdurchlaufzeit verwendet.  

### <a name="to-enter-outbound-warehouse-handling-time-on-location-cards"></a>Ausgehende Lagerdurchlaufzeit der Logistik in Standortkarten eingeben  
1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben Sie **Lagerplätze** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Öffnen Sie die relevante Lagerortkarte.  
3.  Im Inforegister **Lager** im Feld **Ausgeh. Lagerdurchlaufzeit** geben Sie die Anzahl Tage ein, die bei der Berechnung der Lieferterminzusage berücksichtigt werden soll.  

> [!NOTE]  
>  Wenn Sie das Feld **Ausgehende Lagerhausbearbeitungszeit** leer lassen, dass verwendet die Kalkulation den Wert im Fenster **Bestandeinrichtung**

## <a name="to-make-an-item-critical"></a>Einen Artikel als kritisch kennzeichnen  
Bevor ein Artikel bei der Berechnung der Lieferterminzusage berücksichtigt werden kann, muss er als kritisch markiert werden Diese Einstellungen stellen sicher, dass unkritische Artikel nicht irrelevante Lieferterminzusagen verursachen.   
1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (media/ui-search/search_small.png "Nach Seite oder Bericht suchen")aus und geben Sie **Artikel** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Öffnen Sie die entsprechende Artikelkarte.  
3.  Wählen Sie im Inforegister **Planung** das Feld **Kritisch** aus.  

## <a name="to-calculate-an-order-promising-date"></a>Lieferterminzusagen berechnen  
1.  Alternativ wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Verkaufsauftrag** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Öffnen Sie den relevanten Verkaufsauftrag, und wählen Sie die Verkaufszeilen aus, die berechnet werden sollen.  
3.  Wählen Sie die **Lieferterminzusagen** Aktion aus, und wählen Sie die **Lieferterminzusagenzeilen** Aktion aus.  
4.  Wählen Sie eine Zeile aus, und wählen Sie dann eine der folgenden Optionen aus:  

    - Wählen Sie **Verfügbar für Zusage**, wenn die Anwendung das früheste Verfügbarkeitsdatum des Artikels unter Berücksichtigung des Lagerbestands der geplanten Zugänge und des Bruttobedarfs berechnen soll.  
    - Wählen Sie **Geeignet für Zusage**, wenn Sie wissen, dass der Artikel aktuell nicht an Lager ist und das früheste Datum, zu dem der Artikel durch neue Lagerzugänge verfügbar sein wird, errechnen wollen.  
5.  Wählen Sie die Schaltfläche **Akzeptieren**, um das früheste verfügbare Lieferdatum zu akzeptieren.  

## <a name="see-also"></a>Siehe auch  
[Verkauf](sales-manage-sales.md)  
[Terminberechnung für Einkäufe](purchasing-date-calculation-for-purchases.md)  
[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

