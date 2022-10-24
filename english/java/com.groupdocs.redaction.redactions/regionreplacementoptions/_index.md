---
title: RegionReplacementOptions
second_title: GroupDocs.Redaction for Java API Reference
description: Represents color and area parameters for image region replacement.
type: docs
weight: 22
url: /java/com.groupdocs.redaction.redactions/regionreplacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class RegionReplacementOptions
```

Represents color and area parameters for image region replacement. See  ImageAreaRedaction .

--------------------

**Learn more**

 *  More details about image redactions: [Image redactions][]


[Image redactions]: https://docs.groupdocs.com/redaction/java/image-redactions/
## Constructors

| Constructor | Description |
| --- | --- |
| [RegionReplacementOptions(Color fillColor, Dimension size)](#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-) | Initializes a new instance of RegionReplacementOptions class. |
| [RegionReplacementOptions(Color fillColor, Font font, String expectedText)](#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-) | Initializes a new instance of RegionReplacementOptions class which size matches given text. |
## Methods

| Method | Description |
| --- | --- |
| [getFillColor()](#getFillColor--) | Gets the color to fill the redacted area. |
| [setFillColor(Color value)](#setFillColor-java.awt.Color-) | Sets the color to fill the redacted area. |
| [getSize()](#getSize--) | Gets the rectangle with and height. |
| [setSize(Dimension value)](#setSize-java.awt.Dimension-) | Sets the rectangle with and height. |
### RegionReplacementOptions(Color fillColor, Dimension size) {#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-}
```
public RegionReplacementOptions(Color fillColor, Dimension size)
```


Initializes a new instance of RegionReplacementOptions class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fillColor | java.awt.Color | Color to fill the area |
| size | java.awt.Dimension | Filled area size |

### RegionReplacementOptions(Color fillColor, Font font, String expectedText) {#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-}
```
public RegionReplacementOptions(Color fillColor, Font font, String expectedText)
```


Initializes a new instance of RegionReplacementOptions class which size matches given text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fillColor | java.awt.Color | Color to fill the area |
| font | java.awt.Font | Expected text font |
| expectedText | java.lang.String | Expected text |

### getFillColor() {#getFillColor--}
```
public final Color getFillColor()
```


Gets the color to fill the redacted area.

**Returns:**
java.awt.Color - The color to fill the redacted area.
### setFillColor(Color value) {#setFillColor-java.awt.Color-}
```
public final void setFillColor(Color value)
```


Sets the color to fill the redacted area.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color | The color to fill the redacted area. |

### getSize() {#getSize--}
```
public final Dimension getSize()
```


Gets the rectangle with and height.

**Returns:**
java.awt.Dimension - The rectangle with and height.
### setSize(Dimension value) {#setSize-java.awt.Dimension-}
```
public final void setSize(Dimension value)
```


Sets the rectangle with and height.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Dimension | The rectangle with and height. |

