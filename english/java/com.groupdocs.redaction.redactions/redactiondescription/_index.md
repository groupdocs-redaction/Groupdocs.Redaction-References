---
title: RedactionDescription
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a single change action info that performed during redaction process.
type: docs
weight: 23
url: /java/com.groupdocs.redaction.redactions/redactiondescription/
---
**Inheritance:**
java.lang.Object
```
public class RedactionDescription
```

Represents a single change action info that performed during redaction process.

--------------------

**Learn more**

 *  More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback][]


[Use redaction callback]: https://docs.groupdocs.com/redaction/java/use-redaction-callback/
## Constructors

| Constructor | Description |
| --- | --- |
| [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-) | Initializes a new instance of RedactionDescription class without replacement information. |
| [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-) | Initializes a new instance of RedactionDescription class with replacement information. |
| [RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-) | Initializes a new instance of RedactionDescription class with image area replacement information. |
## Methods

| Method | Description |
| --- | --- |
| [getRedactionType()](#getRedactionType--) | Gets the type of document's data - text, metadata or annotations. |
| [getActionType()](#getActionType--) | Gets the redaction operation: replacement, cleanup or deletion. |
| [getOriginalText()](#getOriginalText--) | Gets the matched text, if any expression is provided. |
| [getReplacement()](#getReplacement--) | Gets the replacement information, can be null. |
| [getImageAreaReplacement()](#getImageAreaReplacement--) | Gets the replacement information for image area redactions, returns null for textual redactions. |
| [getDetails()](#getDetails--) | Gets an optional details information for the item being redacted. |
| [setDetails(String value)](#setDetails-java.lang.String-) | Sets an optional details information for the item being redacted. |
### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)
```


Initializes a new instance of RedactionDescription class without replacement information.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| redactionType | int | Type of data being redacted |
| actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Action to be performed on these data |
| originalText | java.lang.String | Matched text, comment or annotation body |

### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)
```


Initializes a new instance of RedactionDescription class with replacement information.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| redactionType | int | Type of data being redacted |
| actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Action to be performed on these data |
| originalText | java.lang.String | Matched text, comment or annotation body |
| replacement | [TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) | Replacement text, matched text and its position within original string |

### RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)
```


Initializes a new instance of RedactionDescription class with image area replacement information.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| redactionType | int | Type of data being redacted |
| actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Action to be performed on these data |
| imageAreaReplacement | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Image area replacement information |
| imageDetails | java.lang.String | Image textual description, by default it is String.Empty |

### getRedactionType() {#getRedactionType--}
```
public final int getRedactionType()
```


Gets the type of document's data - text, metadata or annotations.

**Returns:**
int - The type of document's data - text, metadata or annotations.
### getActionType() {#getActionType--}
```
public final RedactionActionType getActionType()
```


Gets the redaction operation: replacement, cleanup or deletion.

**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) - The redaction operation: replacement, cleanup or deletion.
### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Gets the matched text, if any expression is provided.

**Returns:**
java.lang.String - The matched text, if any expression is provided.
### getReplacement() {#getReplacement--}
```
public final TextReplacement getReplacement()
```


Gets the replacement information, can be null.

**Returns:**
[TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) - The replacement information, can be null.
### getImageAreaReplacement() {#getImageAreaReplacement--}
```
public final RegionReplacementOptions getImageAreaReplacement()
```


Gets the replacement information for image area redactions, returns null for textual redactions.

**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The replacement information for image area redactions, returns null for textual redactions.
### getDetails() {#getDetails--}
```
public final String getDetails()
```


Gets an optional details information for the item being redacted.

**Returns:**
java.lang.String - An optional details information for the item being redacted.
### setDetails(String value) {#setDetails-java.lang.String-}
```
public final void setDetails(String value)
```


Sets an optional details information for the item being redacted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | An optional details information for the item being redacted. |

