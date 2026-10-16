---
title: "RedactionPolicy"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa una política de sanitización que contiene un conjunto de redacciones específicas para aplicar."
type: docs
weight: 14
url: /es/java/com.groupdocs.redaction/redactionpolicy/
---
**Inheritance:**
java.lang.Object
```
public class RedactionPolicy
```

Representa una política de saneamiento, que contiene un conjunto de redacciones específicas a aplicar.

*** ** * ** ***


**Learn more**

* More details about policies: [Use of redaction policies](../https://docs.groupdocs.com/redaction/java/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [RedactionPolicy()](#RedactionPolicy--) | Crea una nueva instancia de la política Redaction. |
|
|  | [RedactionPolicy(Redaction[] redactions)](#RedactionPolicy-com.groupdocs.redaction.Redaction---) | Crea una nueva instancia de la política Redaction con una lista específica de redacciones. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getRedactions()](#getRedactions--) | Obtiene una matriz de completamente configurada |
Redaction
-derived classes.
|
|  | [load(String filePath)](#load-java.lang.String-) | Carga una instancia de |
RedactionPolicy
desde una ruta de archivo.
|
|  | [load(InputStream input)](#load-java.io.InputStream-) | Carga una instancia de |
RedactionPolicy
desde un flujo.
|
|  | [save(String filePath)](#save-java.lang.String-) | Guarda la redaction policy en un archivo. |
|
|  | [save(OutputStream output)](#save-java.io.OutputStream-) | Guarda la redaction policy en un flujo. |
|
### RedactionPolicy() {#RedactionPolicy--}
```
public RedactionPolicy()
```


Crea una nueva instancia de la política Redaction.


### RedactionPolicy(Redaction[] redactions) {#RedactionPolicy-com.groupdocs.redaction.Redaction---}
```
public RedactionPolicy(Redaction[] redactions)
```


Crea una nueva instancia de la política Redaction con una lista específica de redacciones.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | Una matriz de redacciones para la política |
|

### getRedactions() {#getRedactions--}
```
public final Redaction[] getRedactions()
```


Obtiene una matriz de completamente configurada
Redaction
-derived classes.


**Returns:**
com.groupdocs.redaction.Redaction[] - Una matriz de clases derivadas de Redaction completamente configuradas.

### load(String filePath) {#load-java.lang.String-}
```
public static RedactionPolicy load(String filePath)
```


Carga una instancia de
RedactionPolicy
desde una ruta de archivo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | Ruta al archivo XML |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### load(InputStream input) {#load-java.io.InputStream-}
```
public static RedactionPolicy load(InputStream input)
```


Carga una instancia de
RedactionPolicy
desde un flujo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | entrada | java.io.InputStream | Flujo que contiene la configuración XML |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### save(String filePath) {#save-java.lang.String-}
```
public final void save(String filePath)
```


Guarda la redaction policy en un archivo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | Ruta al archivo. |
|

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Guarda la redaction policy en un flujo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | salida | java.io.OutputStream | Flujo de destino para guardar la política |
|

