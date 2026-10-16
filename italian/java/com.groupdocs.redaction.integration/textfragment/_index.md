---
title: "TextFragment"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta una parte del testo riconosciuto, parola, simbolo, ecc., estratta dal motore OCR."
type: docs
weight: 15
url: /it/java/com.groupdocs.redaction.integration/textfragment/
---
**Inheritance:**
java.lang.Object
```
public class TextFragment
```

Rappresenta una parte del testo riconosciuto (parola, simbolo, ecc.), estratta dal motore OCR.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TextFragment(String text, Rectangle rectangle)](#TextFragment-java.lang.String-java.awt.Rectangle-) | Inizializza una nuova istanza del frammento di testo riconosciuto. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getText()](#getText--) | Ottiene un contenuto testuale del frammento di testo riconosciuto. |
|
|  | [getRectangle()](#getRectangle--) | Ottiene un rettangolo di delimitazione del frammento di testo riconosciuto. |
|
|  | [toString()](#toString--) | Restituisce il contenuto testuale del frammento di testo riconosciuto. |
|
### TextFragment(String text, Rectangle rectangle) {#TextFragment-java.lang.String-java.awt.Rectangle-}
```
public TextFragment(String text, Rectangle rectangle)
```


Inizializza una nuova istanza del frammento di testo riconosciuto.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | testo | java.lang.String | contenuto testuale del frammento di testo riconosciuto |
|
|  | rectangle | java.awt.Rectangle | rettangolo di delimitazione del frammento di testo riconosciuto |
|

### getText() {#getText--}
```
public final String getText()
```


Ottiene un contenuto testuale del frammento di testo riconosciuto.


**Returns:**
java.lang.String - Un contenuto testuale del frammento di testo riconosciuto.

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Ottiene un rettangolo di delimitazione del frammento di testo riconosciuto.


**Returns:**
java.awt.Rectangle - Un rettangolo di delimitazione del frammento di testo riconosciuto.

### toString() {#toString--}
```
public String toString()
```


Restituisce il contenuto testuale del frammento di testo riconosciuto.


**Returns:**
java.lang.String - contenuto testuale del frammento di testo riconosciuto

