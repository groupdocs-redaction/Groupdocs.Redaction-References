---
title: "RegexRedaction"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt eine Text-Redaktion dar, die Text im Dokument sucht und ersetzt, indem sie den bereitgestellten regulären Ausdruck abgleicht."
type: docs
weight: 28
url: /de/java/com.groupdocs.redaction.redactions/regexredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class RegexRedaction extends TextRedaction
```

Stellt eine Text-Redaktion dar, die Text im Dokument sucht und ersetzt, indem sie den bereitgestellten regulären Ausdruck abgleicht.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [RegexRedaction(String pattern, ReplacementOptions options)](#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initialisiert eine neue Instanz der Klasse RegexRedaction. |
|
|  | [RegexRedaction(Pattern regex, ReplacementOptions options)](#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initialisiert eine neue Instanz der Klasse RegexRedaction. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getRegularExpression()](#getRegularExpression--) | Liefert den regulären Ausdruck zum Abgleichen. |
|
|  | [getDescription()](#getDescription--) | Gibt eine Zeichenkette zurück, die die Redaktion und ihre Parameter beschreibt. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Wendet die Redaktion auf eine gegebene Formatinstanz an. |
|
### RegexRedaction(String pattern, ReplacementOptions options) {#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(String pattern, ReplacementOptions options)
```


Initialisiert eine neue Instanz der Klasse RegexRedaction.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pattern | java.lang.String | Regulärer Ausdruck zum Suchen und Ersetzen |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Ersetzungsoptionen (textuell, Farbe) |
|

### RegexRedaction(Pattern regex, ReplacementOptions options) {#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(Pattern regex, ReplacementOptions options)
```


Initialisiert eine neue Instanz der Klasse RegexRedaction.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Regulärer Ausdruck zum Suchen und Ersetzen |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Ersetzungsoptionen (textuell, Farbe) |
|

### getRegularExpression() {#getRegularExpression--}
```
public final Pattern getRegularExpression()
```


Liefert den regulären Ausdruck zum Abgleichen.


**Returns:**
java.util.regex.Pattern - Der reguläre Ausdruck zum Abgleichen.

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

