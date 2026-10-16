---
title: "ImageAreaRedaction"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "एक रेडैक्शन को दर्शाता है जो इमेज दस्तावेज़ के दिए गए क्षेत्र में रंगीन आयत रखता है।"
type: docs
weight: 18
url: /hi/java/com.groupdocs.redaction.redactions/imagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class ImageAreaRedaction extends Redaction
```

एक रेडैक्शन को दर्शाता है जो इमेज दस्तावेज़ के दिए गए क्षेत्र में रंगीन आयत रखता है।

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)](#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | विशिष्ट क्षेत्र आकार को हटाने के लिए ImageAreaRedaction क्लास का नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getOptions()](#getOptions--) | प्राप्त करता है |
RegionReplacementOptions
रंग और क्षेत्र पैरामीटरों के साथ विकल्प।
|
|  | [getTopLeft()](#getTopLeft--) | हटाने के क्षेत्र की शीर्ष-बाएँ स्थिति प्राप्त करता है। |
|
|  | [getDescription()](#getDescription--) | एक स्ट्रिंग लौटाता है, जो रेडैक्शन और उसके पैरामीटरों का वर्णन करती है। |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | दिए गए फ़ॉर्मेट इंस्टेंस पर रेडैक्शन लागू करता है। |
|
### ImageAreaRedaction(Point topLeft, RegionReplacementOptions options) {#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)
```


विशिष्ट क्षेत्र आकार को हटाने के लिए ImageAreaRedaction क्लास का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | topLeft | java.awt.Point | ऊपरी-बाएँ क्षेत्र के निर्देशांक |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | क्षेत्र का आकार और रंग |
|

### getOptions() {#getOptions--}
```
public final RegionReplacementOptions getOptions()
```


प्राप्त करता है
RegionReplacementOptions
रंग और क्षेत्र पैरामीटरों के साथ विकल्प।


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### getTopLeft() {#getTopLeft--}
```
public final Point getTopLeft()
```


हटाने के क्षेत्र की शीर्ष-बाएँ स्थिति प्राप्त करता है।


**Returns:**
java.awt.Point - हटाने के क्षेत्र की शीर्ष-बाएँ स्थिति।

### getDescription() {#getDescription--}
```
public String getDescription()
```


एक स्ट्रिंग लौटाता है, जो रेडैक्शन और उसके पैरामीटरों का वर्णन करती है।


**Returns:**
java.lang.String - टेक्स्ट, जिसमें रेडैक्शन नाम और पैरामीटर होते हैं।

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


दिए गए फ़ॉर्मेट इंस्टेंस पर रेडैक्शन लागू करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | रेडैक्शन लागू करने के लिए दस्तावेज़ का एक इंस्टेंस |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

