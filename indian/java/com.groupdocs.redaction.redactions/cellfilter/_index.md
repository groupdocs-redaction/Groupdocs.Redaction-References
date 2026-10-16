---
title: "CellFilter"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "CellColumnRedaction की सीमा को एक वर्कशीट और एक कॉलम तक सीमित करने का विकल्प प्रदान करता है।"
type: docs
weight: 12
url: /hi/java/com.groupdocs.redaction.redactions/cellfilter/
---
**Inheritance:**
java.lang.Object
```
public class CellFilter
```

एक विकल्प प्रदान करता है जिससे किसी चीज़ का दायरा सीमित किया जा सके।
CellColumnRedaction
एक वर्कशीट और एक कॉलम तक।

*** ** * ** ***


**Learn more**

* More details about spreadsheet redactions: [Spreadsheet redactions](../https://docs.groupdocs.com/redaction/java/spreadsheet-redactions/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [CellFilter()](#CellFilter--) | एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## फ़ील्ड्स

| फ़ील्ड | विवरण |
| --- | --- |
|  | [NoIndex](#NoIndex) | फ़िल्टर के लिए डिफ़ॉल्ट मान दर्शाता है, जो -1 है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getWorkSheetName()](#getWorkSheetName--) | वर्कशीट का नाम प्राप्त करता है (यदि लागू हो)। |
|
|  | [setWorkSheetName(String value)](#setWorkSheetName-java.lang.String-) | वर्कशीट का नाम सेट करता है (यदि लागू हो)। |
|
|  | [getWorkSheetIndex()](#getWorkSheetIndex--) | वर्कशीट का इंडेक्स प्राप्त करता है (शून्य-आधारित)। |
|
|  | [setWorkSheetIndex(int value)](#setWorkSheetIndex-int-) | वर्कशीट का इंडेक्स सेट करता है (शून्य-आधारित)। |
|
|  | [hasWorkSheetIndex()](#hasWorkSheetIndex--) | एक मान प्राप्त करता है जो दर्शाता है कि क्या |
WorkSheetIndex
सेट है या नहीं।
|
|  | [getColumnIndex()](#getColumnIndex--) | कॉलम इंडेक्स प्राप्त करता है (शून्य-आधारित)। |
|
|  | [setColumnIndex(int value)](#setColumnIndex-int-) | कॉलम इंडेक्स सेट करता है (शून्य-आधारित)। |
|
### CellFilter() {#CellFilter--}
```
public CellFilter()
```


एक नया इंस्टेंस इनिशियलाइज़ करता है।


### NoIndex {#NoIndex}
```
public static final int NoIndex
```


फ़िल्टर के लिए डिफ़ॉल्ट मान दर्शाता है, जो -1 है।


### getWorkSheetName() {#getWorkSheetName--}
```
public final String getWorkSheetName()
```


वर्कशीट का नाम प्राप्त करता है (यदि लागू हो)।


**Returns:**
java.lang.String - एक कार्यपत्रक नाम (यदि लागू हो)।

### setWorkSheetName(String value) {#setWorkSheetName-java.lang.String-}
```
public final void setWorkSheetName(String value)
```


वर्कशीट का नाम सेट करता है (यदि लागू हो)।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String | एक कार्यपत्रक नाम (यदि लागू हो)। |
|

### getWorkSheetIndex() {#getWorkSheetIndex--}
```
public final int getWorkSheetIndex()
```


वर्कशीट का इंडेक्स प्राप्त करता है (शून्य-आधारित)।


**Returns:**
int - एक कार्यपत्रक इंडेक्स (शून्य-आधारित)।

### setWorkSheetIndex(int value) {#setWorkSheetIndex-int-}
```
public final void setWorkSheetIndex(int value)
```


वर्कशीट का इंडेक्स सेट करता है (शून्य-आधारित)।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | एक कार्यपत्रक इंडेक्स (शून्य-आधारित)। |
|

### hasWorkSheetIndex() {#hasWorkSheetIndex--}
```
public final boolean hasWorkSheetIndex()
```


एक मान प्राप्त करता है जो दर्शाता है कि क्या
WorkSheetIndex
सेट है या नहीं।


**Returns:**
boolean - एक मान जो दर्शाता है कि WorkSheetIndex सेट है या नहीं।

### getColumnIndex() {#getColumnIndex--}
```
public final int getColumnIndex()
```


कॉलम इंडेक्स प्राप्त करता है (शून्य-आधारित)।


**Returns:**
int - एक कॉलम इंडेक्स (शून्य-आधारित)।

### setColumnIndex(int value) {#setColumnIndex-int-}
```
public final void setColumnIndex(int value)
```


कॉलम इंडेक्स सेट करता है (शून्य-आधारित)।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | एक कॉलम इंडेक्स (शून्य-आधारित)। |
|

