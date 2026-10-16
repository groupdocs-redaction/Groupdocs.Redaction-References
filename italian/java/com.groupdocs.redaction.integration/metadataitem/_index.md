---
title: "MetadataItem"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta un elemento di metadati comune a tutti i formati supportati e utilizzato nelle redazioni di metadati."
type: docs
weight: 12
url: /it/java/com.groupdocs.redaction.integration/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Rappresenta un elemento di metadati, comune a tutti i formati supportati e utilizzato nelle redazioni dei metadati.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [MetadataItem()](#MetadataItem--) | Inizializza una nuova istanza. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getOriginalName()](#getOriginalName--) | Ottiene il nome originale dell'elemento di metadati, così come appare nel documento. |
|
|  | [setOriginalName(String value)](#setOriginalName-java.lang.String-) | Imposta il nome originale dell'elemento di metadati, così come appare nel documento. |
|
|  | [getCategory()](#getCategory--) | Ottiene una categoria dell'elemento di metadati, ad esempio l'ID risorsa per un elemento di metadati di risorsa incorporata. |
|
|  | [setCategory(String value)](#setCategory-java.lang.String-) | Imposta una categoria dell'elemento di metadati, ad esempio l'ID della risorsa per un elemento di metadati di risorsa incorporata. |
|
|  | [getFilter()](#getFilter--) | Ottiene un valore di |
MetadataFilters
, assegnato a questo elemento di metadati che è usato nella filtrazione degli elementi.
|
|  | [setFilter(int value)](#setFilter-int-) | Imposta un valore di |
MetadataFilters
, assegnato a questo elemento di metadati che è usato nella filtrazione degli elementi.
|
|  | [getValues()](#getValues--) | Ottiene il valore dell'elemento di metadati. |
|
|  | [setValues(List<String> value)](#setValues-java.util.List-java.lang.String--) | Imposta il valore dell'elemento di metadati. |
|
|  | [isCustom()](#isCustom--) | Ottiene un valore che indica se questo elemento è personalizzato (aggiunto dagli autori del documento). |
|
|  | [setCustom(boolean value)](#setCustom-boolean-) | Imposta un valore che indica se questo elemento è personalizzato (aggiunto dagli autori del documento). |
|
|  | [getDictionaryKey()](#getDictionaryKey--) | Ottiene una chiave di dizionario per , usando il suo OriginalName e altri dati. |
|
|  | [createClone()](#createClone--) | Crea una copia profonda dell'istanza corrente. |
|
|  | [getActualValue()](#getActualValue--) | Ottiene la rappresentazione stringa del valore dell'elemento di metadati. |
|
### MetadataItem() {#MetadataItem--}
```
public MetadataItem()
```


Inizializza una nuova istanza.


### getOriginalName() {#getOriginalName--}
```
public final String getOriginalName()
```


Ottiene il nome originale dell'elemento di metadati, così come appare nel documento.


**Returns:**
java.lang.String - Un nome originale dell'elemento di metadati, così come appare nel documento.

### setOriginalName(String value) {#setOriginalName-java.lang.String-}
```
public final void setOriginalName(String value)
```


Imposta il nome originale dell'elemento di metadati, così come appare nel documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String | Un nome originale dell'elemento di metadati, così come appare nel documento. |
|

### getCategory() {#getCategory--}
```
public final String getCategory()
```


Ottiene una categoria dell'elemento di metadati, ad esempio l'ID risorsa per un elemento di metadati di risorsa incorporata.


**Returns:**
java.lang.String - Una categoria dell'elemento di metadati, ad esempio l'ID della risorsa per un elemento di metadati di risorsa incorporata.

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


Imposta una categoria dell'elemento di metadati, ad esempio l'ID della risorsa per un elemento di metadati di risorsa incorporata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String | Una categoria dell'elemento di metadati, ad esempio l'ID della risorsa per un elemento di metadati di risorsa incorporata. |
|

### getFilter() {#getFilter--}
```
public final int getFilter()
```


Ottiene un valore di
MetadataFilters
, assegnato a questo elemento di metadati che è usato nella filtrazione degli elementi.


**Returns:**
int - Un valore di  MetadataFilters , assegnato a questo elemento di metadati che è usato nella filtrazione degli elementi.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Imposta un valore di
MetadataFilters
, assegnato a questo elemento di metadati che è usato nella filtrazione degli elementi.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Un valore di  MetadataFilters , assegnato a questo elemento di metadati che è usato nella filtrazione degli elementi. |
|

### getValues() {#getValues--}
```
public final List<String> getValues()
```


Ottiene il valore dell'elemento di metadati.


**Returns:**
java.util.List<java.lang.String> - Il valore dell'elemento di metadati.

### setValues(List<String> value) {#setValues-java.util.List-java.lang.String--}
```
public final void setValues(List<String> value)
```


Imposta il valore dell'elemento di metadati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.util.List<java.lang.String> | Il valore dell'elemento di metadati. |
|

### isCustom() {#isCustom--}
```
public final boolean isCustom()
```


Ottiene un valore che indica se questo elemento è personalizzato (aggiunto dagli autori del documento).


**Returns:**
boolean - Un valore che indica se questo elemento è personalizzato (aggiunto dagli autori del documento).

### setCustom(boolean value) {#setCustom-boolean-}
```
public final void setCustom(boolean value)
```


Imposta un valore che indica se questo elemento è personalizzato (aggiunto dagli autori del documento).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se questo elemento è personalizzato (aggiunto dagli autori del documento). |
|

### getDictionaryKey() {#getDictionaryKey--}
```
public String getDictionaryKey()
```


Ottiene una chiave di dizionario per , usando il suo OriginalName e altri dati.


**Returns:**
java.lang.String - Una chiave di dizionario per , usando il suo OriginalName e altri dati.

### createClone() {#createClone--}
```
public MetadataItem createClone()
```


Crea una copia profonda dell'istanza corrente.


**Returns:**
[MetadataItem](../../com.groupdocs.redaction.integration/metadataitem) - Object clone

### getActualValue() {#getActualValue--}
```
public final String getActualValue()
```


Ottiene la rappresentazione stringa del valore dell'elemento di metadati.


**Returns:**
java.lang.String - La rappresentazione stringa del valore dell'elemento di metadati.

