---
title: "ReplacementOptions"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta le opzioni per la sostituzione del testo corrispondente."
type: docs
weight: 31
url: /it/java/com.groupdocs.redaction.redactions/replacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class ReplacementOptions
```

Rappresenta le opzioni per la sostituzione del testo corrispondente.

*** ** * ** ***


**Learn more**

* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [ReplacementOptions(String replacement)](#ReplacementOptions-java.lang.String-) | Inizializza una nuova istanza della classe ReplacementOptions con il testo di sostituzione come opzione. |
|
|  | [ReplacementOptions(Color color)](#ReplacementOptions-java.awt.Color-) | Inizializza una nuova istanza della classe ReplacementOptions con un rettangolo colorato come opzione. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getActionType()](#getActionType--) | Ottiene l'azione di sostituzione: disegnare un riquadro o sostituire il testo. |
|
|  | [getReplacement()](#getReplacement--) | Ottiene il valore di sostituzione testuale. |
|
|  | [setReplacement(String value)](#setReplacement-java.lang.String-) | Imposta il valore di sostituzione testuale. |
|
|  | [getBoxColor()](#getBoxColor--) | Ottiene il colore per un |
ReplacementType.DrawBox
opzione (ignorata altrimenti).
|
|  | [setBoxColor(Color value)](#setBoxColor-java.awt.Color-) | Imposta il colore per un |
ReplacementType.DrawBox
opzione (ignorata altrimenti).
|
|  | [getFilters()](#getFilters--) | Ottiene un array di filtri da applicare con questa redazione. |
|
|  | [setFilters(RedactionFilter[] value)](#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---) | Imposta un array di filtri da applicare con questa redazione. |
|
|  | [getCustomRedaction()](#getCustomRedaction--) | Ottiene un gestore di redazione personalizzato. |
|
|  | [setCustomRedaction(ICustomRedactionHandler value)](#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-) | Imposta un gestore di redazione personalizzato. |
|
| [fromFilters(RedactionFilter[] filters)](#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---) |  |
### ReplacementOptions(String replacement) {#ReplacementOptions-java.lang.String-}
```
public ReplacementOptions(String replacement)
```


Inizializza una nuova istanza della classe ReplacementOptions con il testo di sostituzione come opzione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | sostituzione | java.lang.String | Sostituzione testuale |
|

### ReplacementOptions(Color color) {#ReplacementOptions-java.awt.Color-}
```
public ReplacementOptions(Color color)
```


Inizializza una nuova istanza della classe ReplacementOptions con un rettangolo colorato come opzione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | colore | java.awt.Color | Colore del rettangolo |
|

### getActionType() {#getActionType--}
```
public final ReplacementType getActionType()
```


Ottiene l'azione di sostituzione: disegnare un riquadro o sostituire il testo.


**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype) - The replacement action: draw box or replace text.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Ottiene il valore di sostituzione testuale.


**Returns:**
java.lang.String - Il valore di sostituzione testuale.

### setReplacement(String value) {#setReplacement-java.lang.String-}
```
public final void setReplacement(String value)
```


Imposta il valore di sostituzione testuale.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String | Il valore di sostituzione testuale. |
|

### getBoxColor() {#getBoxColor--}
```
public final Color getBoxColor()
```


Ottiene il colore per un
ReplacementType.DrawBox
opzione (ignorata altrimenti).


**Returns:**
java.awt.Color - Il colore per un  ReplacementType.DrawBox  opzione (ignorata altrimenti).

### setBoxColor(Color value) {#setBoxColor-java.awt.Color-}
```
public final void setBoxColor(Color value)
```


Imposta il colore per un
ReplacementType.DrawBox
opzione (ignorata altrimenti).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.awt.Color | Il colore per un  ReplacementType.DrawBox  opzione (ignorata altrimenti). |
|

### getFilters() {#getFilters--}
```
public final RedactionFilter[] getFilters()
```


Ottiene un array di filtri da applicare con questa redazione.


**Returns:**
com.groupdocs.redaction.redactions.RedactionFilter[] - Un array di filtri da applicare con questa redazione.

### setFilters(RedactionFilter[] value) {#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public final void setFilters(RedactionFilter[] value)
```


Imposta un array di filtri da applicare con questa redazione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) | Un array di filtri da applicare con questa redazione. |
|

### getCustomRedaction() {#getCustomRedaction--}
```
public final ICustomRedactionHandler getCustomRedaction()
```


Ottiene un gestore di redazione personalizzato. Supportato solo per PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Returns:**
[ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) - An instance of [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler), or  null  if not set.

### setCustomRedaction(ICustomRedactionHandler value) {#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-}
```
public final void setCustomRedaction(ICustomRedactionHandler value)
```


Imposta un gestore di redazione personalizzato. Supportato solo per PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) | Un'istanza di [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler). |
|

### fromFilters(RedactionFilter[] filters) {#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public static ReplacementOptions fromFilters(RedactionFilter[] filters)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filters | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) |  |

**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions)
