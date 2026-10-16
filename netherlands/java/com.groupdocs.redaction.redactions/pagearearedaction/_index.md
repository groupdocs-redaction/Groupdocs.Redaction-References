---
title: "PageAreaRedaction"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt een complexe tekstuele redactie voor die tekstafbeeldingen en annotaties in een gebied van de pagina beïnvloedt."
type: docs
weight: 23
url: /nl/java/com.groupdocs.redaction.redactions/pagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction), [com.groupdocs.redaction.redactions.RegexRedaction](../../com.groupdocs.redaction.redactions/regexredaction)
```
public class PageAreaRedaction extends RegexRedaction
```

Vertegenwoordigt een complexe tekstuele redactie die tekst, afbeeldingen en annotaties in een gebied van de pagina beïnvloedt.

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](../https://docs.groupdocs.com/redaction/java/use-page-area-redaction/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [PageAreaRedaction(Pattern regex, ReplacementOptions options)](#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initialiseert een nieuw exemplaar van de PageAreaRedaction‑klasse. |
|
|  | [PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions)](#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Initialiseert een nieuw exemplaar van de PageAreaRedaction‑klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getImageOptions()](#getImageOptions--) | Haalt de |
RegionReplacementOptions
opties met kleur- en gebiedsparameters.
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Past de redactie toe op een gegeven formaatinstantie. |
|
### PageAreaRedaction(Pattern regex, ReplacementOptions options) {#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public PageAreaRedaction(Pattern regex, ReplacementOptions options)
```


Initialiseert een nieuw exemplaar van de PageAreaRedaction‑klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Reguliere expressie om te zoeken en te vervangen |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Vervangingsopties (tekstueel, kleur) |
|

### PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions) {#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions)
```


Initialiseert een nieuw exemplaar van de PageAreaRedaction‑klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Reguliere expressie om te zoeken en te vervangen |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Vervangingsopties (tekstueel, kleur) |
|
|  | imageOptions | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Vervangingsopties (beeldgebied) |
|

### getImageOptions() {#getImageOptions--}
```
public final RegionReplacementOptions getImageOptions()
```


Haalt de
RegionReplacementOptions
opties met kleur- en gebiedsparameters.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Past de redactie toe op een gegeven formaatinstantie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Een instantie van een document om redactie toe te passen |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

