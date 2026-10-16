---
title: "RegexRedaction"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta una redazione di testo che ricerca e sostituisce il testo nel documento corrispondendo all'espressione regolare fornita."
type: docs
weight: 28
url: /it/java/com.groupdocs.redaction.redactions/regexredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class RegexRedaction extends TextRedaction
```

Rappresenta una redazione di testo che ricerca e sostituisce il testo nel documento corrispondendo all'espressione regolare fornita.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [RegexRedaction(String pattern, ReplacementOptions options)](#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Inizializza una nuova istanza della classe RegexRedaction. |
|
|  | [RegexRedaction(Pattern regex, ReplacementOptions options)](#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Inizializza una nuova istanza della classe RegexRedaction. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getRegularExpression()](#getRegularExpression--) | Ottiene l'espressione regolare da confrontare. |
|
|  | [getDescription()](#getDescription--) | Restituisce una stringa che descrive la redazione e i suoi parametri. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applica la redazione a una determinata istanza di formato. |
|
### RegexRedaction(String pattern, ReplacementOptions options) {#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(String pattern, ReplacementOptions options)
```


Inizializza una nuova istanza della classe RegexRedaction.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | modello | java.lang.String | Espressione regolare per la ricerca e la sostituzione |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Opzioni di sostituzione (testuale, colore) |
|

### RegexRedaction(Pattern regex, ReplacementOptions options) {#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(Pattern regex, ReplacementOptions options)
```


Inizializza una nuova istanza della classe RegexRedaction.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Espressione regolare per la ricerca e la sostituzione |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Opzioni di sostituzione (testuale, colore) |
|

### getRegularExpression() {#getRegularExpression--}
```
public final Pattern getRegularExpression()
```


Ottiene l'espressione regolare da confrontare.


**Returns:**
java.util.regex.Pattern - L'espressione regolare da corrispondere.

### getDescription() {#getDescription--}
```
public String getDescription()
```


Restituisce una stringa che descrive la redazione e i suoi parametri.


**Returns:**
java.lang.String - Testo, contenente il nome della redazione e i parametri.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Applica la redazione a una determinata istanza di formato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Un'istanza di un documento a cui applicare la redazione |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

