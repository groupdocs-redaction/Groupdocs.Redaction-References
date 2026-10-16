---
title: "CustomRedactionContext"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "डेटा इनपुट प्रदान करता है।"
type: docs
weight: 13
url: /hi/java/com.groupdocs.redaction.redactions/customredactioncontext/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionContext
```

डेटा इनपुट प्रदान करता है [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler)।

## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
| [CustomRedactionContext()](#CustomRedactionContext--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | मैच किए गए फ्रैगमेंट का पेज नंबर प्राप्त करता है, जब उपलब्ध हो। |
|
|  | [setPageNumber(int value)](#setPageNumber-int-) | मैच किए गए फ्रैगमेंट का पेज नंबर सेट करता है। |
|
|  | [getText()](#getText--) | रेडैक्शन के लिए मैच किया गया टेक्स्ट प्राप्त करता है। |
|
|  | [setText(String value)](#setText-java.lang.String-) | रेडैक्शन के लिए मैच किया गया टेक्स्ट सेट करता है। |
|
### CustomRedactionContext() {#CustomRedactionContext--}
```
public CustomRedactionContext()
```


### getPageNumber() {#getPageNumber--}
```
public final int getPageNumber()
```


मैच किए गए फ्रैगमेंट का पेज नंबर प्राप्त करता है, जब उपलब्ध हो।


**Returns:**
int - पेज नंबर, या यदि पेज ज्ञात नहीं है तो फ़ॉर्मेट-विशिष्ट मान।

### setPageNumber(int value) {#setPageNumber-int-}
```
public final void setPageNumber(int value)
```


मैच किए गए फ्रैगमेंट का पेज नंबर सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | पेज नंबर। |
|

### getText() {#getText--}
```
public final String getText()
```


रेडैक्शन के लिए मैच किया गया टेक्स्ट प्राप्त करता है।


**Returns:**
java.lang.String - मैच किया गया टेक्स्ट।

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


रेडैक्शन के लिए मैच किया गया टेक्स्ट सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String | मैच किया गया टेक्स्ट। |
|

