---
title: Lagerverwaltung (Schweiz)
description: Schweizer Erweiterungen enthalten spezielle Lagerverwaltungsfunktionen.
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
ms.openlocfilehash: 98e1c1dd52127710cedf3c849eee0fffc876e02b
ms.contentlocale: de-ch
ms.lasthandoff: 10/26/2017

---
# <a name="swiss-inventory-management"></a>Lagerverwaltung (Schweiz)
[!INCLUDE[navnow](../../includes/navnow_md.md)] enthält Schweizer Erweiterungen für Lagerverwaltung. Dies beinhaltet Folgendes:  

- Detaillierte Berichte.  Weitere Informationen finden Sie unter Verkaufstatistikbericht und Lagerlistenbericht.  
- Die Fähigkeit, eine Rechnung mit mehreren Lieferungen nachzuverfolgen.  
- Einschliessen eines Artikelkarten-Lagerortcodes als Standardlagerortcode für Verkaufszeilen und Artikelerfassungsjournale. Weitere Informationen finden Sie unter [Gewusst wie: Einrichten von Lagerplätzen](../../inventory-how-setup-locations.md). 

## <a name="managing-item-details"></a>Verwalten von Artikeldetails  
Unternehmen haben u. U. verschiedene Lager für verschiedene Produktkategorien. In diesem Fall muss der von der Artikelkarte abgerufene Standardlagerortcode verwendet werden. Wenn Sie einen Lagerortcode für einen Artikel definieren, wird dieser auf die Verkaufszeilen und Artikelerfassungsjournale als Standardlagerortcode übertragen. Weitere Informationen finden Sie unter Verkaufszeile und Artikel Erf.-Journalzeile.  

Sie können eine Artikelbeschreibung mit bis zu 50 Zeichen und eine Zollposition mit bis zu 15 Zeichen angeben. Weitere Informationen finden Sie im Fenster Artikelkarte.  

Zusätzliche Informationen, wie Debitorennummer, Lieferadresscode und Debitorenvertriebsmitarbeitercode wird in Lagerposten gespeichert. Diese Informationen sollen dabei helfen, benutzerdefinierte Berichterstellungskriterien wie Einnahmen pro Debitor zu erstellen und Artikel oder Debitoren für Verkäufer bereitzustellen. Weitere Informationen erhalten Sie in der Tabelle "Lagerposten".  

## <a name="invoices-with-multiple-shipments"></a>Rechnungen mit mehreren Lieferungen  
Sind mehrere Lieferungen für einen Kunden gebucht worden, können Sie Sammelrechnungen mit der Funktion **Lieferzeilen abrufen** erstellen. Weitere Informationen finden Sie im Fenster Versandzeilen abrufen. Wenn Sie diese Funktion verwenden, enthält der Text, der in den Rechnungszeilen erstellt wird, die Informationen über die Nummer der Auslieferung und das Lieferdatum. Beispielsweise kann der Text als Lieferungsnummer erscheinen. 102040 von 25.01.01. Auf diese Weise können Sie Rechnungen mit mehreren Lieferungen verfolgen.  

## <a name="see-also"></a>Siehe auch  
 [Gewusst wie: Sperren der Lieferung bei negativem Lagerbestand](how-to-block-shipment-for-negative-inventory.md)   
 [Gewusst wie: Sperren von Lagerartikeln für Verkäufe oder Einkäufe](how-to-block-inventory-items-for-sales-or-purchases.md)   
 [Gewusst wie: Kopieren vorhandener Artikel in neue Artikel](how-to-copy-existing-items-to-new-items.md)   
 [Gewusst wie: Deaktivieren des Artikelpreistracking](how-to-deactivate-item-cost-tracking.md)   
 [Lokale Funktion (Schweiz)](switzerland-local-functionality.md)   
 [So wird's gemacht: Standorte einrichten](../../inventory-how-setup-locations.md)

