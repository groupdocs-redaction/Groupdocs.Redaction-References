---
title: "TextLine"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta una riga di testo estratta dal motore OCR da un'immagine."
type: docs
weight: 16
url: /it/java/com.groupdocs.redaction.integration/textline/
---
**Inheritance:**
java.lang.Object
```
public class TextLine
```

Rappresenta una riga di testo, estratta dal motore OCR da un'immagine.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TextLine(TextFragment[] fragments)](#TextLine-com.groupdocs.redaction.integration.TextFragment---) | Inizializza una nuova istanza di una riga di testo, estratta dal motore OCR da un'immagine. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getFragments()](#getFragments--) | Ottiene un array di frammenti di testo, come simboli e parole, riconosciuti nella riga. |
|
|  | [toString()](#toString--) | Restituisce il contenuto testuale della riga di testo riconosciuta. |
|
### TextLine(TextFragment[] fragments) {#TextLine-com.groupdocs.redaction.integration.TextFragment---}
```
public TextLine(TextFragment[] fragments)
```


Inizializza una nuova istanza di una riga di testo, estratta dal motore OCR da un'immagine.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | fragments | [TextFragment\[\]](../../com.groupdocs.redaction.integration/textfragment) | insieme iniziale di frammenti di testo |
|

### getFragments() {#getFragments--}
```
public final TextFragment[] getFragments()
```


Ottiene un array di frammenti di testo, come simboli e parole, riconosciuti nella riga.


**Returns:**
com.groupdocs.redaction.integration.TextFragment[] - Un array di frammenti di testo, come simboli e parole, riconosciuti nella riga.

### toString() {#toString--}
```
public String toString()
```


Restituisce il contenuto testuale della riga di testo riconosciuta.


**Returns:**
java.lang.String - contenuto testuale della riga di testo riconosciuta

