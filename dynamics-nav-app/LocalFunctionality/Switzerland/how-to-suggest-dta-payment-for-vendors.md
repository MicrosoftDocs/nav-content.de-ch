---
title: "Gewusst wie: DTA Zahlungen für Kreditoren vorschlagen"
description: "Sie können Kreditorenzahlungen mithilfe des Zahlungsausgangs Erf.-Journals vorschlagen und die überfälligen Rechnungen für einzelne Kreditoren an das Erf.-Journal übertragen. Sie können jeden Kreditor für verknüpfte offene Gutschriften oder offene Zahlungen auch überprüfen und erstellen eine Kreditorenliste für die Datenträgeraustausch-Bearbeitung (DTA)."
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
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: b51b3f9273e9e737ef09901b0718d55350d44f87
ms.contentlocale: de-ch
ms.lasthandoff: 10/26/2017

---
# <a name="how-to-suggest-dta-payment-for-vendors"></a>Gewusst wie: DTA Zahlungen für Kreditoren vorschlagen
Sie können Kreditorenzahlungen mithilfe des Zahlungsausgangs Erf.-Journals vorschlagen und die überfälligen Rechnungen für einzelne Kreditoren an das Erf.-Journal übertragen. Sie können jeden Kreditor für verknüpfte offene Gutschriften oder offene Zahlungen auch überprüfen und erstellen eine Kreditorenliste für die Datenträgeraustausch-Bearbeitung (DTA). Weitere Informationen finden Sie unter [Gewusst wie: Überprüfen einer Liste von Kreditoren für DTA-Zahlungen](how-to-verify-a-list-of-vendors-for-dta-payments.md).  

Während der Batchverarbeitung der DTA-Zahlungsvorschläge wir der Fremdwährung (FCY)- Betrag zur Mandantenwährung (LCY) mit dem Tageskurs für FCY-Zahlungen erstellt und in das Zahlungsausgangs Erf.-Journal übertragen. Weitere Informationen finden Sie im Fenster **Zahlungs-Erf.-Journal**. Im Falle einer Kontobelastung wird der Betrag mit dem debitierten Mandantenwährungsbetrag überschrieben, und der Wechselkurs oder der Wechselkursfaktor wird berechnet.

## <a name="to-suggest-dta-payment-for-vendors"></a>So schlagen Sie DTA-Zahlungen für Kreditoren vor  

1.  Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Zahlungs-Buchblatt** ein und wählen den zugehörenden Link aus.  
2.  Wählen Sie im Feld **Erf.-Journalname** den erforderlichen Erf.-Journalnamen aus.  
3.  Wählen Sie die erforderliche vorgeschlagene Zahlungszeilen aus, und wählen Sie die Aktion **Vorgeschlagene DTA-Kreditorenzahlung** aus.  
4.  Füllen Sie im Fenster **DTA Zahlungsvorschlag** auf dem Inforegister **Optionen** die Felder gemäss der Beschreibung in der folgenden Tabelle aus.  

    |Feld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Buchungsdatum**|Geben Sie das Gutschriftsdatum für die Zahlung an. Dieses Datum ist hilfreich, um zu bestimmen, ob ein Skonto angegeben wurde.|  
    |**Fälligkeitsdatum ab**|Geben Sie das Startdatum an, sodass die offenen Rechnungen im Zahlungsvorschlag berücksichtigt werden.|  
    |**Fälligkeitsdatum bis**|Geben Sie das Enddatum an, sodass die offenen Rechnungen im Zahlungsvorschlag berücksichtigt werden.|  
    |**Skonto berücksichtigen**|Geben Sie an, ob die Skontozahlungen außerhalb des Fälligkeitsdatumsbereichs für den Zahlungsvorschlag berücksichtigt werden.|  
    |**Skontodatum von**|Geben Sie das Startdatum für das Skonto an. Die offenen Posten mit Skontodatum innerhalb eines bestimmten Datumsbereichs sind in einem Zahlungsvorschlag berücksichtigt.|  
    |**Skontodatum bis**|Geben Sie das Enddatum für das Skonto an. Die offenen Posten mit Skontodatum innerhalb eines bestimmten Datumsbereichs sind in einem Zahlungsvorschlag berücksichtigt.|  
    |**Verfügbarer Betrag (MW)**|Geben Sie den Betrag der Summe aller Zahlungen ein.|  
    |**Erste Belegnr.**|Geben Sie die Zahlungsvorschlagsbelegnummer an. Diese Nummer wird gemäss der Nummernserie für das aktuelle Protokoll zugeordnet.|  
    |**Belastung auf Bank**|Wählen Sie den Code der Bank, die die Gutschrift erhält. Die Bank muss für DTA aktiviert werden.|  
    |**Auto. Belastungsbank**|Geben Sie an, ob die Bank automatisch die Gutschrift erhält, abhängig vom Währungscode.|  

5.  Wählen Sie die Schaltfläche **OK** aus.  

Während der Verarbeitung wird jeder Kreditor auf offene Gutschriften oder offene Zahlungen überprüft, und am Ende des Vorgangs wird eine Meldung angezeigt. Alle zugehörigen Zeilen werden an das Zahlungsausgangs Erf.-Journal übertragen. Die zugehörigen Kreditorenposten werden mit **DTA** gekennzeichnet, um die Übertragung von doppelten Einträgen an das Zahlungsausgangs Erf.-Journal zu verhindern. Sie können die vorgeschlagenen Zahlungen anzeigen, überprüfen und ändern und entscheiden, ob Sie die Zahlungen um die Gutschriftsbeträge verringern oder ob Sie die offenen Gutschriften und Rechnungen übernehmen möchten.  

## <a name="see-also"></a>Siehe auch  
 [Elektronische Zahlungen mit DTA (Schweiz)](swiss-electronic-payments-using-dta.md)   
 [Gewusst wie: Überprüfen einer Liste von Kreditoren für DTA-Zahlungen](how-to-verify-a-list-of-vendors-for-dta-payments.md)   
 [Gewusst wie: Senden von DTA-Zahlungen](how-to-submit-dta-payments.md)   
 [Gewusst wie: Exportieren von Zahlungen mit EZAG](how-to-export-payments-using-ezag.md)   
 [Zahlungen vornehmen](../../payables-make-payments.md)

