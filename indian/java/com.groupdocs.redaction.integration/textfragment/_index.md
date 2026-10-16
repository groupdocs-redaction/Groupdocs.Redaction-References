---
title: "TextFragment"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "OCR इंजन द्वारा निकाले गए पहचाने गए पाठ, शब्द, प्रतीक आदि का एक भाग दर्शाता है।"
type: docs
weight: 15
url: /hi/java/com.groupdocs.redaction.integration/textfragment/
---
**Inheritance:**
java.lang.Object
```
public class TextFragment
```

OCR इंजन द्वारा निकाले गए पहचाने गए पाठ (शब्द, प्रतीक, आदि) का भाग दर्शाता है।

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [TextFragment(String text, Rectangle rectangle)](#TextFragment-java.lang.String-java.awt.Rectangle-) | पहचाने गए पाठ फ्रैगमेंट का नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getText()](#getText--) | पहचाने गए टेक्स्ट फ्रैगमेंट की टेक्स्ट सामग्री प्राप्त करता है। |
|
|  | [getRectangle()](#getRectangle--) | पहचाने गए टेक्स्ट फ्रैगमेंट का बाउंडिंग आयत प्राप्त करता है। |
|
|  | [toString()](#toString--) | पहचाने गए टेक्स्ट फ्रैगमेंट की टेक्स्ट सामग्री लौटाता है। |
|
### TextFragment(String text, Rectangle rectangle) {#TextFragment-java.lang.String-java.awt.Rectangle-}
```
public TextFragment(String text, Rectangle rectangle)
```


पहचाने गए पाठ फ्रैगमेंट का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | टेक्स्ट | java.lang.String | पहचाने गए टेक्स्ट फ्रैगमेंट की टेक्स्ट सामग्री |
|
|  | rectangle | java.awt.Rectangle | पहचाने गए टेक्स्ट फ्रैगमेंट का बाउंडिंग आयत |
|

### getText() {#getText--}
```
public final String getText()
```


पहचाने गए टेक्स्ट फ्रैगमेंट की टेक्स्ट सामग्री प्राप्त करता है।


**Returns:**
java.lang.String - पहचाने गए टेक्स्ट फ्रैगमेंट की टेक्स्ट सामग्री।

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


पहचाने गए टेक्स्ट फ्रैगमेंट का बाउंडिंग आयत प्राप्त करता है।


**Returns:**
java.awt.Rectangle - पहचाने गए टेक्स्ट फ्रैगमेंट का बाउंडिंग आयत।

### toString() {#toString--}
```
public String toString()
```


पहचाने गए टेक्स्ट फ्रैगमेंट की टेक्स्ट सामग्री लौटाता है।


**Returns:**
java.lang.String - पहचाने गए टेक्स्ट फ्रैगमेंट की टेक्स्ट सामग्री

