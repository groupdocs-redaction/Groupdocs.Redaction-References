---
title: "CustomRedactionContext"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Fornisce i dati di input per ."
type: docs
weight: 13
url: /it/java/com.groupdocs.redaction.redactions/customredactioncontext/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionContext
```

Fornisce i dati di input per [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [CustomRedactionContext()](#CustomRedactionContext--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Restituisce il numero di pagina del frammento corrispondente, se disponibile. |
|
|  | [setPageNumber(int value)](#setPageNumber-int-) | Imposta il numero di pagina del frammento corrispondente. |
|
|  | [getText()](#getText--) | Restituisce il testo corrispondente per la redazione. |
|
|  | [setText(String value)](#setText-java.lang.String-) | Imposta il testo corrispondente per la redazione. |
|
### CustomRedactionContext() {#CustomRedactionContext--}
```
public CustomRedactionContext()
```


### getPageNumber() {#getPageNumber--}
```
public final int getPageNumber()
```


Restituisce il numero di pagina del frammento corrispondente, se disponibile.


**Returns:**
int - Il numero di pagina, o un valore specifico del formato se la pagina non è nota.

### setPageNumber(int value) {#setPageNumber-int-}
```
public final void setPageNumber(int value)
```


Imposta il numero di pagina del frammento corrispondente.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Il numero di pagina. |
|

### getText() {#getText--}
```
public final String getText()
```


Restituisce il testo corrispondente per la redazione.


**Returns:**
java.lang.String - Il testo corrispondente.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Imposta il testo corrispondente per la redazione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String | Il testo corrispondente. |
|

