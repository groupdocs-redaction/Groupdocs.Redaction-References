---
title: RemovePageRedaction
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a redaction that removes a page slide worksheet etc. from a document.
type: docs
weight: 27
url: /java/com.groupdocs.redaction.redactions/removepageredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class RemovePageRedaction extends Redaction
```

Represents a redaction that removes a page (slide, worksheet, etc.) from a document.

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More details about removing pages: [Remove page redaction][]

The following example demonstrates how to remove the last page of the document.

```

  try (Redactor redactor = new Redactor("C:\\test.pdf"))
 {
    redactor.apply(new RemovePageRedaction(PageSeekOrigin.END, 0, 1));
    redactor.save()
 }
 
```


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Remove page redaction]: https://docs.groupdocs.com/redaction/java/remove-page-redaction/
## Constructors

| Constructor | Description |
| --- | --- |
| [RemovePageRedaction(PageSeekOrigin origin, int index, int count)](#RemovePageRedaction-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-) | Initializes a new instance of RemovePageRedaction class. |
## Methods

| Method | Description |
| --- | --- |
| [getOrigin()](#getOrigin--) | Gets seek reference position, the beginning or the end of a document. |
| [getIndex()](#getIndex--) | Gets start position index (0-based). |
| [getCount()](#getCount--) | Gets the count of pages to remove. |
| [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applies the redaction to a given format instance. |
### RemovePageRedaction(PageSeekOrigin origin, int index, int count) {#RemovePageRedaction-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-}
```
public RemovePageRedaction(PageSeekOrigin origin, int index, int count)
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
### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Applies the redaction to a given format instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | An instance of a document to apply redaction |

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any
