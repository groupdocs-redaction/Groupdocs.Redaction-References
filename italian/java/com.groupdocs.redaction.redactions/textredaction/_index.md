---
title: "TextRedaction"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta una classe astratta di base per le redazioni testuali del documento."
type: docs
weight: 32
url: /it/java/com.groupdocs.redaction.redactions/textredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class TextRedaction extends Redaction
```

Rappresenta una classe astratta di base per le redazioni testuali del documento.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getActionOptions()](#getActionOptions--) | Ottiene il |
ReplacementOptions
istanza, specificando il tipo di sostituzione del testo.
|
|  | [getOcrConnector()](#getOcrConnector--) | Ottiene il |
IOcrConnector
implementazione, necessaria per estrarre il testo dal contenuto grafico.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Imposta il |
IOcrConnector
implementazione, necessaria per estrarre il testo dal contenuto grafico.
|
### getActionOptions() {#getActionOptions--}
```
public final ReplacementOptions getActionOptions()
```


Ottiene il
ReplacementOptions
istanza, specificando il tipo di sostituzione del testo.


**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) - The  ReplacementOptions  instance, specifying type of text replacement.

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Ottiene il
IOcrConnector
implementazione, necessaria per estrarre il testo dal contenuto grafico.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - The  IOcrConnector  implementation, required to extract text from graphic content.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Imposta il
IOcrConnector
implementazione, necessaria per estrarre il testo dal contenuto grafico.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | L'implementazione  IOcrConnector  , necessaria per estrarre il testo dal contenuto grafico. |
|

