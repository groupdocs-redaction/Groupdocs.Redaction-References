---
title: "RedactionResult"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "रिडैक्शन ऑपरेशन के परिणाम का प्रतिनिधित्व करता है।"
type: docs
weight: 15
url: /hi/java/com.groupdocs.redaction/redactionresult/
---
**Inheritance:**
java.lang.Object
```
public class RedactionResult
```

रिडैक्शन ऑपरेशन के परिणाम का प्रतिनिधित्व करता है।

*** ** * ** ***


**Learn more**

* More details about redaction results: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getStatus()](#getStatus--) | कार्य निष्पादन स्थिति प्राप्त करता है। |
|
|  | [getErrorMessage()](#getErrorMessage--) | डायग्नॉस्टिक्स के लिए त्रुटि संदेश प्राप्त करता है। |
|
|  | [skipped(String description)](#skipped-java.lang.String-) | Skipped स्थिति के साथ RedactionResult क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [partial(String description)](#partial-java.lang.String-) | PartiallyApplied स्थिति के साथ RedactionResult क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [failed(String description)](#failed-java.lang.String-) | Failed स्थिति के साथ RedactionResult क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [successful()](#successful--) | Applied (सफल) स्थिति के साथ RedactionResult क्लास का नया उदाहरण प्रारंभ करता है। |
|
### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


कार्य निष्पादन स्थिति प्राप्त करता है।


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The execution status.

### getErrorMessage() {#getErrorMessage--}
```
public final String getErrorMessage()
```


डायग्नॉस्टिक्स के लिए त्रुटि संदेश प्राप्त करता है।


**Returns:**
java.lang.String - डायग्नॉस्टिक्स के लिए त्रुटि संदेश।

### skipped(String description) {#skipped-java.lang.String-}
```
public static RedactionResult skipped(String description)
```


Skipped स्थिति के साथ RedactionResult क्लास का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | विवरण | java.lang.String | ऑपरेशन को छोड़ने का कारण |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Sskipped redaction result

### partial(String description) {#partial-java.lang.String-}
```
public static RedactionResult partial(String description)
```


PartiallyApplied स्थिति के साथ RedactionResult क्लास का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | विवरण | java.lang.String | ऑपरेशन को पूरी तरह लागू न करने का कारण |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Partially applied redaction result

### failed(String description) {#failed-java.lang.String-}
```
public static RedactionResult failed(String description)
```


Failed स्थिति के साथ RedactionResult क्लास का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | विवरण | java.lang.String | विफलता या अपवाद विवरण |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Failed redaction result

### successful() {#successful--}
```
public static RedactionResult successful()
```


Applied (सफल) स्थिति के साथ RedactionResult क्लास का नया उदाहरण प्रारंभ करता है।


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Successful redaction result

