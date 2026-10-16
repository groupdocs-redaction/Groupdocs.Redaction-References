---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta le informazioni di una singola azione di modifica eseguita durante il processo di redazione."
type: docs
weight: 25
url: /it/java/com.groupdocs.redaction.redactions/redactiondescription/
---
**Inheritance:**
java.lang.Object
```
public class RedactionDescription
```

Rappresenta le informazioni di una singola azione di modifica eseguita durante il processo di redazione.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-) | Inizializza una nuova istanza della classe RedactionDescription senza informazioni di sostituzione. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-) | Inizializza una nuova istanza della classe RedactionDescription con informazioni di sostituzione. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-) | Inizializza una nuova istanza della classe RedactionDescription con informazioni di sostituzione dell'area immagine. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getRedactionType()](#getRedactionType--) | Ottiene il tipo di dati del documento - testo, metadati o annotazioni. |
|
|  | [getActionType()](#getActionType--) | Ottiene l'operazione di redazione: sostituzione, pulizia o eliminazione. |
|
|  | [getOriginalText()](#getOriginalText--) | Ottiene il testo corrispondente, se è fornita un'espressione. |
|
|  | [getReplacement()](#getReplacement--) | Ottiene le informazioni di sostituzione, può essere null. |
|
|  | [getImageAreaReplacement()](#getImageAreaReplacement--) | Ottiene le informazioni di sostituzione per le redazioni di aree immagine, restituisce null per le redazioni testuali. |
|
|  | [getDetails()](#getDetails--) | Ottiene un'informazione opzionale di dettaglio per l'elemento in fase di redazione. |
|
|  | [setDetails(String value)](#setDetails-java.lang.String-) | Imposta un'informazione opzionale di dettaglio per l'elemento in fase di redazione. |
|
### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)
```


Inizializza una nuova istanza della classe RedactionDescription senza informazioni di sostituzione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | redactionType | int | Tipo di dati in fase di redazione |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Azione da eseguire su questi dati |
|
|  | originalText | java.lang.String | Testo corrispondente, commento o corpo dell'annotazione |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)
```


Inizializza una nuova istanza della classe RedactionDescription con informazioni di sostituzione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | redactionType | int | Tipo di dati in fase di redazione |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Azione da eseguire su questi dati |
|
|  | originalText | java.lang.String | Testo corrispondente, commento o corpo dell'annotazione |
|
|  | replacement | [TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) | Testo di sostituzione, testo corrispondente e la sua posizione nella stringa originale |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)
```


Inizializza una nuova istanza della classe RedactionDescription con informazioni di sostituzione dell'area immagine.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | redactionType | int | Tipo di dati in fase di redazione |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Azione da eseguire su questi dati |
|
|  | imageAreaReplacement | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Informazioni di sostituzione dell'area immagine |
|
|  | imageDetails | java.lang.String | Descrizione testuale dell'immagine, per impostazione predefinita è String.Empty |
|

### getRedactionType() {#getRedactionType--}
```
public final int getRedactionType()
```


Ottiene il tipo di dati del documento - testo, metadati o annotazioni.


**Returns:**
int - Il tipo di dati del documento - testo, metadati o annotazioni.

### getActionType() {#getActionType--}
```
public final RedactionActionType getActionType()
```


Ottiene l'operazione di redazione: sostituzione, pulizia o eliminazione.


**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) - The redaction operation: replacement, cleanup or deletion.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Ottiene il testo corrispondente, se è fornita un'espressione.


**Returns:**
java.lang.String - Il testo corrispondente, se è fornita un'espressione.

### getReplacement() {#getReplacement--}
```
public final TextReplacement getReplacement()
```


Ottiene le informazioni di sostituzione, può essere null.


**Returns:**
[TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) - The replacement information, can be null.

### getImageAreaReplacement() {#getImageAreaReplacement--}
```
public final RegionReplacementOptions getImageAreaReplacement()
```


Ottiene le informazioni di sostituzione per le redazioni di aree immagine, restituisce null per le redazioni testuali.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The replacement information for image area redactions, returns null for textual redactions.

### getDetails() {#getDetails--}
```
public final String getDetails()
```


Ottiene un'informazione opzionale di dettaglio per l'elemento in fase di redazione.


**Returns:**
java.lang.String - Un'informazione opzionale di dettaglio per l'elemento in fase di redazione.

### setDetails(String value) {#setDetails-java.lang.String-}
```
public final void setDetails(String value)
```


Imposta un'informazione opzionale di dettaglio per l'elemento in fase di redazione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String | Un'informazione opzionale di dettaglio per l'elemento in fase di redazione. |
|

