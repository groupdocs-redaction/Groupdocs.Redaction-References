---
title: TextReplacement
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a textual replacement information.
type: docs
weight: 30
url: /java/com.groupdocs.redaction.redactions/textreplacement/
---
**Inheritance:**
java.lang.Object
```
public class TextReplacement
```

Represents a textual replacement information.

--------------------

**Learn more**

 *  More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback][]


[Use redaction callback]: https://docs.groupdocs.com/redaction/java/use-redaction-callback/
## Constructors

| Constructor | Description |
| --- | --- |
| [TextReplacement(int index, String original, String replacement)](#TextReplacement-int-java.lang.String-java.lang.String-) | Initializes a new instance of TextReplacement class. |
## Methods

| Method | Description |
| --- | --- |
| [getIndex()](#getIndex--) | Gets an index of the matched text within source string. |
| [getOriginalText()](#getOriginalText--) | Gets the original matched string. |
| [getReplacement()](#getReplacement--) | Gets the string, replacing OriginalText. |
| [toString()](#toString--) | Provides text replacement description and its position. |
### TextReplacement(int index, String original, String replacement) {#TextReplacement-int-java.lang.String-java.lang.String-}
```
public TextReplacement(int index, String original, String replacement)
```


Initializes a new instance of TextReplacement class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | Index of a matched text within source string |
| original | java.lang.String | Original matched string |
| replacement | java.lang.String | String, replacing OriginalText in source string |

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Gets an index of the matched text within source string.

**Returns:**
int - An index of the matched text within source string.
### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Gets the original matched string.

**Returns:**
java.lang.String - The original matched string.
### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Gets the string, replacing OriginalText.

**Returns:**
java.lang.String - The string, replacing OriginalText.
### toString() {#toString--}
```
public String toString()
```


Provides text replacement description and its position.

**Returns:**
java.lang.String - Replacement description
