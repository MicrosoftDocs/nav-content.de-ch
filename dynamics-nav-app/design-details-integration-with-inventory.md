---
title: "Designdetails – Integration mit dem Lagerbestand"
description: Der Logistik-Anwendungsbereich und der Lager-Anwendungsbereich interagieren miteinander im physischen Bestand und in der Bestands- und Lageranpassung.
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ca9a1b5b1ea20fc125107f3fb5b7a74814a85837
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-integration-with-inventory"></a>Designdetails: Integration mit dem Lagerbestand
Der Logistik-Anwendungsbereich und der Lager-Anwendungsbereich interagieren miteinander im physischen Bestand und in der Bestands- und Lageranpassung.  
  
## <a name="physical-inventory"></a>Inventur  
 Das **Logistik-Inventur-Erf.-Journal**-Fenster wird mit dem **Inventur Erf.-Journal**-Fenster für alle erweiterten Lagerorte verwendet. Der Bestand auf Lagerplatzebene wird berechnet, und eine gedruckte Liste wird für den Lagermitarbeiter bereitgestellt. Die Liste zeigt, welche Artikel an welchen Lagerplätzen gezählt werden müssen.  
  
 Der Lagermitarbeiter gibt die gezählte Menge im **Logistik-Inventur-Erf.-Journal** Fenster ein und bucht das Erf.-Journal.  
  
 Wenn die gezählte Menge größer als die Menge auf der Erf.-Journalzeile ist, wird eine Umlagerung für diese Differenz aus dem Standard-Ausgleichslagerplatz zum gezählten Lagerplatz gebucht. Dieses erhöht die Menge im gezählten Lagerplatz und vermindert die Menge im Standard-Ausgleichslagerplatz.  
  
 Wenn die gezählte Menge geringer als die Menge auf der Erf.-Journalzeile ist, wird eine Umlagerung für diese Differenz aus dem gezählten Lagerplatz zum Standard-Ausgleichslagerplatz gebucht. Dieses reduziert die Menge im gezählten Lagerplatz und erhöht die Menge im Standard-Ausgleichslagerplatz.  
  
 In erweiterten Lagerfunktionskonfigurationen wird der Wert im Feld **Menge (berechnet)** aus den Lagerposten einbezogen und der Wert im Feld **Menge (Phys. Lagerbestand)** aus den Lagerplatzposten ohne Ausgleichslagerplatzinhalt abgerufen. Das Feld **Menge** gibt die Differenz zwischen den ersten beiden Feldern an, die dem Inhalt des Regulierungslagerplatzes entsprechen sollte.  
  
 Wenn Sie das Inventur Erf.-Journal buchen, werden der Lagerbestand und der Ausgleichslagerplatz aktualisiert.  
  
### <a name="warehouse-adjustments-to-the-item-ledger"></a>Lagerplatz-Ausgleich mit dem Artikelposten  
 Sie verwenden das Fenster **Artikel Erf.-Journal** und die Funktion **Ausgleich berechnen**, um den Lagerbestand im Lagerposten in Übereinstimmung mit einem Ausgleich anzupassen, der für die Artikelmenge in einem Lagerplatz vorgenommen wurde. Um eine Verbindung zwischen den Lagerbestand und der Logistik zu erstellen, müssen Sie einen Vorgabe-Ausgleichslagerplatz pro Lagerort festlegen.  
  
 Der Standard-Regulierungslagerplatz registriert Artikel im Lager, wenn Sie einen Zugang für den Bestand buchen. Wenn Sie jedoch einen Lagerabgang buchen, wird die Menge am Lagerplatz ebenfalls verringert. In beiden Fällen werden Lagerposten und Lagerposten erstellt.  
  
> [!NOTE]  
>  Der Ausgleichslagerplatz ist nicht in der Verfügbarkeitsberechnung enthalten.  
  
 Wenn Sie den Lagerplatzinhalt anpassen wollen, können Sie das Logistik Artikel-Erf.-Journal verwenden, von dem Sie die Artikelnummer, den Zonencode, den Lagerplatzcode und die Menge angeben können, die Sie anpassen möchten.  
  
 Wenn Sie eine positive Menge eingeben und die Zeile buchen, wird der Bestand an dem Lagerplatz erhöht, und die Menge des Standard-Ausgleichslagerplatzes wird entsprechend vermindert.  
  
## <a name="see-also"></a>Siehe auch  
 [Designdetails: Logistik](design-details-warehouse-management.md)   
 [Designdetails: Verfügbarkeit im Lager](design-details-availability-in-the-warehouse.md)
