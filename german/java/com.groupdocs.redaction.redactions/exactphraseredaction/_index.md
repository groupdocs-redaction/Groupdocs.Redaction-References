---
title: "ExactPhraseRedaction"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt eine Textredaktion dar, die standardmäßig die genaue Phrase im Dokumententext ohne Berücksichtigung der Groß‑ und Kleinschreibung ersetzt."
type: docs
weight: 17
url: /de/java/com.groupdocs.redaction.redactions/exactphraseredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class ExactPhraseRedaction extends TextRedaction
```

Stellt eine Textredaktion dar, die eine exakte Phrase im Dokumenttext ersetzt, standardmäßig ohne Berücksichtigung der Groß‑ und Kleinschreibung.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />

Das folgende Beispiel demonstriert die Durchführung einer groß-/kleinschreibungssensitiven Suche und Ersetzung von Phrasen.

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
// Standardmäßig ist isCaseSensitive = false;
doc.apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(System.Drawing.Color.Red)));
doc.save();
}
 
``` 
````


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initialisiert eine neue Instanz der Klasse ExactPhraseRedaction im Modus ohne Groß‑ und Kleinschreibung. |
|
|  | [ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initialisiert eine neue Instanz der Klasse ExactPhraseRedaction. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getSearchPhrase()](#getSearchPhrase--) | Ruft die zu suchende und zu ersetzende Zeichenkette ab. |
|
|  | [isCaseSensitive()](#isCaseSensitive--) | Ruft einen Wert ab, der angibt, ob die Suche groß-/kleinschreibungssensitiv ist oder nicht. |
|
|  | [isRightToLeft()](#isRightToLeft--) | Ruft einen Wert ab, der angibt, ob dieser Text von rechts nach links verläuft oder nicht, standardmäßig false. |
|
|  | [setRightToLeft(boolean value)](#setRightToLeft-boolean-) | Setzt einen Wert, der angibt, ob dieser Text von rechts nach links verläuft oder nicht, standardmäßig false. |
|
|  | [getDescription()](#getDescription--) | Gibt eine Zeichenkette zurück, die die Redaktion und ihre Parameter beschreibt. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Wendet die Redaktion auf eine gegebene Formatinstanz an. |
|
### ExactPhraseRedaction(String searchPhrase, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)
```


Initialisiert eine neue Instanz der Klasse ExactPhraseRedaction im Modus ohne Groß‑ und Kleinschreibung.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | Zeichenkette zum Suchen und Ersetzen |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Ersetzungsoptionen (textuell, Farbe) |
|

### ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)
```


Initialisiert eine neue Instanz der Klasse ExactPhraseRedaction.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | Zeichenkette zum Suchen und Ersetzen |
|
|  | isCaseSensitive | boolean | True, wenn eine groß-/kleinschreibungssensible Suche erforderlich ist |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Ersetzungsoptionen (textuell, Farbe) |
|

### getSearchPhrase() {#getSearchPhrase--}
```
public final String getSearchPhrase()
```


Ruft die zu suchende und zu ersetzende Zeichenkette ab.


**Returns:**
java.lang.String - Die Zeichenkette zum Suchen und Ersetzen.

### isCaseSensitive() {#isCaseSensitive--}
```
public final boolean isCaseSensitive()
```


Ruft einen Wert ab, der angibt, ob die Suche groß-/kleinschreibungssensitiv ist oder nicht.


**Returns:**
boolean - Ein Wert, der angibt, ob die Suche groß-/kleinschreibungssensitiv ist oder nicht.

### isRightToLeft() {#isRightToLeft--}
```
public final boolean isRightToLeft()
```


Ruft einen Wert ab, der angibt, ob dieser Text von rechts nach links verläuft oder nicht, standardmäßig false.


**Returns:**
boolean - Ein Wert, der angibt, ob dieser Text von rechts nach links verläuft oder nicht, standardmäßig false.

### setRightToLeft(boolean value) {#setRightToLeft-boolean-}
```
public final void setRightToLeft(boolean value)
```


Setzt einen Wert, der angibt, ob dieser Text von rechts nach links verläuft oder nicht, standardmäßig false.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob dieser Text von rechts nach links verläuft oder nicht, standardmäßig false. |
|

### getDescription() {#getDescription--}
```
public String getDescription()
```


Gibt eine Zeichenkette zurück, die die Redaktion und ihre Parameter beschreibt.


**Returns:**
java.lang.String - Text, der den Namen der Redaktion und Parameter enthält.

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

