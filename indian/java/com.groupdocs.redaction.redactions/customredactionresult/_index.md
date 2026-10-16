---
title: "CustomRedactionResult"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "एक परिणाम का प्रतिनिधित्व करता है जो द्वारा लौटाया गया है।"
type: docs
weight: 14
url: /hi/java/com.groupdocs.redaction.redactions/customredactionresult/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionResult
```

एक परिणाम का प्रतिनिधित्व करता है जो [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) द्वारा लौटाया गया है।

## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
| [CustomRedactionResult()](#CustomRedactionResult--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getApply()](#getApply--) | यह दर्शाने वाला मान प्राप्त करता है कि प्रतिस्थापन लागू किया जाना चाहिए या नहीं। |
|
|  | [setApply(boolean value)](#setApply-boolean-) | यह दर्शाने वाला मान सेट करता है कि प्रतिस्थापन लागू किया जाना चाहिए या नहीं। |
|
|  | [getText()](#getText--) | जब #getApply().getApply() है तो उपयोग किया जाने वाला प्रतिस्थापन पाठ प्राप्त करता है |
true
.
|
|  | [setText(String value)](#setText-java.lang.String-) | जब #getApply().getApply() है तो उपयोग किया जाने वाला प्रतिस्थापन पाठ सेट करता है |
true
.
|
### CustomRedactionResult() {#CustomRedactionResult--}
```
public CustomRedactionResult()
```


### getApply() {#getApply--}
```
public final boolean getApply()
```


यह दर्शाने वाला मान प्राप्त करता है कि प्रतिस्थापन लागू किया जाना चाहिए या नहीं।


**Returns:**
boolean -  true  मिलते हुए पाठ को #getText().getText() से बदलने के लिए; अन्यथा,  false ।

### setApply(boolean value) {#setApply-boolean-}
```
public final void setApply(boolean value)
```


यह दर्शाने वाला मान सेट करता है कि प्रतिस्थापन लागू किया जाना चाहिए या नहीं।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | true  प्रतिस्थापन लागू करने के लिए; अन्यथा,  false । |
|

### getText() {#getText--}
```
public final String getText()
```


जब #getApply().getApply() है तो उपयोग किया जाने वाला प्रतिस्थापन पाठ प्राप्त करता है
true
.


**Returns:**
java.lang.String - प्रतिस्थापन पाठ।

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


जब #getApply().getApply() है तो उपयोग किया जाने वाला प्रतिस्थापन पाठ सेट करता है
true
.


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String | प्रतिस्थापन पाठ। |
|

