---
title: Elektronische Zahlungen (Schweiz)
description: "Schweizer Erweiterungen ermöglichen Ihnen, elektronisch Rechnungen an Debitoren zu senden. Sie können Rechnungen direkt mithilfe der Onlinebankingsoftware des Debitors ausstellen und bezahlen."
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
ms.openlocfilehash: e08f2c3d911e20c631f32683c284c0988a2b55b9
ms.contentlocale: de-ch
ms.lasthandoff: 10/26/2017

---
# <a name="swiss-electronic-payments"></a>Elektronische Zahlungen (Schweiz)
[!INCLUDE[navnow](../../includes/navnow_md.md)]ermöglicht Ihnen, elektronisch Rechnungen an Debitoren zu senden. Sie können Rechnungen direkt mithilfe der Onlinebankingsoftware des Debitors ausstellen und bezahlen.  

## <a name="electronic-payment-methods"></a>Elektronische Zahlungsformen  
Elektronische Zahlungen können mithilfe der folgenden Zahlungsformen durchgeführt werden:  

- Datenträgeraustausch (DTA)  
- Elektronischer Zahlungsauftrag (EZAG)  
- Einzahlungsschein mit Referenznummer (ESR)  
- Lastschrift Verfahren (LSV+)  
- SEPA Kreditübertragungen  

## <a name="dta-and-ezag"></a>DTA und EZAG  
Die elektronische Zahlungsmethode DTA ist ein universaler Dienst, der von Schweizer Banken für die elektronische Begleichung von Rechnungen im DTA-Format mithilfe von standardisierten Zahlungsdatensätzen zur Verfügung gestellt wird. Diese Methode basiert auf Datenträgern und Datenübertragung. Die Spezifikationen werden von Swiss Interbank Clearing (SIC) koordiniert. Weitere Informationen erhalten Sie unter [Elektronische Zahlungen mit DTA (Schweiz)](swiss-electronic-payments-using-dta.md).  

EZAG ist die elektronische Zahlungsmethode von PostFinance und erfordert ein Girokonto. Aufträge für Kreditorenzahlungen können im DTA-Bankformat oder PostFinance-EZAG-Format erstellt und übermittelt werden.  

## <a name="esr"></a>ESR  
ESR ist ein elektronischer Kreditorendienst, der Zahlungsscheine zum Einziehen von Geld verwendet. Es ist das elektronische Standardzahlungssystem, das von Swiss Post ins Leben gerufen wurde. ESR-Zahlungsscheine können als Rechnungsanlage gedruckt, ESR-Referenznummern berechnet und ESR-Dateien, die Zahlungsinformationen von Banken enthalten, importiert werden. Weitere Informationen erhalten Sie unter [Elektronische Zahlungen mit ESR (Schweiz)](how-to-print-esr-invoices.md). Sie können auch ESR- und ESR+-Zahlungen mithilfe der Version dieser Zahlungsform der Bank machen, die Bank-ESR (BESR) heißt.  

## <a name="lsv"></a>LSV+  
LSV+ ist ein Abbuchungsdienst, der für das Bearbeiten von Zahlungen verwendet wird. Unternehmen können Debitorenzahlungen direkt von der Bank des Debitors mit der Abbuchung freigeben. Debitorenzahlungen per Lastschrift können im LSV+-Bankformat oder im DebitDirect PostFinance-Format angefordert bzw. eingezogen werden. Weitere Informationen erhalten Sie unter [Elektronische Zahlungen mit LSV+ (Schweiz)](swiss-electronic-payments-using-lsv-.md).  

## <a name="sepa-credit-transfers"></a>SEPA Kreditübertragungen  
Um Zahlungsvorschläge entsprechend dem SEPA-Standard zu exportieren, müssen Sie ein Bankkonto verwenden. Um sicherzustellen, dass die entsprechenden Fibuposten mit den generierten für lokale Schweizer Zahlungsmethoden übereinstimmen (siehe oben), muss der Wert im Feld **Bankkonto Buchungsgruppe** im Fenster **Bankkontokarte** auf das jeweilige Fibukonto weisen. Weitere Informationen finden Sie unter [Gewusst wie: SEPA-Lastschrifteinzugsposten erstellen und in eine Bankdatei exportieren](../../finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md)  

## <a name="see-also"></a>Siehe auch  
 [Gewusst wie: Importieren von Bankenclearing-Nummern (Schweiz)](how-to-import-swiss-bank-clearing-numbers.md)   
 [Elektronische Zahlungen mit DTA (Schweiz)](swiss-electronic-payments-using-dta.md)   
 [Elektronische Zahlungen mit ESR (Schweiz)](swiss-electronic-payments-using-esr.md)   
 [Gewusst wie: Drucken von ESR-Rechnungen](how-to-print-esr-invoices.md)   
 [Schweizer Elektronische Zahlungen mithilfe von LSV+](swiss-electronic-payments-using-lsv-.md)   
 [Lokale Funktionalität für die Schweiz](switzerland-local-functionality.md) [Gewusst wie: SEPA-Lastschrifteinzugsposten erstellen und in eine Bankdatei exportieren](../../finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md)  
 [Zahlungen vornehmen](../../payables-make-payments.md)

