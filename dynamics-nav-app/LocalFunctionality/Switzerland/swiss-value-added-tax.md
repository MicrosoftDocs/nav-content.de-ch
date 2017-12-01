---
title: Mehrwertsteuer (Schweiz)
description: Schweizer Erweiterungen enthalten spezielle Mehrwertsteuerberichterstellungsfunktionen.
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
ms.openlocfilehash: 2060d66d895c907186ac3dbcf22ada1925b73f17
ms.contentlocale: de-ch
ms.lasthandoff: 10/26/2017

---
# <a name="swiss-value-added-tax"></a>Mehrwertsteuer (Schweiz)
[!INCLUDE[navnow](../../includes/navnow_md.md)] enthält die folgenden Erweiterungen für die Schweizer Mehrwertsteuerberichterstellung:  

- Automatische Regulierung von MWST-Beträgen für Rechnungen entsprechend dem Rabatt  
- Zusätzliche MWST-Wechselkurse für Rechnungen in Fremdwährungen  
- Einbeziehung von MWST-Prozentsätzen und -Beträgen in Erfassungsjournalen  

Weitere Informationen über die Schweizer Mehrwertsteuerberichterstellung und die Codierungsanforderungen finden Sie unter [Schweizer MwSt Informationen](http://www.estv.admin.ch/mwst/dokumentation/00130/00947/00948/index.html?lang=fr), im Besonderen Beleg 605.525.01. Die Information ist für Französisch, Deutsch und Italienisch verfügbar.  

## <a name="vat-amounts-and-vat-exchange-rates"></a>MWST-Beträge und MWST-Wechselkurse  
Entsprechend den lokalen Mehrwertsteuer-Gesetzen kann der MWST Basisbetrag um den Skontobetrag reduziert werden, wenn Skonto gewährt wird. Um automatische Mehrwertsteueranpassungen für einen Zahlungsrabatt einer Rechnung zuzulassen wir das Feld **Skonto berichtigen** standardmäßig im Fenster **Fibuposten Einrichtung** ausgeführt. Sie können diese Funktion in der MWST-Buchungsmatrix-Einrichtung " aktivieren. Weitere Informationen finden Sie in der Tabelle "Fibuposten einrichten" und "MWST-Buchungsmatrix einrichten".  

### <a name="currency-exchange-rates-for-vat-reporting"></a>Währungswechselkurse für die MWST-Abrechnung  
Für Rechnungen in Fremdwährungen muss der offizielle Wechselkurs der Regierung für die MWST-Berechnung verwendet werden. Sie können zusätzliche MWST-Wechselkurse einrichten, die für andere Rechnungsbelange als die MWST-Berechnung verwendet werden können. Der korrekte offizielle MWST-Wechselkurs kann für jede relevante Fremdwährung in der Wechselkurseinrichtung für Rechnungen angegeben werden. Weitere Informationen finden Sie in der Tabelle "Wechselkurse".  

Es ist auch möglich, alle aus Fremdwährungstransaktionen resultierenden MWST-Beträge in MWST-Posten zu regulieren. Wenn Sie die Funktion für die MWST-Wechselkursregulierung aktivieren, werden die MWST-Wechselkurse automatisch reguliert. Die durch Wechselkurse verursachten positiven Differenzen werden auf Kursgewinnkonten gebucht. Die durch Wechselkurse verursachten negativen Differenzen werden auf Kursverlustkonten gebucht. Weitere Informationen finden Sie unter Stapelverarbeitungsauftrag "Wechselkurse regulieren".  

In die MWST-Posten werden weitere Angaben übertragen, z. B. der MWST-Satz und der ursprüngliche Währungsbetrag. Weitere Informationen finden Sie in der MWST-Postentabelle.  

## <a name="vat-information-in-journals"></a>MWST-Informationen in Erfassungsjournalen  
Wenn Sie in einem Erfassungsjournal eine neue Zeile hinzufügen, werden die MWST-Prozentsätze und MWST-Beträge für das Konto und Gegenkonto der ausgewählten Erfassungsjournalzeile im Statusbereich des Erfassungsjournals ausgefüllt. Weitere Informationen finden Sie unter Fibu Erf.-Journal, Warenausgangsbuchfenster und Einkaufs-Erf.-Journal.  

## <a name="see-also"></a>Siehe auch  
 [MWST-Sätze für die Schweiz](vat-rates-for-switzerland.md)   
 [Gewusst wie: Erstellen und Drucken einer Schweizer MWST-Abrechnung](how-to-create-and-print-a-swiss-vat-statement.md)   
 [Lokale Funktion (Schweiz)](switzerland-local-functionality.md)   

