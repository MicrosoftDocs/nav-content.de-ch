---
title: Elektronischer Zahlungsverkehr (Schweiz) mit LSV+
description: "Die elektronische Zahlungsmethode Lastschrift Verfahren (LSV+) oder Einzug, eine optimierte Version von LSV, ermöglicht Firmen das direkte Abrufen von Zahlungen von Debitorenbankkonten. Zum Abrufen von Debitorenzahlungen muss eine LSV-Datei an die Bank gesendet werden, die dann die Abbuchung der in der Datei angeforderten Zahlungen abwickelt."
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: d7f41ba3ad0706bad87d98b590eda38304bddf85
ms.contentlocale: de-ch
ms.lasthandoff: 10/23/2017

---
# <a name="swiss-electronic-payments-using-lsv"></a>Elektronischer Zahlungsverkehr (Schweiz) mit LSV+
Die elektronische Zahlungsmethode Lastschrift Verfahren (LSV+) oder Einzug, eine optimierte Version von LSV, ermöglicht Firmen das direkte Abrufen von Zahlungen von Debitorenbankkonten. Zum Abrufen von Debitorenzahlungen muss eine LSV-Datei an die Bank gesendet werden, die dann die Abbuchung der in der Datei angeforderten Zahlungen abwickelt.  

Die LSV+-Methode ist ein Einzugsverfahren mit Recht auf Widerspruch. BDD (Business Direct Debit) ist ein Einzugsverfahren ohne Recht auf Widerspruch. Die Formate der an die Bank gesendeten Dateien sind für LSV+ und BDD identisch.  

Bevor Sie das LSV-Modul verwenden, müssen die Einstellungen im Fenster **LSV Einrichtung** festgelegt werden. Weitere Informationen finden Sie in der Tabelle "LSV Einrichtung".  

## <a name="automatic-esr-processing"></a>Automatische ESR-Verarbeitung  
Sie können Zahlungsgutschrifttransaktionen im Einzahlungsschein mit Referenznummer (ESR)-Dateiformat von der Bank herunterladen. Wenn die ESR-Referenznummer in das LSV+-System integriert ist, können Sie verarbeitete LSV-Zahlungen in der ESR-Datei erhalten. Wenn LSV+-Zahlungen in Ihren importierten LSV-Dateien enthalten sind, werden die entsprechenden LSV-Journalzeilen automatisch geschlossen. Die automatische ESR-Verarbeitung wird nur bei Zahlungen in Schweizer Franken (CHF) durchgeführt. Hierzu müssen Sie folgende Schritte durchführen:  

- Nachdem Sie die LSV+-Datei an die Bank gesendet haben, übermitteln Sie innerhalb von drei Tagen nach dem angeforderten LSV-Verarbeitungsdatum einen Zahlungsbericht.  

- Importieren Sie die ESR-Dateien, und buchen Sie die ESR-Journale. Falls eine importierte ESR-Transaktion mit einer offenen LSV+-Zahlungszeile verknüpft ist, wird die entsprechende LSV-Journalzeile automatisch von ESR geschlossen.  

    > [!NOTE]  
    >  Beim Importieren einer ESR-Datei wird die LSV-Journalzeile unabhängig vom ESR-Transaktionstyp von ESR geschlossen, falls das entsprechende LSV-Journal gefunden wird.  

- Nach dem LSV-Verarbeitungsdatum können Sie die LSV-Journalzeilen überprüfen. Wenn alle LSV-Journalzeilen geschlossen sind, wird der **LSV-Status** zu **Beendet** aktualisiert.  

## <a name="see-also"></a>Siehe auch  
 [Gewusst wie: Verarbeiten eines LSV-Einzugs](how-to-process-an-lsv-collection.md)   
 [Gewusst wie: Abschliessen eines LSV-Einzugs](how-to-close-an-lsv-collection.md)   
 [Gewusst wie: Buchen von LSV+-Zahlungen](how-to-post-lsv-payments.md)   
 [Gewusst wie: Exportieren von Zahlungen mit LSV](how-to-export-payments-using-lsv.md)   
 [Elektronische Zahlungen (Schweiz)](swiss-electronic-payments.md)   
 [Elektronische Zahlungen mit DTA (Schweiz)](swiss-electronic-payments-using-dta.md)   
 [Elektronische Zahlungen mit ESR (Schweiz)](swiss-electronic-payments-using-esr.md)   
 [Zahlungen vornehmen](../../payables-make-payments.md)

