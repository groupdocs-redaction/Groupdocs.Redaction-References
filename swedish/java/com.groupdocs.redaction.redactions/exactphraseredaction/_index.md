---
title: "ExactPhraseRedaction"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar en textredigering som ersätter en exakt fras i dokumentets text utan att ta hänsyn till skiftläge som standard."
type: docs
weight: 17
url: /sv/java/com.groupdocs.redaction.redactions/exactphraseredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class ExactPhraseRedaction extends TextRedaction
```

Representerar en textradering som ersätter exakt fras i dokumentets text, skiftlägesokänslig som standard.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />

Följande exempel demonstrerar utförandet av skiftlägeskänslig frassökning och ersättning.

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
   // By default, the second parameter, isCaseSensitive = false;
   doc.apply(new ExactPhraseRedaction("John Doe", true, new ReplacementOptions("[personal]")));
   doc.save();
 }
 
``` 
````

The following example demonstrates replacing phrase (case insensitive) with solid red rectangle.

````

try (Redactor redactor = new Redactor("C:\\sample.pdf"))
{
// Som standard, isCaseSensitive = false;
doc.apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(System.Drawing.Color.Red)));
doc.save();
}
 
``` 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initierar en ny instans av ExactPhraseRedaction-klassen i läge utan skiftlägeskänslighet. |
|
|  | [ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initierar en ny instans av ExactPhraseRedaction-klassen. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getSearchPhrase()](#getSearchPhrase--) | Hämtar strängen att söka och ersätta. |
|
|  | [isCaseSensitive()](#isCaseSensitive--) | Hämtar ett värde som indikerar om sökningen är skiftlägeskänslig eller inte. |
|
|  | [isRightToLeft()](#isRightToLeft--) | Hämtar ett värde som indikerar om denna text är från höger till vänster eller inte, falskt som standard. |
|
|  | [setRightToLeft(boolean value)](#setRightToLeft-boolean-) | Ställer in ett värde som indikerar om denna text är från höger till vänster eller inte, falskt som standard. |
|
|  | [getDescription()](#getDescription--) | Returnerar en sträng som beskriver redigeringen och dess parametrar. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Tillämpar redigeringen på en given formatinstans. |
|
### ExactPhraseRedaction(String searchPhrase, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)
```


Initierar en ny instans av ExactPhraseRedaction-klassen i läge utan skiftlägeskänslighet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | Sträng att söka och ersätta |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Ersättningsalternativ (textuell, färg) |
|

### ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)
```


Initierar en ny instans av ExactPhraseRedaction-klassen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | Sträng att söka och ersätta |
|
|  | isCaseSensitive | boolean | Sant om skiftlägeskänslig sökning krävs |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Ersättningsalternativ (textuell, färg) |
|

### getSearchPhrase() {#getSearchPhrase--}
```
public final String getSearchPhrase()
```


Hämtar strängen att söka och ersätta.


**Returns:**
java.lang.String - Strängen att söka och ersätta.

### isCaseSensitive() {#isCaseSensitive--}
```
public final boolean isCaseSensitive()
```


Hämtar ett värde som indikerar om sökningen är skiftlägeskänslig eller inte.


**Returns:**
boolean - Ett värde som indikerar om sökningen är skiftlägeskänslig eller inte.

### isRightToLeft() {#isRightToLeft--}
```
public final boolean isRightToLeft()
```


Hämtar ett värde som indikerar om denna text är från höger till vänster eller inte, falskt som standard.


**Returns:**
boolean - Ett värde som indikerar om denna text är från höger till vänster eller inte, falskt som standard.

### setRightToLeft(boolean value) {#setRightToLeft-boolean-}
```
public final void setRightToLeft(boolean value)
```


Ställer in ett värde som indikerar om denna text är från höger till vänster eller inte, falskt som standard.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om denna text är från höger till vänster eller inte, falskt som standard. |
|

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

