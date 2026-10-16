---
title: "FileType"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示一种文件类型。"
type: docs
weight: 11
url: /zh/java/com.groupdocs.redaction/filetype/
---
**Inheritance:**
java.lang.Object
```
public final class FileType
```

表示文件类型。提供获取 GroupDocs.Redaction 支持的所有文件类型列表、通过扩展名检测文件类型等方法。

*** ** * ** ***


**Learn more**

* [Supported Document Formats](../https://docs.groupdocs.com/redaction/java/supported-document-formats/)
* [Get supported file formats](../https://docs.groupdocs.com/redaction/java/get-supported-file-formats/)
* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | 获取文件类型名称，例如 "Microsoft Word Document"。 |
|
|  | [getExtension()](#getExtension--) | 获取文件名后缀（包括句点 "."），例如 ".doc"。 |
|
|  | [getUnknown()](#getUnknown--) | 表示未知文件类型。 |
|
|  | [getTIF()](#getTIF--) | 标签图像文件（.tif） |
|
|  | [getTIFF()](#getTIFF--) | 标签图像文件格式（.tiff） |
|
|  | [getJPG()](#getJPG--) | JPEG 图像 (.jpg) |
|
|  | [getJPEG()](#getJPEG--) | JPEG 图像 (.jpeg) |
|
|  | [getPNG()](#getPNG--) | 便携式网络图形 (.png) |
|
|  | [getGIF()](#getGIF--) | 图形交换格式文件 (.gif) |
|
|  | [getBMP()](#getBMP--) | 位图图像文件 (.bmp) |
|
|  | [getJP2()](#getJP2--) | JPEG 2000 核心图像文件 (.jp2) |
|
|  | [getHTM()](#getHTM--) | 超文本标记语言文件 (.htm) |
|
|  | [getHTML()](#getHTML--) | 超文本标记语言文件 (.html) |
|
|  | [getPDF()](#getPDF--) | 便携式文档格式文件 (.pdf) |
|
|  | [getPPT()](#getPPT--) | PowerPoint 演示文稿 (.ppt) |
|
|  | [getPPTX()](#getPPTX--) | PowerPoint Open XML 演示文稿 (.pptx) |
|
|  | [getODP()](#getODP--) | OpenDocument 演示文稿 (.odp) |
|
|  | [getPOTX()](#getPOTX--) | PowerPoint Open XML 演示文稿模板 (.potx) |
|
|  | [getPOTM()](#getPOTM--) | PowerPoint Open XML 启用宏的演示文稿模板 (.potm) |
|
|  | [getOTP()](#getOTP--) | OpenDocument 演示文稿模板 (.otp) |
|
|  | [getXLS()](#getXLS--) | Excel 电子表格 (.xls) |
|
|  | [getXLSX()](#getXLSX--) | Microsoft Excel Open XML 电子表格 (.xlsx) |
|
|  | [getXLSM()](#getXLSM--) | Excel Open XML 启用宏的电子表格 (.xlsm) |
|
|  | [getXLSB()](#getXLSB--) | Excel 二进制电子表格 (.xlsb) |
|
|  | [getXLTX()](#getXLTX--) | Excel Open XML 电子表格模板 (.xltx) |
|
|  | [getXLTM()](#getXLTM--) | Excel Open XML 启用宏的电子表格模板 (.xltm) |
|
|  | [getXLT()](#getXLT--) | Excel 模板 (.xlt) |
|
|  | [getCSV()](#getCSV--) | 逗号分隔值文件 (.csv) |
|
|  | [getTSV()](#getTSV--) | 制表符分隔值文件 (.tsv) |
|
|  | [getTAB()](#getTAB--) | 制表符分隔值文件 (.tab) |
|
|  | [getODS()](#getODS--) | OpenDocument 电子表格 (.ods) |
|
|  | [getOTS()](#getOTS--) | OpenDocument 电子表格模板 (.ots) |
|
|  | [getNUMBERS()](#getNUMBERS--) | Apple Numbers 电子表格 (.numbers) |
|
|  | [getMD()](#getMD--) | Markdown 文档文件 (.md) |
|
|  | [getDOC()](#getDOC--) | Microsoft Word 文档 (.doc) |
|
|  | [getDOCX()](#getDOCX--) | Microsoft Word Open XML 文档 (.docx) |
|
|  | [getDOCM()](#getDOCM--) | Word Open XML 启用宏的文档 (.docm) |
|
|  | [getDOT()](#getDOT--) | Word 文档模板 (.dot) |
|
|  | [getDOTX()](#getDOTX--) | Word Open XML 文档模板 (.dotx) |
|
|  | [getDOTM()](#getDOTM--) | Word Open XML 启用宏的文档模板 (.dotm) |
|
|  | [getRTF()](#getRTF--) | 富文本格式文件 (.rtf) |
|
|  | [getTXT()](#getTXT--) | 纯文本文件 (.txt) |
|
|  | [getODT()](#getODT--) | OpenDocument 文本文档 (.odt) |
|
|  | [getOTT()](#getOTT--) | OpenDocument 文档模板 (.ott) |
|
|  | [fromExtension(String extension)](#fromExtension-java.lang.String-) | 将文件扩展名映射到文件类型。 |
|
|  | [getSupportedFileTypes()](#getSupportedFileTypes--) | 检索受支持的文件类型 |
|
|  | [equals(FileType other)](#equals-com.groupdocs.redaction.FileType-) | 确定当前的 |
FileType
是否与指定的相同
FileType
对象。
|
|  | [equals(Object obj)](#equals-java.lang.Object-) | 确定当前的 |
FileType
是否与指定的对象相同。
|
|  | [hashCode()](#hashCode--) | 返回当前的哈希码 |
FileType
对象。
|
|  | [op_Equality(FileType left, FileType right)](#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | 确定两个 |
FileType
对象是否相同。
|
|  | [op_Inequality(FileType left, FileType right)](#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | 确定两个 |
FileType
对象不相同。
|
|  | [toString()](#toString--) | 返回表示当前对象的字符串。 |
|
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


获取文件类型名称，例如 "Microsoft Word Document"。


**Returns:**
java.lang.String - 文件类型名称，例如 "Microsoft Word Document".

### getExtension() {#getExtension--}
```
public final String getExtension()
```


获取文件名后缀（包括句点 "."），例如 ".doc"。


**Returns:**
java.lang.String - 文件名后缀（包括句点 "."），例如 ".doc".

### getUnknown() {#getUnknown--}
```
public static FileType getUnknown()
```


表示未知文件类型。


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIF() {#getTIF--}
```
public static FileType getTIF()
```


标签图像文件（.tif）


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIFF() {#getTIFF--}
```
public static FileType getTIFF()
```


标签图像文件格式（.tiff）


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPG() {#getJPG--}
```
public static FileType getJPG()
```


JPEG 图像 (.jpg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPEG() {#getJPEG--}
```
public static FileType getJPEG()
```


JPEG 图像 (.jpeg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPNG() {#getPNG--}
```
public static FileType getPNG()
```


便携式网络图形 (.png)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getGIF() {#getGIF--}
```
public static FileType getGIF()
```


图形交换格式文件 (.gif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getBMP() {#getBMP--}
```
public static FileType getBMP()
```


位图图像文件 (.bmp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJP2() {#getJP2--}
```
public static FileType getJP2()
```


JPEG 2000 核心图像文件 (.jp2)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTM() {#getHTM--}
```
public static FileType getHTM()
```


超文本标记语言文件 (.htm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTML() {#getHTML--}
```
public static FileType getHTML()
```


超文本标记语言文件 (.html)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPDF() {#getPDF--}
```
public static FileType getPDF()
```


便携式文档格式文件 (.pdf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPT() {#getPPT--}
```
public static FileType getPPT()
```


PowerPoint 演示文稿 (.ppt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPTX() {#getPPTX--}
```
public static FileType getPPTX()
```


PowerPoint Open XML 演示文稿 (.pptx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODP() {#getODP--}
```
public static FileType getODP()
```


OpenDocument 演示文稿 (.odp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTX() {#getPOTX--}
```
public static FileType getPOTX()
```


PowerPoint Open XML 演示文稿模板 (.potx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTM() {#getPOTM--}
```
public static FileType getPOTM()
```


PowerPoint Open XML 启用宏的演示文稿模板 (.potm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTP() {#getOTP--}
```
public static FileType getOTP()
```


OpenDocument 演示文稿模板 (.otp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLS() {#getXLS--}
```
public static FileType getXLS()
```


Excel 电子表格 (.xls)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSX() {#getXLSX--}
```
public static FileType getXLSX()
```


Microsoft Excel Open XML 电子表格 (.xlsx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSM() {#getXLSM--}
```
public static FileType getXLSM()
```


Excel Open XML 启用宏的电子表格 (.xlsm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSB() {#getXLSB--}
```
public static FileType getXLSB()
```


Excel 二进制电子表格 (.xlsb)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTX() {#getXLTX--}
```
public static FileType getXLTX()
```


Excel Open XML 电子表格模板 (.xltx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTM() {#getXLTM--}
```
public static FileType getXLTM()
```


Excel Open XML 启用宏的电子表格模板 (.xltm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLT() {#getXLT--}
```
public static FileType getXLT()
```


Excel 模板 (.xlt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getCSV() {#getCSV--}
```
public static FileType getCSV()
```


逗号分隔值文件 (.csv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTSV() {#getTSV--}
```
public static FileType getTSV()
```


制表符分隔值文件 (.tsv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTAB() {#getTAB--}
```
public static FileType getTAB()
```


制表符分隔值文件 (.tab)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODS() {#getODS--}
```
public static FileType getODS()
```


OpenDocument 电子表格 (.ods)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTS() {#getOTS--}
```
public static FileType getOTS()
```


OpenDocument 电子表格模板 (.ots)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getNUMBERS() {#getNUMBERS--}
```
public static FileType getNUMBERS()
```


Apple Numbers 电子表格 (.numbers)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getMD() {#getMD--}
```
public static FileType getMD()
```


Markdown 文档文件 (.md)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOC() {#getDOC--}
```
public static FileType getDOC()
```


Microsoft Word 文档 (.doc)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCX() {#getDOCX--}
```
public static FileType getDOCX()
```


Microsoft Word Open XML 文档 (.docx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCM() {#getDOCM--}
```
public static FileType getDOCM()
```


Word Open XML 启用宏的文档 (.docm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOT() {#getDOT--}
```
public static FileType getDOT()
```


Word 文档模板 (.dot)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTX() {#getDOTX--}
```
public static FileType getDOTX()
```


Word Open XML 文档模板 (.dotx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTM() {#getDOTM--}
```
public static FileType getDOTM()
```


Word Open XML 启用宏的文档模板 (.dotm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getRTF() {#getRTF--}
```
public static FileType getRTF()
```


富文本格式文件 (.rtf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTXT() {#getTXT--}
```
public static FileType getTXT()
```


纯文本文件 (.txt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODT() {#getODT--}
```
public static FileType getODT()
```


OpenDocument 文本文档 (.odt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTT() {#getOTT--}
```
public static FileType getOTT()
```


OpenDocument 文档模板 (.ott)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### fromExtension(String extension) {#fromExtension-java.lang.String-}
```
public static FileType fromExtension(String extension)
```


将文件扩展名映射到文件类型。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 扩展名 | java.lang.String | 文件扩展名（包括句点 "."）。 |
|

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - When file type is supported returns it, otherwise returns default  Unknown  file type.

### getSupportedFileTypes() {#getSupportedFileTypes--}
```
public static Iterable<FileType> getSupportedFileTypes()
```


检索受支持的文件类型


**Returns:**
java.lang.Iterable<com.groupdocs.redaction.FileType> - 返回受支持文件类型的序列

### equals(FileType other) {#equals-com.groupdocs.redaction.FileType-}
```
public final boolean equals(FileType other)
```


确定当前的
FileType
是否与指定的相同
FileType
对象。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | other | [FileType](../../com.groupdocs.redaction/filetype) | 与当前  FileType  对象比较的对象。 |
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

如果

```
obj
```

参数是  FileType  并且与当前  FileType  对象相同；否则，

```
false
```


### hashCode() {#hashCode--}
```
public int hashCode()
```


返回当前的哈希码
FileType
对象。


**Returns:**
int - 当前  FileType  对象的哈希码。

### op_Equality(FileType left, FileType right) {#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Equality(FileType left, FileType right)
```


确定两个
FileType
对象是否相同。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | left | [FileType](../../com.groupdocs.redaction/filetype) | 左侧  FileType  对象。 |
|
|  | right | [FileType](../../com.groupdocs.redaction/filetype) | 右侧  FileType  对象。 |
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

如果两个  FileType  对象不相同；否则，

```
false
```


### toString() {#toString--}
```
public String toString()
```


返回表示当前对象的字符串。


**Returns:**
java.lang.String - 表示当前对象的字符串。

