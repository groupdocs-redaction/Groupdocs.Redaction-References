---
title: "IImageFormatInstance"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "रास्टर इमेज स्वरूप रेडैक्शन के लिए आवश्यक विधियों को परिभाषित करता है।"
type: docs
weight: 20
url: /hi/java/com.groupdocs.redaction.integration/iimageformatinstance/
---```
public interface IImageFormatInstance
```

Defines methods that are required for raster image format redactions.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)
* More details about implementing custom formats: [Create custom format handler](../https://docs.groupdocs.com/redaction/java/create-custom-format-handler/)

<br />


## Methods

| Method | Description |
| --- | --- |
| [editArea(Point topLeft, RegionReplacementOptions options)](#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Replaces the area at given point with a rectangle of specific color and size.
 |
### editArea(Point topLeft, RegionReplacementOptions options) {#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public abstract RedactionResult editArea(Point topLeft, RegionReplacementOptions options)
```


Replaces the area at given point with a rectangle of specific color and size.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topLeft | java.awt.Point | Top-left corner coordinates of filled area
 |
| options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Color and size settings
 |

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image area redaction result

