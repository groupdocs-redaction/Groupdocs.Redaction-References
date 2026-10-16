---
title: "RedactableImage"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "सभी रास्टर इमेज रेडैक्शन ऑपरेशनों के लिए एक फ़ेसाड प्रदान करता है।"
type: docs
weight: 14
url: /hi/java/com.groupdocs.redaction.integration/redactableimage/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.integration.IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance), [com.groupdocs.redaction.integration.IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable)
```
public class RedactableImage implements IImageFormatInstance, IMultipleAreaRedactable
```

सभी रास्टर इमेज रेडैक्शन ऑपरेशनों के लिए एक फ़ेसाड प्रदान करता है।

## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [RedactableImage(IImageFormatInstance img)](#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-) | एक ऑब्जेक्ट का उपयोग करके नई इंस्टेंस बनाता है, जो लागू करता है |
IImageFormatInstance
इंटरफ़ेस।
|
|  | [RedactableImage(IMultipleAreaRedactable img)](#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-) | एक ऑब्जेक्ट का उपयोग करके नई इंस्टेंस बनाता है, जो लागू करता है |
IMultipleAreaRedactable
इंटरफ़ेस।
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getRawStream()](#getRawStream--) | वास्तविक इमेज सामग्री के साथ एक स्ट्रीम प्राप्त करता है। |
|
|  | [editAreas(Rectangle[] rectangles, Color boxColor)](#editAreas-java.awt.Rectangle---java.awt.Color-) | एक ही रंग के साथ कई इमेज क्षेत्रों को एक साथ रीडैक्ट करता है। |
|
|  | [editArea(Point topLeft, RegionReplacementOptions options)](#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | दिए गए बिंदु पर क्षेत्र को विशिष्ट रंग और आकार के आयत से बदलता है। |
|
### RedactableImage(IImageFormatInstance img) {#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-}
```
public RedactableImage(IImageFormatInstance img)
```


एक ऑब्जेक्ट का उपयोग करके नई इंस्टेंस बनाता है, जो लागू करता है
IImageFormatInstance
इंटरफ़ेस।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | img | [IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance) | एक इंस्टेंस, जो IImageFormatInstance इंटरफ़ेस को लागू करता है |
|

### RedactableImage(IMultipleAreaRedactable img) {#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-}
```
public RedactableImage(IMultipleAreaRedactable img)
```


एक ऑब्जेक्ट का उपयोग करके नई इंस्टेंस बनाता है, जो लागू करता है
IMultipleAreaRedactable
इंटरफ़ेस।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | img | [IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable) | एक इंस्टेंस, जो IMultipleAreaRedactable इंटरफ़ेस को लागू करता है |
|

### getRawStream() {#getRawStream--}
```
public final InputStream getRawStream()
```


वास्तविक इमेज सामग्री के साथ एक स्ट्रीम प्राप्त करता है।


**Returns:**
java.io.InputStream - इमेज डेटा वाली स्ट्रीम

### editAreas(Rectangle[] rectangles, Color boxColor) {#editAreas-java.awt.Rectangle---java.awt.Color-}
```
public final RedactionResult editAreas(Rectangle[] rectangles, Color boxColor)
```


एक ही रंग के साथ कई इमेज क्षेत्रों को एक साथ रीडैक्ट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | आयत | java.awt.Rectangle[] | आयत क्षेत्रों की एक एरे |
|
|  | boxColor | java.awt.Color | क्षेत्रों को भरने के लिए रंग |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image areas redaction result

### editArea(Point topLeft, RegionReplacementOptions options) {#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public final RedactionResult editArea(Point topLeft, RegionReplacementOptions options)
```


दिए गए बिंदु पर क्षेत्र को विशिष्ट रंग और आकार के आयत से बदलता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | topLeft | java.awt.Point | भरे हुए क्षेत्र के शीर्ष-बाएँ कोने के निर्देशांक |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | रंग और आकार सेटिंग्स |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image area redaction result

