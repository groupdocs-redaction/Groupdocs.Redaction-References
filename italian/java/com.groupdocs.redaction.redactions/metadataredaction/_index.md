---
title: "MetadataRedaction"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta una classe astratta di base per le redazioni dei metadati del documento."
type: docs
weight: 20
url: /it/java/com.groupdocs.redaction.redactions/metadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class MetadataRedaction extends Redaction
```

Rappresenta una classe astratta di base per le redazioni dei metadati del documento.

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Metadata redactions](../https://docs.groupdocs.com/redaction/java/metadata-redactions/)

<br />


## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getFilter()](#getFilter--) | Ottiene il filtro, che viene utilizzato per selezionare tutti o specifici metadati, ad esempio Autore o Azienda. |
|
|  | [setFilter(int value)](#setFilter-int-) | Imposta il filtro, che viene utilizzato per selezionare tutti o specifici metadati, ad esempio Autore o Azienda. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applica la redazione a una determinata istanza di formato. |
|
### getFilter() {#getFilter--}
```
public final int getFilter()
```


Ottiene il filtro, che viene utilizzato per selezionare tutti o specifici metadati, ad esempio Autore o Azienda.


**Returns:**
int - Il filtro, che viene utilizzato per selezionare tutti o specifici metadati, ad esempio Autore o Azienda.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Imposta il filtro, che viene utilizzato per selezionare tutti o specifici metadati, ad esempio Autore o Azienda.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Il filtro, che viene utilizzato per selezionare tutti o specifici metadati, ad esempio Autore o Azienda. |
|

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Applica la redazione a una determinata istanza di formato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Un'istanza di un documento a cui applicare la redazione |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

