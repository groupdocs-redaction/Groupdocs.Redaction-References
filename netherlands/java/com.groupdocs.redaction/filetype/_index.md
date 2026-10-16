---
title: "FileType"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt een bestandstype voor."
type: docs
weight: 11
url: /nl/java/com.groupdocs.redaction/filetype/
---
**Inheritance:**
java.lang.Object
```
public final class FileType
```

Stelt een bestandstype voor. Biedt methoden om een lijst te verkrijgen van alle bestandstypen die door GroupDocs.Redaction worden ondersteund, het bestandstype te detecteren op basis van extensie, enz.

*** ** * ** ***


**Learn more**

* [Supported Document Formats](../https://docs.groupdocs.com/redaction/java/supported-document-formats/)
* [Get supported file formats](../https://docs.groupdocs.com/redaction/java/get-supported-file-formats/)
* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Haalt de bestandstypenaam op, bijvoorbeeld "Microsoft Word Document". |
|
|  | [getExtension()](#getExtension--) | Haalt het bestandsnaameinde (inclusief de punt ".") op, bijvoorbeeld ".doc". |
|
|  | [getUnknown()](#getUnknown--) | Stelt een onbekend bestandstype voor. |
|
|  | [getTIF()](#getTIF--) | Tagged Image File (.tif) |
|
|  | [getTIFF()](#getTIFF--) | Tagged Image File Format (.tiff) |
|
|  | [getJPG()](#getJPG--) | JPEG-afbeelding (.jpg) |
|
|  | [getJPEG()](#getJPEG--) | JPEG-afbeelding (.jpeg) |
|
|  | [getPNG()](#getPNG--) | Portable Network Graphic (.png) |
|
|  | [getGIF()](#getGIF--) | Grafisch Interchange Format-bestand (.gif) |
|
|  | [getBMP()](#getBMP--) | Bitmap-afbeeldingsbestand (.bmp) |
|
|  | [getJP2()](#getJP2--) | JPEG 2000 Core-afbeeldingsbestand (.jp2) |
|
|  | [getHTM()](#getHTM--) | Hypertext Markup Language-bestand (.htm) |
|
|  | [getHTML()](#getHTML--) | Hypertext Markup Language-bestand (.html) |
|
|  | [getPDF()](#getPDF--) | Portable Document Format-bestand (.pdf) |
|
|  | [getPPT()](#getPPT--) | PowerPoint-presentatie (.ppt) |
|
|  | [getPPTX()](#getPPTX--) | PowerPoint Open XML-presentatie (.pptx) |
|
|  | [getODP()](#getODP--) | OpenDocument-presentatie (.odp) |
|
|  | [getPOTX()](#getPOTX--) | PowerPoint Open XML-presentatiesjabloon (.potx) |
|
|  | [getPOTM()](#getPOTM--) | PowerPoint Open XML-macro-ingeschakelde presentatiesjabloon (.potm) |
|
|  | [getOTP()](#getOTP--) | OpenDocument-presentatiesjabloon (.otp) |
|
|  | [getXLS()](#getXLS--) | Excel-werkblad (.xls) |
|
|  | [getXLSX()](#getXLSX--) | Microsoft Excel Open XML-werkblad (.xlsx) |
|
|  | [getXLSM()](#getXLSM--) | Excel Open XML-macro-ingeschakeld werkblad (.xlsm) |
|
|  | [getXLSB()](#getXLSB--) | Excel binair werkblad (.xlsb) |
|
|  | [getXLTX()](#getXLTX--) | Excel Open XML-werkbladsjabloon (.xltx) |
|
|  | [getXLTM()](#getXLTM--) | Excel Open XML-macro-ingeschakeld werkbladsjabloon (.xltm) |
|
|  | [getXLT()](#getXLT--) | Excel-sjabloon (.xlt) |
|
|  | [getCSV()](#getCSV--) | Komma-gescheiden waardenbestand (.csv) |
|
|  | [getTSV()](#getTSV--) | Tab-gescheiden waardenbestand (.tsv) |
|
|  | [getTAB()](#getTAB--) | Tab-gescheiden waardenbestand (.tab) |
|
|  | [getODS()](#getODS--) | OpenDocument Spreadsheet (.ods) |
|
|  | [getOTS()](#getOTS--) | OpenDocument Spreadsheet Template (.ots) |
|
|  | [getNUMBERS()](#getNUMBERS--) | Apple Numbers Spreadsheet (.numbers) |
|
|  | [getMD()](#getMD--) | Markdown Documentatiebestand (.md) |
|
|  | [getDOC()](#getDOC--) | Microsoft Word-document (.doc) |
|
|  | [getDOCX()](#getDOCX--) | Microsoft Word Open XML-document (.docx) |
|
|  | [getDOCM()](#getDOCM--) | Word Open XML-macro-ingeschakeld document (.docm) |
|
|  | [getDOT()](#getDOT--) | Word-documenttemplate (.dot) |
|
|  | [getDOTX()](#getDOTX--) | Word Open XML-documenttemplate (.dotx) |
|
|  | [getDOTM()](#getDOTM--) | Word Open XML-macro-ingeschakeld documenttemplate (.dotm) |
|
|  | [getRTF()](#getRTF--) | Rich Text Format-bestand (.rtf) |
|
|  | [getTXT()](#getTXT--) | Platte tekstbestand (.txt) |
|
|  | [getODT()](#getODT--) | OpenDocument Tekstdocument (.odt) |
|
|  | [getOTT()](#getOTT--) | OpenDocument Documenttemplate (.ott) |
|
|  | [fromExtension(String extension)](#fromExtension-java.lang.String-) | Koppelt bestandsextensie aan bestandstype. |
|
|  | [getSupportedFileTypes()](#getSupportedFileTypes--) | Haalt ondersteunde bestandstypen op |
|
|  | [equals(FileType other)](#equals-com.groupdocs.redaction.FileType-) | Bepaalt of de huidige |
FileType
hetzelfde is als gespecificeerd
FileType
object.
|
|  | [equals(Object obj)](#equals-java.lang.Object-) | Bepaalt of de huidige |
FileType
is hetzelfde als het gespecificeerde object.
|
|  | [hashCode()](#hashCode--) | Retourneert de hashcode voor de huidige |
FileType
object.
|
|  | [op_Equality(FileType left, FileType right)](#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Bepaalt of twee |
FileType
objecten hetzelfde zijn.
|
|  | [op_Inequality(FileType left, FileType right)](#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Bepaalt of twee |
FileType
objecten niet hetzelfde zijn.
|
|  | [toString()](#toString--) | Retourneert een string die het huidige object vertegenwoordigt. |
|
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


Haalt de bestandstypenaam op, bijvoorbeeld "Microsoft Word Document".


**Returns:**
java.lang.String - Bestandstype naam, bijvoorbeeld "Microsoft Word Document".

### getExtension() {#getExtension--}
```
public final String getExtension()
```


Haalt het bestandsnaameinde (inclusief de punt ".") op, bijvoorbeeld ".doc".


**Returns:**
java.lang.String - Bestandsnaamextensie (inclusief de punt "."), bijvoorbeeld ".doc".

### getUnknown() {#getUnknown--}
```
public static FileType getUnknown()
```


Stelt een onbekend bestandstype voor.


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


JPEG-afbeelding (.jpg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPEG() {#getJPEG--}
```
public static FileType getJPEG()
```


JPEG-afbeelding (.jpeg)


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


Grafisch Interchange Format-bestand (.gif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getBMP() {#getBMP--}
```
public static FileType getBMP()
```


Bitmap-afbeeldingsbestand (.bmp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJP2() {#getJP2--}
```
public static FileType getJP2()
```


JPEG 2000 Core-afbeeldingsbestand (.jp2)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTM() {#getHTM--}
```
public static FileType getHTM()
```


Hypertext Markup Language-bestand (.htm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTML() {#getHTML--}
```
public static FileType getHTML()
```


Hypertext Markup Language-bestand (.html)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPDF() {#getPDF--}
```
public static FileType getPDF()
```


Portable Document Format-bestand (.pdf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPT() {#getPPT--}
```
public static FileType getPPT()
```


PowerPoint-presentatie (.ppt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPTX() {#getPPTX--}
```
public static FileType getPPTX()
```


PowerPoint Open XML-presentatie (.pptx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODP() {#getODP--}
```
public static FileType getODP()
```


OpenDocument-presentatie (.odp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTX() {#getPOTX--}
```
public static FileType getPOTX()
```


PowerPoint Open XML-presentatiesjabloon (.potx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTM() {#getPOTM--}
```
public static FileType getPOTM()
```


PowerPoint Open XML-macro-ingeschakelde presentatiesjabloon (.potm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTP() {#getOTP--}
```
public static FileType getOTP()
```


OpenDocument-presentatiesjabloon (.otp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLS() {#getXLS--}
```
public static FileType getXLS()
```


Excel-werkblad (.xls)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSX() {#getXLSX--}
```
public static FileType getXLSX()
```


Microsoft Excel Open XML-werkblad (.xlsx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSM() {#getXLSM--}
```
public static FileType getXLSM()
```


Excel Open XML-macro-ingeschakeld werkblad (.xlsm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSB() {#getXLSB--}
```
public static FileType getXLSB()
```


Excel binair werkblad (.xlsb)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTX() {#getXLTX--}
```
public static FileType getXLTX()
```


Excel Open XML-werkbladsjabloon (.xltx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTM() {#getXLTM--}
```
public static FileType getXLTM()
```


Excel Open XML-macro-ingeschakeld werkbladsjabloon (.xltm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLT() {#getXLT--}
```
public static FileType getXLT()
```


Excel-sjabloon (.xlt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getCSV() {#getCSV--}
```
public static FileType getCSV()
```


Komma-gescheiden waardenbestand (.csv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTSV() {#getTSV--}
```
public static FileType getTSV()
```


Tab-gescheiden waardenbestand (.tsv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTAB() {#getTAB--}
```
public static FileType getTAB()
```


Tab-gescheiden waardenbestand (.tab)


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


Markdown Documentatiebestand (.md)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOC() {#getDOC--}
```
public static FileType getDOC()
```


Microsoft Word-document (.doc)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCX() {#getDOCX--}
```
public static FileType getDOCX()
```


Microsoft Word Open XML-document (.docx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCM() {#getDOCM--}
```
public static FileType getDOCM()
```


Word Open XML-macro-ingeschakeld document (.docm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOT() {#getDOT--}
```
public static FileType getDOT()
```


Word-documenttemplate (.dot)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTX() {#getDOTX--}
```
public static FileType getDOTX()
```


Word Open XML-documenttemplate (.dotx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTM() {#getDOTM--}
```
public static FileType getDOTM()
```


Word Open XML-macro-ingeschakeld documenttemplate (.dotm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getRTF() {#getRTF--}
```
public static FileType getRTF()
```


Rich Text Format-bestand (.rtf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTXT() {#getTXT--}
```
public static FileType getTXT()
```


Platte tekstbestand (.txt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODT() {#getODT--}
```
public static FileType getODT()
```


OpenDocument Tekstdocument (.odt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTT() {#getOTT--}
```
public static FileType getOTT()
```


OpenDocument Documenttemplate (.ott)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### fromExtension(String extension) {#fromExtension-java.lang.String-}
```
public static FileType fromExtension(String extension)
```


Koppelt bestandsextensie aan bestandstype.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | extensie | java.lang.String | Bestandsextensie (inclusief de punt "."). |
|

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - When file type is supported returns it, otherwise returns default  Unknown  file type.

### getSupportedFileTypes() {#getSupportedFileTypes--}
```
public static Iterable<FileType> getSupportedFileTypes()
```


Haalt ondersteunde bestandstypen op


**Returns:**
java.lang.Iterable<com.groupdocs.redaction.FileType> - Retourneert een reeks ondersteunde bestandstypen

### equals(FileType other) {#equals-com.groupdocs.redaction.FileType-}
```
public final boolean equals(FileType other)
```


Bepaalt of de huidige
FileType
hetzelfde is als gespecificeerd
FileType
object.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | other | [FileType](../../com.groupdocs.redaction/filetype) | Het object om te vergelijken met de huidige  FileType  object. |
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

als

```
obj
```

parameter is  FileType  en is hetzelfde als de huidige  FileType  object; anders,

```
false
```


### hashCode() {#hashCode--}
```
public int hashCode()
```


Retourneert de hashcode voor de huidige
FileType
object.


**Returns:**
int - Een hashcode voor de huidige  FileType  object.

### op_Equality(FileType left, FileType right) {#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Equality(FileType left, FileType right)
```


Bepaalt of twee
FileType
objecten hetzelfde zijn.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | left | [FileType](../../com.groupdocs.redaction/filetype) | Links  FileType  object. |
|
|  | right | [FileType](../../com.groupdocs.redaction/filetype) | Rechts  FileType  object. |
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

als beide  FileType  objecten niet hetzelfde zijn; anders,

```
false
```


### toString() {#toString--}
```
public String toString()
```


Retourneert een string die het huidige object vertegenwoordigt.


**Returns:**
java.lang.String - Een string die het huidige object vertegenwoordigt.

