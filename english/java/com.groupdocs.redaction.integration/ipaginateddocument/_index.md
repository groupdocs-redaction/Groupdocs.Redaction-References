---
title: IPaginatedDocument
second_title: GroupDocs.Redaction for Java API Reference
description: Defines methods that are required to manipulate a documents pages.
type: docs
weight: 25
url: /java/com.groupdocs.redaction.integration/ipaginateddocument/
---```
public interface IPaginatedDocument
```

Defines methods that are required to manipulate a document's pages. Needs to be implemented by  DocumentFormatInstance -derived class to perform page redactions.

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More details about manipulating pages: [Remove page redaction][]


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Remove page redaction]: https://docs.groupdocs.com/redaction/java/remove-page-redaction/
## Methods

| Method | Description |
| --- | --- |
| [removePages(PageSeekOrigin origin, int index, int count)](#removePages-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-) | Removes one or multiple pages depending on its start position, offset and count. |
### removePages(PageSeekOrigin origin, int index, int count) {#removePages-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-}
```
public abstract RedactionResult removePages(PageSeekOrigin origin, int index, int count)
```


Removes one or multiple pages depending on its start position, offset and count.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| origin | [PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) | Search origin position, the beginning or the end of the document |
| index | int | Start position index (0-based) |
| count | int | Count of pages to remove |

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Pages removal redaction result
