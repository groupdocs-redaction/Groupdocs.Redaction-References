---
title: "TextReplacement"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "टेक्स्टुअल प्रतिस्थापन जानकारी का प्रतिनिधित्व करता है।"
type: docs
weight: 33
url: /hi/java/com.groupdocs.redaction.redactions/textreplacement/
---
**Inheritance:**
java.lang.Object
```
public class TextReplacement
```

टेक्स्टुअल प्रतिस्थापन जानकारी का प्रतिनिधित्व करता है।

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [TextReplacement(int index, String original, String replacement)](#TextReplacement-int-java.lang.String-java.lang.String-) | TextReplacement क्लास की नई इंस्टेंस को प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getIndex()](#getIndex--) | स्रोत स्ट्रिंग के भीतर मेल खाए टेक्स्ट का इंडेक्स प्राप्त करता है। |
|
|  | [getOriginalText()](#getOriginalText--) | मूल मेल खाए स्ट्रिंग को प्राप्त करता है। |
|
|  | [getReplacement()](#getReplacement--) | OriginalText को बदलते हुए स्ट्रिंग प्राप्त करता है। |
|
|  | [toString()](#toString--) | पाठ प्रतिस्थापन विवरण और उसकी स्थिति प्रदान करता है। |
|
### TextReplacement(int index, String original, String replacement) {#TextReplacement-int-java.lang.String-java.lang.String-}
```
public TextReplacement(int index, String original, String replacement)
```


TextReplacement क्लास की नई इंस्टेंस को प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | इंडेक्स | int | स्रोत स्ट्रिंग में मिलते हुए पाठ का सूचकांक |
|
|  | मूल | java.lang.String | मूल मिलती स्ट्रिंग |
|
|  | प्रतिस्थापन | java.lang.String | स्ट्रिंग, स्रोत स्ट्रिंग में OriginalText को बदलते हुए |
|

### getIndex() {#getIndex--}
```
public final int getIndex()
```


स्रोत स्ट्रिंग के भीतर मेल खाए टेक्स्ट का इंडेक्स प्राप्त करता है।


**Returns:**
int - स्रोत स्ट्रिंग में मिलते हुए पाठ का सूचकांक।

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


मूल मेल खाए स्ट्रिंग को प्राप्त करता है।


**Returns:**
java.lang.String - मूल मिलती स्ट्रिंग।

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


OriginalText को बदलते हुए स्ट्रिंग प्राप्त करता है।


**Returns:**
java.lang.String - स्ट्रिंग, OriginalText को बदलते हुए।

### toString() {#toString--}
```
public String toString()
```


पाठ प्रतिस्थापन विवरण और उसकी स्थिति प्रदान करता है।


**Returns:**
java.lang.String - प्रतिस्थापन विवरण

