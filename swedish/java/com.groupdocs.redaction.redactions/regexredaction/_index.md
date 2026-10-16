---
title: "RegexRedaction"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar en textredigering som söker och ersätter text i dokumentet genom att matcha det angivna reguljära uttrycket."
type: docs
weight: 28
url: /sv/java/com.groupdocs.redaction.redactions/regexredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class RegexRedaction extends TextRedaction
```

Representerar en textredigering som söker och ersätter text i dokumentet genom att matcha det angivna reguljära uttrycket.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [RegexRedaction(String pattern, ReplacementOptions options)](#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initierar en ny instans av klassen RegexRedaction. |
|
|  | [RegexRedaction(Pattern regex, ReplacementOptions options)](#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initierar en ny instans av klassen RegexRedaction. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getRegularExpression()](#getRegularExpression--) | Hämtar det reguljära uttrycket att matcha. |
|
|  | [getDescription()](#getDescription--) | Returnerar en sträng som beskriver redigeringen och dess parametrar. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Tillämpar redigeringen på en given formatinstans. |
|
### RegexRedaction(String pattern, ReplacementOptions options) {#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(String pattern, ReplacementOptions options)
```


Initierar en ny instans av klassen RegexRedaction.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | mönster | java.lang.String | Reguljärt uttryck för sökning och ersättning |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Ersättningsalternativ (textuell, färg) |
|

### RegexRedaction(Pattern regex, ReplacementOptions options) {#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(Pattern regex, ReplacementOptions options)
```


Initierar en ny instans av klassen RegexRedaction.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Reguljärt uttryck för sökning och ersättning |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Ersättningsalternativ (textuell, färg) |
|

### getRegularExpression() {#getRegularExpression--}
```
public final Pattern getRegularExpression()
```


Hämtar det reguljära uttrycket att matcha.


**Returns:**
java.util.regex.Pattern - Det reguljära uttrycket att matcha.

### getDescription() {#getDescription--}
```
public String getDescription()
```


Returnerar en sträng som beskriver redigeringen och dess parametrar.


**Returns:**
java.lang.String - Text som innehåller redigeringsnamn och parametrar.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Tillämpar redigeringen på en given formatinstans.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | En instans av ett dokument för att tillämpa redigering |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

