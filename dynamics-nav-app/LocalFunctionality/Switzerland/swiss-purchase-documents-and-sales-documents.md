---
title: Einkaufsbelege und Verkaufsbelege (Schweiz)
description: Schweizer Erweiterungen enthalten Sonderkauf- und Verkaufsbelegfunktionen.
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
ms.openlocfilehash: 9142631a84e8b756d4fa99b220d2cca15c4b8e79
ms.contentlocale: de-ch
ms.lasthandoff: 10/26/2017

---
# <a name="swiss-purchase-documents-and-sales-documents"></a>Einkaufsbelege und Verkaufsbelege (Schweiz)
[!INCLUDE[navnow](../../includes/navnow_md.md)]Enthält Schweizer Erweiterungen für Kauf- und Verkaufsbelege. Dies beinhaltet Folgendes:  

- Verbesserte Buchungsbeschreibung für Finanzbuchhaltungseinträge, Debitorenposten und Kreditorenposten. Weitere Informationen finden Sie in der Tabelle Fibuposten, der Debitor-Tabelle und der Tabelle Kreditorenposten.  
- Die Möglichkeit, Untertitel, Zwischensummen sowie Von- und Bis-Summen in Verkaufsofferten und Verkaufsaufträgen anzuzeigen.  
- Die Möglichkeit, Rechnungssummen in Zahlungsjournalzeilen zu runden, wenn ein Rabatt gewährt wird.  
- Die Möglichkeit, den Ausdruck zusätzlicher Lieferbelege für Einkaufs- und Verkaufsrechnungen zu deaktivieren.  

## <a name="purchase-documents-and-sales-documents"></a>Einkaufsbelege und Verkaufsbelege  
Die in Posten für Einkaufs- und Verkaufsaufträge gebuchten Buchungsbeschreibungen enthalten den Namen der Kreditoren oder Debitoren und die Rechnungs- oder Gutschriftsnummern. Zum Beispiel ist **Inv 103020/The Cannon Group PLC** eine Buchungsbeschreibung. Diese Buchungsbeschreibung enthält immer eine für Finanztransaktionen geltende Nummer, die die Analyse der Transaktionen erleichtert.  

### <a name="sales-quotes-and-sales-orders"></a>Verkaufsofferten und Verkaufsaufträge  
Wenn die Art der Verkaufsofferten- oder Verkaufsauftragszeile beim Erstellen einer Verkaufsofferte bzw. eines Verkaufsauftrags **Von-Summe** oder **Bis-Summe** lautet, werden die in den Zeilen aufgeführten Artikel als physische Artikel oder Serviceartikel markiert. Für die Artikel werden dann Untertitel für jede Artikelgruppe angezeigt, und für jede Artikelgruppe wird eine Zwischensumme erstellt.  

Die Artikel werden basierend auf den vom System generierten Werten im Feld **Ebene** unterteilt.  

Sie können einen Artikel in der Verkaufsoffertenzeile als Variante angeben. So können Sie die alternativen Artikel auflisten, ohne den Preis in die Offerte einzuschliessen. Sie können auch basierend auf dem Wert im Feld **Position** der Verkaufsofferten- oder Verkaufsauftragszeile auf bestimmte Teile einer Verkaufsofferte oder eines Verkaufsauftrags verweisen. Weitere Informationen finden Sie in der Tabelle Verkaufszeilen.  

## <a name="purchase-invoices-and-sales-invoices-with-payment-discounts"></a>Einkaufsrechnungen und Verkaufsrechnungen mit Rabatten  
Für Einkaufs- und Verkaufsrechnungen wird der Rechnungsbetrag um den Rabattbetrag reduziert und dann gerundet. Die Rechnungssumme wird ebenfalls gerundet, wenn ein Rabatt gewährt wird. Weitere Informationen finden Sie unter Fibuposten Einrichtungtabelle.  

## <a name="shipment-documents"></a>Lieferbelege  
Im Fenster **Debitoren & Verkauf Einr.** wird das **Lieferung für Liefern und Rechnung** Feld verwendet, damit der Druck für zusätzlicher Warenausgangsbelegen für Einkaufsrechnungen und Verkaufsrechnungen ausgeschaltet werden kann. Wenn Sie einen Auftrag buchen, wird automatisch eine gebuchte Lieferung und eine gebuchte Rechnung erstellt. Wenn die ausgedruckte Rechnung auch als Lieferbeleg verwendet wird, muss die Lieferungsdokumentation nicht zusätzlich ausgedruckt werden. Sie können das Drucken von zusätzlichen Versanddokumenten für Verkaufs- und Einkaufsrechnungen deaktivieren, indem Sie das Feld **Lieferung für Liefern und Rechnung** im Fenster**Verkauf und Kauf einrichten** deaktivieren. Weitere Informationen finden Sie unter der Tabelle Debitoren & Verkauf Einr.  

## <a name="see-also"></a>Siehe auch  
 [Gewusst wie: Einrichten der automatischen Archivierung von Belegen in der Schweiz](how-to-set-up-automatic-archiving-of-documents-in-switzerland.md)   
 [Gewusst wie: Importieren von Schweizer Postleitzahlen](how-to-import-swiss-post-codes.md)   
 [Gewusst wie: Drucken einer Lager-Kommissionierliste aus Verkaufsaufträgen](how-to-print-an-inventory-picking-list-from-a-sales-order.md)   
 [Gewusst wie: Drucken von Verkaufsaufträgen und Bestellungen während der Stapelbuchung.](how-to-print-sales-and-purchase-orders-during-batch-posting.md)   
 [Lokale Funktion (Schweiz)](switzerland-local-functionality.md)

