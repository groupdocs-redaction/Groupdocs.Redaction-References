---
title: "RecognizedImage"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta il testo estratto da un'immagine come risultato del suo processo di riconoscimento."
type: docs
weight: 13
url: /it/java/com.groupdocs.redaction.integration/recognizedimage/
---
**Inheritance:**
java.lang.Object
```
public class RecognizedImage
```

Rappresenta il testo, estratto da un'immagine come risultato del suo processo di riconoscimento.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [RecognizedImage(TextLine[] lines)](#RecognizedImage-com.groupdocs.redaction.integration.TextLine---) | Inizializza una nuova istanza della classe, utilizzando un insieme di righe riconosciute. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getText()](#getText--) | Ottiene l'equivalente testuale del testo strutturato. |
|
|  | [getLines()](#getLines--) | Ottiene le righe di testo, con i loro frammenti, riconosciute all'interno del documento. |
|
|  | [toString()](#toString--) | Ottiene l'equivalente testuale del testo strutturato. |
|
### RecognizedImage(TextLine[] lines) {#RecognizedImage-com.groupdocs.redaction.integration.TextLine---}
```
public RecognizedImage(TextLine[] lines)
```


Inizializza una nuova istanza della classe, utilizzando un insieme di righe riconosciute.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | lines | [TextLine\[\]](../../com.groupdocs.redaction.integration/textline) | un IEnumerable (ad esempio un elenco o un array) di righe riconosciute |
|

### getText() {#getText--}
```
public final String getText()
```


Ottiene l'equivalente testuale del testo strutturato.


**Returns:**
java.lang.String - Equivalente testuale del testo strutturato.

### getLines() {#getLines--}
```
public final TextLine[] getLines()
```


Ottiene le righe di testo, con i loro frammenti, riconosciute all'interno del documento.


**Returns:**
com.groupdocs.redaction.integration.TextLine[] - Righe di testo, con i loro frammenti, riconosciute all'interno del documento.

### toString() {#toString--}
```
public String toString()
```


Ottiene l'equivalente testuale del testo strutturato.


**Returns:**
java.lang.String - Testo riconosciuto

