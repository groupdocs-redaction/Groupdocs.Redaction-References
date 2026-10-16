---
title: "RedactorLogEntry"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "रिडैक्शन लागू करने के परिणामों का प्रतिनिधित्व करता है।"
type: docs
weight: 18
url: /hi/java/com.groupdocs.redaction/redactorlogentry/
---
**Inheritance:**
java.lang.Object
```
public class RedactorLogEntry
```

रिडैक्शन लागू करने के परिणामों का प्रतिनिधित्व करता है।

*** ** * ** ***


**Learn more**

* More details about redaction log entries: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [RedactorLogEntry(Redaction redaction, RedactionResult result)](#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-) | रिडैक्शन के लिए RedactorLogEntry क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getResult()](#getResult--) | परिणाम प्राप्त करता है, जो द्वारा लौटाया गया है |
GroupDocs.Redaction.Integration.DocumentFormatInstance
.
|
|  | [getRedaction()](#getRedaction--) | रेडैक्शन और उसके विकल्पों का संदर्भ प्राप्त करता है। |
|
### RedactorLogEntry(Redaction redaction, RedactionResult result) {#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-}
```
public RedactorLogEntry(Redaction redaction, RedactionResult result)
```


रिडैक्शन के लिए RedactorLogEntry क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | रेडैक्शन का संदर्भ |
|
|  | result | [RedactionResult](../../com.groupdocs.redaction/redactionresult) | फ़ॉर्मेट हैंडलर द्वारा रिपोर्ट किया गया रेडैक्शन परिणाम |
|

### getResult() {#getResult--}
```
public final RedactionResult getResult()
```


परिणाम प्राप्त करता है, जो द्वारा लौटाया गया है
GroupDocs.Redaction.Integration.DocumentFormatInstance
.


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - The result, returned by  GroupDocs.Redaction.Integration.DocumentFormatInstance .

### getRedaction() {#getRedaction--}
```
public final Redaction getRedaction()
```


रेडैक्शन और उसके विकल्पों का संदर्भ प्राप्त करता है।


**Returns:**
[Redaction](../../com.groupdocs.redaction/redaction) - The reference to redaction and its options.

