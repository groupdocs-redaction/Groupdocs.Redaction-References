---
title: "PageRangeFilter"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет фильтр редактирования, задающий диапазон страниц внутри документа для применения редактирования."
type: docs
weight: 24
url: /ru/java/com.groupdocs.redaction.redactions/pagerangefilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageRangeFilter extends RedactionFilter
```

Представляет фильтр редактирования, задающий диапазон страниц внутри документа для применения редактирования.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [PageRangeFilter(PageSeekOrigin origin, int index, int count)](#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-) | Инициализирует новый экземпляр класса RemovePageRedaction. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getOrigin()](#getOrigin--) | Получает позицию ссылки поиска, начало или конец документа. |
|
|  | [getIndex()](#getIndex--) | Получает индекс начальной позиции (нумерация с нуля). |
|
|  | [getCount()](#getCount--) | Получает количество страниц для удаления. |
|
|  | [isPageInRange(int pageIndex, int pageCount)](#isPageInRange-int-int-) | Проверяет, содержит ли диапазон страниц этого фильтра заданную страницу. |
|
### PageRangeFilter(PageSeekOrigin origin, int index, int count) {#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-}
```
public PageRangeFilter(PageSeekOrigin origin, int index, int count)
```


Инициализирует новый экземпляр класса RemovePageRedaction.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | origin | [PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) | Позиция ссылки поиска, начало или конец документа |
|
|  | индекс | int | Индекс начальной позиции (нумерация с нуля) |
|
|  | количество | int | Количество страниц для удаления |
|

### getOrigin() {#getOrigin--}
```
public final PageSeekOrigin getOrigin()
```


Получает позицию ссылки поиска, начало или конец документа.


**Returns:**
[PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) - Seek reference position, the beginning or the end of a document.

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Получает индекс начальной позиции (нумерация с нуля).


**Returns:**
int - Начальный индекс позиции (ноль-ориентированный).

### getCount() {#getCount--}
```
public final int getCount()
```


Получает количество страниц для удаления.


**Returns:**
int - Количество страниц для удаления.

### isPageInRange(int pageIndex, int pageCount) {#isPageInRange-int-int-}
```
public final boolean isPageInRange(int pageIndex, int pageCount)
```


Проверяет, содержит ли диапазон страниц этого фильтра заданную страницу.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | индекс страницы (ноль-ориентированный) |
|
|  | pageCount | int | общее количество страниц |
|

**Returns:**
boolean - true, если этот диапазон фильтра содержит страницу

