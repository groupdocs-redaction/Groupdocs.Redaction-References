---
title: "FileType"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "फ़ाइल प्रकार का प्रतिनिधित्व करता है।"
type: docs
weight: 11
url: /hi/java/com.groupdocs.redaction/filetype/
---
**Inheritance:**
java.lang.Object
```
public final class FileType
```

एक फ़ाइल प्रकार का प्रतिनिधित्व करता है। GroupDocs.Redaction द्वारा समर्थित सभी फ़ाइल प्रकारों की सूची प्राप्त करने, एक्सटेंशन द्वारा फ़ाइल प्रकार का पता लगाने आदि के लिए मेथड प्रदान करता है।

*** ** * ** ***


**Learn more**

* [Supported Document Formats](../https://docs.groupdocs.com/redaction/java/supported-document-formats/)
* [Get supported file formats](../https://docs.groupdocs.com/redaction/java/get-supported-file-formats/)
* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | फ़ाइल प्रकार का नाम प्राप्त करता है, उदाहरण के लिए "Microsoft Word Document"। |
|
|  | [getExtension()](#getExtension--) | फ़ाइलनाम प्रत्यय प्राप्त करता है (जिसमें बिंदु "." शामिल है), उदाहरण के लिए ".doc"। |
|
|  | [getUnknown()](#getUnknown--) | अज्ञात फ़ाइल प्रकार का प्रतिनिधित्व करता है। |
|
|  | [getTIF()](#getTIF--) | Tagged Image File (.tif) |
|
|  | [getTIFF()](#getTIFF--) | Tagged Image File Format (.tiff) |
|
|  | [getJPG()](#getJPG--) | JPEG छवि (.jpg) |
|
|  | [getJPEG()](#getJPEG--) | JPEG छवि (.jpeg) |
|
|  | [getPNG()](#getPNG--) | पोर्टेबल नेटवर्क ग्राफ़िक (.png) |
|
|  | [getGIF()](#getGIF--) | ग्राफ़िकल इंटरचेंज फ़ॉर्मेट फ़ाइल (.gif) |
|
|  | [getBMP()](#getBMP--) | बिटमैप छवि फ़ाइल (.bmp) |
|
|  | [getJP2()](#getJP2--) | JPEG 2000 कोर छवि फ़ाइल (.jp2) |
|
|  | [getHTM()](#getHTM--) | हाइपरटेक्स्ट मार्कअप लैंग्वेज फ़ाइल (.htm) |
|
|  | [getHTML()](#getHTML--) | हाइपरटेक्स्ट मार्कअप लैंग्वेज फ़ाइल (.html) |
|
|  | [getPDF()](#getPDF--) | पोर्टेबल डॉक्यूमेंट फ़ॉर्मेट फ़ाइल (.pdf) |
|
|  | [getPPT()](#getPPT--) | पावरपॉइंट प्रस्तुति (.ppt) |
|
|  | [getPPTX()](#getPPTX--) | पावरपॉइंट ओपन XML प्रस्तुति (.pptx) |
|
|  | [getODP()](#getODP--) | ओपनडॉक्यूमेंट प्रस्तुति (.odp) |
|
|  | [getPOTX()](#getPOTX--) | पावरपॉइंट ओपन XML प्रस्तुति टेम्पलेट (.potx) |
|
|  | [getPOTM()](#getPOTM--) | पावरपॉइंट ओपन XML मैक्रो-सक्षम प्रस्तुति टेम्पलेट (.potm) |
|
|  | [getOTP()](#getOTP--) | ओपनडॉक्यूमेंट प्रस्तुति टेम्पलेट (.otp) |
|
|  | [getXLS()](#getXLS--) | एक्सेल स्प्रेडशीट (.xls) |
|
|  | [getXLSX()](#getXLSX--) | माइक्रोसॉफ्ट एक्सेल ओपन XML स्प्रेडशीट (.xlsx) |
|
|  | [getXLSM()](#getXLSM--) | एक्सेल ओपन XML मैक्रो-सक्षम स्प्रेडशीट (.xlsm) |
|
|  | [getXLSB()](#getXLSB--) | एक्सेल बाइनरी स्प्रेडशीट (.xlsb) |
|
|  | [getXLTX()](#getXLTX--) | एक्सेल ओपन XML स्प्रेडशीट टेम्पलेट (.xltx) |
|
|  | [getXLTM()](#getXLTM--) | एक्सेल ओपन XML मैक्रो-सक्षम स्प्रेडशीट टेम्पलेट (.xltm) |
|
|  | [getXLT()](#getXLT--) | एक्सेल टेम्पलेट (.xlt) |
|
|  | [getCSV()](#getCSV--) | कॉमा सेपरेटेड वैल्यूज़ फ़ाइल (.csv) |
|
|  | [getTSV()](#getTSV--) | टैब सेपरेटेड वैल्यूज़ फ़ाइल (.tsv) |
|
|  | [getTAB()](#getTAB--) | टैब सेपरेटेड वैल्यूज़ फ़ाइल (.tab) |
|
|  | [getODS()](#getODS--) | OpenDocument स्प्रेडशीट (.ods) |
|
|  | [getOTS()](#getOTS--) | OpenDocument स्प्रेडशीट टेम्पलेट (.ots) |
|
|  | [getNUMBERS()](#getNUMBERS--) | Apple Numbers स्प्रेडशीट (.numbers) |
|
|  | [getMD()](#getMD--) | Markdown दस्तावेज़ फ़ाइल (.md) |
|
|  | [getDOC()](#getDOC--) | Microsoft Word दस्तावेज़ (.doc) |
|
|  | [getDOCX()](#getDOCX--) | Microsoft Word Open XML दस्तावेज़ (.docx) |
|
|  | [getDOCM()](#getDOCM--) | Word Open XML मैक्रो-सक्षम दस्तावेज़ (.docm) |
|
|  | [getDOT()](#getDOT--) | Word दस्तावेज़ टेम्पलेट (.dot) |
|
|  | [getDOTX()](#getDOTX--) | Word Open XML दस्तावेज़ टेम्पलेट (.dotx) |
|
|  | [getDOTM()](#getDOTM--) | Word Open XML मैक्रो-सक्षम दस्तावेज़ टेम्पलेट (.dotm) |
|
|  | [getRTF()](#getRTF--) | रिच टेक्स्ट फ़ॉर्मेट फ़ाइल (.rtf) |
|
|  | [getTXT()](#getTXT--) | सादा टेक्स्ट फ़ाइल (.txt) |
|
|  | [getODT()](#getODT--) | OpenDocument टेक्स्ट दस्तावेज़ (.odt) |
|
|  | [getOTT()](#getOTT--) | OpenDocument दस्तावेज़ टेम्पलेट (.ott) |
|
|  | [fromExtension(String extension)](#fromExtension-java.lang.String-) | फ़ाइल एक्सटेंशन को फ़ाइल प्रकार से मैप करता है। |
|
|  | [getSupportedFileTypes()](#getSupportedFileTypes--) | समर्थित फ़ाइल प्रकारों को प्राप्त करता है |
|
|  | [equals(FileType other)](#equals-com.groupdocs.redaction.FileType-) | निर्धारित करता है कि वर्तमान |
FileType
निर्दिष्ट के समान है
FileType
ऑब्जेक्ट।
|
|  | [equals(Object obj)](#equals-java.lang.Object-) | निर्धारित करता है कि वर्तमान |
FileType
निर्दिष्ट ऑब्जेक्ट के समान है।
|
|  | [hashCode()](#hashCode--) | वर्तमान के लिए हैश कोड लौटाता है |
FileType
ऑब्जेक्ट।
|
|  | [op_Equality(FileType left, FileType right)](#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | निर्धारित करता है कि दो |
FileType
ऑब्जेक्ट समान हैं।
|
|  | [op_Inequality(FileType left, FileType right)](#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | निर्धारित करता है कि दो |
FileType
ऑब्जेक्ट समान नहीं हैं।
|
|  | [toString()](#toString--) | वर्तमान ऑब्जेक्ट का प्रतिनिधित्व करने वाली स्ट्रिंग लौटाता है। |
|
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


फ़ाइल प्रकार का नाम प्राप्त करता है, उदाहरण के लिए "Microsoft Word Document"।


**Returns:**
java.lang.String - फ़ाइल प्रकार का नाम, उदाहरण के लिए "Microsoft Word Document".

### getExtension() {#getExtension--}
```
public final String getExtension()
```


फ़ाइलनाम प्रत्यय प्राप्त करता है (जिसमें बिंदु "." शामिल है), उदाहरण के लिए ".doc"।


**Returns:**
java.lang.String - फ़ाइलनाम प्रत्यय (जिसमें बिंदु "." शामिल है), उदाहरण के लिए ".doc".

### getUnknown() {#getUnknown--}
```
public static FileType getUnknown()
```


अज्ञात फ़ाइल प्रकार का प्रतिनिधित्व करता है।


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIF() {#getTIF--}
```
public static FileType getTIF()
```


Tagged Image File (.tif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIFF() {#getTIFF--}
```
public static FileType getTIFF()
```


Tagged Image File Format (.tiff)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPG() {#getJPG--}
```
public static FileType getJPG()
```


JPEG छवि (.jpg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPEG() {#getJPEG--}
```
public static FileType getJPEG()
```


JPEG छवि (.jpeg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPNG() {#getPNG--}
```
public static FileType getPNG()
```


पोर्टेबल नेटवर्क ग्राफ़िक (.png)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getGIF() {#getGIF--}
```
public static FileType getGIF()
```


ग्राफ़िकल इंटरचेंज फ़ॉर्मेट फ़ाइल (.gif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getBMP() {#getBMP--}
```
public static FileType getBMP()
```


बिटमैप छवि फ़ाइल (.bmp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJP2() {#getJP2--}
```
public static FileType getJP2()
```


JPEG 2000 कोर छवि फ़ाइल (.jp2)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTM() {#getHTM--}
```
public static FileType getHTM()
```


हाइपरटेक्स्ट मार्कअप लैंग्वेज फ़ाइल (.htm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTML() {#getHTML--}
```
public static FileType getHTML()
```


हाइपरटेक्स्ट मार्कअप लैंग्वेज फ़ाइल (.html)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPDF() {#getPDF--}
```
public static FileType getPDF()
```


पोर्टेबल डॉक्यूमेंट फ़ॉर्मेट फ़ाइल (.pdf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPT() {#getPPT--}
```
public static FileType getPPT()
```


पावरपॉइंट प्रस्तुति (.ppt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPTX() {#getPPTX--}
```
public static FileType getPPTX()
```


पावरपॉइंट ओपन XML प्रस्तुति (.pptx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODP() {#getODP--}
```
public static FileType getODP()
```


ओपनडॉक्यूमेंट प्रस्तुति (.odp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTX() {#getPOTX--}
```
public static FileType getPOTX()
```


पावरपॉइंट ओपन XML प्रस्तुति टेम्पलेट (.potx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTM() {#getPOTM--}
```
public static FileType getPOTM()
```


पावरपॉइंट ओपन XML मैक्रो-सक्षम प्रस्तुति टेम्पलेट (.potm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTP() {#getOTP--}
```
public static FileType getOTP()
```


ओपनडॉक्यूमेंट प्रस्तुति टेम्पलेट (.otp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLS() {#getXLS--}
```
public static FileType getXLS()
```


एक्सेल स्प्रेडशीट (.xls)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSX() {#getXLSX--}
```
public static FileType getXLSX()
```


माइक्रोसॉफ्ट एक्सेल ओपन XML स्प्रेडशीट (.xlsx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSM() {#getXLSM--}
```
public static FileType getXLSM()
```


एक्सेल ओपन XML मैक्रो-सक्षम स्प्रेडशीट (.xlsm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSB() {#getXLSB--}
```
public static FileType getXLSB()
```


एक्सेल बाइनरी स्प्रेडशीट (.xlsb)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTX() {#getXLTX--}
```
public static FileType getXLTX()
```


एक्सेल ओपन XML स्प्रेडशीट टेम्पलेट (.xltx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTM() {#getXLTM--}
```
public static FileType getXLTM()
```


एक्सेल ओपन XML मैक्रो-सक्षम स्प्रेडशीट टेम्पलेट (.xltm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLT() {#getXLT--}
```
public static FileType getXLT()
```


एक्सेल टेम्पलेट (.xlt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getCSV() {#getCSV--}
```
public static FileType getCSV()
```


कॉमा सेपरेटेड वैल्यूज़ फ़ाइल (.csv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTSV() {#getTSV--}
```
public static FileType getTSV()
```


टैब सेपरेटेड वैल्यूज़ फ़ाइल (.tsv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTAB() {#getTAB--}
```
public static FileType getTAB()
```


टैब सेपरेटेड वैल्यूज़ फ़ाइल (.tab)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODS() {#getODS--}
```
public static FileType getODS()
```


OpenDocument स्प्रेडशीट (.ods)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTS() {#getOTS--}
```
public static FileType getOTS()
```


OpenDocument स्प्रेडशीट टेम्पलेट (.ots)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getNUMBERS() {#getNUMBERS--}
```
public static FileType getNUMBERS()
```


Apple Numbers स्प्रेडशीट (.numbers)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getMD() {#getMD--}
```
public static FileType getMD()
```


Markdown दस्तावेज़ फ़ाइल (.md)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOC() {#getDOC--}
```
public static FileType getDOC()
```


Microsoft Word दस्तावेज़ (.doc)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCX() {#getDOCX--}
```
public static FileType getDOCX()
```


Microsoft Word Open XML दस्तावेज़ (.docx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCM() {#getDOCM--}
```
public static FileType getDOCM()
```


Word Open XML मैक्रो-सक्षम दस्तावेज़ (.docm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOT() {#getDOT--}
```
public static FileType getDOT()
```


Word दस्तावेज़ टेम्पलेट (.dot)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTX() {#getDOTX--}
```
public static FileType getDOTX()
```


Word Open XML दस्तावेज़ टेम्पलेट (.dotx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTM() {#getDOTM--}
```
public static FileType getDOTM()
```


Word Open XML मैक्रो-सक्षम दस्तावेज़ टेम्पलेट (.dotm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getRTF() {#getRTF--}
```
public static FileType getRTF()
```


रिच टेक्स्ट फ़ॉर्मेट फ़ाइल (.rtf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTXT() {#getTXT--}
```
public static FileType getTXT()
```


सादा टेक्स्ट फ़ाइल (.txt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODT() {#getODT--}
```
public static FileType getODT()
```


OpenDocument टेक्स्ट दस्तावेज़ (.odt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTT() {#getOTT--}
```
public static FileType getOTT()
```


OpenDocument दस्तावेज़ टेम्पलेट (.ott)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### fromExtension(String extension) {#fromExtension-java.lang.String-}
```
public static FileType fromExtension(String extension)
```


फ़ाइल एक्सटेंशन को फ़ाइल प्रकार से मैप करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | विस्तार | java.lang.String | फ़ाइल विस्तार (जिसमें बिंदु "." शामिल है). |
|

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - When file type is supported returns it, otherwise returns default  Unknown  file type.

### getSupportedFileTypes() {#getSupportedFileTypes--}
```
public static Iterable<FileType> getSupportedFileTypes()
```


समर्थित फ़ाइल प्रकारों को प्राप्त करता है


**Returns:**
java.lang.Iterable<com.groupdocs.redaction.FileType> - समर्थित फ़ाइल प्रकारों की क्रमबद्धता लौटाता है

### equals(FileType other) {#equals-com.groupdocs.redaction.FileType-}
```
public final boolean equals(FileType other)
```


निर्धारित करता है कि वर्तमान
FileType
निर्दिष्ट के समान है
FileType
ऑब्जेक्ट।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | other | [FileType](../../com.groupdocs.redaction/filetype) | वर्तमान  FileType  वस्तु के साथ तुलना करने के लिए वस्तु। |
|

**Returns:**
boolean - ```
true
```

if both  FileType  objects are the same; otherwise,

```
false
```


### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determines whether the current 
FileType
 is the same as specified object.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The object to compare with the current  FileType  object.
 |

**Returns:**
boolean - ```
true
```

यदि

```
obj
```

पैरामीटर  FileType  है और वर्तमान  FileType  वस्तु के समान है; अन्यथा,

```
false
```


### hashCode() {#hashCode--}
```
public int hashCode()
```


वर्तमान के लिए हैश कोड लौटाता है
FileType
ऑब्जेक्ट।


**Returns:**
int - वर्तमान  FileType  वस्तु के लिए हैश कोड।

### op_Equality(FileType left, FileType right) {#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Equality(FileType left, FileType right)
```


निर्धारित करता है कि दो
FileType
ऑब्जेक्ट समान हैं।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | left | [FileType](../../com.groupdocs.redaction/filetype) | बाएँ  FileType  वस्तु। |
|
|  | right | [FileType](../../com.groupdocs.redaction/filetype) | दाएँ  FileType  वस्तु। |
|

**Returns:**
boolean - ```
true
```

if both  FileType  objects are the same; otherwise,

```
false
```


### op_Inequality(FileType left, FileType right) {#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Inequality(FileType left, FileType right)
```


Determines whether two 
FileType
 objects are not the same.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| left | [FileType](../../com.groupdocs.redaction/filetype) | Left  FileType  object.
 |
| right | [FileType](../../com.groupdocs.redaction/filetype) | Right  FileType  object.
 |

**Returns:**
boolean - ```
true
```

यदि दोनों  FileType  वस्तुएँ समान नहीं हैं; अन्यथा,

```
false
```


### toString() {#toString--}
```
public String toString()
```


वर्तमान ऑब्जेक्ट का प्रतिनिधित्व करने वाली स्ट्रिंग लौटाता है।


**Returns:**
java.lang.String - एक स्ट्रिंग जो वर्तमान वस्तु का प्रतिनिधित्व करती है।

