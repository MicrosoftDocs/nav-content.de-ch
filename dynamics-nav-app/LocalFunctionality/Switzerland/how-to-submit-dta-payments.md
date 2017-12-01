---
title: "Gewusst wie: Übermitteln Sie DTA-Zahlungen"
description: "Um Datenträgeraustausch-Zahlungen (DTA) an Ihre Bank für Zahlung zu buchen, müssen Sie einige Aufgaben ausführen."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: bf79d68ddb398672cccec48812266b8808e1e714
ms.contentlocale: de-ch
ms.lasthandoff: 10/26/2017

---
# <a name="how-to-submit-dta-payments"></a>Gewusst wie: Senden von DTA-Zahlungen
Um Datenträgeraustausch-Zahlungen (DTA) an Ihre Bank für Zahlung zu buchen, müssen Sie Folgendes tun:  

- Generieren einer DTA-Datei für elektronische Zahlung, nachdem Sie die Zahlungsavis gedruckt haben.  
- DTA-Zahlungsauftrag drucken.  

Bevor Sie DTA-Zahlungen buchen, müssen Sie die Liste von Kreditoren für DTA-Zahlung prüfen. Weitere Informationen finden Sie unter [Gewusst wie: Überprüfen einer Liste von Kreditoren für DTA-Zahlungen](how-to-verify-a-list-of-vendors-for-dta-payments.md).  

Sie können das Erf.-Journal buchen, nachdem die Bankzahlungen vollständig sind. Sie können im Zahlungsausgangs-Erfassungsjournal DTA-Zahlungen auf Grundlage gebuchter Rechnungen vorschlagen lassen. Die vorgeschlagenen Zahlungen enthalten Informationen zum Kreditor und zur externen Belegnummer und können geändert werden. Weitere Informationen finden Sie unter [Gewusst wie: Vorschlagen einer DTA-Zahlung für Kreditoren](how-to-suggest-dta-payment-for-vendors.md).  

## <a name="to-generate-a-dta-file"></a>So generieren Sie eine DTA-Datei  

1.  Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Zahlungs-Buchblatt** ein und wählen den zugehörenden Link aus.  
2.  Wählen Sie im Feld **Erf.-Journalname** den erforderlichen Erf.-Journalnamen aus.  
3.  Wählen Sie die Art aus, den Sie erstellen möchten beispielsweise eine DTA-Datei und dann die Aktion **DTA-Datei generieren** auswählen.  
4.  Füllen Sie im Stapelverarbeitungsauftrag **DTA Datei** die Felder wie in der folgenden Tabelle beschrieben aus.  

    |Feld|Description|  
    |---------------------------------|---------------------------------------|  
    |**DTA Bank für Datei**|Wählen Sie die DTA-Bankleitzahl, aus der die Daten für den gewünschten Namen und die Sicherungskopie übertragen werden müssen. Dieses Feld nutzt die Hauptbankadresse als Vorgabe, Sie können diese Informationen ändern, wenn Sie möchten.|  
    |**Sammelzahlung pro Kreditor**|Geben Sie an, ob die Zahlungszeilen, die denselben Kreditor haben, Währung, Bank und gutzuschreibende Bank in der erzeugten DTA-Datei zusammenfassen soll.|  

5.  Wählen Sie die Schaltfläche **OK** aus. Die DTA-Datei wird im angegebenen Ordner erstellt.  

Nachdem Sie die DTA-Datei generiert haben, können Sie den DTA-Vergütungsauftrag ausdrucken und sowohl die Datei als auch den Vergütungsauftrag an die Bank übertragen. Im DTA-Vergütungsauftrag sind alle vorgeschlagenen Kreditorenzahlungen in einem Fenster **Zahlungsausgangs Erf.-Journal** basierend auf dem Währungscode aufgelistet. Dieser Auftrag wird an die Bank gesendet, um die DTA-Datei zur Zahlung freizugeben.  

## <a name="to-print-a-dta-payment-order"></a>So drucken Sie einen DTA-Vergütungsauftrag  

1.  Alternativ wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Zahlungs-Buchblatt** ein und wählen den zugehörenden Link aus.  
2.  Wählen Sie im Feld **Erf.-Journalname** den erforderlichen Erf.-Journalnamen aus.  
3.  Wählen Sie die erforderliche vorgeschlagene Zahlungszeilen aus, und wählen Sie die Aktion **Vorgeschlagener DTA-Zahlungsauftrag** aus.  
4.  Geben Sie im Feld **Nachricht** eine Nachricht an die Bank ein, die unten auf dem Vergütungsauftrag ausgedruckt wird.  
5.  Wählen Sie die Schaltfläche **Drucken** aus, um den DTA-Zahlungsbericht zu drucken, oder die Schaltfläche **Vorschau**, um den Bericht auf dem Bildschirm anzuzeigen.  

    Sie müssen den DTA-Zahlungsauftrag und die DTA-Datei für die Bank buchen, in der Zahlungen an Kreditoren in mehrere Stunden freigegeben werden. Nachdem die Zahlungen von der Bank verarbeitet wurden, können Sie das Zahlungsjournal buchen.  

## <a name="see-also"></a>Siehe auch  
 [Elektronische Zahlungen mit DTA (Schweiz)](swiss-electronic-payments-using-dta.md)   
 [Gewusst wie: Vorschlagen einer DTA-Zahlung für Kreditoren](how-to-suggest-dta-payment-for-vendors.md)   
 [Gewusst wie: Überprüfen einer Liste von Kreditoren für DTA-Zahlungen](how-to-verify-a-list-of-vendors-for-dta-payments.md)   
 [Gewusst wie: Exportieren von Zahlungen mit EZAG](how-to-export-payments-using-ezag.md)

