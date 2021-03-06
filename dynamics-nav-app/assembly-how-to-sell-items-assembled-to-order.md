---
title: Vorgehensweise beim Verkaufen von Auftragsmontageartikeln
description: "Wenn der Montageartikels für die Auftragsmontage eingerichtet ist, dann nimmt der Standard-Verkaufsauftragsprozess an, dass der Artikel nicht auf Lager ist und für den jeweiligen Verkaufsauftrag speziell montiert werden muss. Wenn Sie den Artikel auf einer Verkaufsauftragszeile eingeben, wird ein Montageauftrag automatisch erstellt und mit dem Verkaufsauftrag verknüpft."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: fc140a0fa7d58c38234f67471323241ac94ca489
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-sell-items-assembled-to-order"></a>Vorgehensweise: Verkaufen von Auftragsmontageartikeln
Wenn das Feld **Montagerichtlinie** auf der Artikelkarte eines Montageartikels  **Auftragsmontage** anzeigt, wird nicht erwartet, dass der Artikel im Lagerbestand vorhanden ist, und er muss speziell für einen Verkaufsauftrag montiert werden. Wenn Sie den Artikel auf einer Verkaufsauftragszeile eingeben, wird ein Montageauftrag automatisch erstellt und mit dem Verkaufsauftrag verknüpft.  

> [!NOTE]  
>  Wenn einige Auftragsmontageartikel bereits im Lager vorhanden sind, dann können Sie die Menge von dem Montageauftrag abziehen und sie aus dem Lager reservieren. Weitere Informationen finden Sie unter [Vorgehensweise: Verkaufen von Lagerartikeln in Programmfertigungs-Flüssen](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md)  

Bei diesem Verfahren verarbeiten Sie den verkauf eines Artikels, der gemäss den Spezifikationen montiert wird, die vom Debitor gewünscht werden. Die Schritte enthalten das Initiieren der Verkaufsauftragszeile, das Anpassen der Montageartikels durch Bearbeitung seiner Komponenten und Ressourcen, die Prüfung der Verfügbarkeit, um ein Lieferdatum festzulegen und die Freigabe des Verkaufsauftrag für die Montage und den sofortigen Versand.  

> [!NOTE]  
>  Die folgende Vorgehensweise enthält nicht die Standard-Verkaufsauftragsschritte vor dem Schritt, in dem Sie den Auftragsmontageartikel in eine Verkaufsauftragszeile eingeben.  

