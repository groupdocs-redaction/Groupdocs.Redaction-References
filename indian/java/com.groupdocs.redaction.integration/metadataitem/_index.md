---
title: "MetadataItem"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "सभी समर्थित फ़ॉर्मेट्स के लिए सामान्य मेटाडेटा आइटम का प्रतिनिधित्व करता है और मेटाडेटा रिडैक्शन में उपयोग किया जाता है।"
type: docs
weight: 12
url: /hi/java/com.groupdocs.redaction.integration/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

सभी समर्थित स्वरूपों के लिए सामान्य मेटाडेटा आइटम को दर्शाता है, जो मेटाडेटा रेडैक्शन में उपयोग किया जाता है।

## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [MetadataItem()](#MetadataItem--) | एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getOriginalName()](#getOriginalName--) | दस्तावेज़ में जैसा दिखता है, मेटाडेटा आइटम का मूल नाम प्राप्त करता है। |
|
|  | [setOriginalName(String value)](#setOriginalName-java.lang.String-) | दस्तावेज़ में जैसा दिखता है, मेटाडेटा आइटम का मूल नाम सेट करता है। |
|
|  | [getCategory()](#getCategory--) | मेटाडेटा आइटम की श्रेणी प्राप्त करता है, उदाहरण के लिए एम्बेडेड रिसोर्स मेटाडेटा आइटम के लिए रिसोर्स ID। |
|
|  | [setCategory(String value)](#setCategory-java.lang.String-) | मेटाडेटा आइटम की एक श्रेणी सेट करता है, उदाहरण के लिए एम्बेडेड रिसोर्स मेटाडेटा आइटम के लिए रिसोर्स ID। |
|
|  | [getFilter()](#getFilter--) | एक मान प्राप्त करता है |
MetadataFilters
, जो इस मेटाडेटा आइटम को सौंपा गया है और आइटम फ़िल्ट्रेशन में उपयोग होता है।
|
|  | [setFilter(int value)](#setFilter-int-) | एक मान सेट करता है |
MetadataFilters
, जो इस मेटाडेटा आइटम को सौंपा गया है और आइटम फ़िल्ट्रेशन में उपयोग होता है।
|
|  | [getValues()](#getValues--) | मेटाडेटा आइटम का मान प्राप्त करता है। |
|
|  | [setValues(List<String> value)](#setValues-java.util.List-java.lang.String--) | मेटाडेटा आइटम का मान सेट करता है। |
|
|  | [isCustom()](#isCustom--) | एक मान प्राप्त करता है जो दर्शाता है कि यह आइटम कस्टम है (दस्तावेज़ के लेखकों द्वारा जोड़ा गया)। |
|
|  | [setCustom(boolean value)](#setCustom-boolean-) | एक मान सेट करता है जो दर्शाता है कि यह आइटम कस्टम है (दस्तावेज़ के लेखकों द्वारा जोड़ा गया)। |
|
|  | [getDictionaryKey()](#getDictionaryKey--) | डिक्शनरी कुंजी प्राप्त करता है , इसके OriginalName और अन्य डेटा का उपयोग करके। |
|
|  | [createClone()](#createClone--) | वर्तमान इंस्टेंस की एक डीप क्लोन बनाता है। |
|
|  | [getActualValue()](#getActualValue--) | मेटाडेटा आइटम मान का स्ट्रिंग प्रतिनिधित्व प्राप्त करता है। |
|
### MetadataItem() {#MetadataItem--}
```
public MetadataItem()
```


एक नया इंस्टेंस इनिशियलाइज़ करता है।


### getOriginalName() {#getOriginalName--}
```
public final String getOriginalName()
```


दस्तावेज़ में जैसा दिखता है, मेटाडेटा आइटम का मूल नाम प्राप्त करता है।


**Returns:**
java.lang.String - मेटाडेटा आइटम का मूल नाम, जैसा कि दस्तावेज़ में दिखाई देता है।

### setOriginalName(String value) {#setOriginalName-java.lang.String-}
```
public final void setOriginalName(String value)
```


दस्तावेज़ में जैसा दिखता है, मेटाडेटा आइटम का मूल नाम सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String | मेटाडेटा आइटम का मूल नाम, जैसा कि दस्तावेज़ में दिखाई देता है। |
|

### getCategory() {#getCategory--}
```
public final String getCategory()
```


मेटाडेटा आइटम की श्रेणी प्राप्त करता है, उदाहरण के लिए एम्बेडेड रिसोर्स मेटाडेटा आइटम के लिए रिसोर्स ID।


**Returns:**
java.lang.String - मेटाडेटा आइटम की एक श्रेणी, उदाहरण के लिए एम्बेडेड रिसोर्स मेटाडेटा आइटम के लिए रिसोर्स ID।

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


मेटाडेटा आइटम की एक श्रेणी सेट करता है, उदाहरण के लिए एम्बेडेड रिसोर्स मेटाडेटा आइटम के लिए रिसोर्स ID।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String | मेटाडेटा आइटम की एक श्रेणी, उदाहरण के लिए एम्बेडेड रिसोर्स मेटाडेटा आइटम के लिए रिसोर्स ID। |
|

### getFilter() {#getFilter--}
```
public final int getFilter()
```


एक मान प्राप्त करता है
MetadataFilters
, जो इस मेटाडेटा आइटम को सौंपा गया है और आइटम फ़िल्ट्रेशन में उपयोग होता है।


**Returns:**
int - MetadataFilters का एक मान, जो इस मेटाडेटा आइटम को सौंपा गया है और आइटम फ़िल्ट्रेशन में उपयोग होता है।

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


एक मान सेट करता है
MetadataFilters
, जो इस मेटाडेटा आइटम को सौंपा गया है और आइटम फ़िल्ट्रेशन में उपयोग होता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | MetadataFilters का एक मान, जो इस मेटाडेटा आइटम को सौंपा गया है और आइटम फ़िल्ट्रेशन में उपयोग होता है। |
|

### getValues() {#getValues--}
```
public final List<String> getValues()
```


मेटाडेटा आइटम का मान प्राप्त करता है।


**Returns:**
java.util.List<java.lang.String> - मेटाडेटा आइटम का मान।

### setValues(List<String> value) {#setValues-java.util.List-java.lang.String--}
```
public final void setValues(List<String> value)
```


मेटाडेटा आइटम का मान सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.util.List<java.lang.String> | मेटाडेटा आइटम का मान। |
|

### isCustom() {#isCustom--}
```
public final boolean isCustom()
```


एक मान प्राप्त करता है जो दर्शाता है कि यह आइटम कस्टम है (दस्तावेज़ के लेखकों द्वारा जोड़ा गया)।


**Returns:**
boolean - एक मान जो दर्शाता है कि यह आइटम कस्टम है (दस्तावेज़ के लेखकों द्वारा जोड़ा गया)।

### setCustom(boolean value) {#setCustom-boolean-}
```
public final void setCustom(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि यह आइटम कस्टम है (दस्तावेज़ के लेखकों द्वारा जोड़ा गया)।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | एक मान जो दर्शाता है कि यह आइटम कस्टम है (दस्तावेज़ के लेखकों द्वारा जोड़ा गया)। |
|

### getDictionaryKey() {#getDictionaryKey--}
```
public String getDictionaryKey()
```


डिक्शनरी कुंजी प्राप्त करता है , इसके OriginalName और अन्य डेटा का उपयोग करके।


**Returns:**
java.lang.String - एक डिक्शनरी कुंजी , इसके OriginalName और अन्य डेटा का उपयोग करके।

### createClone() {#createClone--}
```
public MetadataItem createClone()
```


वर्तमान इंस्टेंस की एक डीप क्लोन बनाता है।


**Returns:**
[MetadataItem](../../com.groupdocs.redaction.integration/metadataitem) - Object clone

### getActualValue() {#getActualValue--}
```
public final String getActualValue()
```


मेटाडेटा आइटम मान का स्ट्रिंग प्रतिनिधित्व प्राप्त करता है।


**Returns:**
java.lang.String - मेटाडेटा आइटम मान का स्ट्रिंग प्रतिनिधित्व।

