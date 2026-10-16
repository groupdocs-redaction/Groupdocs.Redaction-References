---
title: "com.groupdocs.redaction.integration"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Das Paket stellt Schnittstellen und Klassen bereit, die verwendet werden, um Dokumente verschiedener Formate mit GroupDocs.Redactions zu integrieren."
type: docs
weight: 13
url: /de/java/com.groupdocs.redaction.integration/
---

Das Paket stellt Schnittstellen und Klassen bereit, die zur Integration von Dokumenten verschiedener Formate mit GroupDocs.Redactions verwendet werden.



## Klassen

| Klasse | Beschreibung |
| --- | --- |
| [DocumentFormatInstance](../com.groupdocs.redaction.integration/documentformatinstance) | Stellt ein spezifisches Format eines Dokuments dar. |
| [MetadataCollection](../com.groupdocs.redaction.integration/metadatacollection) | Stellt ein Wörterbuch von MetadataItem mit dessen Titel als Schlüssel dar. |
| [MetadataItem](../com.groupdocs.redaction.integration/metadataitem) | Stellt ein Metadaten-Element dar, das für alle unterstützten Formate gemeinsam ist und bei Metadaten-Redaktionen verwendet wird. |
| [RecognizedImage](../com.groupdocs.redaction.integration/recognizedimage) | Stellt Text dar, der aus einem Bild als Ergebnis seines Erkennungsprozesses extrahiert wurde. |
| [RedactableImage](../com.groupdocs.redaction.integration/redactableimage) | Bietet eine Fassade für alle Rasterbild-Redaktionsvorgänge. |
| [TextFragment](../com.groupdocs.redaction.integration/textfragment) | Stellt einen Teil des erkannten Textes (Wort, Symbol usw.) dar, der von der OCR-Engine extrahiert wurde. |
| [TextLine](../com.groupdocs.redaction.integration/textline) | Stellt eine Textzeile dar, die von der OCR-Engine aus einem Bild extrahiert wurde. |

## Schnittstellen

| Schnittstelle | Beschreibung |
| --- | --- |
| [IAnnotatedDocument](../com.groupdocs.redaction.integration/iannotateddocument) | Definiert Methoden, die für den Zugriff auf Anmerkungen, wie Kommentare, erforderlich sind. |
| [ICellularFormatInstance](../com.groupdocs.redaction.integration/icellularformatinstance) | Definiert Methoden, die für den Zugriff auf Tabellenkalkulationsformate mit einem oder mehreren Arbeitsblättern erforderlich sind. |
| [IFixedFormatDocument](../com.groupdocs.redaction.integration/ifixedformatdocument) | Definiert Methoden, die für den Zugriff auf Formate fester Struktur, wie PDF oder Präsentationen, erforderlich sind. |
| [IImageFormatInstance](../com.groupdocs.redaction.integration/iimageformatinstance) | Definiert Methoden, die für Rasterbildformat-Redaktionen erforderlich sind. |
| [IMetadataAccess](../com.groupdocs.redaction.integration/imetadataaccess) | Definiert Methoden, die für den Zugriff auf Metadaten eines Dokuments erforderlich sind, sofern das Format dies unterstützt. |
| [IMultipleAreaRedactable](../com.groupdocs.redaction.integration/imultiplearearedactable) | Definiert Methoden, die erforderlich sind, um mehrere Bildbereiche gleichzeitig mit derselben Farbe zu redigieren. |
| [IOcrConnector](../com.groupdocs.redaction.integration/iocrconnector) | Definiert Methoden, die erforderlich sind, um textuelle Redaktionen auf Bilddokumente und eingebettete Bilder anzuwenden. |
| [IPaginatedDocument](../com.groupdocs.redaction.integration/ipaginateddocument) | Definiert Methoden, die erforderlich sind, um die Seiten eines Dokuments zu manipulieren. |
| [IPreviewable](../com.groupdocs.redaction.integration/ipreviewable) | Definiert Methoden, um eine Vorschau des Dokuments zu erstellen. |
| [IRasterizableDocument](../com.groupdocs.redaction.integration/irasterizabledocument) | Definiert Methoden, die für das Speichern eines Dokuments in beliebiger Binärform erforderlich sind. |
| [ITextualFormatInstance](../com.groupdocs.redaction.integration/itextualformatinstance) | Definiert Methoden, die für das Redigieren von Textdaten in jedem Dokument, das Text enthält, erforderlich sind. |
