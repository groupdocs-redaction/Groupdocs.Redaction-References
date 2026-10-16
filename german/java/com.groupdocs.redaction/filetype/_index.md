---
title: "FileType"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt einen Dateityp dar."
type: docs
weight: 11
url: /de/java/com.groupdocs.redaction/filetype/
---
**Inheritance:**
java.lang.Object
```
public final class FileType
```

Stellt einen Dateityp dar. Bietet Methoden, um eine Liste aller von GroupDocs.Redaction unterstützten Dateitypen zu erhalten, den Dateityp anhand der Erweiterung zu erkennen usw.

*** ** * ** ***


**Learn more**

* [Supported Document Formats](../https://docs.groupdocs.com/redaction/java/supported-document-formats/)
* [Get supported file formats](../https://docs.groupdocs.com/redaction/java/get-supported-file-formats/)
* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Liefert den Namen des Dateityps, zum Beispiel "Microsoft Word Document". |
|
|  | [getExtension()](#getExtension--) | Liefert die Dateinamensuffix (einschließlich des Punktes "."), zum Beispiel ".doc". |
|
|  | [getUnknown()](#getUnknown--) | Stellt einen unbekannten Dateityp dar. |
|
|  | [getTIF()](#getTIF--) | Tagged Image File (.tif) |
|
|  | [getTIFF()](#getTIFF--) | Tagged Image File Format (.tiff) |
|
|  | [getJPG()](#getJPG--) | JPEG Image (.jpg) |
|
|  | [getJPEG()](#getJPEG--) | JPEG Image (.jpeg) |
|
|  | [getPNG()](#getPNG--) | Portable Network Graphic (.png) |
|
|  | [getGIF()](#getGIF--) | Graphical Interchange Format File (.gif) |
|
|  | [getBMP()](#getBMP--) | Bitmap Image File (.bmp) |
|
|  | [getJP2()](#getJP2--) | JPEG 2000 Core Image File (.jp2) |
|
|  | [getHTM()](#getHTM--) | Hypertext Markup Language File (.htm) |
|
|  | [getHTML()](#getHTML--) | Hypertext Markup Language File (.html) |
|
|  | [getPDF()](#getPDF--) | Portable Document Format File (.pdf) |
|
|  | [getPPT()](#getPPT--) | PowerPoint Presentation (.ppt) |
|
|  | [getPPTX()](#getPPTX--) | PowerPoint Open XML Presentation (.pptx) |
|
|  | [getODP()](#getODP--) | OpenDocument Presentation (.odp) |
|
|  | [getPOTX()](#getPOTX--) | PowerPoint Open XML Presentation Template (.potx) |
|
|  | [getPOTM()](#getPOTM--) | PowerPoint Open XML Macro-Enabled Presentation Template (.potm) |
|
|  | [getOTP()](#getOTP--) | OpenDocument Presentation Template (.otp) |
|
|  | [getXLS()](#getXLS--) | Excel-Tabelle (.xls) |
|
|  | [getXLSX()](#getXLSX--) | Microsoft Excel Open XML-Tabellendatei (.xlsx) |
|
|  | [getXLSM()](#getXLSM--) | Excel Open XML-Makroaktivierte Tabellendatei (.xlsm) |
|
|  | [getXLSB()](#getXLSB--) | Excel Binär-Tabellendatei (.xlsb) |
|
|  | [getXLTX()](#getXLTX--) | Excel Open XML-Tabellenvorlage (.xltx) |
|
|  | [getXLTM()](#getXLTM--) | Excel Open XML-Makroaktivierte Tabellenvorlage (.xltm) |
|
|  | [getXLT()](#getXLT--) | Excel-Vorlage (.xlt) |
|
|  | [getCSV()](#getCSV--) | Kommagetrennte Werte-Datei (.csv) |
|
|  | [getTSV()](#getTSV--) | Tabulatorgetrennte Werte-Datei (.tsv) |
|
|  | [getTAB()](#getTAB--) | Tabulatorgetrennte Werte-Datei (.tab) |
|
|  | [getODS()](#getODS--) | OpenDocument-Tabellendatei (.ods) |
|
|  | [getOTS()](#getOTS--) | OpenDocument-Tabellenvorlage (.ots) |
|
|  | [getNUMBERS()](#getNUMBERS--) | Apple Numbers-Tabellendatei (.numbers) |
|
|  | [getMD()](#getMD--) | Markdown-Dokumentationsdatei (.md) |
|
|  | [getDOC()](#getDOC--) | Microsoft Word-Dokument (.doc) |
|
|  | [getDOCX()](#getDOCX--) | Microsoft Word Open XML-Dokument (.docx) |
|
|  | [getDOCM()](#getDOCM--) | Word Open XML-Makroaktiviertes Dokument (.docm) |
|
|  | [getDOT()](#getDOT--) | Word-Dokumentvorlage (.dot) |
|
|  | [getDOTX()](#getDOTX--) | Word Open XML-Dokumentvorlage (.dotx) |
|
|  | [getDOTM()](#getDOTM--) | Word Open XML-Makroaktivierte Dokumentvorlage (.dotm) |
|
|  | [getRTF()](#getRTF--) | Rich Text Format-Datei (.rtf) |
|
|  | [getTXT()](#getTXT--) | Nur-Text-Datei (.txt) |
|
|  | [getODT()](#getODT--) | OpenDocument-Textdokument (.odt) |
|
|  | [getOTT()](#getOTT--) | OpenDocument-Dokumentvorlage (.ott) |
|
|  | [fromExtension(String extension)](#fromExtension-java.lang.String-) | Ordnet Dateierweiterungen dem Dateityp zu. |
|
|  | [getSupportedFileTypes()](#getSupportedFileTypes--) | Ruft unterstützte Dateitypen ab |
|
|  | [equals(FileType other)](#equals-com.groupdocs.redaction.FileType-) | Bestimmt, ob das aktuelle |
FileType
gleich dem angegebenen
FileType
Objekt.
|
|  | [equals(Object obj)](#equals-java.lang.Object-) | Bestimmt, ob das aktuelle |
FileType
ist dasselbe wie das angegebene Objekt.
|
|  | [hashCode()](#hashCode--) | Gibt den Hashcode für das aktuelle |
FileType
Objekt.
|
|  | [op_Equality(FileType left, FileType right)](#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Bestimmt, ob zwei |
FileType
Objekte sind gleich.
|
|  | [op_Inequality(FileType left, FileType right)](#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Bestimmt, ob zwei |
FileType
Objekte sind nicht gleich.
|
|  | [toString()](#toString--) | Gibt eine Zeichenkette zurück, die das aktuelle Objekt darstellt. |
|
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


Liefert den Namen des Dateityps, zum Beispiel "Microsoft Word Document".


**Returns:**
java.lang.String - Dateitypname, zum Beispiel "Microsoft Word Document".

### getExtension() {#getExtension--}
```
public final String getExtension()
```


Liefert die Dateinamensuffix (einschließlich des Punktes "."), zum Beispiel ".doc".


**Returns:**
java.lang.String - Dateinamensuffix (einschließlich des Punktes "."), zum Beispiel ".doc".

### getUnknown() {#getUnknown--}
```
public static FileType getUnknown()
```


Stellt einen unbekannten Dateityp dar.


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
### getPOTX() {#getPOTX--}
```
public static FileType getPOTX()
```


PowerPoint Open XML Presentation Template (.potx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTM() {#getPOTM--}
```
public static FileType getPOTM()
```


PowerPoint Open XML Macro-Enabled Presentation Template (.potm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTP() {#getOTP--}
```
public static FileType getOTP()
```


OpenDocument Presentation Template (.otp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLS() {#getXLS--}
```
public static FileType getXLS()
```


Excel-Tabelle (.xls)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSX() {#getXLSX--}
```
public static FileType getXLSX()
```


Microsoft Excel Open XML-Tabellendatei (.xlsx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSM() {#getXLSM--}
```
public static FileType getXLSM()
```


Excel Open XML-Makroaktivierte Tabellendatei (.xlsm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSB() {#getXLSB--}
```
public static FileType getXLSB()
```


Excel Binär-Tabellendatei (.xlsb)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTX() {#getXLTX--}
```
public static FileType getXLTX()
```


Excel Open XML-Tabellenvorlage (.xltx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTM() {#getXLTM--}
```
public static FileType getXLTM()
```


Excel Open XML-Makroaktivierte Tabellenvorlage (.xltm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLT() {#getXLT--}
```
public static FileType getXLT()
```


Excel-Vorlage (.xlt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getCSV() {#getCSV--}
```
public static FileType getCSV()
```


Kommagetrennte Werte-Datei (.csv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTSV() {#getTSV--}
```
public static FileType getTSV()
```


Tabulatorgetrennte Werte-Datei (.tsv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTAB() {#getTAB--}
```
public static FileType getTAB()
```


Tabulatorgetrennte Werte-Datei (.tab)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODS() {#getODS--}
```
public static FileType getODS()
```


OpenDocument-Tabellendatei (.ods)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTS() {#getOTS--}
```
public static FileType getOTS()
```


OpenDocument-Tabellenvorlage (.ots)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getNUMBERS() {#getNUMBERS--}
```
public static FileType getNUMBERS()
```


Apple Numbers-Tabellendatei (.numbers)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getMD() {#getMD--}
```
public static FileType getMD()
```


Markdown-Dokumentationsdatei (.md)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOC() {#getDOC--}
```
public static FileType getDOC()
```


Microsoft Word-Dokument (.doc)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCX() {#getDOCX--}
```
public static FileType getDOCX()
```


Microsoft Word Open XML-Dokument (.docx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCM() {#getDOCM--}
```
public static FileType getDOCM()
```


Word Open XML-Makroaktiviertes Dokument (.docm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOT() {#getDOT--}
```
public static FileType getDOT()
```


Word-Dokumentvorlage (.dot)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTX() {#getDOTX--}
```
public static FileType getDOTX()
```


Word Open XML-Dokumentvorlage (.dotx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTM() {#getDOTM--}
```
public static FileType getDOTM()
```


Word Open XML-Makroaktivierte Dokumentvorlage (.dotm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getRTF() {#getRTF--}
```
public static FileType getRTF()
```


Rich Text Format-Datei (.rtf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTXT() {#getTXT--}
```
public static FileType getTXT()
```


Nur-Text-Datei (.txt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODT() {#getODT--}
```
public static FileType getODT()
```


OpenDocument-Textdokument (.odt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTT() {#getOTT--}
```
public static FileType getOTT()
```


OpenDocument-Dokumentvorlage (.ott)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### fromExtension(String extension) {#fromExtension-java.lang.String-}
```
public static FileType fromExtension(String extension)
```


Ordnet Dateierweiterungen dem Dateityp zu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Erweiterung | java.lang.String | Dateierweiterung (einschließlich des Punktes "."). |
|

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - When file type is supported returns it, otherwise returns default  Unknown  file type.

### getSupportedFileTypes() {#getSupportedFileTypes--}
```
public static Iterable<FileType> getSupportedFileTypes()
```


Ruft unterstützte Dateitypen ab


**Returns:**
java.lang.Iterable<com.groupdocs.redaction.FileType> - Gibt eine Sequenz unterstützter Dateitypen zurück

### equals(FileType other) {#equals-com.groupdocs.redaction.FileType-}
```
public final boolean equals(FileType other)
```


Bestimmt, ob das aktuelle
FileType
gleich dem angegebenen
FileType
Objekt.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | other | [FileType](../../com.groupdocs.redaction/filetype) | Das Objekt, das mit dem aktuellen  FileType  Objekt verglichen wird. |
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

wenn

```
obj
```

Parameter ist  FileType  und ist dasselbe wie das aktuelle  FileType  Objekt; andernfalls,

```
false
```


### hashCode() {#hashCode--}
```
public int hashCode()
```


Gibt den Hashcode für das aktuelle
FileType
Objekt.


**Returns:**
int - Ein Hashcode für das aktuelle  FileType  Objekt.

### op_Equality(FileType left, FileType right) {#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Equality(FileType left, FileType right)
```


Bestimmt, ob zwei
FileType
Objekte sind gleich.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | left | [FileType](../../com.groupdocs.redaction/filetype) | Linkes  FileType  Objekt. |
|
|  | right | [FileType](../../com.groupdocs.redaction/filetype) | Rechtes  FileType  Objekt. |
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

wenn beide  FileType  Objekte nicht gleich sind; andernfalls,

```
false
```


### toString() {#toString--}
```
public String toString()
```


Gibt eine Zeichenkette zurück, die das aktuelle Objekt darstellt.


**Returns:**
java.lang.String - Ein String, der das aktuelle Objekt darstellt.

