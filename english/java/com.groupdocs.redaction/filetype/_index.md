---
title: FileType
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a file type.
type: docs
weight: 11
url: /java/com.groupdocs.redaction/filetype/
---
**Inheritance:**
java.lang.Object
```
public final class FileType
```

Represents a file type. Provides methods to obtain a list of all file types supported by GroupDocs.Redaction, detect file type by extension, etc.

--------------------

**Learn more**

 *  [Supported Document Formats][]
 *  [Get supported file formats][]
 *  [Get file info][]


[Supported Document Formats]: https://docs.groupdocs.com/redaction/java/supported-document-formats/
[Get supported file formats]: https://docs.groupdocs.com/redaction/java/get-supported-file-formats/
[Get file info]: https://docs.groupdocs.com/redaction/java/get-file-info/
## Methods

| Method | Description |
| --- | --- |
| [getFileFormat()](#getFileFormat--) | Gets file type name, for example "Microsoft Word Document". |
| [getExtension()](#getExtension--) | Gets filename suffix (including the period "."), for instance ".doc". |
| [getUnknown()](#getUnknown--) | Represents unknown file type. |
| [getTIF()](#getTIF--) | Tagged Image File (.tif) |
| [getTIFF()](#getTIFF--) | Tagged Image File Format (.tiff) |
| [getJPG()](#getJPG--) | JPEG Image (.jpg) |
| [getJPEG()](#getJPEG--) | JPEG Image (.jpeg) |
| [getPNG()](#getPNG--) | Portable Network Graphic (.png) |
| [getGIF()](#getGIF--) | Graphical Interchange Format File (.gif) |
| [getBMP()](#getBMP--) | Bitmap Image File (.bmp) |
| [getJP2()](#getJP2--) | JPEG 2000 Core Image File (.jp2) |
| [getHTM()](#getHTM--) | Hypertext Markup Language File (.htm) |
| [getHTML()](#getHTML--) | Hypertext Markup Language File (.html) |
| [getPDF()](#getPDF--) | Portable Document Format File (.pdf) |
| [getPPT()](#getPPT--) | PowerPoint Presentation (.ppt) |
| [getPPTX()](#getPPTX--) | PowerPoint Open XML Presentation (.pptx) |
| [getODP()](#getODP--) | OpenDocument Presentation (.odp) |
| [getXLS()](#getXLS--) | Excel Spreadsheet (.xls) |
| [getXLSX()](#getXLSX--) | Microsoft Excel Open XML Spreadsheet (.xlsx) |
| [getXLSM()](#getXLSM--) | Excel Open XML Macro-Enabled Spreadsheet (.xlsm) |
| [getXLSB()](#getXLSB--) | Excel Binary Spreadsheet (.xlsb) |
| [getCSV()](#getCSV--) | Comma Separated Values File (.csv) |
| [getTSV()](#getTSV--) | Tab Separated Values File (.tsv) |
| [getODS()](#getODS--) | OpenDocument Spreadsheet (.ods) |
| [getOTS()](#getOTS--) | OpenDocument Spreadsheet Template (.ots) |
| [getNUMBERS()](#getNUMBERS--) | Apple Numbers Spreadsheet (.numbers) |
| [getMD()](#getMD--) | Markdown Documentation File (.md) |
| [getDOC()](#getDOC--) | Microsoft Word Document (.doc) |
| [getDOCX()](#getDOCX--) | Microsoft Word Open XML Document (.docx) |
| [getDOCM()](#getDOCM--) | Word Open XML Macro-Enabled Document (.docm) |
| [getDOT()](#getDOT--) | Word Document Template (.dot) |
| [getDOTX()](#getDOTX--) | Word Open XML Document Template (.dotx) |
| [getDOTM()](#getDOTM--) | Word Open XML Macro-Enabled Document Template (.dotm) |
| [getRTF()](#getRTF--) | Rich Text Format File (.rtf) |
| [getTXT()](#getTXT--) | Plain Text File (.txt) |
| [getODT()](#getODT--) | OpenDocument Text Document (.odt) |
| [getOTT()](#getOTT--) | OpenDocument Document Template (.ott) |
| [fromExtension(String extension)](#fromExtension-java.lang.String-) | Maps file extension to file type. |
| [getSupportedFileTypes()](#getSupportedFileTypes--) | Retrieves supported file types |
| [equals(FileType other)](#equals-com.groupdocs.redaction.FileType-) | Determines whether the current  FileType  is the same as specified  FileType  object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determines whether the current  FileType  is the same as specified object. |
| [hashCode()](#hashCode--) | Returns the hash code for the current  FileType  object. |
| [op_Equality(FileType left, FileType right)](#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Determines whether two  FileType  objects are the same. |
| [op_Inequality(FileType left, FileType right)](#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Determines whether two  FileType  objects are not the same. |
| [toString()](#toString--) | Returns a string that represents the current object. |
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


Gets file type name, for example "Microsoft Word Document".

**Returns:**
java.lang.String - File type name, for example "Microsoft Word Document".
### getExtension() {#getExtension--}
```
public final String getExtension()
```


Gets filename suffix (including the period "."), for instance ".doc".

**Returns:**
java.lang.String - Filename suffix (including the period "."), for instance ".doc".
### getUnknown() {#getUnknown--}
```
public static FileType getUnknown()
```


Represents unknown file type.

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


JPEG Image (.jpg)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPEG() {#getJPEG--}
```
public static FileType getJPEG()
```


JPEG Image (.jpeg)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPNG() {#getPNG--}
```
public static FileType getPNG()
```


Portable Network Graphic (.png)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getGIF() {#getGIF--}
```
public static FileType getGIF()
```


Graphical Interchange Format File (.gif)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getBMP() {#getBMP--}
```
public static FileType getBMP()
```


Bitmap Image File (.bmp)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJP2() {#getJP2--}
```
public static FileType getJP2()
```


JPEG 2000 Core Image File (.jp2)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTM() {#getHTM--}
```
public static FileType getHTM()
```


Hypertext Markup Language File (.htm)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTML() {#getHTML--}
```
public static FileType getHTML()
```


Hypertext Markup Language File (.html)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPDF() {#getPDF--}
```
public static FileType getPDF()
```


Portable Document Format File (.pdf)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPT() {#getPPT--}
```
public static FileType getPPT()
```


PowerPoint Presentation (.ppt)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPTX() {#getPPTX--}
```
public static FileType getPPTX()
```


PowerPoint Open XML Presentation (.pptx)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODP() {#getODP--}
```
public static FileType getODP()
```


OpenDocument Presentation (.odp)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLS() {#getXLS--}
```
public static FileType getXLS()
```


Excel Spreadsheet (.xls)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSX() {#getXLSX--}
```
public static FileType getXLSX()
```


Microsoft Excel Open XML Spreadsheet (.xlsx)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSM() {#getXLSM--}
```
public static FileType getXLSM()
```


Excel Open XML Macro-Enabled Spreadsheet (.xlsm)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSB() {#getXLSB--}
```
public static FileType getXLSB()
```


Excel Binary Spreadsheet (.xlsb)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getCSV() {#getCSV--}
```
public static FileType getCSV()
```


Comma Separated Values File (.csv)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTSV() {#getTSV--}
```
public static FileType getTSV()
```


Tab Separated Values File (.tsv)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODS() {#getODS--}
```
public static FileType getODS()
```


OpenDocument Spreadsheet (.ods)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTS() {#getOTS--}
```
public static FileType getOTS()
```


OpenDocument Spreadsheet Template (.ots)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getNUMBERS() {#getNUMBERS--}
```
public static FileType getNUMBERS()
```


Apple Numbers Spreadsheet (.numbers)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getMD() {#getMD--}
```
public static FileType getMD()
```


Markdown Documentation File (.md)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOC() {#getDOC--}
```
public static FileType getDOC()
```


Microsoft Word Document (.doc)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCX() {#getDOCX--}
```
public static FileType getDOCX()
```


Microsoft Word Open XML Document (.docx)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCM() {#getDOCM--}
```
public static FileType getDOCM()
```


Word Open XML Macro-Enabled Document (.docm)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOT() {#getDOT--}
```
public static FileType getDOT()
```


Word Document Template (.dot)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTX() {#getDOTX--}
```
public static FileType getDOTX()
```


Word Open XML Document Template (.dotx)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTM() {#getDOTM--}
```
public static FileType getDOTM()
```


Word Open XML Macro-Enabled Document Template (.dotm)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getRTF() {#getRTF--}
```
public static FileType getRTF()
```


Rich Text Format File (.rtf)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTXT() {#getTXT--}
```
public static FileType getTXT()
```


Plain Text File (.txt)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODT() {#getODT--}
```
public static FileType getODT()
```


OpenDocument Text Document (.odt)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTT() {#getOTT--}
```
public static FileType getOTT()
```


OpenDocument Document Template (.ott)

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### fromExtension(String extension) {#fromExtension-java.lang.String-}
```
public static FileType fromExtension(String extension)
```


Maps file extension to file type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| extension | java.lang.String | File extension (including the period "."). |

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - When file type is supported returns it, otherwise returns default  Unknown  file type.
### getSupportedFileTypes() {#getSupportedFileTypes--}
```
public static Iterable<FileType> getSupportedFileTypes()
```


Retrieves supported file types

**Returns:**
java.lang.Iterable<com.groupdocs.redaction.FileType> - Returns sequence of supported file types
### equals(FileType other) {#equals-com.groupdocs.redaction.FileType-}
```
public final boolean equals(FileType other)
```


Determines whether the current  FileType  is the same as specified  FileType  object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [FileType](../../com.groupdocs.redaction/filetype) | The object to compare with the current  FileType  object. |

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


Determines whether the current  FileType  is the same as specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The object to compare with the current  FileType  object. |

**Returns:**
boolean - ```
true
```

if

```
obj
```

parameter is  FileType  and is the same as current  FileType  object; otherwise,

```
false
```
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns the hash code for the current  FileType  object.

**Returns:**
int - A hash code for the current  FileType  object.
### op_Equality(FileType left, FileType right) {#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Equality(FileType left, FileType right)
```


Determines whether two  FileType  objects are the same.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| left | [FileType](../../com.groupdocs.redaction/filetype) | Left  FileType  object. |
| right | [FileType](../../com.groupdocs.redaction/filetype) | Right  FileType  object. |

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


Determines whether two  FileType  objects are not the same.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| left | [FileType](../../com.groupdocs.redaction/filetype) | Left  FileType  object. |
| right | [FileType](../../com.groupdocs.redaction/filetype) | Right  FileType  object. |

**Returns:**
boolean - ```
true
```

if both  FileType  objects are not the same; otherwise,

```
false
```
### toString() {#toString--}
```
public String toString()
```


Returns a string that represents the current object.

**Returns:**
java.lang.String - A string that represents the current object.
