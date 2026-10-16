---
title: "WordProcessingComplianceLevel"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "वर्ड प्रोसेसिंग दस्तावेज़ों के लिए OOXML अनुपालन स्तर।"
type: docs
weight: 22
url: /hi/java/com.groupdocs.redaction.options/wordprocessingcompliancelevel/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum WordProcessingComplianceLevel extends Enum<WordProcessingComplianceLevel>
```

वर्ड प्रोसेसिंग दस्तावेज़ों के लिए OOXML अनुपालन स्तर। Strict को केवल Transitional में डाउनग्रेड किया जा सकता है, Ecma में नहीं।

## फ़ील्ड्स

| फ़ील्ड | विवरण |
| --- | --- |
|  | [Ecma](#Ecma) | ECMA-376 प्रथम संस्करण, 2006। |
|
|  | [Transitional](#Transitional) | ISO/IEC 29500:2008 Transitional। |
|
|  | [Strict](#Strict) | ISO/IEC 29500:2008 Strict। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ecma {#Ecma}
```
public static final WordProcessingComplianceLevel Ecma
```


ECMA-376 प्रथम संस्करण, 2006।


### Transitional {#Transitional}
```
public static final WordProcessingComplianceLevel Transitional
```


ISO/IEC 29500:2008 Transitional।


### Strict {#Strict}
```
public static final WordProcessingComplianceLevel Strict
```


ISO/IEC 29500:2008 Strict।


### values() {#values--}
```
public static WordProcessingComplianceLevel[] values()
```




**Returns:**
com.groupdocs.redaction.options.WordProcessingComplianceLevel[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static WordProcessingComplianceLevel valueOf(String name)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String |  |

**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
