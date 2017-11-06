---
title: "Sperren von Lagerartikeln für Verkäufe oder Einkäufe"
description: "In [!INCLUDE[navnow](../../includes/navnow_md.md)] kann ein Artikel als für Verkäufe, Einkäufe oder alle Verwendungszwecke gesperrt gekennzeichnet werden."
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 7e2559aca6a8b73bcd11ea6251dee13b30f7267b
ms.contentlocale: de-ch
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-block-inventory-items-for-sales-or-purchases"></a>Gewusst wie: Sperren von Lagerartikeln für Verkäufe oder Einkäufe
In [!INCLUDE[navnow](../../includes/navnow_md.md)] kann ein Artikel als für Verkäufe, Einkäufe oder alle Verwendungszwecke gesperrt gekennzeichnet werden.  

In der folgenden Tabelle wird veranschaulicht, was beim Sperren von Artikeln passiert.  

|Artikel gekennzeichnet als|Ergebnis|  
|--------------------|------------|  
|**Verkauf gesperrt**|Der Artikel kann nicht in einem Verkaufsbeleg oder einem Erf.-Journal für Verkaufsartikel verwendet werden.|  
|**Einkauf gesperrt**|Der Artikel kann nicht in einem Einkaufsbeleg, einem Erf.-Journal für Einkaufsartikel oder in Einkaufsplanungsprozessen verwendet werden.|  
|**Gesperrt**|Der Artikel kann für keine Artikeltransaktion verwendet werden. Weitere Informationen zum Sperren eines Artikels für alle Zwecke erhalten Sie unter "Artikelkarte".|  

## <a name="to-block-inventory-items-for-sales"></a>So sperren Sie Lagerartikel für den Verkauf  

1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen] (../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen")aus und geben Sie **Artikel** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Wählen Sie den Artikel, den Sie sperren möchten, und wählen Sie dann die Aktion **Bearbeiten** aus.  
3.  Aktivieren Sie auf dem Inforegister **Fakturierung** das Kontrollkästchen **Verkauf gesperrt**, um den ausgewählten Artikel für Verkaufstransaktionen zu sperren.  
4.  Wählen Sie die Schaltfläche **OK** aus.  

## <a name="to-block-inventory-items-for-purchase"></a>So sperren Sie Lagerartikel für den Einkauf  

1.  Wählen Sie ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Symbol nach Seite oder Bericht suchen") aus und geben Sie **Artikel** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Wählen Sie den Artikel, den Sie sperren möchten, und wählen Sie dann die Aktion **Bearbeiten** aus.  
3.  Aktivieren Sie auf dem Inforegister **Beschaffung** das Kontrollkästchen **Einkauf gesperrt**, um den ausgewählten Artikel für Einkaufstransaktionen zu sperren.  
4.  Wählen Sie die Schaltfläche **OK** aus.  

Für folgende Aktionen erhalten Sie eine Fehlermeldung:  

- Eingeben von Verkaufs- und Einkaufszeilen in Verkaufs- bzw. Einkaufsbelege für gesperrte Artikel. Weitere Informationen erhalten Sie in den Tabellen "Verkaufszeile" und "Einkaufszeile".  
- Erstellen von Artikel-Erf.-Journalen für gesperrte Artikel. Weitere Informationen erhalten Sie im Fenster "Artikel Erf.-Journal".  
- Buchen von Artikeltransaktionen für gesperrte Artikel.  

## <a name="see-also"></a>Siehe auch  
 [Lagerverwaltung (Schweiz)](swiss-inventory-management.md)   
 [Gewusst wie: Sperren der Lieferung bei negativem Lagerbestand](how-to-block-shipment-for-negative-inventory.md)   
 [Gewusst wie: Kopieren vorhandener Artikel in neue Artikel](how-to-copy-existing-items-to-new-items.md)   
 [Gewusst wie: Deaktivieren des Artikelpreistracking](how-to-deactivate-item-cost-tracking.md)

