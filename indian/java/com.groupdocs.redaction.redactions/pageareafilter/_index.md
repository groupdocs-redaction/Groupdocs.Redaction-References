---
title: "PageAreaFilter"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "एक दस्तावेज़ के पृष्ठ के भीतर एक क्षेत्र को रेडैक्शन लागू करने के लिए सेट करने वाले रेडैक्शन फ़िल्टर का प्रतिनिधित्व करता है।"
type: docs
weight: 22
url: /hi/java/com.groupdocs.redaction.redactions/pageareafilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageAreaFilter extends RedactionFilter
```

रिडैक्शन फ़िल्टर का प्रतिनिधित्व करता है, जो दस्तावेज़ के पृष्ठ के भीतर एक क्षेत्र निर्धारित करता है जहाँ रिडैक्शन लागू किया जाता है।

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [PageAreaFilter(Point topLeft, Dimension size)](#PageAreaFilter-java.awt.Point-java.awt.Dimension-) | विशिष्ट क्षेत्र को रेडैक्ट करने के लिए PageAreaFilter क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | पृष्ठ पर आयत (ऊपरी-बाएँ स्थिति और क्षेत्र का आकार) प्राप्त करता है। |
|
|  | [isInTheArea(Rectangle rectangle)](#isInTheArea-java.awt.Rectangle-) | जाँचता है कि यह फ़िल्टर क्षेत्र दिए गए आयत के साथ प्रतिच्छेद करता है या नहीं। |
|
### PageAreaFilter(Point topLeft, Dimension size) {#PageAreaFilter-java.awt.Point-java.awt.Dimension-}
```
public PageAreaFilter(Point topLeft, Dimension size)
```


विशिष्ट क्षेत्र को रेडैक्ट करने के लिए PageAreaFilter क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | topLeft | java.awt.Point | ऊपरी-बाएँ क्षेत्र के निर्देशांक |
|
|  | size | java.awt.Dimension | क्षेत्र का आकार और रंग |
|

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


पृष्ठ पर आयत (ऊपरी-बाएँ स्थिति और क्षेत्र का आकार) प्राप्त करता है।


**Returns:**
java.awt.Rectangle - पृष्ठ पर आयत (ऊपरी-बाएँ स्थिति और क्षेत्र का आकार)।

### isInTheArea(Rectangle rectangle) {#isInTheArea-java.awt.Rectangle-}
```
public final boolean isInTheArea(Rectangle rectangle)
```


जाँचता है कि यह फ़िल्टर क्षेत्र दिए गए आयत के साथ प्रतिच्छेद करता है या नहीं।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | java.awt.Rectangle | जाँचने के लिए आयत |
|

**Returns:**
boolean - true, यदि यह फ़िल्टर क्षेत्र प्रतिच्छेद करता है

