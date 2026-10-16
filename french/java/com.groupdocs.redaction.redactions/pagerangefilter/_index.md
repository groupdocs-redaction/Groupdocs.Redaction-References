---
title: "PageRangeFilter"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente le filtre de redaction définissant la plage de pages à l'intérieur d'un document pour appliquer la redaction."
type: docs
weight: 24
url: /fr/java/com.groupdocs.redaction.redactions/pagerangefilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageRangeFilter extends RedactionFilter
```

Représente un filtre de rédaction, définissant une plage de pages à l'intérieur d'un document pour appliquer la rédaction.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [PageRangeFilter(PageSeekOrigin origin, int index, int count)](#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-) | Initialise une nouvelle instance de la classe RemovePageRedaction. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getOrigin()](#getOrigin--) | Obtient la position de référence de recherche, le début ou la fin d'un document. |
|
|  | [getIndex()](#getIndex--) | Obtient l'index de position de départ (à partir de 0). |
|
|  | [getCount()](#getCount--) | Obtient le nombre de pages à supprimer. |
|
|  | [isPageInRange(int pageIndex, int pageCount)](#isPageInRange-int-int-) | Vérifie si cette plage de pages du filtre contient la page donnée. |
|
### PageRangeFilter(PageSeekOrigin origin, int index, int count) {#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-}
```
public PageRangeFilter(PageSeekOrigin origin, int index, int count)
```


Initialise une nouvelle instance de la classe RemovePageRedaction.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | origin | [PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) | Position de référence de recherche, le début ou la fin d'un document |
|
|  | index | int | Index de position de départ (à partir de 0) |
|
|  | nombre | int | Nombre de pages à supprimer |
|

### getOrigin() {#getOrigin--}
```
public final PageSeekOrigin getOrigin()
```


Obtient la position de référence de recherche, le début ou la fin d'un document.


**Returns:**
[PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) - Seek reference position, the beginning or the end of a document.

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Obtient l'index de position de départ (à partir de 0).


**Returns:**
int - Index de position de départ (à partir de 0).

### getCount() {#getCount--}
```
public final int getCount()
```


Obtient le nombre de pages à supprimer.


**Returns:**
int - Le nombre de pages à supprimer.

### isPageInRange(int pageIndex, int pageCount) {#isPageInRange-int-int-}
```
public final boolean isPageInRange(int pageIndex, int pageCount)
```


Vérifie si cette plage de pages du filtre contient la page donnée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | pageIndex | int | indice de la page (base zéro) |
|
|  | pageCount | int | nombre total de pages |
|

**Returns:**
booléen - true, si cette plage de filtre contient la page

