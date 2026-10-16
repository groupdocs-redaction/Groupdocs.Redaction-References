---
title: "RedactionActionType"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "रिडैक्शन करने के लिए ली जा सकने वाली कार्रवाइयों का प्रतिनिधित्व करता है।"
type: docs
weight: 37
url: /hi/java/com.groupdocs.redaction.redactions/redactionactiontype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionActionType extends Enum<RedactionActionType>
```

रिडैक्शन करने के लिए ली जा सकने वाली कार्रवाइयों का प्रतिनिधित्व करता है।

## फ़ील्ड्स

| फ़ील्ड | विवरण |
| --- | --- |
|  | [Replacement](#Replacement) | रेडैक्टेड टेक्स्ट को किसी अन्य से बदल दिया गया या ब्लॉक से ढका गया। |
|
|  | [Cleanup](#Cleanup) | डेटा हटा दिया गया, लेकिन एक खाली ऑब्जेक्ट दस्तावेज़ में बना रहता है। |
|
|  | [Deletion](#Deletion) | डेटा और संबंधित संरचनाएँ दस्तावेज़ से हटा दी गईं। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Replacement {#Replacement}
```
public static final RedactionActionType Replacement
```


रेडैक्टेड टेक्स्ट को किसी अन्य से बदल दिया गया या ब्लॉक से ढका गया।


### Cleanup {#Cleanup}
```
public static final RedactionActionType Cleanup
```


डेटा हटा दिया गया, लेकिन एक खाली ऑब्जेक्ट दस्तावेज़ में बना रहता है।


### Deletion {#Deletion}
```
public static final RedactionActionType Deletion
```


डेटा और संबंधित संरचनाएँ दस्तावेज़ से हटा दी गईं।


### values() {#values--}
```
public static RedactionActionType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.RedactionActionType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionActionType valueOf(String name)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String |  |

**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype)
