---
title: "ExactPhraseRedaction"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta una redazione di testo che sostituisce una frase esatta nel testo del documento, non sensibile al maiuscolo/minuscolo per impostazione predefinita."
type: docs
weight: 17
url: /it/java/com.groupdocs.redaction.redactions/exactphraseredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class ExactPhraseRedaction extends TextRedaction
```

Rappresenta una redazione di testo che sostituisce una frase esatta nel testo del documento, senza distinzione tra maiuscole e minuscole per impostazione predefinita.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />

Il seguente esempio dimostra l'esecuzione di una ricerca e sostituzione di frase sensibile al maiuscolo/minuscolo.

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
// Per impostazione predefinita, isCaseSensitive = false;
doc.apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(System.Drawing.Color.Red)));
doc.save();
}
 
``` 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Inizializza una nuova istanza della classe ExactPhraseRedaction in modalità non sensibile al maiuscolo/minuscolo. |
|
|  | [ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-) | Inizializza una nuova istanza della classe ExactPhraseRedaction. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getSearchPhrase()](#getSearchPhrase--) | Ottiene la stringa da cercare e sostituire. |
|
|  | [isCaseSensitive()](#isCaseSensitive--) | Ottiene un valore che indica se la ricerca è sensibile alle maiuscole o meno. |
|
|  | [isRightToLeft()](#isRightToLeft--) | Ottiene un valore che indica se questo testo è da destra a sinistra o meno, false per impostazione predefinita. |
|
|  | [setRightToLeft(boolean value)](#setRightToLeft-boolean-) | Imposta un valore che indica se questo testo è da destra a sinistra o meno, false per impostazione predefinita. |
|
|  | [getDescription()](#getDescription--) | Restituisce una stringa che descrive la redazione e i suoi parametri. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applica la redazione a una determinata istanza di formato. |
|
### ExactPhraseRedaction(String searchPhrase, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)
```


Inizializza una nuova istanza della classe ExactPhraseRedaction in modalità non sensibile al maiuscolo/minuscolo.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | Stringa da cercare e sostituire |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Opzioni di sostituzione (testuale, colore) |
|

### ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)
```


Inizializza una nuova istanza della classe ExactPhraseRedaction.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | Stringa da cercare e sostituire |
|
|  | isCaseSensitive | boolean | True se è necessaria una ricerca sensibile alle maiuscole |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Opzioni di sostituzione (testuale, colore) |
|

### getSearchPhrase() {#getSearchPhrase--}
```
public final String getSearchPhrase()
```


Ottiene la stringa da cercare e sostituire.


**Returns:**
java.lang.String - La stringa da cercare e sostituire.

### isCaseSensitive() {#isCaseSensitive--}
```
public final boolean isCaseSensitive()
```


Ottiene un valore che indica se la ricerca è sensibile alle maiuscole o meno.


**Returns:**
boolean - Un valore che indica se la ricerca è sensibile alle maiuscole o meno.

### isRightToLeft() {#isRightToLeft--}
```
public final boolean isRightToLeft()
```


Ottiene un valore che indica se questo testo è da destra a sinistra o meno, false per impostazione predefinita.


**Returns:**
boolean - Un valore che indica se questo testo è da destra a sinistra o meno, false per impostazione predefinita.

### setRightToLeft(boolean value) {#setRightToLeft-boolean-}
```
public final void setRightToLeft(boolean value)
```


Imposta un valore che indica se questo testo è da destra a sinistra o meno, false per impostazione predefinita.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se questo testo è da destra a sinistra o meno, false per impostazione predefinita. |
|

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

