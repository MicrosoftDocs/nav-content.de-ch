---
title: "Vorgehensweise: Hinzufügen von Feldern zu einem Word-Berichtlayout"
description: "In diesem Thema wird das Verfahren zum Hinzufügen von Feldern aus einem Berichtsdatasets in ein bestehendes Word-Berichtslayout für einen Bericht beschrieben."
documentationcenter: 
author: jswymer
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 1085c5390cf6f20cc2bd5c2a95057e6499dbac8c
ms.contentlocale: de-ch
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-add-fields-to-a-word-report-layout"></a>Vorgehensweise: Hinzufügen von Feldern zu einem Word-Berichtlayout
Ein Berichtsdataset kann aus Feldern bestehen, die Bezeichnungen, Daten und Bilder anzeigen. In diesem Thema wird das Verfahren zum Hinzufügen von Feldern aus einem Berichtsdatasets in ein bestehendes Word-Berichtslayout für einen Bericht beschrieben. Fügen Sie Felder hinzu, indem Sie benutzerdefinierte XML-Abschnitt in Words für den Bericht verwenden und Inhaltssteuerelemente hinzufügen, die den Feldern des Berichtsdatasets zugeordnet sind. Beim Hinzufügen von Feldern ist es erforderlich, dass Sie einiges Wissen über das Dataset des Berichts haben, damit Sie die Felder identifizieren können, die Sie dem Layout hinzufügen möchten.  
  
> [!NOTE]  
>  Sie können keine integrierten Berichtslayouts in<!--Onprem. Built-in layouts can only be modified by using the development environment--> ändern.  

##  <a name="OpenXMLPart"></a>Um den benutzerdefinierten XML-Abschnitt für den Bericht in Word zu öffnen  
  
1.  Wenn nicht bereits offen, öffnen Sie den Word-Berichtlayoutbeleg in Word.  
  
     Weitere Informationen finden Sie unter [Vorgehensweise: Erstellen und bearbeiten  eines benutzerdefinierten Berichts- oder Dokumentenlayout](ui-how-create-custom-report-layout.md).  
  
