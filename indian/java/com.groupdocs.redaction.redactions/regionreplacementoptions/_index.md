---
title: "RegionReplacementOptions"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "इमेज रीजन प्रतिस्थापन के लिए रंग और क्षेत्र पैरामीटर का प्रतिनिधित्व करता है।"
type: docs
weight: 29
url: /hi/java/com.groupdocs.redaction.redactions/regionreplacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class RegionReplacementOptions
```

इमेज रीजन रिप्लेसमेंट के लिए रंग और क्षेत्र पैरामीटर का प्रतिनिधित्व करता है। देखें
ImageAreaRedaction
.

*** ** * ** ***


**Learn more**

* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [RegionReplacementOptions(Color fillColor, Dimension size)](#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-) | RegionReplacementOptions क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [RegionReplacementOptions(Color fillColor, Font font, String expectedText)](#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-) | RegionReplacementOptions क्लास का नया इंस्टेंस इनिशियलाइज़ करता है जिसका आकार दिए गए टेक्स्ट से मेल खाता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getFillColor()](#getFillColor--) | रेडैक्टेड एरिया को भरने के लिए रंग प्राप्त करता है। |
|
|  | [setFillColor(Color value)](#setFillColor-java.awt.Color-) | रेडैक्टेड एरिया को भरने के लिए रंग सेट करता है। |
|
|  | [getSize()](#getSize--) | आयत के चौड़ाई और ऊँचाई को प्राप्त करता है। |
|
|  | [setSize(Dimension value)](#setSize-java.awt.Dimension-) | आयत की चौड़ाई और ऊँचाई को सेट करता है। |
|
### RegionReplacementOptions(Color fillColor, Dimension size) {#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-}
```
public RegionReplacementOptions(Color fillColor, Dimension size)
```


RegionReplacementOptions क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | fillColor | java.awt.Color | क्षेत्र को भरने के लिए रंग |
|
|  | size | java.awt.Dimension | भरे हुए क्षेत्र का आकार |
|

### RegionReplacementOptions(Color fillColor, Font font, String expectedText) {#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-}
```
public RegionReplacementOptions(Color fillColor, Font font, String expectedText)
```


RegionReplacementOptions क्लास का नया इंस्टेंस इनिशियलाइज़ करता है जिसका आकार दिए गए टेक्स्ट से मेल खाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | fillColor | java.awt.Color | क्षेत्र को भरने के लिए रंग |
|
|  | font | java.awt.Font | अपेक्षित पाठ फ़ॉन्ट |
|
|  | expectedText | java.lang.String | अपेक्षित पाठ |
|

### getFillColor() {#getFillColor--}
```
public final Color getFillColor()
```


रेडैक्टेड एरिया को भरने के लिए रंग प्राप्त करता है।


**Returns:**
java.awt.Color - हटाए गए क्षेत्र को भरने के लिए रंग।

### setFillColor(Color value) {#setFillColor-java.awt.Color-}
```
public final void setFillColor(Color value)
```


रेडैक्टेड एरिया को भरने के लिए रंग सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.awt.Color | हटाए गए क्षेत्र को भरने के लिए रंग। |
|

### getSize() {#getSize--}
```
public final Dimension getSize()
```


आयत के चौड़ाई और ऊँचाई को प्राप्त करता है।


**Returns:**
java.awt.Dimension - आयत की चौड़ाई और ऊँचाई।

### setSize(Dimension value) {#setSize-java.awt.Dimension-}
```
public final void setSize(Dimension value)
```


आयत की चौड़ाई और ऊँचाई को सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.awt.Dimension | आयत की चौड़ाई और ऊँचाई। |
|

