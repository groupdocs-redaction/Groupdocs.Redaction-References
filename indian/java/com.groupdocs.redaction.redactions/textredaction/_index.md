---
title: "TextRedaction"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "दस्तावेज़ टेक्स्ट रिडैक्शन के लिए एक बेस एब्स्ट्रैक्ट क्लास का प्रतिनिधित्व करता है।"
type: docs
weight: 32
url: /hi/java/com.groupdocs.redaction.redactions/textredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class TextRedaction extends Redaction
```

दस्तावेज़ टेक्स्ट रिडैक्शन के लिए एक बेस एब्स्ट्रैक्ट क्लास का प्रतिनिधित्व करता है।

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getActionOptions()](#getActionOptions--) | प्राप्त करता है |
ReplacementOptions
इंस्टेंस, टेक्स्ट प्रतिस्थापन के प्रकार को निर्दिष्ट करता है।
|
|  | [getOcrConnector()](#getOcrConnector--) | प्राप्त करता है |
IOcrConnector
इम्प्लीमेंटेशन, ग्राफिक सामग्री से टेक्स्ट निकालने के लिए आवश्यक है।
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | सेट करता है |
IOcrConnector
इम्प्लीमेंटेशन, ग्राफिक सामग्री से टेक्स्ट निकालने के लिए आवश्यक है।
|
### getActionOptions() {#getActionOptions--}
```
public final ReplacementOptions getActionOptions()
```


प्राप्त करता है
ReplacementOptions
इंस्टेंस, टेक्स्ट प्रतिस्थापन के प्रकार को निर्दिष्ट करता है।


**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) - The  ReplacementOptions  instance, specifying type of text replacement.

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


प्राप्त करता है
IOcrConnector
इम्प्लीमेंटेशन, ग्राफिक सामग्री से टेक्स्ट निकालने के लिए आवश्यक है।


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - The  IOcrConnector  implementation, required to extract text from graphic content.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


सेट करता है
IOcrConnector
इम्प्लीमेंटेशन, ग्राफिक सामग्री से टेक्स्ट निकालने के लिए आवश्यक है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector इम्प्लीमेंटेशन, ग्राफिक सामग्री से टेक्स्ट निकालने के लिए आवश्यक है। |
|

