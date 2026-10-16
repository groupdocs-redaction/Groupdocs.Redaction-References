---
title: "RegexRedaction"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "प्रदान किए गए रेगुलर एक्सप्रेशन से मिलाते हुए दस्तावेज़ में टेक्स्ट खोजता और बदलता है, ऐसी टेक्स्ट रिडैक्शन का प्रतिनिधित्व करता है।"
type: docs
weight: 28
url: /hi/java/com.groupdocs.redaction.redactions/regexredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class RegexRedaction extends TextRedaction
```

प्रदान किए गए रेगुलर एक्सप्रेशन से मिलाते हुए दस्तावेज़ में टेक्स्ट खोजता और बदलता है, ऐसी टेक्स्ट रिडैक्शन का प्रतिनिधित्व करता है।

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [RegexRedaction(String pattern, ReplacementOptions options)](#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | RegexRedaction क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [RegexRedaction(Pattern regex, ReplacementOptions options)](#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | RegexRedaction क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getRegularExpression()](#getRegularExpression--) | मैच करने के लिए नियमित अभिव्यक्ति प्राप्त करता है। |
|
|  | [getDescription()](#getDescription--) | एक स्ट्रिंग लौटाता है, जो रेडैक्शन और उसके पैरामीटरों का वर्णन करती है। |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | दिए गए फ़ॉर्मेट इंस्टेंस पर रेडैक्शन लागू करता है। |
|
### RegexRedaction(String pattern, ReplacementOptions options) {#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(String pattern, ReplacementOptions options)
```


RegexRedaction क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | पैटर्न | java.lang.String | खोज और प्रतिस्थापन के लिए नियमित अभिव्यक्ति |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | प्रतिस्थापन विकल्प (पाठ्य, रंग) |
|

### RegexRedaction(Pattern regex, ReplacementOptions options) {#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(Pattern regex, ReplacementOptions options)
```


RegexRedaction क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | रेजेक्स | java.util.regex.Pattern | खोज और प्रतिस्थापन के लिए नियमित अभिव्यक्ति |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | प्रतिस्थापन विकल्प (पाठ्य, रंग) |
|

### getRegularExpression() {#getRegularExpression--}
```
public final Pattern getRegularExpression()
```


मैच करने के लिए नियमित अभिव्यक्ति प्राप्त करता है।


**Returns:**
java.util.regex.Pattern - मिलाने के लिए नियमित अभिव्यक्ति।

### getDescription() {#getDescription--}
```
public String getDescription()
```


एक स्ट्रिंग लौटाता है, जो रेडैक्शन और उसके पैरामीटरों का वर्णन करती है।


**Returns:**
java.lang.String - टेक्स्ट, जिसमें रेडैक्शन नाम और पैरामीटर होते हैं।

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

