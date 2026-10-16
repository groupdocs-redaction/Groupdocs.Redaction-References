---
title: "Redactor"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "एक मुख्य क्लास का प्रतिनिधित्व करता है जो दस्तावेज़ रिडैक्शन प्रक्रिया को नियंत्रित करता है, जिससे दस्तावेज़ खोलना, रिडैक्ट करना और सहेजना संभव होता है।"
type: docs
weight: 16
url: /hi/java/com.groupdocs.redaction/redactor/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable, [com.groupdocs.redaction.integration.IPreviewable](../../com.groupdocs.redaction.integration/ipreviewable)
```
public final class Redactor implements Closeable, IPreviewable
```

डॉक्यूमेंट रिडैक्शन प्रक्रिया को नियंत्रित करने वाली मुख्य क्लास का प्रतिनिधित्व करता है, जिससे दस्तावेज़ खोलना, रिडैक्ट करना और सहेजना संभव होता है।

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [Redactor(String filePath)](#Redactor-java.lang.String-) | एक नया इंस्टेंस इनिशियलाइज़ करता है |
Redactor
फ़ाइल पाथ का उपयोग करने वाली क्लास।
|
|  | [Redactor(InputStream document)](#Redactor-java.io.InputStream-) | एक नया इंस्टेंस इनिशियलाइज़ करता है |
Redactor
स्ट्रीम का उपयोग करने वाली क्लास।
|
|  | [Redactor(String filePath, LoadOptions loadOptions)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-) | एक नया इंस्टेंस इनिशियलाइज़ करता है |
Redactor
पाथ का उपयोग करके पासवर्ड-प्रोटेक्टेड दस्तावेज़ के लिए क्लास।
|
|  | [Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | एक नया इंस्टेंस इनिशियलाइज़ करता है |
Redactor
पाथ और सेटिंग्स का उपयोग करके पासवर्ड-प्रोटेक्टेड दस्तावेज़ के लिए क्लास।
|
|  | [Redactor(InputStream document, LoadOptions loadOptions)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-) | एक नया इंस्टेंस इनिशियलाइज़ करता है |
Redactor
स्ट्रीम का उपयोग करके पासवर्ड-प्रोटेक्टेड दस्तावेज़ के लिए क्लास।
|
|  | [Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | एक नया इंस्टेंस इनिशियलाइज़ करता है |
Redactor
स्ट्रीम और सेटिंग्स का उपयोग करके पासवर्ड-प्रोटेक्टेड दस्तावेज़ के लिए क्लास।
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [close()](#close--) | संसाधनों को रिलीज़ करता है। |
|
|  | [apply(Redaction redaction)](#apply-com.groupdocs.redaction.Redaction-) | दस्तावेज़ पर रिडैक्शन लागू करता है। |
|
|  | [apply(Redaction[] redactions)](#apply-com.groupdocs.redaction.Redaction---) | दस्तावेज़ पर रिडैक्शन का सेट लागू करता है। |
|
|  | [apply(RedactionPolicy policy)](#apply-com.groupdocs.redaction.RedactionPolicy-) | दस्तावेज़ पर रिडैक्शन नीति लागू करता है। |
|
|  | [save()](#save--) | दस्तावेज़ को फ़ाइल में निम्न विकल्पों के साथ सहेजता है: AddSuffix = true, RasterizeToPDF = true। |
|
|  | [save(SaveOptions saveOptions)](#save-com.groupdocs.redaction.options.SaveOptions-) | दस्तावेज़ को फ़ाइल में सहेजता है। |
|
|  | [save(OutputStream document)](#save-java.io.OutputStream-) | दस्तावेज़ को स्ट्रीम में सहेजता है। |
|
|  | [save(OutputStream document, SaveOptions saveOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-) | दस्तावेज़ को स्ट्रीम में सहेजता है। |
|
|  | [save(OutputStream document, RasterizationOptions rasterizationOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-) | कस्टम लोकेशन सहित दस्तावेज़ को स्ट्रीम में सहेजता है। |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.redaction.options.PreviewOptions-) | निर्दिष्ट इमेज फ़ॉर्मेट में विशिष्ट पृष्ठों की प्रीव्यू इमेज बनाता है। |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | दस्तावेज़ की सामान्य जानकारी प्राप्त करता है - आकार, पृष्ठ गिनती, आदि। |
|
### Redactor(String filePath) {#Redactor-java.lang.String-}
```
public Redactor(String filePath)
```


एक नया इंस्टेंस इनिशियलाइज़ करता है
Redactor
फ़ाइल पाथ का उपयोग करने वाली क्लास।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filePath | java.lang.String | फ़ाइल का पाथ |


निम्न उदाहरण दर्शाता है कि रिडैक्शन के लिए दस्तावेज़ कैसे खोलें।

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
     // Here we can use document instance to perform redactions
 }
 
``` 
````

 |

### Redactor(InputStream document) {#Redactor-java.io.InputStream-}
```
public Redactor(InputStream document)
```


Initializes a new instance of 
Redactor
 class using stream.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.InputStream | Source stream of the document


The following example demonstrates how to open a document from stream.

````

try (InputStream stream = new FileInputStream("C:\\sample.pdf"))
{
try (Redactor redactor = new Redactor(stream))
{
// यहाँ हम दस्तावेज़ इंस्टेंस का उपयोग करके रेडैक्शन कर सकते हैं
}
}
 
``` 
````

|

### Redactor(String filePath, LoadOptions loadOptions) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(String filePath, LoadOptions loadOptions)
```


एक नया इंस्टेंस इनिशियलाइज़ करता है
Redactor
पाथ का उपयोग करके पासवर्ड-प्रोटेक्टेड दस्तावेज़ के लिए क्लास।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filePath | java.lang.String | फ़ाइल का पथ। |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | विकल्प, जिसमें पासवर्ड शामिल है। |
|

### Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)
```


एक नया इंस्टेंस इनिशियलाइज़ करता है
Redactor
पाथ और सेटिंग्स का उपयोग करके पासवर्ड-प्रोटेक्टेड दस्तावेज़ के लिए क्लास।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filePath | java.lang.String | फ़ाइल का पथ। |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | फ़ाइल-निर्भर विकल्प, जिसमें पासवर्ड शामिल है। |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | रेडैक्शन प्रक्रिया के लिए डिफ़ॉल्ट सेटिंग्स। |
|

### Redactor(InputStream document, LoadOptions loadOptions) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(InputStream document, LoadOptions loadOptions)
```


एक नया इंस्टेंस इनिशियलाइज़ करता है
Redactor
स्ट्रीम का उपयोग करके पासवर्ड-प्रोटेक्टेड दस्तावेज़ के लिए क्लास।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | दस्तावेज़ | java.io.InputStream | स्रोत इनपुट स्ट्रीम। |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | विकल्प, जिसमें पासवर्ड शामिल है। |
|

### Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)
```


एक नया इंस्टेंस इनिशियलाइज़ करता है
Redactor
स्ट्रीम और सेटिंग्स का उपयोग करके पासवर्ड-प्रोटेक्टेड दस्तावेज़ के लिए क्लास।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | दस्तावेज़ | java.io.InputStream | स्रोत इनपुट स्ट्रीम। |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | विकल्प, जिसमें पासवर्ड शामिल है। |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | रेडैक्शन प्रक्रिया के लिए डिफ़ॉल्ट सेटिंग्स। |
|

### close() {#close--}
```
public final void close()
```


संसाधनों को रिलीज़ करता है।


### apply(Redaction redaction) {#apply-com.groupdocs.redaction.Redaction-}
```
public final RedactorChangeLog apply(Redaction redaction)
```


दस्तावेज़ पर रिडैक्शन लागू करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | एक उदाहरण  Redaction  लागू करने के लिए |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(Redaction[] redactions) {#apply-com.groupdocs.redaction.Redaction---}
```
public final RedactorChangeLog apply(Redaction[] redactions)
```


दस्तावेज़ पर रिडैक्शन का सेट लागू करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | एक सरणी redactions लागू करने के लिए |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(RedactionPolicy policy) {#apply-com.groupdocs.redaction.RedactionPolicy-}
```
public final RedactorChangeLog apply(RedactionPolicy policy)
```


दस्तावेज़ पर रिडैक्शन नीति लागू करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | policy | [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) | Redaction नीति |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### save() {#save--}
```
public final String save()
```


दस्तावेज़ को फ़ाइल में निम्न विकल्पों के साथ सहेजता है: AddSuffix = true, RasterizeToPDF = true।


**Returns:**
java.lang.String - रेडैक्टेड दस्तावेज़ का पथ

### save(SaveOptions saveOptions) {#save-com.groupdocs.redaction.options.SaveOptions-}
```
public final String save(SaveOptions saveOptions)
```


दस्तावेज़ को फ़ाइल में सहेजता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | सफ़िक्स जोड़ने या रास्टराइज़ करने के विकल्प |
|

**Returns:**
java.lang.String - रेडैक्टेड दस्तावेज़ का पथ

### save(OutputStream document) {#save-java.io.OutputStream-}
```
public final void save(OutputStream document)
```


दस्तावेज़ को स्ट्रीम में सहेजता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | दस्तावेज़ | java.io.OutputStream | लक्ष्य स्ट्रीम |
|

### save(OutputStream document, SaveOptions saveOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-}
```
public final void save(OutputStream document, SaveOptions saveOptions)
```


दस्तावेज़ को स्ट्रीम में सहेजता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | दस्तावेज़ | java.io.OutputStream | लक्ष्य स्ट्रीम |
|
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | सहेजने के विकल्प |
|

### save(OutputStream document, RasterizationOptions rasterizationOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-}
```
public final void save(OutputStream document, RasterizationOptions rasterizationOptions)
```


कस्टम लोकेशन सहित दस्तावेज़ को स्ट्रीम में सहेजता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | दस्तावेज़ | java.io.OutputStream | लक्ष्य स्ट्रीम |
|
|  | rasterizationOptions | [RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) | रास्टराइज़ करने या न करने और रास्टराइज़ेशन के लिए पृष्ठ निर्दिष्ट करने के विकल्प |
|

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.redaction.options.PreviewOptions-}
```
public final void generatePreview(PreviewOptions previewOptions)
```


निर्दिष्ट इमेज फ़ॉर्मेट में विशिष्ट पृष्ठों की प्रीव्यू इमेज बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.redaction.options/previewoptions) | छवि गुण और पृष्ठ रेंज सेटिंग्स |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public final IDocumentInfo getDocumentInfo()
```


दस्तावेज़ की सामान्य जानकारी प्राप्त करता है - आकार, पृष्ठ गिनती, आदि।


**Returns:**
[IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo) - An instance of IDocumentInfo