2.  Zeigen Sie die Registerkarte **Entwickler** im Menüband von Microsoft Word an.  
  
     Standardmäßig wird die Registerkarte **Entwickler** nicht im Menüband angezeigt. Weitere Informationen finden Sie unter [Vorgehensweise: Anzeigen der Entwickler-Registerkarte auf dem Menüband](http://go.microsoft.com/fwlink/?LinkID=389631).  
  
3.  Wählen Sie auf der Registerkarte **Entwickler** die Option **XML-Zuordnungs-Bereich** aus.  
  
4.  Im Bereich **XML-Zuordnung** in der Dropdownliste **Benutzerdefinierter XML-Abschnitt** wählen Sie den benutzerdefinierten XML-Abschnitt für ADD INCLUDE<!--[!INCLUDE[navnow](../../includes/navnow_md.md)]-->-Bericht, normalerweise der letzte in der Liste. Der Name des benutzerdefinierten XML-Abschnitts hat folgendes Format:  
  
     urn:microsoft-dynamics-nav/reports/*report_name*/*ID*  
  
     *reportname*entspricht dem Namen, der dem Berichtsobjekt in <!--OnPrem as specified by the report's [Name Property-duplicate](../FullExperience/nav_dev_long_md.md)]--> zugeordnet ist.  
  
     *ID* ist die Kennnummer des Berichts.  
  
     Nachdem Sie den benutzerdefinierten XML-Abschnitt auswählen, zeigt der XML-Zuordnungsbereich die Beschriftungen und die Feldsteuerelemente an, die für den Bericht verfügbar sind.  
  
### <a name="to-add-a-label-or-data-field"></a>Um eine Beschriftung oder ein Datenfeld hinzufügen  
  
1.  Setzen Sie den Cursor in dem Beleg an der Stelle ab, an dem Sie das Steuerelement hinzufügen möchten.  
  
2.  Klicken Sie im **XML-Zuordnung**-Bereich auf das Steuerelement, das Sie hinzufügen möchten, und klicken Sie dann mit der rechten Maustaste auf **Inhaltssteuerelement einfügen** und dann auf **Reiner Text**.  
  
    > [!NOTE]  
    >  Sie können kein Feld hinzufügen, indem Sie manuell den Datasetfeldnamen in das Inhaltssteuerelement eingeben. Sie müssen den **XML-Zuordnung**-Bereich verwenden, um die Felder zuzuordnen.  
  
### <a name="to-add-repeating-rows-of-data-fields-to-create-a-list"></a>Um wiederholente Zeilen aus Datenfeldern hinzufügen, um eine Liste zu erstellen  
  
1.  Fügen Sie in einer Tabelle eine Tabellenzeile hinzu, die eine Spalte für jedes Feld umfasst, das wiederholt werden soll.  
  
     Diese Zeile fungiert als als Platzhalter für wiederkehrenden Felder.  
  
2.  Wählen Sie die gesamte Zeile aus.  
  
3.  Klicken Sie im **XML-Zuordnung**-Bereich mit der rechten Maustaste auf das Steuerelement, das dem Berichtsdatenelement entspricht, das die Felder enthält, die wiederholt werden sollen, und wählen Sie dann **Inhaltssteuerelement einfügen** und **Wiederholt**.  
  
4.  Fügen Sie die wiederkehrenden Felder der Zeile hinzu, wie folgt:  
  
    1.  Setzen Sie den Mauszeiger in einer Spalte ab.  
  
    2.  Klicken Sie im **XML-Zuordnung**-Bereich auf das Steuerelement, das Sie hinzufügen möchten, und klicken Sie dann mit der rechten Maustaste auf **Inhaltssteuerelement einfügen** und dann auf **Reiner Text**.  
  
    3.  Wiederholen Sie die Schritte a und b für jedes Feld.  
  
## <a name="adding-image-fields"></a>Hinzufügen von Bild-Feldern  
 Ein Berichtsdataset kann einen Feld enthalten, das ein Bild enthält, beispielsweise ein Firmenlogo oder ein Bild eines Artikels. Um ein Bild aus dem Berichtsdataset hinzuzufügen, fügen Sie ein **Bild**-Inhaltssteuerelement ein.  
  
 Bilder werden im linken oberen Teil des Inhaltssteuerelements ausgerichtet und ändern automatisch Ihre Größe proportional entsprechend den Grenze des Inhaltssteuerelements.  
  
> [!IMPORTANT]  
>  Außerdem können Sie Bilder nur hinzufügen, die in einem Format vorliegen, das von Word unterstützt wird, wie .bmp, .jpeg und PNG-Datei-Typen. Wenn Sie ein Bild hinzufügen, das ein Format hat, das nicht von Word unterstützt wird, erhalten Sie einen Fehler, wenn Sie den Bericht im ADD INCLUDE<!--[!INCLUDE[navnow](../../includes/navnow_md.md)]-->-Client ausführen.  
  
#### <a name="to-add-an-image"></a>Um ein Bild hinzuzufügen  
  
1.  Setzen Sie den Zeiger in dem Beleg an der Stelle ab, an dem Sie das Steuerelement hinzufügen möchten.  
  
2.  Klicken Sie im **XML-Zuordnung**-Bereich auf das Steuerelement, das Sie hinzufügen möchten, und klicken Sie dann mit der rechten Maustaste auf **Inhaltssteuerelement einfügen** und dann auf **Bild**.  
  
3.  Um die Bildgröße zu erhöhen oder zu verringern, ziehen Sie einen der Ziehpunkte zur Mitte des Inhaltssteuerelements hin oder von der Mitte weg.  

## <a name="custom-xml-part-overview"></a>Benutzerdefinierter XML-Teil, Übersicht
Word-Berichtlayouts werden anhand von *benutzerdefinierten XML-Abschnitten* erstellt. Ein kundenspezifischer XML-Abschnitt für einen  Bericht besteht aus Elementen, die den Datenelementen, den Spalten und den Beschriftungen entsprechen, die das Dataset des Berichts enthalten, wie im Berichts-DataSet-Designer in  definiert. <!--OnPrem The data as defined in the Report Dataset Designer in Microsoft Dynamics NAV Development Environment. -->Der benutzerdefinierte XML-Abschnitt wird verwendet, um die Daten in einem Bericht zuzuordnen, wenn der Bericht ausgeführt wird.

  
### <a name="xml-structure-of-custom-xml-part"></a>XML-Struktur des benutzerdefinierten XML-Abschnitts  
Die folgende Tabelle enthält eine vereinfachte Übersicht der XML eines benutzerdefinierten XML-Abschnitts.  
  
|XML-Elemente|Description|  
|------------------|-----------------|  
|`<?xml version="1.0" encoding="utf-16"?>`|Header|  
|`<WordReportXmlPart xmlns="urn:microsoft-dynamics-365/report/<reportname>/<id>/"`|XML-Namespacespezifikation. `<reportname>` ist der Namee, der dem Bericht zugewiesen ist. `<id>`ist die ID, die dem Bericht zugewiesen ist.|  
|`..<Labels>`<br /><br /> `....<ColumnNameCaption>ColumnNameCaption</ColumnNameCaption>`<br /><br /> `....<LabelName>LabelCaption</LabelName>`<br /><br /> `..</Labels>`|Enthält alle Beschriftungen für den Bericht.<!--OnPren The element includes labels that are related to columns that have the [IncludeCaption Property](../FullExperience/Name%20Property-duplicate.md).--><br />-   Beschriftungs-Elemente, die mit Spalten verknüpft sind, die das Format `<ColumnNameCaption>ColumnNameCaption</ColumnNameCaption>`<!--OnPrem where `ColumnName` is determined by the column's Name Property.--> haben.<br />- Bezeichnungselemente haben das Format`<LabelName>LabelName</LableName`<!--OnPrem where LabelName is determined by the label's Name Property.-->.<br />-    Beschriftungen sind in alphabetischer Reihenfolge aufgeführt.|  
|`..<DataItem1>`<br /><br /> `....<DataItem1Column1>DataItem1Column1</DataItem1Column1>`|Dateneinträge und Spalten auf oberster Ebene. Spalten werden in alphabetischer Reihenfolge aufgeführt.<!--OnPrem <br /><br /> The element names and values are determined by the [Name Property-duplicate](../FullExperience/Name%20Property-duplicate.md) of the data item or column.-->|  
|`....<DataItem2>`<br /><br /> `......<DataItem2Column1>DataItem2Column1</DataItem2Column1>`<br /><br /> `....</DataItem2>`<br /><br /> `....<DataItem3>`<br /><br /> `......<DataItem3Column1>DataItem3Column1</DataItem3Column1>`<br /><br /> `....</DataItem3>`|Datenelemente und Spalten, die im Dateneintrag auf oberster Ebene verschachtelt sind. Spalten werden in alphabetischer Reihenfolge unter dem entsprechenden Dateneintrag aufgelistet.|  
|`..</DataItem1>`<br /><br /> `</WordReportXmlPart>`|Abschließendes Element.|  
  
### <a name="custom-xml-part-in-word"></a>Benutzerdefinierter XML-Abschnitt in Word  
 In Word öffnen Sie den benutzerdefinierten XML-Abschnitt im **XML-Zuordnung**-Bereich und verwenden anschließend diesen Bereich, um Elemente zu den Inhaltssteuerelementen im Word-Dokument zuzuordnen. Der Bereich **XML-Zuordnung**ist zugänglich von der Registerkarte **Entwickler** (weitere Informationen unter[ Vorgehensweise: Anzeigen der Entwickler-Registerkarte auf dem Menüband](http://go.microsoft.com/fwlink/?LinkID=389631)).  
  
 Die Elemente im **XML-Zuordnung**-Bereich erscheinen in einer Struktur ähnlich dem XML-Quellcode. Beschriftungsfelder werden unter einem allgemeinen element **Beschriftungen** gruppiert, und Dateneintrag und Spalten sind in einer hierarchischen Struktur angeordnet, die der XML-Quelle entspricht, wobei die Spalten in alphabetischer Reihenfolge aufgeführt werden. Elemente werden durch ihren Namen, wie durch die Eigenschaft "Name" im Berichts-DataSet-Designer in ADD INCLUDE<!--[!INCLUDE[nav_dev_short](../../includes/nav_dev_short_md.md)]--> definiert, identifiziert.  
  
 In der folgenden Abbildung wird der einfache benutzerdefinierte XML-Abschnitt aus dem vorherigen Abschnitt im **XML-Zuordnung**-Bereich eines Word-Dokuments dargestellt.  
  
 ![Clip des XML-Zuordnungsbereichs in Word](media/nav_reportlayout_xmlmappingpane.png "NAV_ReportLayout_XMLMappingPane")  
  
-   Um dem Layout eine Beschriftung oder ein Feld hinzuzufügen, fügen Sie ein Inhaltssteuerelement ein, das dem Element im **XML-Zuordnung**-Bereich zugeordnet ist.  
  
-   Um wiederholen Zeilen aus Spalten zu erstellen, fügen Sie ein **Wiederholen**-Inhaltssteuerelement für das übergeordnete Datenelement ein, und fügen Sie dann ein Inhaltssteuerelement für die Spalten hinzu.  
  
-   Bei Beschriftungen ist der tatsächliche Text, der im generierten Angabe erscheint, der Wert der **Caption**-Eigenschaft für das Feld in der Datenelementtabelle (wenn die Beschriftung mit der Spalte im Berichtsdataset verknüpft ist), oder entspricht einer Beschriftung im Berichts-Bezeichnungs-Designer (wenn die Beschriftung nicht mit einer Spalte im Dataset verknüpft ist).  
  
-   Die Sprache der Beschriftung, die angezeigt wird, wenn Sie den Bericht ausführen, hängt von der Spracheneinstellung des Berichtsobjekts ab. <!--OnPrem For more information, see [Multiple Document Languages](../FullExperience/Viewing%20the%20Application%20in%20Different%20Languages.md).-->  
  
## <a name="see-also"></a>Siehe auch  
 [Vorgehensweise: Erstellen und bearbeiten Sie einen benutzerdefinierten Bericht](ui-how-create-custom-report-layout.md)   