## <a name="to-sell-an-item-that-is-assembled-to-order"></a>So verkaufen Sie einen Auftragsmontageartikel:  
1.  Alternativ wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Verkaufsauftrag** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Erstellen Sie einen Auftrag. Weitere Informationen finden Sie unter [So geht's: Produkte verkaufen](sales-how-sell-products.md)  
3.  Geben Sie im Feld **Nr.** Geben Sie im Feld Nr. einen Artikel ein, der als Auftragsmontageartikel eingerichtet ist.  
4.  Geben Sie im Feld **Lagerortcode** den Lagerort an, von dem aus der Artikel verkauft werden wird. Der Montageprozess wird an diesem Lagerort durchgeführt.  
5.  Geben Sie im Feld **Menge** ein, wie viele Einheiten zu verkaufen sind.  

    > [!NOTE]  
    >  Wenn eine oder mehrere Komponenten der angefragten Montageartikelmenge nicht verfügbar sind, dann wird ein detailliertes Verfügbarkeitswarnungsfenster geöffnet. Weitere Informationen finden Sie unter Montageverfügbarkeit.  

    Ein Montageauftrag wird automatisch erstellt und mit der Verkaufsauftragszeile verknüpft. Das Fälligkeitsdatum dieses Montageauftrags wird mit dem Lieferdatum der Verkaufsauftragszeile synchronisiert.  

    Die zu verkaufende Menge wird in das Feld **Menge für Auftragsmontage** kopiert, das angibt, dass die Artikeleinrichtung erwartet, dass die gesamte Menge auf der Verkaufsauftragszeile gemäss dem Auftrag montiert wird. Sie können die Menge für die Auftragsmontage vermindern, etwa wenn Sie wissen, dass mehrere Artikel bereits verfügbar sind. Weitere Informationen finden Sie unter [Vorgehensweise: Verkaufen von Auftragsmontageartikeln](assembly-how-to-sell-inventory-items-in-assemble-to-order-flows.md).  

6.  Um zu berücksichtigen, dass der Debitor einen weiteren Artikel in einem Kit wünscht, wählen Sie auf dem Inforegister **Zeilen** die Aktion **Zeile**, wählen die Aktion **Auftragsmontage** und dann die Aktion **Auftragsmontagezeilen**, um die Standardmontagekomponenten anzuzeigen und zu ändern. Alternativ wählen Sie das Feld **Menge für Auftragsmontage** aus.  
7.  Erstellen Sie im Fenster **Auftragsmontagezeilen** eine neue Zeile der Art **Artikel** für den angeforderten zusätzlichen Kit-Inhalt. Die Zeile stellt eine zusätzliche Montagekomponente dar.  

    Sie können den Auftrag auch anpassen, indem Sie die Menge eines Standardartikels im Kit erhöhen. Sie können dies tun, indem Sie den Wert im Feld **Komponentenmenge** auf der jeweiligen Montageauftragszeile erhöhen.  

    > [!NOTE]  
    >  Das Fenster **Auftragsmontagezeilen** enthält nur die grundlegenden Felder, die ein Verkäufer für die Anpassung der Komponentenliste, die Hinzufügung von Artikeltrackingnummern oder zur Lösung von Artikelverfügbarkeitsproblemen benötigt. Wählen Sie zur Anzeige weiterer Auftragsmontageinformationen, wie etwa das Anfangsdatums der Auftragsmontage, auf der Registerkarte **Start**, in der Gruppe **Prozess**, die Option **Belege anzeigen**. Dadurch wird eine vollständige Ansicht des Montageauftrags angezeigt, der mit der Verkaufsauftragszeile verknüpft ist. Sie können die Inhalte der meisten Felder des Auftragsmontagekopfes nicht ändern, und Sie können daraus auch keine Montageausgaben buchen, da Sie dazu die Lieferungsbuchung der Verkaufsauftragszeile verwenden müssen.  
    >   
    >  Im Kopfbereich von verknüpften Montageaufträgen kann nur das Feld **Startdatum** geändert werden, um Montagearbeitern bei Beginn des Prozesses zu ermöglichen, ein Datum anzugeben, das vor dem Fälligkeitsdatum liegt. Alle Felder auf den Zeilen des verknüpften Montageauftrags können geändert werden, so dass die Lagermitarbeiter während des Prozesses Verbrauchsdaten eingeben können.  

8.  Prüfen Sie Komponentenverfügbarkeitsprobleme und reagieren Sie darauf. Wählen Sie beispielsweise einen verfügbaren Ersatzartikel, oder richten Sie ein späteres Fälligkeitsdatum ein.  
9. Schliessen Sie das Fenster **Auftragsmontagezeilen**. Der verknüpfte Montageauftrag ist jetzt bereit damit zu beginnen, die angepassten Komponenten nach Fälligkeitsdatum zu montieren.  
10. Wählen Sie im Verkaufsauftrag die Aktion **Freigeben**, um die Montageabteilung zu benachrichtigen, dass der Montagevorgang begonnen werden kann.  
11. Führen Sie in der Montageabteilung die Schritte zur Montage der Artikel aus, die in diesem Prozess verkauft werden. Weitere Informationen finden Sie unter [Artikel zusammenführen](assembly-how-to-assemble-items.md).  

## <a name="see-also"></a>Siehe auch  
[Montageverwaltung](assembly-assemble-items.md)  
[Vorgehensweise: Arbeiten mit Stücklisten](inventory-how-work-BOMs.md)  
[Lagerbest.](inventory-manage-inventory.md)  
[Designdetails: Logistik](design-details-warehouse-management.md)  
[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

