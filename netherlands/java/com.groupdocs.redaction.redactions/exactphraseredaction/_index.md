---
title: "ExactPhraseRedaction"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt een tekstredactie voor die standaard een exacte zin in de documenttekst vervangt zonder hoofdlettergevoeligheid."
type: docs
weight: 17
url: /nl/java/com.groupdocs.redaction.redactions/exactphraseredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class ExactPhraseRedaction extends TextRedaction
```

Stelt een tekstredactie voor die exacte zinnen in de documenttekst vervangt, standaard zonder hoofdlettergevoeligheid.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />

Het volgende voorbeeld toont het uitvoeren van een hoofdlettergevoelige zoekopdracht en vervanging van een zin.

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
// Standaard is isCaseSensitive = false;
doc.apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(System.Drawing.Color.Red)));
doc.save();
}
 
``` 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initialiseert een nieuw exemplaar van de ExactPhraseRedaction-klasse in niet-hoofdlettergevoelige modus. |
|
|  | [ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initialiseert een nieuw exemplaar van de ExactPhraseRedaction-klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getSearchPhrase()](#getSearchPhrase--) | Haalt de string op om te zoeken en te vervangen. |
|
|  | [isCaseSensitive()](#isCaseSensitive--) | Haalt een waarde op die aangeeft of de zoekopdracht hoofdlettergevoelig is of niet. |
|
|  | [isRightToLeft()](#isRightToLeft--) | Haalt een waarde op die aangeeft of deze tekst van rechts naar links is of niet, standaard false. |
|
|  | [setRightToLeft(boolean value)](#setRightToLeft-boolean-) | Stelt een waarde in die aangeeft of deze tekst van rechts naar links is of niet, standaard false. |
|
|  | [getDescription()](#getDescription--) | Retourneert een string die de redactie en de parameters beschrijft. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Past de redactie toe op een gegeven formaatinstantie. |
|
### ExactPhraseRedaction(String searchPhrase, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)
```


Initialiseert een nieuw exemplaar van de ExactPhraseRedaction-klasse in niet-hoofdlettergevoelige modus.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | String om te zoeken en te vervangen |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Vervangingsopties (tekstueel, kleur) |
|

### ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)
```


Initialiseert een nieuw exemplaar van de ExactPhraseRedaction-klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | String om te zoeken en te vervangen |
|
|  | isCaseSensitive | boolean | True als een hoofdlettergevoelige zoekopdracht vereist is |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Vervangingsopties (tekstueel, kleur) |
|

### getSearchPhrase() {#getSearchPhrase--}
```
public final String getSearchPhrase()
```


Haalt de string op om te zoeken en te vervangen.


**Returns:**
java.lang.String - De string om te zoeken en te vervangen.

### isCaseSensitive() {#isCaseSensitive--}
```
public final boolean isCaseSensitive()
```


Haalt een waarde op die aangeeft of de zoekopdracht hoofdlettergevoelig is of niet.


**Returns:**
boolean - Een waarde die aangeeft of de zoekopdracht hoofdlettergevoelig is of niet.

### isRightToLeft() {#isRightToLeft--}
```
public final boolean isRightToLeft()
```


Haalt een waarde op die aangeeft of deze tekst van rechts naar links is of niet, standaard false.


**Returns:**
boolean - Een waarde die aangeeft of deze tekst van rechts naar links is of niet, standaard false.

### setRightToLeft(boolean value) {#setRightToLeft-boolean-}
```
public final void setRightToLeft(boolean value)
```


Stelt een waarde in die aangeeft of deze tekst van rechts naar links is of niet, standaard false.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft of deze tekst van rechts naar links is of niet, standaard false. |
|

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

