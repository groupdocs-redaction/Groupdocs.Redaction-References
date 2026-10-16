---
title: "PageRangeFilter"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt die Einstellung des Seitenbereichs für den Redaktionsfilter in einem Dokument dar, auf die die Redaktion angewendet wird."
type: docs
weight: 24
url: /de/java/com.groupdocs.redaction.redactions/pagerangefilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageRangeFilter extends RedactionFilter
```

Stellt einen Redaktionsfilter dar, der einen Seitenbereich innerhalb eines Dokuments festlegt, in dem die Redaktion angewendet wird.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [PageRangeFilter(PageSeekOrigin origin, int index, int count)](#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-) | Initialisiert eine neue Instanz der Klasse RemovePageRedaction. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getOrigin()](#getOrigin--) | Liefert die Referenzposition für das Suchen, den Anfang oder das Ende eines Dokuments. |
|
|  | [getIndex()](#getIndex--) | Liefert den Startpositionsindex (0-basiert). |
|
|  | [getCount()](#getCount--) | Liefert die Anzahl der zu entfernenden Seiten. |
|
|  | [isPageInRange(int pageIndex, int pageCount)](#isPageInRange-int-int-) | Überprüft, ob dieser Filterseitenbereich die angegebene Seite enthält. |
|
### PageRangeFilter(PageSeekOrigin origin, int index, int count) {#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-}
```
public PageRangeFilter(PageSeekOrigin origin, int index, int count)
```


Initialisiert eine neue Instanz der Klasse RemovePageRedaction.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | origin | [PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) | Referenzposition für das Suchen, der Anfang oder das Ende eines Dokuments |
|
|  | Index | int | Startpositionsindex (0-basiert) |
|
|  | Anzahl | int | Anzahl der zu entfernenden Seiten |
|

### getOrigin() {#getOrigin--}
```
public final PageSeekOrigin getOrigin()
```


Liefert die Referenzposition für das Suchen, den Anfang oder das Ende eines Dokuments.


**Returns:**
[PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) - Seek reference position, the beginning or the end of a document.

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Liefert den Startpositionsindex (0-basiert).


**Returns:**
int – Startpositionsindex (0-basiert).

### getCount() {#getCount--}
```
public final int getCount()
```


Liefert die Anzahl der zu entfernenden Seiten.


**Returns:**
int – Die Anzahl der zu entfernenden Seiten.

### isPageInRange(int pageIndex, int pageCount) {#isPageInRange-int-int-}
```
public final boolean isPageInRange(int pageIndex, int pageCount)
```


Überprüft, ob dieser Filterseitenbereich die angegebene Seite enthält.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Index der Seite (nullbasiert) |
|
|  | pageCount | int | Gesamtseitenanzahl |
|

**Returns:**
boolean – true, wenn dieser Filterbereich die Seite enthält

