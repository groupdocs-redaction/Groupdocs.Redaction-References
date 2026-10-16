---
title: "CustomRedactionResult"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa un resultado devuelto por ."
type: docs
weight: 14
url: /es/java/com.groupdocs.redaction.redactions/customredactionresult/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionResult
```

Representa un resultado devuelto por [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Constructores

| Constructor | Descripción |
| --- | --- |
| [CustomRedactionResult()](#CustomRedactionResult--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getApply()](#getApply--) | Obtiene un valor que indica si se debe aplicar el reemplazo. |
|
|  | [setApply(boolean value)](#setApply-boolean-) | Establece un valor que indica si se debe aplicar el reemplazo. |
|
|  | [getText()](#getText--) | Obtiene el texto de reemplazo usado cuando #getApply().getApply() es |
true
.
|
|  | [setText(String value)](#setText-java.lang.String-) | Establece el texto de reemplazo usado cuando #getApply().getApply() es |
true
.
|
### CustomRedactionResult() {#CustomRedactionResult--}
```
public CustomRedactionResult()
```


### getApply() {#getApply--}
```
public final boolean getApply()
```


Obtiene un valor que indica si se debe aplicar el reemplazo.


**Returns:**
boolean -  true  para reemplazar el texto coincidente con #getText().getText(); de lo contrario,  false .

### setApply(boolean value) {#setApply-boolean-}
```
public final void setApply(boolean value)
```


Establece un valor que indica si se debe aplicar el reemplazo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | true  para aplicar el reemplazo; de lo contrario,  false . |
|

### getText() {#getText--}
```
public final String getText()
```


Obtiene el texto de reemplazo usado cuando #getApply().getApply() es
true
.


**Returns:**
java.lang.String - El texto de reemplazo.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Establece el texto de reemplazo usado cuando #getApply().getApply() es
true
.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String | El texto de reemplazo. |
|

