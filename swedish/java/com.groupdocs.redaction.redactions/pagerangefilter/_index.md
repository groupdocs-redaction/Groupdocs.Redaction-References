---
title: "PageRangeFilter"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar redigeringsfilter som anger sidintervall i ett dokument för att tillämpa redigering."
type: docs
weight: 24
url: /sv/java/com.groupdocs.redaction.redactions/pagerangefilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageRangeFilter extends RedactionFilter
```

Representerar ett redigeringsfilter som anger sidintervall i ett dokument för att tillämpa redigering.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [PageRangeFilter(PageSeekOrigin origin, int index, int count)](#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-) | Initierar en ny instans av klassen RemovePageRedaction. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getOrigin()](#getOrigin--) | Hämtar sökreferensposition, början eller slutet av ett dokument. |
|
|  | [getIndex()](#getIndex--) | Hämtar startpositionsindex (0-baserat). |
|
|  | [getCount()](#getCount--) | Hämtar antalet sidor som ska tas bort. |
|
|  | [isPageInRange(int pageIndex, int pageCount)](#isPageInRange-int-int-) | Kontrollerar om detta filtersidintervall innehåller den angivna sidan. |
|
### PageRangeFilter(PageSeekOrigin origin, int index, int count) {#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-}
```
public PageRangeFilter(PageSeekOrigin origin, int index, int count)
```


Initierar en ny instans av klassen RemovePageRedaction.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | origin | [PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) | Sökreferensposition, början eller slutet av ett dokument |
|
|  | index | int | Startpositionsindex (0-baserat) |
|
|  | antal | int | Antal sidor att ta bort |
|

### getOrigin() {#getOrigin--}
```
public final PageSeekOrigin getOrigin()
```


Hämtar sökreferensposition, början eller slutet av ett dokument.


**Returns:**
[PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) - Seek reference position, the beginning or the end of a document.

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Hämtar startpositionsindex (0-baserat).


**Returns:**
int - Startpositionsindex (0-baserad).

### getCount() {#getCount--}
```
public final int getCount()
```


Hämtar antalet sidor som ska tas bort.


**Returns:**
int - Antalet sidor att ta bort.

### isPageInRange(int pageIndex, int pageCount) {#isPageInRange-int-int-}
```
public final boolean isPageInRange(int pageIndex, int pageCount)
```


Kontrollerar om detta filtersidintervall innehåller den angivna sidan.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | index för sidan (nollbaserad) |
|
|  | pageCount | int | totalt sidantal |
|

**Returns:**
boolean - sant, om detta filterintervall innehåller sidan

