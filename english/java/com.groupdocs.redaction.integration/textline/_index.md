---
title: TextLine
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a line of text extracted by OCR engine from an image.
type: docs
weight: 16
url: /java/com.groupdocs.redaction.integration/textline/
---
**Inheritance:**
java.lang.Object
```
public class TextLine
```

Represents a line of text, extracted by OCR engine from an image.

--------------------

**Learn more**

 *  More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics][]


[OCR Usage Basics]: https://docs.groupdocs.com/redaction/java/ocr-usage-basics/
## Constructors

| Constructor | Description |
| --- | --- |
| [TextLine(TextFragment[] fragments)](#TextLine-com.groupdocs.redaction.integration.TextFragment---) | Initializes a new instance of a line of text, extracted by OCR engine from an image. |
## Methods

| Method | Description |
| --- | --- |
| [getFragments()](#getFragments--) | Gets an array of text fragments, such as symbols and words, recognized in the line. |
| [toString()](#toString--) | Returns textual content of the recognised line of text. |
### TextLine(TextFragment[] fragments) {#TextLine-com.groupdocs.redaction.integration.TextFragment---}
```
public TextLine(TextFragment[] fragments)
```


Initializes a new instance of a line of text, extracted by OCR engine from an image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fragments | [TextFragment\[\]](../../com.groupdocs.redaction.integration/textfragment) | initial set of text fragments |

### getFragments() {#getFragments--}
```
public final TextFragment[] getFragments()
```


Gets an array of text fragments, such as symbols and words, recognized in the line.

**Returns:**
com.groupdocs.redaction.integration.TextFragment[] - An array of text fragments, such as symbols and words, recognized in the line.
### toString() {#toString--}
```
public String toString()
```


Returns textual content of the recognised line of text.

**Returns:**
java.lang.String - textual content of the recognised line of text
