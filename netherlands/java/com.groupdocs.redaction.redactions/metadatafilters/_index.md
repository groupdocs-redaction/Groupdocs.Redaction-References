---
title: "MetadataFilters"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt een lijst voor van de meest voorkomende typen documentmetadata."
type: docs
weight: 19
url: /nl/java/com.groupdocs.redaction.redactions/metadatafilters/
---
**Inheritance:**
java.lang.Object
```
public final class MetadataFilters
```

Stelt een lijst voor van de meest voorkomende typen documentmetadata.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [MetadataFilters()](#MetadataFilters--) |  |
## Velden

| Veld | Beschrijving |
| --- | --- |
|  | [None](#None) | Lege filterinstelling, komt niet overeen met metadata‑items. |
|
|  | [Author](#Author) | Auteur van het document. |
|
|  | [Category](#Category) | Categorie van het document. |
|
|  | [Comments](#Comments) | Opmerking voor het document. |
|
|  | [Company](#Company) | Bedrijf van de auteur. |
|
|  | [ContentStatus](#ContentStatus) | Inhoudstatus. |
|
|  | [CreatedTime](#CreatedTime) | Aanmaaktijd. |
|
|  | [HyperlinkBase](#HyperlinkBase) | Hyperlinkbasis. |
|
|  | [LastPrinted](#LastPrinted) | Datum en tijd van laatste afdruk. |
|
|  | [LastSavedBy](#LastSavedBy) | Laatst opgeslagen door gebruiker. |
|
|  | [LastSavedTime](#LastSavedTime) | Datum en tijd van laatste opslaan. |
|
|  | [NameOfApplication](#NameOfApplication) | Naam van de applicatie waarin het document is gemaakt. |
|
|  | [Manager](#Manager) | Naam van de manager van de auteur. |
|
|  | [RevisionNumber](#RevisionNumber) | Revisienummer. |
|
|  | [Subject](#Subject) | Onderwerp van het document. |
|
|  | [Template](#Template) | Naam van het documentsjabloon. |
|
|  | [Title](#Title) | Documenttitel. |
|
|  | [TotalEditingTime](#TotalEditingTime) | Totale bewerkingstijd. |
|
|  | [Version](#Version) | Versie van het document. |
|
|  | [Description](#Description) | Beschrijving van het document. |
|
|  | [Keywords](#Keywords) | Trefwoorden van het document. |
|
|  | [ContentType](#ContentType) | Inhoudstype. |
|
|  | [All](#All) | Alle typen metadata-items. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getNames()](#getNames--) | Haalt een set op met alle gedeclareerde filtertypen. |
|
|  | [getValueByName(String valueName)](#getValueByName-java.lang.String-) | Haalt de waarde van MetadataFiler op op basis van de naam. |
|
|  | [parse(String values)](#parse-java.lang.String-) | Parseert een door komma's gescheiden tekenreeks van MetadataFiler-waarden naar een int. |
|
|  | [toString(int value)](#toString-int-) | Slaat een geheel getal op als een tekenreeks van door komma's gescheiden MetadataFilers-waarden. |
|
### MetadataFilters() {#MetadataFilters--}
```
public MetadataFilters()
```


### None {#None}
```
public static final int None
```


Lege filterinstelling, komt niet overeen met metadata‑items.


### Author {#Author}
```
public static final int Author
```


Auteur van het document.


### Category {#Category}
```
public static final int Category
```


Categorie van het document.


### Comments {#Comments}
```
public static final int Comments
```


Opmerking voor het document.


### Company {#Company}
```
public static final int Company
```


Bedrijf van de auteur.


### ContentStatus {#ContentStatus}
```
public static final int ContentStatus
```


Inhoudstatus.


### CreatedTime {#CreatedTime}
```
public static final int CreatedTime
```


Aanmaaktijd.


### HyperlinkBase {#HyperlinkBase}
```
public static final int HyperlinkBase
```


Hyperlinkbasis.


### LastPrinted {#LastPrinted}
```
public static final int LastPrinted
```


Datum en tijd van laatste afdruk.


### LastSavedBy {#LastSavedBy}
```
public static final int LastSavedBy
```


Laatst opgeslagen door gebruiker.


### LastSavedTime {#LastSavedTime}
```
public static final int LastSavedTime
```


Datum en tijd van laatste opslaan.


### NameOfApplication {#NameOfApplication}
```
public static final int NameOfApplication
```


Naam van de applicatie waarin het document is gemaakt.


### Manager {#Manager}
```
public static final int Manager
```


Naam van de manager van de auteur.


### RevisionNumber {#RevisionNumber}
```
public static final int RevisionNumber
```


Revisienummer.


### Subject {#Subject}
```
public static final int Subject
```


Onderwerp van het document.


### Template {#Template}
```
public static final int Template
```


Naam van het documentsjabloon.


### Title {#Title}
```
public static final int Title
```


Documenttitel.


### TotalEditingTime {#TotalEditingTime}
```
public static final int TotalEditingTime
```


Totale bewerkingstijd.


### Version {#Version}
```
public static final int Version
```


Versie van het document.


### Description {#Description}
```
public static final int Description
```


Beschrijving van het document.


### Keywords {#Keywords}
```
public static final int Keywords
```


Trefwoorden van het document.


### ContentType {#ContentType}
```
public static final int ContentType
```


Inhoudstype.


### All {#All}
```
public static final int All
```


Alle typen metadata-items.


### getNames() {#getNames--}
```
public static Set<String> getNames()
```


Haalt een set op met alle gedeclareerde filtertypen.


**Returns:**
java.util.Set<java.lang.String> - Een set met alle gedeclareerde filtertypen.

### getValueByName(String valueName) {#getValueByName-java.lang.String-}
```
public static int getValueByName(String valueName)
```


Haalt de waarde van MetadataFiler op op basis van de naam.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | valueName | java.lang.String | Naam van MetadataFilter. |
|

**Returns:**
int - Waarde van MetadataFiler.

### parse(String values) {#parse-java.lang.String-}
```
public static int parse(String values)
```


Parseert een door komma's gescheiden tekenreeks van MetadataFiler-waarden naar een int.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarden | java.lang.String | Een tekenreeks van door komma's gescheiden MetadataFilers-waarden. |
|

**Returns:**
int - Waarde van MetadataFilers.

### toString(int value) {#toString-int-}
```
public static String toString(int value)
```


Slaat een geheel getal op als een tekenreeks van door komma's gescheiden MetadataFilers-waarden.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Waarde van MetadataFiler. |
|

**Returns:**
java.lang.String - Een tekenreeks van door komma's gescheiden MetadataFiler-waarden.

