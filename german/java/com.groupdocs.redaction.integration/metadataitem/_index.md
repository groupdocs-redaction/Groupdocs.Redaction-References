---
title: "MetadataItem"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt ein Metadaten-Element dar, das für alle unterstützten Formate gemeinsam ist und bei Metadaten-Redaktionen verwendet wird."
type: docs
weight: 12
url: /de/java/com.groupdocs.redaction.integration/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Stellt ein Metadaten-Element dar, das für alle unterstützten Formate gemeinsam ist und bei Metadaten-Redaktionen verwendet wird.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [MetadataItem()](#MetadataItem--) | Initialisiert eine neue Instanz. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getOriginalName()](#getOriginalName--) | Liefert den Originalnamen des Metadaten-Elements, wie er im Dokument erscheint. |
|
|  | [setOriginalName(String value)](#setOriginalName-java.lang.String-) | Setzt den Originalnamen des Metadaten-Elements, wie er im Dokument erscheint. |
|
|  | [getCategory()](#getCategory--) | Liefert die Kategorie des Metadaten-Elements, zum Beispiel Ressourcen-ID für ein eingebettetes Ressourcen-Metadaten-Element. |
|
|  | [setCategory(String value)](#setCategory-java.lang.String-) | Setzt die Kategorie des Metadaten-Elements, zum Beispiel Ressourcen-ID für ein eingebettetes Ressourcen-Metadaten-Element. |
|
|  | [getFilter()](#getFilter--) | Liefert einen Wert von |
MetadataFilters
, zugewiesen zu diesem Metadaten-Element, das bei der Elementfilterung verwendet wird.
|
|  | [setFilter(int value)](#setFilter-int-) | Setzt einen Wert von |
MetadataFilters
, zugewiesen zu diesem Metadaten-Element, das bei der Elementfilterung verwendet wird.
|
|  | [getValues()](#getValues--) | Liefert den Wert des Metadaten-Elements. |
|
|  | [setValues(List<String> value)](#setValues-java.util.List-java.lang.String--) | Setzt den Wert des Metadaten-Elements. |
|
|  | [isCustom()](#isCustom--) | Liefert einen Wert, der angibt, ob dieses Element benutzerdefiniert ist (von den Autoren des Dokuments hinzugefügt). |
|
|  | [setCustom(boolean value)](#setCustom-boolean-) | Setzt einen Wert, der angibt, ob dieses Element benutzerdefiniert ist (von den Autoren des Dokuments hinzugefügt). |
|
|  | [getDictionaryKey()](#getDictionaryKey--) | Liefert einen Wörterbuchschlüssel für , unter Verwendung seines Originalnamens und anderer Daten. |
|
|  | [createClone()](#createClone--) | Erstellt einen tiefen Klon der aktuellen Instanz. |
|
|  | [getActualValue()](#getActualValue--) | Liefert die String-Darstellung des Werts des Metadaten-Elements. |
|
### MetadataItem() {#MetadataItem--}
```
public MetadataItem()
```


Initialisiert eine neue Instanz.


### getOriginalName() {#getOriginalName--}
```
public final String getOriginalName()
```


Liefert den Originalnamen des Metadaten-Elements, wie er im Dokument erscheint.


**Returns:**
java.lang.String - Ein Originalname des Metadaten-Elements, wie er im Dokument erscheint.

### setOriginalName(String value) {#setOriginalName-java.lang.String-}
```
public final void setOriginalName(String value)
```


Setzt den Originalnamen des Metadaten-Elements, wie er im Dokument erscheint.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String | Ein Originalname des Metadaten-Elements, wie er im Dokument erscheint. |
|

### getCategory() {#getCategory--}
```
public final String getCategory()
```


Liefert die Kategorie des Metadaten-Elements, zum Beispiel Ressourcen-ID für ein eingebettetes Ressourcen-Metadaten-Element.


**Returns:**
java.lang.String - Eine Kategorie des Metadaten-Elements, zum Beispiel Ressourcen-ID für ein eingebettetes Ressourcen-Metadaten-Element.

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


Setzt die Kategorie des Metadaten-Elements, zum Beispiel Ressourcen-ID für ein eingebettetes Ressourcen-Metadaten-Element.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String | Eine Kategorie des Metadaten-Elements, zum Beispiel Ressourcen-ID für ein eingebettetes Ressourcen-Metadaten-Element. |
|

### getFilter() {#getFilter--}
```
public final int getFilter()
```


Liefert einen Wert von
MetadataFilters
, zugewiesen zu diesem Metadaten-Element, das bei der Elementfilterung verwendet wird.


**Returns:**
int - Ein Wert von MetadataFilters, zugewiesen zu diesem Metadaten-Element, das bei der Elementfilterung verwendet wird.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Setzt einen Wert von
MetadataFilters
, zugewiesen zu diesem Metadaten-Element, das bei der Elementfilterung verwendet wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Ein Wert von MetadataFilters, zugewiesen zu diesem Metadaten-Element, das bei der Elementfilterung verwendet wird. |
|

### getValues() {#getValues--}
```
public final List<String> getValues()
```


Liefert den Wert des Metadaten-Elements.


**Returns:**
java.util.List<java.lang.String> - Der Wert des Metadaten-Elements.

### setValues(List<String> value) {#setValues-java.util.List-java.lang.String--}
```
public final void setValues(List<String> value)
```


Setzt den Wert des Metadaten-Elements.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.util.List<java.lang.String> | Der Wert des Metadaten-Elements. |
|

### isCustom() {#isCustom--}
```
public final boolean isCustom()
```


Liefert einen Wert, der angibt, ob dieses Element benutzerdefiniert ist (von den Autoren des Dokuments hinzugefügt).


**Returns:**
boolean - Ein Wert, der angibt, ob dieses Element benutzerdefiniert ist (von den Autoren des Dokuments hinzugefügt).

### setCustom(boolean value) {#setCustom-boolean-}
```
public final void setCustom(boolean value)
```


Setzt einen Wert, der angibt, ob dieses Element benutzerdefiniert ist (von den Autoren des Dokuments hinzugefügt).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob dieses Element benutzerdefiniert ist (von den Autoren des Dokuments hinzugefügt). |
|

### getDictionaryKey() {#getDictionaryKey--}
```
public String getDictionaryKey()
```


Liefert einen Wörterbuchschlüssel für , unter Verwendung seines Originalnamens und anderer Daten.


**Returns:**
java.lang.String - Ein Wörterbuchschlüssel für , unter Verwendung seines OriginalName und anderer Daten.

### createClone() {#createClone--}
```
public MetadataItem createClone()
```


Erstellt einen tiefen Klon der aktuellen Instanz.


**Returns:**
[MetadataItem](../../com.groupdocs.redaction.integration/metadataitem) - Object clone

### getActualValue() {#getActualValue--}
```
public final String getActualValue()
```


Liefert die String-Darstellung des Werts des Metadaten-Elements.


**Returns:**
java.lang.String - Die String-Darstellung des Wertes des Metadaten-Elements.

