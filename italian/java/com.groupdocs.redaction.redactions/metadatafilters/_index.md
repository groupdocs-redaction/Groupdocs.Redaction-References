---
title: "MetadataFilters"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta un elenco dei tipi di metadati di documento più comuni."
type: docs
weight: 19
url: /it/java/com.groupdocs.redaction.redactions/metadatafilters/
---
**Inheritance:**
java.lang.Object
```
public final class MetadataFilters
```

Rappresenta un elenco dei tipi di metadati di documento più comuni.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [MetadataFilters()](#MetadataFilters--) |  |
## Campi

| Campo | Descrizione |
| --- | --- |
|  | [None](#None) | Impostazione filtro vuoto, non corrisponde a nessun elemento di metadati. |
|
|  | [Author](#Author) | Autore del documento. |
|
|  | [Category](#Category) | Categoria del documento. |
|
|  | [Comments](#Comments) | Commento per il documento. |
|
|  | [Company](#Company) | Azienda dell'Autore. |
|
|  | [ContentStatus](#ContentStatus) | Stato del contenuto. |
|
|  | [CreatedTime](#CreatedTime) | Ora di creazione. |
|
|  | [HyperlinkBase](#HyperlinkBase) | Base del collegamento ipertestuale. |
|
|  | [LastPrinted](#LastPrinted) | Data e ora dell'ultima stampa. |
|
|  | [LastSavedBy](#LastSavedBy) | Ultimo salvataggio da parte dell'utente. |
|
|  | [LastSavedTime](#LastSavedTime) | Data e ora dell'ultimo salvataggio. |
|
|  | [NameOfApplication](#NameOfApplication) | Nome dell'applicazione in cui è stato creato il documento. |
|
|  | [Manager](#Manager) | Nome del responsabile dell'autore. |
|
|  | [RevisionNumber](#RevisionNumber) | Numero di revisione. |
|
|  | [Subject](#Subject) | Oggetto del documento. |
|
|  | [Template](#Template) | Nome del modello del documento. |
|
|  | [Title](#Title) | Titolo del documento. |
|
|  | [TotalEditingTime](#TotalEditingTime) | Tempo totale di modifica. |
|
|  | [Version](#Version) | Versione del documento. |
|
|  | [Description](#Description) | Descrizione del documento. |
|
|  | [Keywords](#Keywords) | Parole chiave del documento. |
|
|  | [ContentType](#ContentType) | Tipo di contenuto. |
|
|  | [All](#All) | Tutti i tipi degli elementi di metadati. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getNames()](#getNames--) | Restituisce un insieme con tutti i tipi di filtro dichiarati. |
|
|  | [getValueByName(String valueName)](#getValueByName-java.lang.String-) | Restituisce il valore di MetadataFiler per il suo nome. |
|
|  | [parse(String values)](#parse-java.lang.String-) | Analizza una stringa di valori di MetadataFilers delimitati da virgole in un intero. |
|
|  | [toString(int value)](#toString-int-) | Salva un intero come una stringa di valori di MetadataFilers delimitati da virgole. |
|
### MetadataFilters() {#MetadataFilters--}
```
public MetadataFilters()
```


### None {#None}
```
public static final int None
```


Impostazione filtro vuoto, non corrisponde a nessun elemento di metadati.


### Author {#Author}
```
public static final int Author
```


Autore del documento.


### Category {#Category}
```
public static final int Category
```


Categoria del documento.


### Comments {#Comments}
```
public static final int Comments
```


Commento per il documento.


### Company {#Company}
```
public static final int Company
```


Azienda dell'Autore.


### ContentStatus {#ContentStatus}
```
public static final int ContentStatus
```


Stato del contenuto.


### CreatedTime {#CreatedTime}
```
public static final int CreatedTime
```


Ora di creazione.


### HyperlinkBase {#HyperlinkBase}
```
public static final int HyperlinkBase
```


Base del collegamento ipertestuale.


### LastPrinted {#LastPrinted}
```
public static final int LastPrinted
```


Data e ora dell'ultima stampa.


### LastSavedBy {#LastSavedBy}
```
public static final int LastSavedBy
```


Ultimo salvataggio da parte dell'utente.


### LastSavedTime {#LastSavedTime}
```
public static final int LastSavedTime
```


Data e ora dell'ultimo salvataggio.


### NameOfApplication {#NameOfApplication}
```
public static final int NameOfApplication
```


Nome dell'applicazione in cui è stato creato il documento.


### Manager {#Manager}
```
public static final int Manager
```


Nome del responsabile dell'autore.


### RevisionNumber {#RevisionNumber}
```
public static final int RevisionNumber
```


Numero di revisione.


### Subject {#Subject}
```
public static final int Subject
```


Oggetto del documento.


### Template {#Template}
```
public static final int Template
```


Nome del modello del documento.


### Title {#Title}
```
public static final int Title
```


Titolo del documento.


### TotalEditingTime {#TotalEditingTime}
```
public static final int TotalEditingTime
```


Tempo totale di modifica.


### Version {#Version}
```
public static final int Version
```


Versione del documento.


### Description {#Description}
```
public static final int Description
```


Descrizione del documento.


### Keywords {#Keywords}
```
public static final int Keywords
```


Parole chiave del documento.


### ContentType {#ContentType}
```
public static final int ContentType
```


Tipo di contenuto.


### All {#All}
```
public static final int All
```


Tutti i tipi degli elementi di metadati.


### getNames() {#getNames--}
```
public static Set<String> getNames()
```


Restituisce un insieme con tutti i tipi di filtro dichiarati.


**Returns:**
java.util.Set<java.lang.String> - Un insieme con tutti i tipi di filtro dichiarati.

### getValueByName(String valueName) {#getValueByName-java.lang.String-}
```
public static int getValueByName(String valueName)
```


Restituisce il valore di MetadataFiler per il suo nome.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valueName | java.lang.String | Nome di MetadataFilter. |
|

**Returns:**
int - Valore di MetadataFiler.

### parse(String values) {#parse-java.lang.String-}
```
public static int parse(String values)
```


Analizza una stringa di valori di MetadataFilers delimitati da virgole in un intero.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valori | java.lang.String | Una stringa di valori di MetadataFilers delimitati da virgole. |
|

**Returns:**
int - Valore di MetadataFilers.

### toString(int value) {#toString-int-}
```
public static String toString(int value)
```


Salva un intero come una stringa di valori di MetadataFilers delimitati da virgole.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Valore di MetadataFiler. |
|

**Returns:**
java.lang.String - Una stringa di valori di MetadataFiler delimitati da virgole.

