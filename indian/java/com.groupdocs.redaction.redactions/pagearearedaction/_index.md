---
title: "PageAreaRedaction"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "पृष्ठ के एक क्षेत्र में टेक्स्ट इमेज़ और एनोटेशन को प्रभावित करने वाले जटिल टेक्स्टुअल रेडैक्शन का प्रतिनिधित्व करता है।"
type: docs
weight: 23
url: /hi/java/com.groupdocs.redaction.redactions/pagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction), [com.groupdocs.redaction.redactions.RegexRedaction](../../com.groupdocs.redaction.redactions/regexredaction)
```
public class PageAreaRedaction extends RegexRedaction
```

पृष्ठ के एक क्षेत्र में टेक्स्ट, इमेज और एनोटेशन को प्रभावित करने वाली जटिल टेक्स्टुअल रिडैक्शन का प्रतिनिधित्व करता है।

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](../https://docs.groupdocs.com/redaction/java/use-page-area-redaction/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [PageAreaRedaction(Pattern regex, ReplacementOptions options)](#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | PageAreaRedaction क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions)](#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | PageAreaRedaction क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getImageOptions()](#getImageOptions--) | प्राप्त करता है |
RegionReplacementOptions
रंग और क्षेत्र पैरामीटरों के साथ विकल्प।
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | दिए गए फ़ॉर्मेट इंस्टेंस पर रेडैक्शन लागू करता है। |
|
### PageAreaRedaction(Pattern regex, ReplacementOptions options) {#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public PageAreaRedaction(Pattern regex, ReplacementOptions options)
```


PageAreaRedaction क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | रेजेक्स | java.util.regex.Pattern | खोज और प्रतिस्थापन के लिए नियमित अभिव्यक्ति |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | प्रतिस्थापन विकल्प (पाठ्य, रंग) |
|

### PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions) {#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions)
```


PageAreaRedaction क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | रेजेक्स | java.util.regex.Pattern | खोज और प्रतिस्थापन के लिए नियमित अभिव्यक्ति |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | प्रतिस्थापन विकल्प (पाठ्य, रंग) |
|
|  | imageOptions | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | रिप्लेसमेंट विकल्प (इमेज़ क्षेत्र) |
|

### getImageOptions() {#getImageOptions--}
```
public final RegionReplacementOptions getImageOptions()
```


प्राप्त करता है
RegionReplacementOptions
रंग और क्षेत्र पैरामीटरों के साथ विकल्प।


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

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

