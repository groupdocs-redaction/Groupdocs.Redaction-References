---
title: "FileType"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar en filtyp."
type: docs
weight: 11
url: /sv/java/com.groupdocs.redaction/filetype/
---
**Inheritance:**
java.lang.Object
```
public final class FileType
```

Representerar en filtyp. Tillhandahåller metoder för att erhålla en lista över alla filtyper som stöds av GroupDocs.Redaction, upptäcka filtyp via filändelse, etc.

*** ** * ** ***


**Learn more**

* [Supported Document Formats](../https://docs.groupdocs.com/redaction/java/supported-document-formats/)
* [Get supported file formats](../https://docs.groupdocs.com/redaction/java/get-supported-file-formats/)
* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Hämtar filtypens namn, till exempel "Microsoft Word Document". |
|
|  | [getExtension()](#getExtension--) | Hämtar filnamnssuffix (inklusive punkten "."), till exempel ".doc". |
|
|  | [getUnknown()](#getUnknown--) | Representerar okänd filtyp. |
|
|  | [getTIF()](#getTIF--) | Taggad bildfil (.tif) |
|
|  | [getTIFF()](#getTIFF--) | Taggat bildfilformat (.tiff) |
|
|  | [getJPG()](#getJPG--) | JPEG-bild (.jpg) |
|
|  | [getJPEG()](#getJPEG--) | JPEG-bild (.jpeg) |
|
|  | [getPNG()](#getPNG--) | Portable Network-grafik (.png) |
|
|  | [getGIF()](#getGIF--) | Graphics Interchange Format-fil (.gif) |
|
|  | [getBMP()](#getBMP--) | Bitmap-bildfil (.bmp) |
|
|  | [getJP2()](#getJP2--) | JPEG 2000 Core-bildfil (.jp2) |
|
|  | [getHTM()](#getHTM--) | Hypertext Markup Language-fil (.htm) |
|
|  | [getHTML()](#getHTML--) | Hypertext Markup Language-fil (.html) |
|
|  | [getPDF()](#getPDF--) | Portable Document Format-fil (.pdf) |
|
|  | [getPPT()](#getPPT--) | PowerPoint-presentation (.ppt) |
|
|  | [getPPTX()](#getPPTX--) | PowerPoint Open XML-presentation (.pptx) |
|
|  | [getODP()](#getODP--) | OpenDocument-presentation (.odp) |
|
|  | [getPOTX()](#getPOTX--) | PowerPoint Open XML-presentationmall (.potx) |
|
|  | [getPOTM()](#getPOTM--) | PowerPoint Open XML-makroaktiverad presentationmall (.potm) |
|
|  | [getOTP()](#getOTP--) | OpenDocument-presentationmall (.otp) |
|
|  | [getXLS()](#getXLS--) | Excel-kalkylblad (.xls) |
|
|  | [getXLSX()](#getXLSX--) | Microsoft Excel Open XML-kalkylblad (.xlsx) |
|
|  | [getXLSM()](#getXLSM--) | Excel Open XML-makroaktiverat kalkylblad (.xlsm) |
|
|  | [getXLSB()](#getXLSB--) | Excel binärt kalkylblad (.xlsb) |
|
|  | [getXLTX()](#getXLTX--) | Excel Open XML-kalkylbladsmall (.xltx) |
|
|  | [getXLTM()](#getXLTM--) | Excel Open XML-makroaktiverad kalkylbladsmall (.xltm) |
|
|  | [getXLT()](#getXLT--) | Excel-mall (.xlt) |
|
|  | [getCSV()](#getCSV--) | Kommaseparerad värdefil (.csv) |
|
|  | [getTSV()](#getTSV--) | Tabbseparerad värdefil (.tsv) |
|
|  | [getTAB()](#getTAB--) | Tabbseparerad värdefil (.tab) |
|
|  | [getODS()](#getODS--) | OpenDocument-kalkylblad (.ods) |
|
|  | [getOTS()](#getOTS--) | OpenDocument-kalkylbladsmall (.ots) |
|
|  | [getNUMBERS()](#getNUMBERS--) | Apple Numbers-kalkylblad (.numbers) |
|
|  | [getMD()](#getMD--) | Markdown-dokumentationsfil (.md) |
|
|  | [getDOC()](#getDOC--) | Microsoft Word-dokument (.doc) |
|
|  | [getDOCX()](#getDOCX--) | Microsoft Word Open XML-dokument (.docx) |
|
|  | [getDOCM()](#getDOCM--) | Word Open XML-makroaktiverat dokument (.docm) |
|
|  | [getDOT()](#getDOT--) | Word-dokumentmall (.dot) |
|
|  | [getDOTX()](#getDOTX--) | Word Open XML-dokumentmall (.dotx) |
|
|  | [getDOTM()](#getDOTM--) | Word Open XML-makroaktiverad dokumentmall (.dotm) |
|
|  | [getRTF()](#getRTF--) | Rich Text Format-fil (.rtf) |
|
|  | [getTXT()](#getTXT--) | Vanlig textfil (.txt) |
|
|  | [getODT()](#getODT--) | OpenDocument-textdokument (.odt) |
|
|  | [getOTT()](#getOTT--) | OpenDocument-dokumentmall (.ott) |
|
|  | [fromExtension(String extension)](#fromExtension-java.lang.String-) | Kopplar filändelse till filtyp. |
|
|  | [getSupportedFileTypes()](#getSupportedFileTypes--) | Hämtar stödda filtyper |
|
|  | [equals(FileType other)](#equals-com.groupdocs.redaction.FileType-) | Bestämmer om den aktuella |
FileType
är densamma som angiven
FileType
objektet.
|
|  | [equals(Object obj)](#equals-java.lang.Object-) | Bestämmer om den aktuella |
FileType
är densamma som angivet objekt.
|
|  | [hashCode()](#hashCode--) | Returnerar hashkoden för den aktuella |
FileType
objektet.
|
|  | [op_Equality(FileType left, FileType right)](#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Bestämmer om två |
FileType
objekt är samma.
|
|  | [op_Inequality(FileType left, FileType right)](#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Bestämmer om två |
FileType
objekt är inte samma.
|
|  | [toString()](#toString--) | Returnerar en sträng som representerar det aktuella objektet. |
|
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


Hämtar filtypens namn, till exempel "Microsoft Word Document".


**Returns:**
java.lang.String - Filtypnamn, till exempel "Microsoft Word Document".

### getExtension() {#getExtension--}
```
public final String getExtension()
```


Hämtar filnamnssuffix (inklusive punkten "."), till exempel ".doc".


**Returns:**
java.lang.String - Filnamnstillägg (inklusive perioden "."), till exempel ".doc".

### getUnknown() {#getUnknown--}
```
public static FileType getUnknown()
```


Representerar okänd filtyp.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIF() {#getTIF--}
```
public static FileType getTIF()
```


Taggad bildfil (.tif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIFF() {#getTIFF--}
```
public static FileType getTIFF()
```


Taggat bildfilformat (.tiff)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPG() {#getJPG--}
```
public static FileType getJPG()
```


JPEG-bild (.jpg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPEG() {#getJPEG--}
```
public static FileType getJPEG()
```


JPEG-bild (.jpeg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPNG() {#getPNG--}
```
public static FileType getPNG()
```


Portable Network-grafik (.png)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getGIF() {#getGIF--}
```
public static FileType getGIF()
```


Graphics Interchange Format-fil (.gif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getBMP() {#getBMP--}
```
public static FileType getBMP()
```


Bitmap-bildfil (.bmp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJP2() {#getJP2--}
```
public static FileType getJP2()
```


JPEG 2000 Core-bildfil (.jp2)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTM() {#getHTM--}
```
public static FileType getHTM()
```


Hypertext Markup Language-fil (.htm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTML() {#getHTML--}
```
public static FileType getHTML()
```


Hypertext Markup Language-fil (.html)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPDF() {#getPDF--}
```
public static FileType getPDF()
```


Portable Document Format-fil (.pdf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPT() {#getPPT--}
```
public static FileType getPPT()
```


PowerPoint-presentation (.ppt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPTX() {#getPPTX--}
```
public static FileType getPPTX()
```


PowerPoint Open XML-presentation (.pptx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODP() {#getODP--}
```
public static FileType getODP()
```


OpenDocument-presentation (.odp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTX() {#getPOTX--}
```
public static FileType getPOTX()
```


PowerPoint Open XML-presentationmall (.potx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTM() {#getPOTM--}
```
public static FileType getPOTM()
```


PowerPoint Open XML-makroaktiverad presentationmall (.potm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTP() {#getOTP--}
```
public static FileType getOTP()
```


OpenDocument-presentationmall (.otp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLS() {#getXLS--}
```
public static FileType getXLS()
```


Excel-kalkylblad (.xls)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSX() {#getXLSX--}
```
public static FileType getXLSX()
```


Microsoft Excel Open XML-kalkylblad (.xlsx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSM() {#getXLSM--}
```
public static FileType getXLSM()
```


Excel Open XML-makroaktiverat kalkylblad (.xlsm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSB() {#getXLSB--}
```
public static FileType getXLSB()
```


Excel binärt kalkylblad (.xlsb)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTX() {#getXLTX--}
```
public static FileType getXLTX()
```


Excel Open XML-kalkylbladsmall (.xltx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTM() {#getXLTM--}
```
public static FileType getXLTM()
```


Excel Open XML-makroaktiverad kalkylbladsmall (.xltm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLT() {#getXLT--}
```
public static FileType getXLT()
```


Excel-mall (.xlt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getCSV() {#getCSV--}
```
public static FileType getCSV()
```


Kommaseparerad värdefil (.csv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTSV() {#getTSV--}
```
public static FileType getTSV()
```


Tabbseparerad värdefil (.tsv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTAB() {#getTAB--}
```
public static FileType getTAB()
```


Tabbseparerad värdefil (.tab)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODS() {#getODS--}
```
public static FileType getODS()
```


OpenDocument-kalkylblad (.ods)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTS() {#getOTS--}
```
public static FileType getOTS()
```


OpenDocument-kalkylbladsmall (.ots)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getNUMBERS() {#getNUMBERS--}
```
public static FileType getNUMBERS()
```


Apple Numbers-kalkylblad (.numbers)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getMD() {#getMD--}
```
public static FileType getMD()
```


Markdown-dokumentationsfil (.md)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOC() {#getDOC--}
```
public static FileType getDOC()
```


Microsoft Word-dokument (.doc)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCX() {#getDOCX--}
```
public static FileType getDOCX()
```


Microsoft Word Open XML-dokument (.docx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCM() {#getDOCM--}
```
public static FileType getDOCM()
```


Word Open XML-makroaktiverat dokument (.docm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOT() {#getDOT--}
```
public static FileType getDOT()
```


Word-dokumentmall (.dot)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTX() {#getDOTX--}
```
public static FileType getDOTX()
```


Word Open XML-dokumentmall (.dotx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTM() {#getDOTM--}
```
public static FileType getDOTM()
```


Word Open XML-makroaktiverad dokumentmall (.dotm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getRTF() {#getRTF--}
```
public static FileType getRTF()
```


Rich Text Format-fil (.rtf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTXT() {#getTXT--}
```
public static FileType getTXT()
```


Vanlig textfil (.txt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODT() {#getODT--}
```
public static FileType getODT()
```


OpenDocument-textdokument (.odt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTT() {#getOTT--}
```
public static FileType getOTT()
```


OpenDocument-dokumentmall (.ott)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### fromExtension(String extension) {#fromExtension-java.lang.String-}
```
public static FileType fromExtension(String extension)
```


Kopplar filändelse till filtyp.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filändelse | java.lang.String | Filändelse (inklusive perioden "."). |
|

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - When file type is supported returns it, otherwise returns default  Unknown  file type.

### getSupportedFileTypes() {#getSupportedFileTypes--}
```
public static Iterable<FileType> getSupportedFileTypes()
```


Hämtar stödda filtyper


**Returns:**
java.lang.Iterable<com.groupdocs.redaction.FileType> - Returnerar sekvens av stödda filtyper

### equals(FileType other) {#equals-com.groupdocs.redaction.FileType-}
```
public final boolean equals(FileType other)
```


Bestämmer om den aktuella
FileType
är densamma som angiven
FileType
objektet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | other | [FileType](../../com.groupdocs.redaction/filetype) | Objektet att jämföra med det aktuella  FileType  -objektet. |
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

if

```
obj
```

parametern är  FileType  och är samma som det aktuella  FileType  -objektet; annars,

```
false
```


### hashCode() {#hashCode--}
```
public int hashCode()
```


Returnerar hashkoden för den aktuella
FileType
objektet.


**Returns:**
int - En hashkod för det aktuella  FileType  -objektet.

### op_Equality(FileType left, FileType right) {#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Equality(FileType left, FileType right)
```


Bestämmer om två
FileType
objekt är samma.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | left | [FileType](../../com.groupdocs.redaction/filetype) | Vänster  FileType  -objekt. |
|
|  | right | [FileType](../../com.groupdocs.redaction/filetype) | Höger  FileType  -objekt. |
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

om båda  FileType  -objekten inte är samma; annars,

```
false
```


### toString() {#toString--}
```
public String toString()
```


Returnerar en sträng som representerar det aktuella objektet.


**Returns:**
java.lang.String - En sträng som representerar det aktuella objektet.

