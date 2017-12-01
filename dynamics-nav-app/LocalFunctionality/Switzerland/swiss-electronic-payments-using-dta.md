---
title: Elektronische Zahlungen mit DTA (Schweiz)
description: "In [!INCLUDE[navnow](../../includes/navnow_md.md)] können elektronische Zahlungen für Rechnungen mit der elektronischen Zahlungsform \"DatenTrägerAustausch (DTA)\" vorgenommen werden. Schweizer Banken verwenden die elektronische Zahlungsform DTA, um Zahlungen auf effiziente Weise anhand standardisierter Zahlungsdatensätze auszugleichen."
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
ms.openlocfilehash: f2a71eb29a48e5a47c1cb50a10a6ea67d5d2221c
ms.contentlocale: de-ch
ms.lasthandoff: 10/23/2017

---
# <a name="swiss-electronic-payments-using-dta"></a>Elektronische Zahlungen mit DTA (Schweiz)
In [!INCLUDE[navnow](../../includes/navnow_md.md)] können elektronische Zahlungen für Rechnungen mit der elektronischen Zahlungsform "DatenTrägerAustausch (DTA)" vorgenommen werden. Schweizer Banken verwenden die elektronische Zahlungsform DTA, um Zahlungen auf effiziente Weise anhand standardisierter Zahlungsdatensätze auszugleichen. Diese Methode basiert auf Datenträgern und Datenübertragung. Mit diesem elektronischen Dienst können Sie Zahlungen elektronisch in das DTA-Format konvertieren und anschliessend zur Zahlung an die Bank senden.  

> [!NOTE]  
>  Bevor Sie die elektronische Zahlungsform DTA verwenden, müssen Sie die DTA-Einstellungen für elektronische Zahlungen in der DTA-Einrichtung definieren. Weitere Informationen finden Sie in der Tabelle "DTA Einrichtung".  

Elektronische Zahlungen mittels DTA bieten folgende Möglichkeiten:  

- Generieren von Kreditorenzahlungen durch Verarbeitung der automatischen DTA-Zahlung. Weitere Informationen finden Sie unter [Gewusst wie: Vorschlagen einer DTA-Zahlung für Kreditoren](how-to-suggest-dta-payment-for-vendors.md).  

- Überprüfen der Liste von Kreditoren und Zahlungsinformationen. Weitere Informationen finden Sie unter [Gewusst wie: Überprüfen einer Liste von Kreditoren für DTA-Zahlungen](how-to-verify-a-list-of-vendors-for-dta-payments.md).  

- Elektronische Übermittlung der DTA-Datei an die Bank, wo Kreditorenzahlungen in wenigen Stunden freigegeben werden. Weitere Informationen finden Sie unter [Gewusst wie: Senden von DTA-Zahlungen](how-to-submit-dta-payments.md). Anschliessend kann das Zahlungsjournal gebucht werden.  

Sie können im Zahlungsausgangs-Erfassungsjournal DTA-Zahlungen auf Grundlage gebuchter Rechnungen vorschlagen lassen. Die vorgeschlagenen Zahlungen enthalten Informationen zum Kreditor und zur externen Belegnummer und können geändert werden. Weitere Informationen finden Sie unter [Gewusst wie: Vorschlagen einer DTA-Zahlung für Kreditoren](how-to-suggest-dta-payment-for-vendors.md) und im Fenster "DTA Zahlungsjournal".  

Wenn Sie einen Kreditor mittels DTA bezahlen möchten, generieren Sie eine DTA-Datei, die Daten aus der Zahlungsjournalzeile und der Finanzbuchhaltungs-Erfassungsjournalzeile enthält. Optional können in der DTA-Datei mehrere Zahlungen an den Kreditor zusammengefasst werden. Die DTA-Datei enthält auch den Buchungstext.  

> [!NOTE]  
>  Wenn Sie Zahlungen an den Kreditor zusammenfassen, muss der Buchungstext die Belegnummern der Rechnungen enthalten. Ist die Belegnummer länger als 50 Zeichen, wird dem Feld der Zusatz "usw." hinzugefügt.  

## <a name="see-also"></a>Siehe auch  
 [Elektronische Zahlungen (Schweiz)](swiss-electronic-payments.md)   
 [Gewusst wie: Vorschlagen einer DTA-Zahlung für Kreditoren](how-to-suggest-dta-payment-for-vendors.md)   
 [Gewusst wie: Überprüfen einer Liste von Kreditoren für DTA-Zahlungen](how-to-verify-a-list-of-vendors-for-dta-payments.md)   
 [Gewusst wie: Senden von DTA-Zahlungen](how-to-submit-dta-payments.md)   
 [Gewusst wie: Exportieren von Zahlungen mit EZAG](how-to-export-payments-using-ezag.md)   
 [Elektronische Zahlungen mit ESR (Schweiz)](swiss-electronic-payments-using-esr.md)   
 [Elektronische Zahlungen mit LSV+ (Schweiz)](swiss-electronic-payments-using-lsv-.md)  
 [Zahlungen vornehmen](../../payables-make-payments.md) 

