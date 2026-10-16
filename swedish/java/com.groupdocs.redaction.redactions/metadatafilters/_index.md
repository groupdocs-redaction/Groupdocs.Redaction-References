---
title: "MetadataFilters"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar en lista över de vanligaste typerna av dokumentmetadata."
type: docs
weight: 19
url: /sv/java/com.groupdocs.redaction.redactions/metadatafilters/
---
**Inheritance:**
java.lang.Object
```
public final class MetadataFilters
```

Representerar en lista över de vanligaste typerna av dokumentmetadata.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [MetadataFilters()](#MetadataFilters--) |  |
## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [None](#None) | Tom filterinställning, matchar inga metadataobjekt. |
|
|  | [Author](#Author) | Författare till dokumentet. |
|
|  | [Category](#Category) | Kategori för dokumentet. |
|
|  | [Comments](#Comments) | Kommentar för dokumentet. |
|
|  | [Company](#Company) | Företag för författaren. |
|
|  | [ContentStatus](#ContentStatus) | Innehållsstatus. |
|
|  | [CreatedTime](#CreatedTime) | Skapad tid. |
|
|  | [HyperlinkBase](#HyperlinkBase) | Hyperlänkbas. |
|
|  | [LastPrinted](#LastPrinted) | Senast utskrivna datum och tid. |
|
|  | [LastSavedBy](#LastSavedBy) | Senast sparad av användare. |
|
|  | [LastSavedTime](#LastSavedTime) | Senast sparade datum och tid. |
|
|  | [NameOfApplication](#NameOfApplication) | Namn på programmet där dokumentet skapades. |
|
|  | [Manager](#Manager) | Författarens chefsnamn. |
|
|  | [RevisionNumber](#RevisionNumber) | Revisionsnummer. |
|
|  | [Subject](#Subject) | Ämne för dokumentet. |
|
|  | [Template](#Template) | Dokumentmallens namn. |
|
|  | [Title](#Title) | Dokumenttitel. |
|
|  | [TotalEditingTime](#TotalEditingTime) | Total redigeringstid. |
|
|  | [Version](#Version) | Dokumentets version. |
|
|  | [Description](#Description) | Dokumentets beskrivning. |
|
|  | [Keywords](#Keywords) | Dokumentets nyckelord. |
|
|  | [ContentType](#ContentType) | Innehållstyp. |
|
|  | [All](#All) | Alla typer av metadataobjekt. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getNames()](#getNames--) | Hämtar en uppsättning med alla deklarerade filtertyper. |
|
|  | [getValueByName(String valueName)](#getValueByName-java.lang.String-) | Hämtar värdet av MetadataFiler efter dess namn. |
|
|  | [parse(String values)](#parse-java.lang.String-) | Tolkar en sträng med kommaseparerade MetadataFilers‑värden till ett heltal. |
|
|  | [toString(int value)](#toString-int-) | Sparar ett heltal som en sträng med kommaseparerade MetadataFilers-värden. |
|
### MetadataFilters() {#MetadataFilters--}
```
public MetadataFilters()
```


### None {#None}
```
public static final int None
```


Tom filterinställning, matchar inga metadataobjekt.


### Author {#Author}
```
public static final int Author
```


Författare till dokumentet.


### Category {#Category}
```
public static final int Category
```


Kategori för dokumentet.


### Comments {#Comments}
```
public static final int Comments
```


Kommentar för dokumentet.


### Company {#Company}
```
public static final int Company
```


Företag för författaren.


### ContentStatus {#ContentStatus}
```
public static final int ContentStatus
```


Innehållsstatus.


### CreatedTime {#CreatedTime}
```
public static final int CreatedTime
```


Skapad tid.


### HyperlinkBase {#HyperlinkBase}
```
public static final int HyperlinkBase
```


Hyperlänkbas.


### LastPrinted {#LastPrinted}
```
public static final int LastPrinted
```


Senast utskrivna datum och tid.


### LastSavedBy {#LastSavedBy}
```
public static final int LastSavedBy
```


Senast sparad av användare.


### LastSavedTime {#LastSavedTime}
```
public static final int LastSavedTime
```


Senast sparade datum och tid.


### NameOfApplication {#NameOfApplication}
```
public static final int NameOfApplication
```


Namn på programmet där dokumentet skapades.


### Manager {#Manager}
```
public static final int Manager
```


Författarens chefsnamn.


### RevisionNumber {#RevisionNumber}
```
public static final int RevisionNumber
```


Revisionsnummer.


### Subject {#Subject}
```
public static final int Subject
```


Ämne för dokumentet.


### Template {#Template}
```
public static final int Template
```


Dokumentmallens namn.


### Title {#Title}
```
public static final int Title
```


Dokumenttitel.


### TotalEditingTime {#TotalEditingTime}
```
public static final int TotalEditingTime
```


Total redigeringstid.


### Version {#Version}
```
public static final int Version
```


Dokumentets version.


### Description {#Description}
```
public static final int Description
```


Dokumentets beskrivning.


### Keywords {#Keywords}
```
public static final int Keywords
```


Dokumentets nyckelord.


### ContentType {#ContentType}
```
public static final int ContentType
```


Innehållstyp.


### All {#All}
```
public static final int All
```


Alla typer av metadataobjekt.


### getNames() {#getNames--}
```
public static Set<String> getNames()
```


Hämtar en uppsättning med alla deklarerade filtertyper.


**Returns:**
java.util.Set<java.lang.String> - En uppsättning med alla deklarerade filtertyper.

### getValueByName(String valueName) {#getValueByName-java.lang.String-}
```
public static int getValueByName(String valueName)
```


Hämtar värdet av MetadataFiler efter dess namn.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | valueName | java.lang.String | Namn på MetadataFilter. |
|

**Returns:**
int - Värde för MetadataFiler.

### parse(String values) {#parse-java.lang.String-}
```
public static int parse(String values)
```


Tolkar en sträng med kommaseparerade MetadataFilers‑värden till ett heltal.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | values | java.lang.String | En sträng med kommaseparerade MetadataFilers-värden. |
|

**Returns:**
int - Värde för MetadataFilers.

### toString(int value) {#toString-int-}
```
public static String toString(int value)
```


Sparar ett heltal som en sträng med kommaseparerade MetadataFilers-värden.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Värde för MetadataFiler. |
|

**Returns:**
java.lang.String - En sträng med kommaseparerade MetadataFiler-värden.

