---
title: "RegexRedaction"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Vertegenwoordigt een tekstredactie die tekst in het document doorzoekt en vervangt door de opgegeven reguliere expressie te matchen."
type: docs
weight: 28
url: /nl/java/com.groupdocs.redaction.redactions/regexredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class RegexRedaction extends TextRedaction
```

Vertegenwoordigt een tekstredactie die tekst in het document doorzoekt en vervangt door de opgegeven reguliere expressie te matchen.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [RegexRedaction(String pattern, ReplacementOptions options)](#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initialiseert een nieuwe instantie van de RegexRedaction-klasse. |
|
|  | [RegexRedaction(Pattern regex, ReplacementOptions options)](#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initialiseert een nieuwe instantie van de RegexRedaction-klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getRegularExpression()](#getRegularExpression--) | Haalt de reguliere expressie op om te matchen. |
|
|  | [getDescription()](#getDescription--) | Retourneert een string die de redactie en de parameters beschrijft. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Past de redactie toe op een gegeven formaatinstantie. |
|
### RegexRedaction(String pattern, ReplacementOptions options) {#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(String pattern, ReplacementOptions options)
```


Initialiseert een nieuwe instantie van de RegexRedaction-klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pattern | java.lang.String | Reguliere expressie om te zoeken en te vervangen |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Vervangingsopties (tekstueel, kleur) |
|

### RegexRedaction(Pattern regex, ReplacementOptions options) {#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(Pattern regex, ReplacementOptions options)
```


Initialiseert een nieuwe instantie van de RegexRedaction-klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Reguliere expressie om te zoeken en te vervangen |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Vervangingsopties (tekstueel, kleur) |
|

### getRegularExpression() {#getRegularExpression--}
```
public final Pattern getRegularExpression()
```


Haalt de reguliere expressie op om te matchen.


**Returns:**
java.util.regex.Pattern - De reguliere expressie om te matchen.

### getDescription() {#getDescription--}
```
public String getDescription()
```


Retourneert een string die de redactie en de parameters beschrijft.


**Returns:**
java.lang.String - Tekst die de naam van de redactie en parameters bevat.

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

