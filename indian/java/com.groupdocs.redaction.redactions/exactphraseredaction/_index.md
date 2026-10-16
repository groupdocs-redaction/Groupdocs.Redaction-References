---
title: "ExactPhraseRedaction"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "डिफ़ॉल्ट रूप से केस-इन्सेंसिटिव होकर दस्तावेज़ के पाठ में सटीक वाक्यांश को बदलने वाला एक टेक्स्ट रेडैक्शन दर्शाता है।"
type: docs
weight: 17
url: /hi/java/com.groupdocs.redaction.redactions/exactphraseredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class ExactPhraseRedaction extends TextRedaction
```

एक टेक्स्ट रेडैक्शन को दर्शाता है जो दस्तावेज़ के टेक्स्ट में सटीक वाक्यांश को बदलता है, डिफ़ॉल्ट रूप से केस-इंसेंसिटिव।

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />

निम्नलिखित उदाहरण केस-सेंसिटिव वाक्यांश खोज और प्रतिस्थापन को प्रदर्शित करता है।

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
   // By default, the second parameter, isCaseSensitive = false;
   doc.apply(new ExactPhraseRedaction("John Doe", true, new ReplacementOptions("[personal]")));
   doc.save();
 }
 
``` 
````

The following example demonstrates replacing phrase (case insensitive) with solid red rectangle.

````

try (Redactor redactor = new Redactor("C:\\sample.pdf"))
{
// डिफ़ॉल्ट रूप से, isCaseSensitive = false;
doc.apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(System.Drawing.Color.Red)));
doc.save();
}
 
``` 
````


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | केस-इन्सेंसिटिव मोड में ExactPhraseRedaction क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-) | ExactPhraseRedaction क्लास का नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getSearchPhrase()](#getSearchPhrase--) | खोज और प्रतिस्थापन के लिए स्ट्रिंग प्राप्त करता है। |
|
|  | [isCaseSensitive()](#isCaseSensitive--) | एक मान प्राप्त करता है जो दर्शाता है कि खोज केस-सेंसिटिव है या नहीं। |
|
|  | [isRightToLeft()](#isRightToLeft--) | एक मान प्राप्त करता है जो दर्शाता है कि यह टेक्स्ट दाएँ‑से‑बाएँ है या नहीं, डिफ़ॉल्ट रूप से false। |
|
|  | [setRightToLeft(boolean value)](#setRightToLeft-boolean-) | एक मान सेट करता है जो दर्शाता है कि यह टेक्स्ट दाएँ‑से‑बाएँ है या नहीं, डिफ़ॉल्ट रूप से false। |
|
|  | [getDescription()](#getDescription--) | एक स्ट्रिंग लौटाता है, जो रेडैक्शन और उसके पैरामीटरों का वर्णन करती है। |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | दिए गए फ़ॉर्मेट इंस्टेंस पर रेडैक्शन लागू करता है। |
|
### ExactPhraseRedaction(String searchPhrase, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)
```


केस-इन्सेंसिटिव मोड में ExactPhraseRedaction क्लास का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | खोज और प्रतिस्थापन के लिए स्ट्रिंग |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | प्रतिस्थापन विकल्प (पाठ्य, रंग) |
|

### ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)
```


ExactPhraseRedaction क्लास का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | खोज और प्रतिस्थापन के लिए स्ट्रिंग |
|
|  | isCaseSensitive | boolean | यदि केस‑सेंसिटिव खोज आवश्यक है तो true |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | प्रतिस्थापन विकल्प (पाठ्य, रंग) |
|

### getSearchPhrase() {#getSearchPhrase--}
```
public final String getSearchPhrase()
```


खोज और प्रतिस्थापन के लिए स्ट्रिंग प्राप्त करता है।


**Returns:**
java.lang.String - खोज और प्रतिस्थापन के लिए स्ट्रिंग।

### isCaseSensitive() {#isCaseSensitive--}
```
public final boolean isCaseSensitive()
```


एक मान प्राप्त करता है जो दर्शाता है कि खोज केस-सेंसिटिव है या नहीं।


**Returns:**
boolean - एक मान जो दर्शाता है कि खोज केस‑सेंसिटिव है या नहीं।

### isRightToLeft() {#isRightToLeft--}
```
public final boolean isRightToLeft()
```


एक मान प्राप्त करता है जो दर्शाता है कि यह टेक्स्ट दाएँ‑से‑बाएँ है या नहीं, डिफ़ॉल्ट रूप से false।


**Returns:**
boolean - एक मान जो दर्शाता है कि यह टेक्स्ट दाएँ‑से‑बाएँ है या नहीं, डिफ़ॉल्ट रूप से false।

### setRightToLeft(boolean value) {#setRightToLeft-boolean-}
```
public final void setRightToLeft(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि यह टेक्स्ट दाएँ‑से‑बाएँ है या नहीं, डिफ़ॉल्ट रूप से false।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | एक मान जो दर्शाता है कि यह टेक्स्ट दाएँ‑से‑बाएँ है या नहीं, डिफ़ॉल्ट रूप से false। |
|

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

