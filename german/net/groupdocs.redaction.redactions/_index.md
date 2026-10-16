---
title: "GroupDocs.Redaction.Redactions"
second_title: "GroupDocs.Redaction für .NET API-Referenz"
description: "Der Redactions-Namespace stellt Klassen für verschiedene Arten von Redaktionen bereit."
type: docs
weight: 80
url: /de/net/groupdocs.redaction.redactions/
---
Der Redactions-Namespace stellt Klassen für verschiedene Arten von Redaktionen bereit.

## Klassen

| Klasse | Beschreibung |
| --- | --- |
| [AnnotationRedaction](./annotationredaction) | Stellt eine Redaktion dar, die Anmerkungstext (Kommentare usw.) ersetzt, der einem angegebenen regulären Ausdruck entspricht. |
| [CellColumnRedaction](./cellcolumnredaction) | Stellt eine Textredaktion dar, die Text in Tabellenkalkulationsdokumenten (CSV, Excel usw.) ersetzt. |
| [CellFilter](./cellfilter) | Bietet eine Option, den Geltungsbereich einer [`CellColumnRedaction`](../groupdocs.redaction.redactions/cellcolumnredaction) auf ein Arbeitsblatt und eine Spalte zu beschränken. |
| [CustomRedactionContext](./customredactioncontext) | Stellt Kontext für die Verarbeitung benutzerdefinierter Redaktionen bereit. |
| [CustomRedactionResult](./customredactionresult) | Stellt das Ergebnis einer benutzerdefinierten Redaktionsoperation dar. |
| [DeleteAnnotationRedaction](./deleteannotationredaction) | Stellt eine Textredaktion dar, die Anmerkungen löscht, wenn der Text einem angegebenen regulären Ausdruck entspricht (optional werden alle Anmerkungen gelöscht). |
| [EraseMetadataRedaction](./erasemetadataredaction) | Stellt eine Metadaten-Redaktion dar, die alle Metadaten oder Metadaten, die bestimmten MetadataFilters entsprechen, aus dem Dokument löscht. |
| [ExactPhraseRedaction](./exactphraseredaction) | Stellt eine Text-Redaktion dar, die eine exakte Phrase im Text des Dokuments ersetzt, standardmäßig ohne Berücksichtigung der Groß‑ und Kleinschreibung. |
| [ImageAreaRedaction](./imagearearedaction) | Stellt eine Redaktion dar, die ein farbiges Rechteck im angegebenen Bereich eines Bilddokuments platziert. |
| [MetadataRedaction](./metadataredaction) | Stellt eine abstrakte Basisklasse für Dokumenten‑Metadaten‑Redaktionen dar. |
| [MetadataSearchRedaction](./metadatasearchredaction) | Stellt eine Metadaten‑Redaktion dar, die Metadaten mithilfe regulärer Ausdrücke sucht und redigiert und dabei Schlüssel und/oder Werte abgleicht. |
| [PageAreaFilter](./pageareafilter) | Stellt einen Redaktionsfilter dar, der einen Bereich innerhalb einer Seite eines Dokuments festlegt, auf den die Redaktion angewendet wird. |
| [PageAreaRedaction](./pagearearedaction) | Stellt eine komplexe textuelle Redaktion dar, die Text, Bilder und Anmerkungen in einem Bereich der Seite beeinflusst. |
| [PageRangeFilter](./pagerangefilter) | Stellt einen Redaktionsfilter dar, der einen Seitenbereich innerhalb eines Dokuments festlegt, auf den die Redaktion angewendet wird. |
| [RedactionDescription](./redactiondescription) | Stellt Informationen zu einer einzelnen Änderungsaktion dar, die während des Redaktionsprozesses durchgeführt wurde. |
| [RedactionFilter](./redactionfilter) | Stellt einen Redaktionsfilter dar, der den Geltungsbereich innerhalb eines Dokuments festlegt, auf den Redaktionen angewendet werden. |
| [RegexRedaction](./regexredaction) | Stellt eine Text‑Redaktion dar, die Text im Dokument sucht und ersetzt, indem sie den bereitgestellten regulären Ausdruck abgleicht. |
| [RegionReplacementOptions](./regionreplacementoptions) | Stellt Farb‑ und Bereichsparameter für den Austausch von Bildregionen dar. Siehe [`ImageAreaRedaction`](../groupdocs.redaction.redactions/imagearearedaction). |
| [RemovePageRedaction](./removepageredaction) | Stellt eine Redaktion dar, die eine Seite (Folie, Arbeitsblatt usw.) aus einem Dokument entfernt. |
| [ReplacementOptions](./replacementoptions) | Stellt Optionen für den Austausch von übereinstimmendem Text dar. |
| [TextRedaction](./textredaction) | Stellt eine abstrakte Basisklasse für Dokumenten‑Text‑Redaktionen dar. |
| [TextReplacement](./textreplacement) | Stellt Informationen zum textuellen Austausch dar. |
## Schnittstellen

| Schnittstelle | Beschreibung |
| --- | --- |
| [ICustomRedactionHandler](./icustomredactionhandler) | Bietet eine Schnittstelle zur Implementierung benutzerdefinierter Redaktionslogik. |
| [IRedactionCallback](./iredactioncallback) | Definiert Methoden, die erforderlich sind, um Informationen zu jeder Redaktionsänderung zu erhalten und sie optional zu verhindern. |
## Aufzählung

| Aufzählung | Beschreibung |
| --- | --- |
| [MetadataFilters](./metadatafilters) | Stellt eine Liste der gebräuchlichsten Arten von Dokumenten‑Metadaten dar. |
| [PageSeekOrigin](./pageseekorigin) | Stellt die Felder bereit, die Referenzpunkte in einem Dokument zum Suchen darstellen. |
| [RedactionActionType](./redactionactiontype) | Stellt Aktionen dar, die zur Durchführung einer Redaktion ausgeführt werden können. |
| [RedactionType](./redactiontype) | Stellt einen Typ von Dokumentdaten dar, die von der Redaktion betroffen sind. |
| [ReplacementType](./replacementtype) | Stellt einen Typ des Austauschs für den übereinstimmenden Text dar. |

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
