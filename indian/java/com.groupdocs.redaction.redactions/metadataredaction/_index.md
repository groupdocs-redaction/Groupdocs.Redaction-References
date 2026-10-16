---
title: "MetadataRedaction"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "दस्तावेज़ मेटाडेटा रिडैक्शन के लिए एक बेस एब्स्ट्रैक्ट क्लास का प्रतिनिधित्व करता है।"
type: docs
weight: 20
url: /hi/java/com.groupdocs.redaction.redactions/metadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class MetadataRedaction extends Redaction
```

दस्तावेज़ मेटाडेटा रिडैक्शन के लिए एक बेस एब्स्ट्रैक्ट क्लास का प्रतिनिधित्व करता है।

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Metadata redactions](../https://docs.groupdocs.com/redaction/java/metadata-redactions/)

<br />


## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getFilter()](#getFilter--) | फ़िल्टर प्राप्त करता है, जिसका उपयोग सभी या विशिष्ट मेटाडेटा, जैसे Author या Company, चुनने के लिए किया जाता है। |
|
|  | [setFilter(int value)](#setFilter-int-) | फ़िल्टर सेट करता है, जिसका उपयोग सभी या विशिष्ट मेटाडेटा, जैसे Author या Company, चुनने के लिए किया जाता है। |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | दिए गए फ़ॉर्मेट इंस्टेंस पर रेडैक्शन लागू करता है। |
|
### getFilter() {#getFilter--}
```
public final int getFilter()
```


फ़िल्टर प्राप्त करता है, जिसका उपयोग सभी या विशिष्ट मेटाडेटा, जैसे Author या Company, चुनने के लिए किया जाता है।


**Returns:**
int - फ़िल्टर, जिसका उपयोग सभी या विशिष्ट मेटाडेटा, जैसे Author या Company, चुनने के लिए किया जाता है।

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


फ़िल्टर सेट करता है, जिसका उपयोग सभी या विशिष्ट मेटाडेटा, जैसे Author या Company, चुनने के लिए किया जाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | फ़िल्टर, जिसका उपयोग सभी या विशिष्ट मेटाडेटा, जैसे Author या Company, चुनने के लिए किया जाता है। |
|

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

