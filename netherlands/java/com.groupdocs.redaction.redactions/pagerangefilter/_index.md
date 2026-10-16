---
title: "PageRangeFilter"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt de redactiefilter in die een paginabereik binnen een document definieert om redactie toe te passen."
type: docs
weight: 24
url: /nl/java/com.groupdocs.redaction.redactions/pagerangefilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageRangeFilter extends RedactionFilter
```

Vertegenwoordigt een redactiefilter dat een paginabereik binnen een document instelt om redacties toe te passen.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [PageRangeFilter(PageSeekOrigin origin, int index, int count)](#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-) | Initialiseert een nieuwe instantie van de RemovePageRedaction-klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getOrigin()](#getOrigin--) | Haalt de zoekreferentiepositie op, het begin of het einde van een document. |
|
|  | [getIndex()](#getIndex--) | Haalt de startpositie-index op (0-gebaseerd). |
|
|  | [getCount()](#getCount--) | Haalt het aantal te verwijderen pagina's op. |
|
|  | [isPageInRange(int pageIndex, int pageCount)](#isPageInRange-int-int-) | Controleert of dit filterpaginabereik de opgegeven pagina bevat. |
|
### PageRangeFilter(PageSeekOrigin origin, int index, int count) {#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-}
```
public PageRangeFilter(PageSeekOrigin origin, int index, int count)
```


Initialiseert een nieuwe instantie van de RemovePageRedaction-klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | origin | [PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) | Zoekreferentiepositie, het begin of het einde van een document |
|
|  | index | int | Startpositie-index (0-gebaseerd) |
|
|  | aantal | int | Aantal pagina's om te verwijderen |
|

### getOrigin() {#getOrigin--}
```
public final PageSeekOrigin getOrigin()
```


Haalt de zoekreferentiepositie op, het begin of het einde van een document.


**Returns:**
[PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) - Seek reference position, the beginning or the end of a document.

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Haalt de startpositie-index op (0-gebaseerd).


**Returns:**
int - Startpositie-index (0-gebaseerd).

### getCount() {#getCount--}
```
public final int getCount()
```


Haalt het aantal te verwijderen pagina's op.


**Returns:**
int - Het aantal pagina's om te verwijderen.

### isPageInRange(int pageIndex, int pageCount) {#isPageInRange-int-int-}
```
public final boolean isPageInRange(int pageIndex, int pageCount)
```


Controleert of dit filterpaginabereik de opgegeven pagina bevat.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | index van de pagina (nul-gebaseerd) |
|
|  | pageCount | int | totaal aantal pagina's |
|

**Returns:**
boolean - true, als dit filterbereik pagina bevat

