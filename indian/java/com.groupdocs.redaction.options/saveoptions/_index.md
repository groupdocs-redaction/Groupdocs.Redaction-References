---
title: "SaveOptions"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "आउटपुट फ़ाइल नाम बदलने और/या दस्तावेज़ को छवि-आधारित PDF रास्टराइज़ेशन में परिवर्तित करने के विकल्प प्रदान करता है।"
type: docs
weight: 14
url: /hi/java/com.groupdocs.redaction.options/saveoptions/
---
**Inheritance:**
java.lang.Object
```
public class SaveOptions
```

आउटपुट फ़ाइल नाम बदलने और/या दस्तावेज़ को इमेज-आधारित PDF (रास्टराइज़ेशन) में परिवर्तित करने के विकल्प प्रदान करता है।

*** ** * ** ***


**Learn more**

* [Save with default options](../https://docs.groupdocs.com/redaction/java/save-with-default-options/)
* [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](../https://docs.groupdocs.com/redaction/java/save-in-original-format/)
* [Save overwriting original file](../https://docs.groupdocs.com/redaction/java/save-overwriting-original-file/)
* [Save to stream](../https://docs.groupdocs.com/redaction/java/save-to-stream/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [SaveOptions()](#SaveOptions--) | डिफ़ॉल्ट मानों के साथ एक नया उदाहरण प्रारंभ करता है: PDF में रास्टराइज़ करना - false, उपसर्ग जोड़ना - false। |
|
|  | [SaveOptions(boolean rasterizeToPdf, String suffix)](#SaveOptions-boolean-java.lang.String-) | दिए गए पैरामीटरों के साथ एक नया इंस्टेंस प्रारंभ करता है। |
|
## फ़ील्ड्स

| फ़ील्ड | विवरण |
| --- | --- |
|  | [SaveSuffix](#SaveSuffix) | डिफ़ॉल्ट सफ़िक्स मान को दर्शाता है, जो "Redacted" है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getAddSuffix()](#getAddSuffix--) | फ़ाइल नाम को सहेजने से पहले बदलने की आवश्यकता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
|
|  | [setAddSuffix(boolean value)](#setAddSuffix-boolean-) | फ़ाइल नाम को सहेजने से पहले बदलने की आवश्यकता है या नहीं, यह दर्शाने वाला मान सेट करता है। |
|
|  | [getRedactedFileSuffix()](#getRedactedFileSuffix--) | आउटपुट फ़ाइल नाम के लिए एक कस्टम सफ़िक्स प्राप्त करता है। |
|
|  | [setRedactedFileSuffix(String value)](#setRedactedFileSuffix-java.lang.String-) | आउटपुट फ़ाइल नाम के लिए एक कस्टम सफ़िक्स सेट करता है। |
|
|  | [getRasterizeToPDF()](#getRasterizeToPDF--) | दस्तावेज़ के सभी पृष्ठों को छवियों में परिवर्तित करके एक ही PDF फ़ाइल में रखने की आवश्यकता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
|
|  | [setRasterizeToPDF(boolean value)](#setRasterizeToPDF-boolean-) | दस्तावेज़ के सभी पृष्ठों को छवियों में परिवर्तित करके एक ही PDF फ़ाइल में रखने की आवश्यकता है या नहीं, यह दर्शाने वाला मान सेट करता है। |
|
|  | [getRasterization()](#getRasterization--) | रास्टराइज़ेशन सेटिंग्स प्राप्त करता है। |
|
|  | [getWordprocessingSaveOptions()](#getWordprocessingSaveOptions--) | वर्ड प्रोसेसिंग सहेजने के विकल्प। |
|
### SaveOptions() {#SaveOptions--}
```
public SaveOptions()
```


डिफ़ॉल्ट मानों के साथ एक नया उदाहरण प्रारंभ करता है: PDF में रास्टराइज़ करना - false, उपसर्ग जोड़ना - false।


### SaveOptions(boolean rasterizeToPdf, String suffix) {#SaveOptions-boolean-java.lang.String-}
```
public SaveOptions(boolean rasterizeToPdf, String suffix)
```


दिए गए पैरामीटरों के साथ एक नया इंस्टेंस प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rasterizeToPdf | boolean | सही, यदि दस्तावेज़ के सभी पृष्ठों को छवियों में परिवर्तित करके एक ही PDF फ़ाइल में रखना आवश्यक है |
|
|  | suffix | java.lang.String | यदि यह खाली नहीं है तो यह पाठ फ़ाइल नाम के अंत में जोड़ा जाएगा, साथ ही AddSuffix को true सेट करता है। |
|

### SaveSuffix {#SaveSuffix}
```
public static final String SaveSuffix
```


डिफ़ॉल्ट सफ़िक्स मान को दर्शाता है, जो "Redacted" है।


### getAddSuffix() {#getAddSuffix--}
```
public final boolean getAddSuffix()
```


फ़ाइल नाम को सहेजने से पहले बदलने की आवश्यकता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। डिफ़ॉल्ट रूप से false।


**Returns:**
boolean - फ़ाइल नाम को सहेजने से पहले बदलने की आवश्यकता है या नहीं, यह दर्शाने वाला मान। डिफ़ॉल्ट रूप से false।

### setAddSuffix(boolean value) {#setAddSuffix-boolean-}
```
public final void setAddSuffix(boolean value)
```


फ़ाइल नाम को सहेजने से पहले बदलने की आवश्यकता है या नहीं, यह दर्शाने वाला मान सेट करता है। डिफ़ॉल्ट रूप से false।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | फ़ाइल नाम को सहेजने से पहले बदलने की आवश्यकता है या नहीं, यह दर्शाने वाला मान। डिफ़ॉल्ट रूप से false। |
|

### getRedactedFileSuffix() {#getRedactedFileSuffix--}
```
public final String getRedactedFileSuffix()
```


आउटपुट फ़ाइल नाम के लिए एक कस्टम सफ़िक्स प्राप्त करता है। यदि यह निर्दिष्ट नहीं किया गया है, तो
SaveSuffix
स्थिरांक उपयोग किया जाएगा।


**Returns:**
java.lang.String - आउटपुट फ़ाइल नाम के लिए एक कस्टम सफ़िक्स। यदि यह निर्दिष्ट नहीं किया गया है, तो  SaveSuffix  स्थिरांक उपयोग किया जाएगा।

### setRedactedFileSuffix(String value) {#setRedactedFileSuffix-java.lang.String-}
```
public final void setRedactedFileSuffix(String value)
```


आउटपुट फ़ाइल नाम के लिए एक कस्टम सफ़िक्स सेट करता है। यदि यह निर्दिष्ट नहीं किया गया है, तो
SaveSuffix
स्थिरांक उपयोग किया जाएगा।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String | आउटपुट फ़ाइल नाम के लिए एक कस्टम उपसर्ग। यदि इसे निर्दिष्ट नहीं किया गया है, तो  SaveSuffix  स्थिरांक का उपयोग किया जाएगा। |
|

### getRasterizeToPDF() {#getRasterizeToPDF--}
```
public final boolean getRasterizeToPDF()
```


दस्तावेज़ के सभी पृष्ठों को छवियों में परिवर्तित करके एक ही PDF फ़ाइल में रखने की आवश्यकता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।


**Returns:**
boolean - एक मान जो दर्शाता है कि क्या दस्तावेज़ के सभी पृष्ठों को छवियों में परिवर्तित करके एकल PDF फ़ाइल में रखा जाना चाहिए।

### setRasterizeToPDF(boolean value) {#setRasterizeToPDF-boolean-}
```
public final void setRasterizeToPDF(boolean value)
```


दस्तावेज़ के सभी पृष्ठों को छवियों में परिवर्तित करके एक ही PDF फ़ाइल में रखने की आवश्यकता है या नहीं, यह दर्शाने वाला मान सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | एक मान जो दर्शाता है कि क्या दस्तावेज़ के सभी पृष्ठों को छवियों में परिवर्तित करके एकल PDF फ़ाइल में रखा जाना चाहिए। |
|

### getRasterization() {#getRasterization--}
```
public final RasterizationOptions getRasterization()
```


रास्टराइज़ेशन सेटिंग्स प्राप्त करता है।


**Returns:**
[RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) - The rasterization settings.

### getWordprocessingSaveOptions() {#getWordprocessingSaveOptions--}
```
public final WordprocessingSaveOptions getWordprocessingSaveOptions()
```


वर्ड प्रोसेसिंग सहेजने के विकल्प।


**Returns:**
[WordprocessingSaveOptions](../../com.groupdocs.redaction.options/wordprocessingsaveoptions)
