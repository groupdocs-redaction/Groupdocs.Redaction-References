---
title: TextFragment
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a part of recognized text word symbol etc extracted by OCR engine.
type: docs
weight: 15
url: /java/com.groupdocs.redaction.integration/textfragment/
---
**Inheritance:**
java.lang.Object
```
public class TextFragment
```

Represents a part of recognized text (word, symbol, etc), extracted by OCR engine.

--------------------

**Learn more**

 *  More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics][]


[OCR Usage Basics]: https://docs.groupdocs.com/redaction/java/ocr-usage-basics/
## Constructors

| Constructor | Description |
| --- | --- |
| [TextFragment(String text, Rectangle rectangle)](#TextFragment-java.lang.String-java.awt.Rectangle-) | Initializes a new instance of the recognised text fragment. |
## Methods

| Method | Description |
| --- | --- |
| [getText()](#getText--) | Gets a textual content of the recognised text fragment. |
| [getRectangle()](#getRectangle--) | Gets a bounding rectangle of the recognised text fragment. |
| [toString()](#toString--) | Returns textual content of the recognised text fragment. |
### TextFragment(String text, Rectangle rectangle) {#TextFragment-java.lang.String-java.awt.Rectangle-}
```
public TextFragment(String text, Rectangle rectangle)
```


Initializes a new instance of the recognised text fragment.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | textual content of the recognised text fragment |
| rectangle | java.awt.Rectangle | bounding rectangle of the recognised text fragment |

### getText() {#getText--}
```
public final String getText()
```


Gets a textual content of the recognised text fragment.

**Returns:**
java.lang.String - A textual content of the recognised text fragment.
### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Gets a bounding rectangle of the recognised text fragment.

**Returns:**
java.awt.Rectangle - A bounding rectangle of the recognised text fragment.
### toString() {#toString--}
```
public String toString()
```


Returns textual content of the recognised text fragment.

**Returns:**
java.lang.String - textual content of the recognised text fragment
