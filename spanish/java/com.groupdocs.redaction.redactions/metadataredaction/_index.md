---
title: "MetadataRedaction"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa una clase abstracta base para la redacción de metadatos de documentos."
type: docs
weight: 20
url: /es/java/com.groupdocs.redaction.redactions/metadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class MetadataRedaction extends Redaction
```

Representa una clase abstracta base para la redacción de metadatos de documentos.

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Metadata redactions](../https://docs.groupdocs.com/redaction/java/metadata-redactions/)

<br />


## Métodos

| Método | Descripción |
| --- | --- |
|  | [getFilter()](#getFilter--) | Obtiene el filtro, que se usa para seleccionar todo o metadatos específicos, por ejemplo Autor o Empresa. |
|
|  | [setFilter(int value)](#setFilter-int-) | Establece el filtro, que se usa para seleccionar todo o metadatos específicos, por ejemplo Autor o Empresa. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Aplica la redacción a una instancia de formato dada. |
|
### getFilter() {#getFilter--}
```
public final int getFilter()
```


Obtiene el filtro, que se usa para seleccionar todo o metadatos específicos, por ejemplo Autor o Empresa.


**Returns:**
int - El filtro, que se usa para seleccionar todo o metadatos específicos, por ejemplo Autor o Empresa.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Establece el filtro, que se usa para seleccionar todo o metadatos específicos, por ejemplo Autor o Empresa.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El filtro, que se usa para seleccionar todo o metadatos específicos, por ejemplo Autor o Empresa. |
|

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Aplica la redacción a una instancia de formato dada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Una instancia de un documento para aplicar la redacción |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

