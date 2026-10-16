---
title: "रिडैक्शन"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "सभी रिडैक्शन प्रकारों के लिए एक बेस एब्स्ट्रैक्ट क्लास का प्रतिनिधित्व करता है।"
type: docs
weight: 13
url: /hi/java/com.groupdocs.redaction/redaction/
---
**Inheritance:**
java.lang.Object
```
public abstract class Redaction
```

सभी रिडैक्शन प्रकारों के लिए एक बेस एब्स्ट्रैक्ट क्लास का प्रतिनिधित्व करता है।

*** ** * ** ***


**Learn more**

* More details about redaction types: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
| [Redaction()](#Redaction--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getDescription()](#getDescription--) | एक स्ट्रिंग लौटाता है, जो रेडैक्शन और उसके पैरामीटरों का वर्णन करती है। |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | दिए गए फ़ॉर्मेट इंस्टेंस पर रेडैक्शन लागू करता है। |
|
### Redaction() {#Redaction--}
```
public Redaction()
```


### getDescription() {#getDescription--}
```
public String getDescription()
```


एक स्ट्रिंग लौटाता है, जो रेडैक्शन और उसके पैरामीटरों का वर्णन करती है।


**Returns:**
java.lang.String - टेक्स्ट, जिसमें रेडैक्शन नाम और पैरामीटर होते हैं।

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public abstract RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


दिए गए फ़ॉर्मेट इंस्टेंस पर रेडैक्शन लागू करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | रेडैक्शन लागू करने के लिए दस्तावेज़ का एक इंस्टेंस |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

