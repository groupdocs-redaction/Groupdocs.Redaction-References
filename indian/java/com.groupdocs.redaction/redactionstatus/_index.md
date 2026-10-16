---
title: "RedactionStatus"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "रिडैक्शन पूर्णता स्थिति का प्रतिनिधित्व करता है।"
type: docs
weight: 20
url: /hi/java/com.groupdocs.redaction/redactionstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionStatus extends Enum<RedactionStatus>
```

रिडैक्शन पूर्णता स्थिति का प्रतिनिधित्व करता है।

## फ़ील्ड्स

| फ़ील्ड | विवरण |
| --- | --- |
|  | [Applied](#Applied) | रेडैक्शन पूरी तरह और सफलतापूर्वक लागू किया गया। |
|
|  | [PartiallyApplied](#PartiallyApplied) | रेडैक्शन केवल उसके मिलानों के एक भाग पर लागू किया गया। |
|
|  | [Skipped](#Skipped) | रेडैक्शन को छोड़ दिया गया (लागू नहीं किया गया)। |
|
|  | [Failed](#Failed) | रेडैक्शन अपवाद के साथ विफल हुआ। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Applied {#Applied}
```
public static final RedactionStatus Applied
```


रेडैक्शन पूरी तरह और सफलतापूर्वक लागू किया गया।


### PartiallyApplied {#PartiallyApplied}
```
public static final RedactionStatus PartiallyApplied
```


रेडैक्शन केवल उसके मिलानों के एक भाग पर लागू किया गया।


### Skipped {#Skipped}
```
public static final RedactionStatus Skipped
```


रेडैक्शन को छोड़ दिया गया (लागू नहीं किया गया)।


### Failed {#Failed}
```
public static final RedactionStatus Failed
```


रेडैक्शन अपवाद के साथ विफल हुआ।


### values() {#values--}
```
public static RedactionStatus[] values()
```




**Returns:**
com.groupdocs.redaction.RedactionStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionStatus valueOf(String name)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String |  |

**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus)
