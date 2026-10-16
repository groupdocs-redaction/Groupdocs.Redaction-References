---
title: "DocumentInfo"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "दस्तावेज़ के बारे में जानकारी दर्शाता है।"
type: docs
weight: 10
url: /hi/java/com.groupdocs.redaction/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo)
```
public class DocumentInfo implements IDocumentInfo
```

दस्तावेज़ के बारे में जानकारी दर्शाता है। IDocumentInfo इंटरफ़ेस को लागू करता है। देखें
IDocumentInfo
उदाहरणों के लिए।

*** ** * ** ***


**Learn more**

* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getFileType()](#getFileType--) | फ़ाइल फ़ॉर्मेट विवरण प्राप्त करता है। |
|
|  | [getPageCount()](#getPageCount--) | कुल पृष्ठ गिनती प्राप्त करता है। |
|
|  | [getSize()](#getSize--) | दस्तावेज़ का आकार बाइट्स में प्राप्त करता है। |
|
|  | [getPages()](#getPages--) | पृष्ठ जानकारी की सूची प्राप्त करता है। |
|
### getFileType() {#getFileType--}
```
public final FileType getFileType()
```


फ़ाइल फ़ॉर्मेट विवरण प्राप्त करता है।


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - The file format description.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


कुल पृष्ठ गिनती प्राप्त करता है।


**Returns:**
int - कुल पृष्ठ गिनती।

### getSize() {#getSize--}
```
public final long getSize()
```


दस्तावेज़ का आकार बाइट्स में प्राप्त करता है।


**Returns:**
long - दस्तावेज़ का आकार बाइट्स में।

### getPages() {#getPages--}
```
public final List<PageInfo> getPages()
```


पृष्ठ जानकारी की सूची प्राप्त करता है।


**Returns:**
java.util.List<com.groupdocs.redaction.PageInfo> - पृष्ठ जानकारी की सूची।

