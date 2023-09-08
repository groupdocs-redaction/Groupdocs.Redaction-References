---
title: PageAreaFilter
second_title: GroupDocs.Redaction for Java API Reference
description: Represents redaction filter setting an area within a page of a document to apply redaction.
type: docs
weight: 20
url: /java/com.groupdocs.redaction.redactions/pageareafilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageAreaFilter extends RedactionFilter
```

Represents redaction filter, setting an area within a page of a document to apply redaction.

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More details about redaction filters: [Use PDF redaction filters][]


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Use PDF redaction filters]: https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/
## Constructors

| Constructor | Description |
| --- | --- |
| [PageAreaFilter(Point topLeft, Dimension size)](#PageAreaFilter-java.awt.Point-java.awt.Dimension-) | Initializes a new instance of PageAreaFilter class for redacting specific area. |
## Methods

| Method | Description |
| --- | --- |
| [getRectangle()](#getRectangle--) | Gets the rectangle (top-left position and size of the area) on a page. |
| [isInTheArea(Rectangle rectangle)](#isInTheArea-java.awt.Rectangle-) | Checks if this filter area has intersection with given rectangle. |
### PageAreaFilter(Point topLeft, Dimension size) {#PageAreaFilter-java.awt.Point-java.awt.Dimension-}
```
public PageAreaFilter(Point topLeft, Dimension size)
```


Initializes a new instance of PageAreaFilter class for redacting specific area.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topLeft | java.awt.Point | Top-left area coordinates |
| size | java.awt.Dimension | Area size and color |

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Gets the rectangle (top-left position and size of the area) on a page.

**Returns:**
java.awt.Rectangle - The rectangle (top-left position and size of the area) on a page.
### isInTheArea(Rectangle rectangle) {#isInTheArea-java.awt.Rectangle-}
```
public final boolean isInTheArea(Rectangle rectangle)
```


Checks if this filter area has intersection with given rectangle.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangle | java.awt.Rectangle | Rectangle to check |

**Returns:**
boolean - true, if this filter area has intersection
