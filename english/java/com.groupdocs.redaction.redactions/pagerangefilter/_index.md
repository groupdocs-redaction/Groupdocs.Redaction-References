---
title: PageRangeFilter
second_title: GroupDocs.Redaction for Java API Reference
description: Represents redaction filter setting page range inside a document to apply redaction.
type: docs
weight: 22
url: /java/com.groupdocs.redaction.redactions/pagerangefilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageRangeFilter extends RedactionFilter
```

Represents redaction filter, setting page range inside a document to apply redaction.

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More details about redaction filters: [Use PDF redaction filters][]


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Use PDF redaction filters]: https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/
## Constructors

| Constructor | Description |
| --- | --- |
| [PageRangeFilter(PageSeekOrigin origin, int index, int count)](#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-) | Initializes a new instance of RemovePageRedaction class. |
## Methods

| Method | Description |
| --- | --- |
| [getOrigin()](#getOrigin--) | Gets seek reference position, the beginning or the end of a document. |
| [getIndex()](#getIndex--) | Gets start position index (0-based). |
| [getCount()](#getCount--) | Gets the count of pages to remove. |
| [isPageInRange(int pageIndex, int pageCount)](#isPageInRange-int-int-) | Checks if this filter page range contains given page. |
### PageRangeFilter(PageSeekOrigin origin, int index, int count) {#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-}
```
public PageRangeFilter(PageSeekOrigin origin, int index, int count)
```


Initializes a new instance of RemovePageRedaction class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| origin | [PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) | Seek reference position, the beginning or the end of a document |
| index | int | Start position index (0-based) |
| count | int | Count of pages to remove |

### getOrigin() {#getOrigin--}
```
public final PageSeekOrigin getOrigin()
```


Gets seek reference position, the beginning or the end of a document.

**Returns:**
[PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) - Seek reference position, the beginning or the end of a document.
### getIndex() {#getIndex--}
```
public final int getIndex()
```


Gets start position index (0-based).

**Returns:**
int - Start position index (0-based).
### getCount() {#getCount--}
```
public final int getCount()
```


Gets the count of pages to remove.

**Returns:**
int - The count of pages to remove.
### isPageInRange(int pageIndex, int pageCount) {#isPageInRange-int-int-}
```
public final boolean isPageInRange(int pageIndex, int pageCount)
```


Checks if this filter page range contains given page.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | index of the page (zero-bazed) |
| pageCount | int | total page count |

**Returns:**
boolean - true, if this filter range contains page
