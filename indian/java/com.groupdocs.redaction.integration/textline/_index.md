---
title: "TextLine"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "इमेज से OCR इंजन द्वारा निकाली गई टेक्स्ट की एक पंक्ति का प्रतिनिधित्व करता है।"
type: docs
weight: 16
url: /hi/java/com.groupdocs.redaction.integration/textline/
---
**Inheritance:**
java.lang.Object
```
public class TextLine
```

OCR इंजन द्वारा छवि से निकाली गई पाठ की पंक्ति को दर्शाता है।

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [TextLine(TextFragment[] fragments)](#TextLine-com.groupdocs.redaction.integration.TextFragment---) | इमेज से OCR इंजन द्वारा निकाली गई टेक्स्ट की पंक्ति का नया इंस्टेंस प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getFragments()](#getFragments--) | पंक्ति में पहचाने गए टेक्स्ट फ्रैगमेंट्स, जैसे प्रतीक और शब्दों, की एक एरे प्राप्त करता है। |
|
|  | [toString()](#toString--) | पहचानी गई टेक्स्ट पंक्ति की टेक्स्ट सामग्री लौटाता है। |
|
### TextLine(TextFragment[] fragments) {#TextLine-com.groupdocs.redaction.integration.TextFragment---}
```
public TextLine(TextFragment[] fragments)
```


इमेज से OCR इंजन द्वारा निकाली गई टेक्स्ट की पंक्ति का नया इंस्टेंस प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | fragments | [TextFragment\[\]](../../com.groupdocs.redaction.integration/textfragment) | टेक्स्ट फ्रैगमेंट्स का प्रारंभिक सेट |
|

### getFragments() {#getFragments--}
```
public final TextFragment[] getFragments()
```


पंक्ति में पहचाने गए टेक्स्ट फ्रैगमेंट्स, जैसे प्रतीक और शब्दों, की एक एरे प्राप्त करता है।


**Returns:**
com.groupdocs.redaction.integration.TextFragment[] - पंक्ति में पहचाने गए टेक्स्ट फ्रैगमेंट्स, जैसे प्रतीक और शब्दों, की एक एरे।

### toString() {#toString--}
```
public String toString()
```


पहचानी गई टेक्स्ट पंक्ति की टेक्स्ट सामग्री लौटाता है।


**Returns:**
java.lang.String - पहचानी गई टेक्स्ट पंक्ति की टेक्स्ट सामग्री

