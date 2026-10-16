---
title: "MetadataFilters"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt eine Liste der gebräuchlichsten Arten von Dokumenten‑Metadaten dar."
type: docs
weight: 19
url: /de/java/com.groupdocs.redaction.redactions/metadatafilters/
---
**Inheritance:**
java.lang.Object
```
public final class MetadataFilters
```

Stellt eine Liste der gebräuchlichsten Arten von Dokumenten‑Metadaten dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [MetadataFilters()](#MetadataFilters--) |  |
## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [None](#None) | Leere Filtereinstellung, trifft auf keine Metadaten-Elemente zu. |
|
|  | [Author](#Author) | Autor des Dokuments. |
|
|  | [Category](#Category) | Kategorie des Dokuments. |
|
|  | [Comments](#Comments) | Kommentar zum Dokument. |
|
|  | [Company](#Company) | Firma des Autors. |
|
|  | [ContentStatus](#ContentStatus) | Inhaltsstatus. |
|
|  | [CreatedTime](#CreatedTime) | Erstellungszeit. |
|
|  | [HyperlinkBase](#HyperlinkBase) | Hyperlink-Basis. |
|
|  | [LastPrinted](#LastPrinted) | Datum und Uhrzeit des letzten Drucks. |
|
|  | [LastSavedBy](#LastSavedBy) | Zuletzt gespeichert von Benutzer. |
|
|  | [LastSavedTime](#LastSavedTime) | Datum und Uhrzeit der letzten Speicherung. |
|
|  | [NameOfApplication](#NameOfApplication) | Name der Anwendung, in der das Dokument erstellt wurde. |
|
|  | [Manager](#Manager) | Name des Vorgesetzten des Autors. |
|
|  | [RevisionNumber](#RevisionNumber) | Revisionsnummer. |
|
|  | [Subject](#Subject) | Betreff des Dokuments. |
|
|  | [Template](#Template) | Name der Dokumentvorlage. |
|
|  | [Title](#Title) | Dokumenttitel. |
|
|  | [TotalEditingTime](#TotalEditingTime) | Gesamte Bearbeitungszeit. |
|
|  | [Version](#Version) | Version des Dokuments. |
|
|  | [Description](#Description) | Beschreibung des Dokuments. |
|
|  | [Keywords](#Keywords) | Schlüsselwörter des Dokuments. |
|
|  | [ContentType](#ContentType) | Inhaltstyp. |
|
|  | [All](#All) | Alle Typen der Metadaten-Elemente. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getNames()](#getNames--) | Ruft ein Set mit allen deklarierten Filtertypen ab. |
|
|  | [getValueByName(String valueName)](#getValueByName-java.lang.String-) | Ruft den Wert von MetadataFiler anhand seines Namens ab. |
|
|  | [parse(String values)](#parse-java.lang.String-) | Parst eine durch Kommas getrennte Zeichenkette von MetadataFilers-Werten in einen int. |
|
|  | [toString(int value)](#toString-int-) | Speichert einen Integer als Zeichenkette von durch Kommas getrennten MetadataFilers-Werten. |
|
### MetadataFilters() {#MetadataFilters--}
```
public MetadataFilters()
```


### None {#None}
```
public static final int None
```


Leere Filtereinstellung, trifft auf keine Metadaten-Elemente zu.


### Author {#Author}
```
public static final int Author
```


Autor des Dokuments.


### Category {#Category}
```
public static final int Category
```


Kategorie des Dokuments.


### Comments {#Comments}
```
public static final int Comments
```


Kommentar zum Dokument.


### Company {#Company}
```
public static final int Company
```


Firma des Autors.


### ContentStatus {#ContentStatus}
```
public static final int ContentStatus
```


Inhaltsstatus.


### CreatedTime {#CreatedTime}
```
public static final int CreatedTime
```


Erstellungszeit.


### HyperlinkBase {#HyperlinkBase}
```
public static final int HyperlinkBase
```


Hyperlink-Basis.


### LastPrinted {#LastPrinted}
```
public static final int LastPrinted
```


Datum und Uhrzeit des letzten Drucks.


### LastSavedBy {#LastSavedBy}
```
public static final int LastSavedBy
```


Zuletzt gespeichert von Benutzer.


### LastSavedTime {#LastSavedTime}
```
public static final int LastSavedTime
```


Datum und Uhrzeit der letzten Speicherung.


### NameOfApplication {#NameOfApplication}
```
public static final int NameOfApplication
```


Name der Anwendung, in der das Dokument erstellt wurde.


### Manager {#Manager}
```
public static final int Manager
```


Name des Vorgesetzten des Autors.


### RevisionNumber {#RevisionNumber}
```
public static final int RevisionNumber
```


Revisionsnummer.


### Subject {#Subject}
```
public static final int Subject
```


Betreff des Dokuments.


### Template {#Template}
```
public static final int Template
```


Name der Dokumentvorlage.


### Title {#Title}
```
public static final int Title
```


Dokumenttitel.


### TotalEditingTime {#TotalEditingTime}
```
public static final int TotalEditingTime
```


Gesamte Bearbeitungszeit.


### Version {#Version}
```
public static final int Version
```


Version des Dokuments.


### Description {#Description}
```
public static final int Description
```


Beschreibung des Dokuments.


### Keywords {#Keywords}
```
public static final int Keywords
```


Schlüsselwörter des Dokuments.


### ContentType {#ContentType}
```
public static final int ContentType
```


Inhaltstyp.


### All {#All}
```
public static final int All
```


Alle Typen der Metadaten-Elemente.


### getNames() {#getNames--}
```
public static Set<String> getNames()
```


Ruft ein Set mit allen deklarierten Filtertypen ab.


**Returns:**
java.util.Set<java.lang.String> - Ein Set mit allen deklarierten Filtertypen.

### getValueByName(String valueName) {#getValueByName-java.lang.String-}
```
public static int getValueByName(String valueName)
```


Ruft den Wert von MetadataFiler anhand seines Namens ab.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | valueName | java.lang.String | Name des MetadataFilter. |
|

**Returns:**
int - Wert von MetadataFiler.

### parse(String values) {#parse-java.lang.String-}
```
public static int parse(String values)
```


Parst eine durch Kommas getrennte Zeichenkette von MetadataFilers-Werten in einen int.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Werte | java.lang.String | Eine Zeichenkette von durch Kommas getrennten MetadataFilers-Werten. |
|

**Returns:**
int - Wert von MetadataFilers.

### toString(int value) {#toString-int-}
```
public static String toString(int value)
```


Speichert einen Integer als Zeichenkette von durch Kommas getrennten MetadataFilers-Werten.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Wert von MetadataFiler. |
|

**Returns:**
java.lang.String - Eine Zeichenkette von durch Kommas getrennten MetadataFiler-Werten.

