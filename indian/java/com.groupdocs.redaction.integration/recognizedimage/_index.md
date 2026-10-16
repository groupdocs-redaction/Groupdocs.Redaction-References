---
title: "RecognizedImage"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "एक छवि से निकाले गए टेक्स्ट को दर्शाता है, जो उसकी पहचान प्रक्रिया के परिणामस्वरूप है।"
type: docs
weight: 13
url: /hi/java/com.groupdocs.redaction.integration/recognizedimage/
---
**Inheritance:**
java.lang.Object
```
public class RecognizedImage
```

छवि से निकाले गए पाठ को, उसकी पहचान प्रक्रिया के परिणामस्वरूप दर्शाता है।

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [RecognizedImage(TextLine[] lines)](#RecognizedImage-com.groupdocs.redaction.integration.TextLine---) | क्लास की नई इंस्टेंस को प्रारंभ करता है, पहचाने गए लाइनों के सेट का उपयोग करके। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getText()](#getText--) | संरचित पाठ का पाठ्य समकक्ष प्राप्त करता है। |
|
|  | [getLines()](#getLines--) | दस्तावेज़ में पहचानी गई पाठ की लाइनों को उनके टुकड़ों के साथ प्राप्त करता है। |
|
|  | [toString()](#toString--) | संरचित पाठ का पाठ्य समकक्ष प्राप्त करता है। |
|
### RecognizedImage(TextLine[] lines) {#RecognizedImage-com.groupdocs.redaction.integration.TextLine---}
```
public RecognizedImage(TextLine[] lines)
```


क्लास की नई इंस्टेंस को प्रारंभ करता है, पहचाने गए लाइनों के सेट का उपयोग करके।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | lines | [TextLine\[\]](../../com.groupdocs.redaction.integration/textline) | पहचानी गई लाइनों का एक IEnumerable (जैसे सूची या एरे)। |
|

### getText() {#getText--}
```
public final String getText()
```


संरचित पाठ का पाठ्य समकक्ष प्राप्त करता है।


**Returns:**
java.lang.String - संरचित पाठ का पाठ्य समकक्ष।

### getLines() {#getLines--}
```
public final TextLine[] getLines()
```


दस्तावेज़ में पहचानी गई पाठ की लाइनों को उनके टुकड़ों के साथ प्राप्त करता है।


**Returns:**
com.groupdocs.redaction.integration.TextLine[] - दस्तावेज़ में पहचानी गई पाठ की लाइनों के साथ उनके टुकड़े।

### toString() {#toString--}
```
public String toString()
```


संरचित पाठ का पाठ्य समकक्ष प्राप्त करता है।


**Returns:**
java.lang.String - पहचाना गया पाठ

