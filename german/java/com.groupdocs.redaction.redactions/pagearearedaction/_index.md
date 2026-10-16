---
title: "PageAreaRedaction"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt eine komplexe textuelle Schwärzung dar, die Textbilder und Anmerkungen in einem Bereich der Seite beeinflusst."
type: docs
weight: 23
url: /de/java/com.groupdocs.redaction.redactions/pagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction), [com.groupdocs.redaction.redactions.RegexRedaction](../../com.groupdocs.redaction.redactions/regexredaction)
```
public class PageAreaRedaction extends RegexRedaction
```

Stellt eine komplexe textuelle Redaktion dar, die Text, Bilder und Anmerkungen in einem Bereich der Seite betrifft.

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](../https://docs.groupdocs.com/redaction/java/use-page-area-redaction/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [PageAreaRedaction(Pattern regex, ReplacementOptions options)](#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initialisiert eine neue Instanz der Klasse PageAreaRedaction. |
|
|  | [PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions)](#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Initialisiert eine neue Instanz der Klasse PageAreaRedaction. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getImageOptions()](#getImageOptions--) | Liest das |
RegionReplacementOptions
Optionen mit Farb- und Flächenparametern.
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Wendet die Redaktion auf eine gegebene Formatinstanz an. |
|
### PageAreaRedaction(Pattern regex, ReplacementOptions options) {#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public PageAreaRedaction(Pattern regex, ReplacementOptions options)
```


Initialisiert eine neue Instanz der Klasse PageAreaRedaction.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Regulärer Ausdruck zum Suchen und Ersetzen |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Ersetzungsoptionen (textuell, Farbe) |
|

### PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions) {#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions)
```


Initialisiert eine neue Instanz der Klasse PageAreaRedaction.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Regulärer Ausdruck zum Suchen und Ersetzen |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Ersetzungsoptionen (textuell, Farbe) |
|
|  | imageOptions | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Ersetzungsoptionen (Bildbereich) |
|

### getImageOptions() {#getImageOptions--}
```
public final RegionReplacementOptions getImageOptions()
```


Liest das
RegionReplacementOptions
Optionen mit Farb- und Flächenparametern.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Wendet die Redaktion auf eine gegebene Formatinstanz an.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Eine Instanz eines Dokuments, auf das die Redaktion angewendet wird |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

