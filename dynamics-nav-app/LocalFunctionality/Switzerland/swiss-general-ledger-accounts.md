---
title: Finanzbuchhaltungskonten (Schweiz)
description: Schweizer Erweiterungen enthalten spezielle Fibupostenfunktionen.
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
ms.openlocfilehash: 574a9f233798f0e5bc3945af3391039f2e900112
ms.contentlocale: de-ch
ms.lasthandoff: 10/26/2017

---
# <a name="swiss-general-ledger-accounts"></a>Finanzbuchhaltungskonten (Schweiz)
[!INCLUDE[navnow](../../includes/navnow_md.md)] enthält Schweizer Erweiterungen für Fibuposten.

- Verwalten der Fremdwährungssalden eines Bankkontos in der Finanzbuchhaltung  
- Sortieren von Finanzbuchhaltungs-Kontonummern im Fenster **Kontenplan**  
- Korrigieren falscher positiver oder negativer Vorzeichen für manuell in Erfassungsjournalen eingegebene Beträge  
- Anzeigen einer Vorschau, mit deren Hilfe die Auswirkungen von Finanzbuchhaltungs-Erfassungsjournalbuchungen auf die Salden bestimmter Finanzbuchhaltungskonten vor der eigentlichen Buchung überprüft werden können  

## <a name="general-ledger-accounts-and-general-journals"></a>Finanzbuchhaltungskonten und Finanzbuchhaltungs-Erfassungsjournale  
Unternehmen arbeiten häufig mit unterschiedlichen Bankkonten für Fremdwährungen und verwenden für jedes Bankkonto ein Finanzbuchhaltungskonto. In [!INCLUDE[navnow](../../includes/navnow_md.md)], können Sie Fremdwährungssaldoinformationen und Währungscodes und im Fenster **Kontenplan** einrichten. Auf diese Weise kann der ursprüngliche Fremdwährungssaldo eines Bankkontos verwaltet werden. Weitere Informationen finden Sie unter [Kontenplan (Fenster)](assetId:///fa407624-b670-44b6-8397-91aa606e4c39) und [Fibukonto (Tabelle)](assetId:///a65c2b09-9bb2-43db-8c53-c047bfc49777).  

Angenommen, ein Unternehmen verfügt über zwei Bankkonten: eines für Landes- bzw. Mandantenwährung (MW) und eines für Euro (EUR). Sie müssen ein Finanzbuchhaltungskonto für jedes Bankkonto erstellen. Für das EUR-Konto definieren Sie den Währungscode **EUR** und buchen Erfassungsjournale in EUR oder MW.  

Wenn sich der Wechselkurs für EUR und MW ändert, können Sie den Landeswährungssaldo für das EUR-Finanzbuchhaltungskonto mit dem Stapelverarbeitungsauftrag "Wechselkurse regulieren" aktualisieren und anpassen. Bei dieser Stapelverarbeitung werden Währungsregulierungsposten in der Finanzbuchhaltung erstellt und gebucht, und der MW-Saldo wird aktualisiert.  

## <a name="data-type-for-general-ledger-accounts"></a>Datentyp für Finanzbuchhaltungskonten  
Der Datentyp ist in der Fibupostennummer auf Text oder Kontocode festgelegt, um die Sortierungsanforderungen für den standardisierten Kontenplan von kleinen und mittleren Unternehmen (KMU) zu unterstützen. Weitere Informationen finden Sie unter [Kontenplan (Fenster)](assetId:///fa407624-b670-44b6-8397-91aa606e4c39). Die Kontonummernliste ist basierend auf dem Datentyp "Text" sortiert. Der KMU-Kontenplan enthält die folgenden Kontonummern:  

- 1176  
- 119.0  
- 1190  

## <a name="correcting-positive-and-negative-signs-in-general-journals"></a>Korrigieren positiver und negativer Vorzeichen in Finanzbuchhaltungs-Erfassungsjournalen  
Wenn Sie manuell Beträge in das Erfassungsjournal eingeben, werden die positiven und negativen Vorzeichen für die Beträge automatisch überprüft. Falsche Vorzeichen werden abhängig von der Konto- und Belegart automatisch korrigiert, und eine Meldung wird angezeigt. Weitere Informationen finden Sie unter [Fibu Erf.-Journalzeile (Tabelle)](assetId:///5308c791-0964-41d9-bc54-fd87e815d1be).  

Die Beträge für Debitorenrechnungen, Kreditorengutschriften und -zahlungen müssen positiv sein. Die Beträge für Kreditorenrechnungen, Debitorengutschriften und -zahlungen müssen negativ sein.  

## <a name="viewing-temporary-balances-in-general-journals"></a>Anzeigen temporärer Salden in Finanzbuchhaltungs-Erfassungsjournalen  
Bevor Sie ein Finanzbuchhaltungs-Erfassungsjournal buchen, können Sie eine Vorschau anzeigen, die Aufschluss gibt über die Auswirkungen dieser Buchung auf die Salden bestimmter Finanzbuchhaltungskonten. Sie können ein Statistikfenster, das die Salden der Konten anzeigt und die Salden der aktiven Zeilen öffnen, die ungebuchte Werte für das aktuelle Erf.-Journal umfassten. Weitere Informationen finden Sie unter [Gewusst wie: Anzeigen temporärer Salden in Finanzbuchhaltungs-Erfassungsjournalen](how-to-view-temporary-balances-in-general-ledger-journals.md).  

## <a name="see-also"></a>Siehe auch  
 [Gewusst wie: Anzeigen temporärer Salden in Finanzbuchhaltungs-Erfassungsjournalen](how-to-view-temporary-balances-in-general-ledger-journals.md)   
 [Lokale Funktion (Schweiz)](switzerland-local-functionality.md)

