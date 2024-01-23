---
title: ReplacementOptions
second_title: GroupDocs.Redaction for Java API Reference
description: Represents options for matched text replacement.
type: docs
weight: 29
url: /java/com.groupdocs.redaction.redactions/replacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class ReplacementOptions
```

Represents options for matched text replacement.

--------------------

**Learn more**

 *  More details about document text redactions: [Text redactions][]
 *  More details about redaction filters: [Use PDF redaction filters][]


[Text redactions]: https://docs.groupdocs.com/redaction/java/text-redactions/
[Use PDF redaction filters]: https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/
## Constructors

| Constructor | Description |
| --- | --- |
| [ReplacementOptions(String replacement)](#ReplacementOptions-java.lang.String-) | Initializes a new instance of ReplacementOptions class with replacement text as an option. |
| [ReplacementOptions(Color color)](#ReplacementOptions-java.awt.Color-) | Initializes a new instance of ReplacementOptions class with colored rectangle as an option. |
## Methods

| Method | Description |
| --- | --- |
| [getActionType()](#getActionType--) | Gets the replacement action: draw box or replace text. |
| [getReplacement()](#getReplacement--) | Gets the textual replacement value. |
| [setReplacement(String value)](#setReplacement-java.lang.String-) | Sets the textual replacement value. |
| [getBoxColor()](#getBoxColor--) | Gets the color for a  ReplacementType.DrawBox  option (ignored otherwise). |
| [setBoxColor(Color value)](#setBoxColor-java.awt.Color-) | Sets the color for a  ReplacementType.DrawBox  option (ignored otherwise). |
| [getFilters()](#getFilters--) | Gets an array of filters to apply with this redaction. |
| [setFilters(RedactionFilter[] value)](#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---) | Sets an array of filters to apply with this redaction. |
| [fromFilters(RedactionFilter[] filters)](#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---) |  |
### ReplacementOptions(String replacement) {#ReplacementOptions-java.lang.String-}
```
public ReplacementOptions(String replacement)
```


Initializes a new instance of ReplacementOptions class with replacement text as an option.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| replacement | java.lang.String | Textual replacement |

### ReplacementOptions(Color color) {#ReplacementOptions-java.awt.Color-}
```
public ReplacementOptions(Color color)
```


Initializes a new instance of ReplacementOptions class with colored rectangle as an option.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color | java.awt.Color | Rectangle color |

### getActionType() {#getActionType--}
```
public final ReplacementType getActionType()
```


Gets the replacement action: draw box or replace text.

**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype) - The replacement action: draw box or replace text.
### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Gets the textual replacement value.

**Returns:**
java.lang.String - The textual replacement value.
### setReplacement(String value) {#setReplacement-java.lang.String-}
```
public final void setReplacement(String value)
```


Sets the textual replacement value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The textual replacement value. |

### getBoxColor() {#getBoxColor--}
```
public final Color getBoxColor()
```


Gets the color for a  ReplacementType.DrawBox  option (ignored otherwise).

**Returns:**
java.awt.Color - The color for a  ReplacementType.DrawBox  option (ignored otherwise).
### setBoxColor(Color value) {#setBoxColor-java.awt.Color-}
```
public final void setBoxColor(Color value)
```


Sets the color for a  ReplacementType.DrawBox  option (ignored otherwise).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color | The color for a  ReplacementType.DrawBox  option (ignored otherwise). |

### getFilters() {#getFilters--}
```
public final RedactionFilter[] getFilters()
```


Gets an array of filters to apply with this redaction.

**Returns:**
com.groupdocs.redaction.redactions.RedactionFilter[] - An array of filters to apply with this redaction.
### setFilters(RedactionFilter[] value) {#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public final void setFilters(RedactionFilter[] value)
```


Sets an array of filters to apply with this redaction.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) | An array of filters to apply with this redaction. |

### fromFilters(RedactionFilter[] filters) {#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public static ReplacementOptions fromFilters(RedactionFilter[] filters)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filters | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) |  |

**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions)
