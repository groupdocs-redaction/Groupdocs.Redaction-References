---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "फ़ाइलों को PDF में परिवर्तित करने के विकल्प प्रदान करता है।"
type: docs
weight: 12
url: /hi/java/com.groupdocs.redaction.options/rasterizationoptions/
---
**Inheritance:**
java.lang.Object
```
public class RasterizationOptions
```

फ़ाइलों को PDF में परिवर्तित करने के विकल्प प्रदान करता है।

*** ** * ** ***


**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [RasterizationOptions()](#RasterizationOptions--) | एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | दस्तावेज़ के सभी पृष्ठों को छवियों में परिवर्तित करके एक ही PDF फ़ाइल में रखने की आवश्यकता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | दस्तावेज़ के सभी पृष्ठों को छवियों में परिवर्तित करके एक ही PDF फ़ाइल में रखने की आवश्यकता है या नहीं, यह दर्शाने वाला मान सेट करता है। |
|
|  | [getPageIndex()](#getPageIndex--) | PDF में बदलने के लिए पहली पेज (0-आधारित) का इंडेक्स प्राप्त करता है। |
|
|  | [setPageIndex(int value)](#setPageIndex-int-) | PDF में बदलने के लिए पहली पेज (0-आधारित) का इंडेक्स सेट करता है। |
|
|  | [isStartPageIndexSet()](#isStartPageIndexSet--) | एक मान प्राप्त करता है जो दर्शाता है कि PageIndex प्रॉपर्टी को उसके इनिशियलाइज़ेशन के बाद बदल (सेट) किया गया था या नहीं। |
|
|  | [getPageCount()](#getPageCount--) | PDF में बदलने के लिए पेजों की संख्या प्राप्त करता है। |
|
|  | [setPageCount(int value)](#setPageCount-int-) | PDF में परिवर्तित किए जाने वाले पृष्ठों की संख्या सेट करता है। |
|
|  | [isPageCountSet()](#isPageCountSet--) | प्रारंभिककरण के बाद यह दर्शाने वाला मान प्राप्त करता है कि PageCount प्रॉपर्टी बदली (सेट) गई थी या नहीं। |
|
|  | [getCompliance()](#getCompliance--) | PDF अनुपालन स्तर प्राप्त करता है। |
|
|  | [setCompliance(PdfComplianceLevel value)](#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-) | PDF अनुपालन स्तर सेट करता है। |
|
|  | [hasAdvancedOptions()](#hasAdvancedOptions--) | एक संकेतक प्राप्त करता है, जो तब सत्य होता है जब उन्नत रास्टराइज़ेशन विकल्प सेट किए गए हों। |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-) | आप इस मेथड का उपयोग करके लागू करने के लिए एक उन्नत रास्टराइज़ेशन विकल्प पंजीकृत कर सकते हैं। |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--) | आप इस मेथड का उपयोग करके लागू करने के लिए एक उन्नत रास्टराइज़ेशन विकल्प पंजीकृत कर सकते हैं। |
|
### RasterizationOptions() {#RasterizationOptions--}
```
public RasterizationOptions()
```


एक नया इंस्टेंस इनिशियलाइज़ करता है।


### getEnabled() {#getEnabled--}
```
public final boolean getEnabled()
```


एक मान प्राप्त करता है जो दर्शाता है कि क्या दस्तावेज़ के सभी पृष्ठों को छवियों में परिवर्तित करके एकल PDF फ़ाइल में रखा जाना चाहिए। डिफ़ॉल्ट रूप से TRUE, रास्टराइज़ेशन से बचने के लिए FALSE सेट करें।


**Returns:**
boolean - एक मान जो दर्शाता है कि क्या दस्तावेज़ के सभी पृष्ठों को छवियों में परिवर्तित करके एकल PDF फ़ाइल में रखा जाना चाहिए। डिफ़ॉल्ट रूप से TRUE, रास्टराइज़ेशन से बचने के लिए FALSE सेट करें।

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public final void setEnabled(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि क्या दस्तावेज़ के सभी पृष्ठों को छवियों में परिवर्तित करके एकल PDF फ़ाइल में रखा जाना चाहिए। डिफ़ॉल्ट रूप से TRUE, रास्टराइज़ेशन से बचने के लिए FALSE सेट करें।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | एक मान जो दर्शाता है कि क्या दस्तावेज़ के सभी पृष्ठों को छवियों में परिवर्तित करके एकल PDF फ़ाइल में रखा जाना चाहिए। डिफ़ॉल्ट रूप से TRUE, रास्टराइज़ेशन से बचने के लिए FALSE सेट करें। |
|

### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


PDF में बदलने के लिए पहली पेज (0-आधारित) का इंडेक्स प्राप्त करता है।


**Returns:**
int - PDF में परिवर्तित करने के लिए पहले पृष्ठ (0-आधारित) का इंडेक्स।

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


PDF में बदलने के लिए पहली पेज (0-आधारित) का इंडेक्स सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | PDF में परिवर्तित करने के लिए पहले पृष्ठ (0-आधारित) का इंडेक्स। |
|

### isStartPageIndexSet() {#isStartPageIndexSet--}
```
public final boolean isStartPageIndexSet()
```


एक मान प्राप्त करता है जो दर्शाता है कि PageIndex प्रॉपर्टी को उसके इनिशियलाइज़ेशन के बाद बदल (सेट) किया गया था या नहीं।


**Returns:**
boolean - एक मान जो दर्शाता है कि प्रारंभिककरण के बाद PageIndex प्रॉपर्टी बदली (सेट) गई थी या नहीं।

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


PDF में बदलने के लिए पेजों की संख्या प्राप्त करता है।


**Returns:**
int - PDF में परिवर्तित किए जाने वाले पृष्ठों की संख्या।

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


PDF में परिवर्तित किए जाने वाले पृष्ठों की संख्या सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | PDF में परिवर्तित किए जाने वाले पृष्ठों की संख्या। |
|

### isPageCountSet() {#isPageCountSet--}
```
public final boolean isPageCountSet()
```


प्रारंभिककरण के बाद यह दर्शाने वाला मान प्राप्त करता है कि PageCount प्रॉपर्टी बदली (सेट) गई थी या नहीं।


**Returns:**
boolean - एक मान जो दर्शाता है कि प्रारंभिककरण के बाद PageCount प्रॉपर्टी बदली (सेट) गई थी या नहीं।

### getCompliance() {#getCompliance--}
```
public final PdfComplianceLevel getCompliance()
```


PDF अनुपालन स्तर प्राप्त करता है।


**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) - The PDF Compliance level.

### setCompliance(PdfComplianceLevel value) {#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-}
```
public final void setCompliance(PdfComplianceLevel value)
```


PDF अनुपालन स्तर सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) | PDF अनुपालन स्तर। |
|

### hasAdvancedOptions() {#hasAdvancedOptions--}
```
public final boolean hasAdvancedOptions()
```


एक संकेतक प्राप्त करता है, जो तब सत्य होता है जब उन्नत रास्टराइज़ेशन विकल्प सेट किए गए हों।


**Returns:**
boolean - एक संकेतक, जो तब सत्य होता है जब उन्नत रास्टराइज़ेशन विकल्प सेट किए गए हों।

### addAdvancedOption(AdvancedRasterizationOptions optionType) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType)
```


आप इस मेथड का उपयोग करके लागू करने के लिए एक उन्नत रास्टराइज़ेशन विकल्प पंजीकृत कर सकते हैं।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | चयनित प्रभाव प्रकार (ग्रेस्केल, बॉर्डर, आदि) के बारे में जानकारी प्रदान करता है। |
|

### addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)
```


आप इस मेथड का उपयोग करके लागू करने के लिए एक उन्नत रास्टराइज़ेशन विकल्प पंजीकृत कर सकते हैं।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | चयनित प्रभाव प्रकार (ग्रेस्केल, बॉर्डर, आदि) के बारे में जानकारी प्रदान करता है। |
|
|  | पैरामीटर | java.util.HashMap<java.lang.String,java.lang.String> | दिए गए प्रभाव के लिए पैरामीटर, जैसे घूर्णन कोण |
|

