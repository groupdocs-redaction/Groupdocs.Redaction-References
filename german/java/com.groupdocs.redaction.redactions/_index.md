---
title: "com.groupdocs.redaction.redactions"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Das Paket stellt Klassen für verschiedene Arten von Redaktionen bereit."
type: docs
weight: 16
url: /de/java/com.groupdocs.redaction.redactions/
---

Das Paket stellt Klassen für verschiedene Arten von Redaktionen bereit.



## Klassen

| Klasse | Beschreibung |
| --- | --- |
| [AnnotationRedaction](../com.groupdocs.redaction.redactions/annotationredaction) | Stellt eine Redaktion dar, die Anmerkungstexte (Kommentare usw.) ersetzt, die einem angegebenen regulären Ausdruck entsprechen. |
| [CellColumnRedaction](../com.groupdocs.redaction.redactions/cellcolumnredaction) | Stellt eine Textredaktion dar, die Text in Tabellenkalkulationsdokumenten (CSV, Excel usw.) ersetzt. |
| [CellFilter](../com.groupdocs.redaction.redactions/cellfilter) | Bietet eine Option, den Geltungsbereich einer CellColumnRedaction auf ein Arbeitsblatt und eine Spalte zu beschränken. |
| [CustomRedactionContext](../com.groupdocs.redaction.redactions/customredactioncontext) | Stellt Eingabedaten für [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) bereit. |
| [CustomRedactionResult](../com.groupdocs.redaction.redactions/customredactionresult) | Stellt ein Ergebnis dar, das von [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) zurückgegeben wird. |
| [DeleteAnnotationRedaction](../com.groupdocs.redaction.redactions/deleteannotationredaction) | Stellt eine Textredaktion dar, die Anmerkungen löscht, wenn der Text einem angegebenen regulären Ausdruck entspricht (optional werden alle Anmerkungen gelöscht). |
| [EraseMetadataRedaction](../com.groupdocs.redaction.redactions/erasemetadataredaction) | Stellt eine Metadaten‑Redaktion dar, die alle Metadaten oder Metadaten, die bestimmten MetadataFilters entsprechen, aus dem Dokument entfernt. |
| [ExactPhraseRedaction](../com.groupdocs.redaction.redactions/exactphraseredaction) | Stellt eine Textredaktion dar, die eine exakte Phrase im Dokumenttext ersetzt, standardmäßig ohne Berücksichtigung der Groß‑ und Kleinschreibung. |
| [ImageAreaRedaction](../com.groupdocs.redaction.redactions/imagearearedaction) | Stellt eine Redaktion dar, die ein farbiges Rechteck im angegebenen Bereich eines Bilddokuments platziert. |
| [MetadataFilters](../com.groupdocs.redaction.redactions/metadatafilters) | Stellt eine Liste der gebräuchlichsten Arten von Dokumenten‑Metadaten dar. |
| [MetadataRedaction](../com.groupdocs.redaction.redactions/metadataredaction) | Stellt eine abstrakte Basisklasse für Dokument-Metadaten-Redaktionen dar. |
| [MetadataSearchRedaction](../com.groupdocs.redaction.redactions/metadatasearchredaction) | Stellt eine Metadaten-Redaktion dar, die Metadaten mithilfe von regulären Ausdrücken sucht und redigiert, wobei Schlüssel und/oder Werte übereinstimmen. |
| [PageAreaFilter](../com.groupdocs.redaction.redactions/pageareafilter) | Stellt einen Redaktionsfilter dar, der einen Bereich innerhalb einer Seite eines Dokuments festlegt, in dem die Redaktion angewendet wird. |
| [PageAreaRedaction](../com.groupdocs.redaction.redactions/pagearearedaction) | Stellt eine komplexe textuelle Redaktion dar, die Text, Bilder und Anmerkungen in einem Bereich der Seite betrifft. |
| [PageRangeFilter](../com.groupdocs.redaction.redactions/pagerangefilter) | Stellt einen Redaktionsfilter dar, der einen Seitenbereich innerhalb eines Dokuments festlegt, in dem die Redaktion angewendet wird. |
| [RedactionDescription](../com.groupdocs.redaction.redactions/redactiondescription) | Stellt eine einzelne Änderungsaktionsinformation dar, die während des Redaktionsprozesses ausgeführt wird. |
| [RedactionFilter](../com.groupdocs.redaction.redactions/redactionfilter) | Stellt einen Redaktionsfilter dar, der den Geltungsbereich innerhalb eines Dokuments festlegt, in dem Redaktionen angewendet werden. |
| [RedactionType](../com.groupdocs.redaction.redactions/redactiontype) | Stellt einen Typ von Dokumentdaten dar, die von der Redaktion betroffen sind. |
| [RegexRedaction](../com.groupdocs.redaction.redactions/regexredaction) | Stellt eine Text-Redaktion dar, die Text im Dokument sucht und ersetzt, indem sie den bereitgestellten regulären Ausdruck abgleicht. |
| [RegionReplacementOptions](../com.groupdocs.redaction.redactions/regionreplacementoptions) | Stellt Farb- und Bereichsparameter für den Austausch von Bildregionen dar. |
| [RemovePageRedaction](../com.groupdocs.redaction.redactions/removepageredaction) | Stellt eine Redaktion dar, die eine Seite (Folie, Arbeitsblatt usw.) aus einem Dokument entfernt. |
| [ReplacementOptions](../com.groupdocs.redaction.redactions/replacementoptions) | Stellt Optionen für den Austausch von übereinstimmendem Text dar. |
| [TextRedaction](../com.groupdocs.redaction.redactions/textredaction) | Stellt eine abstrakte Basisklasse für Dokument-Text-Redaktionen dar. |
| [TextReplacement](../com.groupdocs.redaction.redactions/textreplacement) | Stellt Informationen zum textuellen Austausch dar. |

## Schnittstellen

| Schnittstelle | Beschreibung |
| --- | --- |
| [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) | Definiert einen benutzerdefinierten Redaktions-Callback. |
| [IRedactionCallback](../com.groupdocs.redaction.redactions/iredactioncallback) | Definiert Methoden, die erforderlich sind, um Informationen zu jeder Redaktionsänderung zu erhalten und diese optional zu verhindern. |

## Aufzählungen

| Aufzählung | Beschreibung |
| --- | --- |
| [PageSeekOrigin](../com.groupdocs.redaction.redactions/pageseekorigin) | Stellt die Felder bereit, die Referenzpunkte in einem Dokument zum Suchen darstellen. |
| [RedactionActionType](../com.groupdocs.redaction.redactions/redactionactiontype) | Stellt Aktionen dar, die zur Durchführung einer Redaktion ausgeführt werden können. |
| [ReplacementType](../com.groupdocs.redaction.redactions/replacementtype) | Stellt einen Typ des Austauschs für den übereinstimmenden Text dar. |
