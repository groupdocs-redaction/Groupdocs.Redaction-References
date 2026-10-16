---
title: "ReplacementType"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "मिलाए गए टेक्स्ट के लिए प्रतिस्थापन के प्रकार का प्रतिनिधित्व करता है।"
type: docs
weight: 38
url: /hi/java/com.groupdocs.redaction.redactions/replacementtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ReplacementType extends Enum<ReplacementType>
```

मिलाए गए टेक्स्ट के लिए प्रतिस्थापन के प्रकार का प्रतिनिधित्व करता है।

## फ़ील्ड्स

| फ़ील्ड | विवरण |
| --- | --- |
|  | [ReplaceString](#ReplaceString) | मिलते हुए पाठ को किसी अन्य स्ट्रिंग से बदलता है, उदाहरण के लिए। |
|
|  | [DrawBox](#DrawBox) | रेडैक्टेड टेक्स्ट के बजाय विशिष्ट रंग (डिफ़ॉल्ट रूप से काला) का आयत बनाता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### ReplaceString {#ReplaceString}
```
public static final ReplacementType ReplaceString
```


मिलते हुए पाठ को किसी अन्य स्ट्रिंग से बदलता है, उदाहरण के लिए छूट कोड।


### DrawBox {#DrawBox}
```
public static final ReplacementType DrawBox
```


रेडैक्टेड टेक्स्ट के बजाय विशिष्ट रंग (डिफ़ॉल्ट रूप से काला) का आयत बनाता है।


### values() {#values--}
```
public static ReplacementType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.ReplacementType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ReplacementType valueOf(String name)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String |  |

**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype)
