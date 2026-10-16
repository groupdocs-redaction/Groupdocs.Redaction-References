---
title: "CustomRedactionContext"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Proporciona datos de entrada para ."
type: docs
weight: 13
url: /es/java/com.groupdocs.redaction.redactions/customredactioncontext/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionContext
```

Proporciona datos de entrada para [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Constructores

| Constructor | Descripción |
| --- | --- |
| [CustomRedactionContext()](#CustomRedactionContext--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Obtiene el número de página del fragmento coincidente, cuando está disponible. |
|
|  | [setPageNumber(int value)](#setPageNumber-int-) | Establece el número de página del fragmento coincidente. |
|
|  | [getText()](#getText--) | Obtiene el texto coincidente para la redacción. |
|
|  | [setText(String value)](#setText-java.lang.String-) | Establece el texto coincidente para la redacción. |
|
### CustomRedactionContext() {#CustomRedactionContext--}
```
public CustomRedactionContext()
```


### getPageNumber() {#getPageNumber--}
```
public final int getPageNumber()
```


Obtiene el número de página del fragmento coincidente, cuando está disponible.


**Returns:**
int - El número de página, o un valor específico del formato si la página no se conoce.

### setPageNumber(int value) {#setPageNumber-int-}
```
public final void setPageNumber(int value)
```


Establece el número de página del fragmento coincidente.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El número de página. |
|

### getText() {#getText--}
```
public final String getText()
```


Obtiene el texto coincidente para la redacción.


**Returns:**
java.lang.String - El texto coincidente.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Establece el texto coincidente para la redacción.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String | El texto coincidente. |
|

