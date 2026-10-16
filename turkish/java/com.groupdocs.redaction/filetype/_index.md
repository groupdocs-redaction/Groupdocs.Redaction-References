---
title: "DosyaTürü"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Bir dosya türünü temsil eder."
type: docs
weight: 11
url: /tr/java/com.groupdocs.redaction/filetype/
---
**Inheritance:**
java.lang.Object
```
public final class FileType
```

Bir dosya türünü temsil eder. GroupDocs.Redaction tarafından desteklenen tüm dosya türlerinin listesini elde etmek, dosya türünü uzantıya göre tespit etmek vb. yöntemler sağlar.

*** ** * ** ***


**Learn more**

* [Supported Document Formats](../https://docs.groupdocs.com/redaction/java/supported-document-formats/)
* [Get supported file formats](../https://docs.groupdocs.com/redaction/java/get-supported-file-formats/)
* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Dosya türü adını alır, örneğin "Microsoft Word Document". |
|
|  | [getExtension()](#getExtension--) | Dosya adı uzantısını (nokta "." dahil) alır, örneğin ".doc". |
|
|  | [getUnknown()](#getUnknown--) | Bilinmeyen dosya türünü temsil eder. |
|
|  | [getTIF()](#getTIF--) | Etiketli Görüntü Dosyası (.tif) |
|
|  | [getTIFF()](#getTIFF--) | Etiketli Görüntü Dosyası Formatı (.tiff) |
|
|  | [getJPG()](#getJPG--) | JPEG Görüntüsü (.jpg) |
|
|  | [getJPEG()](#getJPEG--) | JPEG Görüntüsü (.jpeg) |
|
|  | [getPNG()](#getPNG--) | Taşınabilir Ağ Grafiği (.png) |
|
|  | [getGIF()](#getGIF--) | Grafik Değişim Biçimi Dosyası (.gif) |
|
|  | [getBMP()](#getBMP--) | Bit eşlem Görüntü Dosyası (.bmp) |
|
|  | [getJP2()](#getJP2--) | JPEG 2000 Çekirdek Görüntü Dosyası (.jp2) |
|
|  | [getHTM()](#getHTM--) | Hipermetin İşaretleme Dili Dosyası (.htm) |
|
|  | [getHTML()](#getHTML--) | Hipermetin İşaretleme Dili Dosyası (.html) |
|
|  | [getPDF()](#getPDF--) | Taşınabilir Belge Biçimi Dosyası (.pdf) |
|
|  | [getPPT()](#getPPT--) | PowerPoint Sunumu (.ppt) |
|
|  | [getPPTX()](#getPPTX--) | PowerPoint Açık XML Sunumu (.pptx) |
|
|  | [getODP()](#getODP--) | OpenDocument Sunumu (.odp) |
|
|  | [getPOTX()](#getPOTX--) | PowerPoint Açık XML Sunum Şablonu (.potx) |
|
|  | [getPOTM()](#getPOTM--) | PowerPoint Açık XML Makro Etkin Sunum Şablonu (.potm) |
|
|  | [getOTP()](#getOTP--) | OpenDocument Sunum Şablonu (.otp) |
|
|  | [getXLS()](#getXLS--) | Excel Çalışma Sayfası (.xls) |
|
|  | [getXLSX()](#getXLSX--) | Microsoft Excel Açık XML Çalışma Sayfası (.xlsx) |
|
|  | [getXLSM()](#getXLSM--) | Excel Açık XML Makro Etkin Çalışma Sayfası (.xlsm) |
|
|  | [getXLSB()](#getXLSB--) | Excel İkili Çalışma Sayfası (.xlsb) |
|
|  | [getXLTX()](#getXLTX--) | Excel Açık XML Çalışma Sayfası Şablonu (.xltx) |
|
|  | [getXLTM()](#getXLTM--) | Excel Açık XML Makro Etkin Çalışma Sayfası Şablonu (.xltm) |
|
|  | [getXLT()](#getXLT--) | Excel Şablonu (.xlt) |
|
|  | [getCSV()](#getCSV--) | Virgülle Ayrılmış Değerler Dosyası (.csv) |
|
|  | [getTSV()](#getTSV--) | Sekme Ayrılmış Değerler Dosyası (.tsv) |
|
|  | [getTAB()](#getTAB--) | Sekme Ayrılmış Değerler Dosyası (.tab) |
|
|  | [getODS()](#getODS--) | OpenDocument Çalışma Sayfası (.ods) |
|
|  | [getOTS()](#getOTS--) | OpenDocument Çalışma Sayfası Şablonu (.ots) |
|
|  | [getNUMBERS()](#getNUMBERS--) | Apple Numbers Çalışma Sayfası (.numbers) |
|
|  | [getMD()](#getMD--) | Markdown Dokümantasyon Dosyası (.md) |
|
|  | [getDOC()](#getDOC--) | Microsoft Word Belgesi (.doc) |
|
|  | [getDOCX()](#getDOCX--) | Microsoft Word Açık XML Belgesi (.docx) |
|
|  | [getDOCM()](#getDOCM--) | Word Açık XML Makro Etkin Belgesi (.docm) |
|
|  | [getDOT()](#getDOT--) | Word Belge Şablonu (.dot) |
|
|  | [getDOTX()](#getDOTX--) | Word Açık XML Belge Şablonu (.dotx) |
|
|  | [getDOTM()](#getDOTM--) | Word Açık XML Makro Etkin Belge Şablonu (.dotm) |
|
|  | [getRTF()](#getRTF--) | Zengin Metin Biçimi Dosyası (.rtf) |
|
|  | [getTXT()](#getTXT--) | Düz Metin Dosyası (.txt) |
|
|  | [getODT()](#getODT--) | OpenDocument Metin Belgesi (.odt) |
|
|  | [getOTT()](#getOTT--) | OpenDocument Belge Şablonu (.ott) |
|
|  | [fromExtension(String extension)](#fromExtension-java.lang.String-) | Dosya uzantısını dosya türüne eşler. |
|
|  | [getSupportedFileTypes()](#getSupportedFileTypes--) | Desteklenen dosya türlerini alır |
|
|  | [equals(FileType other)](#equals-com.groupdocs.redaction.FileType-) | Geçerli olanı belirler |
DosyaTürü
belirtilen ile aynı mı
DosyaTürü
nesne.
|
|  | [equals(Object obj)](#equals-java.lang.Object-) | Geçerli olanı belirler |
DosyaTürü
belirtilen nesne ile aynı.
|
|  | [hashCode()](#hashCode--) | Geçerli olan için karma kodunu döndürür |
DosyaTürü
nesne.
|
|  | [op_Equality(FileType left, FileType right)](#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | İki ... olup olmadığını belirler |
DosyaTürü
nesneler aynı.
|
|  | [op_Inequality(FileType left, FileType right)](#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | İki ... olup olmadığını belirler |
DosyaTürü
nesneler aynı değil.
|
|  | [toString()](#toString--) | Geçerli nesneyi temsil eden bir dize döndürür. |
|
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


Dosya türü adını alır, örneğin "Microsoft Word Document".


**Returns:**
java.lang.String - Dosya türü adı, örneğin "Microsoft Word Document".

### getExtension() {#getExtension--}
```
public final String getExtension()
```


Dosya adı uzantısını (nokta "." dahil) alır, örneğin ".doc".


**Returns:**
java.lang.String - Dosya adı uzantısı (nokta "." dahil), örneğin ".doc".

### getUnknown() {#getUnknown--}
```
public static FileType getUnknown()
```


Bilinmeyen dosya türünü temsil eder.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIF() {#getTIF--}
```
public static FileType getTIF()
```


Etiketli Görüntü Dosyası (.tif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIFF() {#getTIFF--}
```
public static FileType getTIFF()
```


Etiketli Görüntü Dosyası Formatı (.tiff)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPG() {#getJPG--}
```
public static FileType getJPG()
```


JPEG Görüntüsü (.jpg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPEG() {#getJPEG--}
```
public static FileType getJPEG()
```


JPEG Görüntüsü (.jpeg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPNG() {#getPNG--}
```
public static FileType getPNG()
```


Taşınabilir Ağ Grafiği (.png)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getGIF() {#getGIF--}
```
public static FileType getGIF()
```


Grafik Değişim Biçimi Dosyası (.gif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getBMP() {#getBMP--}
```
public static FileType getBMP()
```


Bit eşlem Görüntü Dosyası (.bmp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJP2() {#getJP2--}
```
public static FileType getJP2()
```


JPEG 2000 Çekirdek Görüntü Dosyası (.jp2)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTM() {#getHTM--}
```
public static FileType getHTM()
```


Hipermetin İşaretleme Dili Dosyası (.htm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTML() {#getHTML--}
```
public static FileType getHTML()
```


Hipermetin İşaretleme Dili Dosyası (.html)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPDF() {#getPDF--}
```
public static FileType getPDF()
```


Taşınabilir Belge Biçimi Dosyası (.pdf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPT() {#getPPT--}
```
public static FileType getPPT()
```


PowerPoint Sunumu (.ppt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPTX() {#getPPTX--}
```
public static FileType getPPTX()
```


PowerPoint Açık XML Sunumu (.pptx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODP() {#getODP--}
```
public static FileType getODP()
```


OpenDocument Sunumu (.odp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTX() {#getPOTX--}
```
public static FileType getPOTX()
```


PowerPoint Açık XML Sunum Şablonu (.potx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTM() {#getPOTM--}
```
public static FileType getPOTM()
```


PowerPoint Açık XML Makro Etkin Sunum Şablonu (.potm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTP() {#getOTP--}
```
public static FileType getOTP()
```


OpenDocument Sunum Şablonu (.otp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLS() {#getXLS--}
```
public static FileType getXLS()
```


Excel Çalışma Sayfası (.xls)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSX() {#getXLSX--}
```
public static FileType getXLSX()
```


Microsoft Excel Açık XML Çalışma Sayfası (.xlsx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSM() {#getXLSM--}
```
public static FileType getXLSM()
```


Excel Açık XML Makro Etkin Çalışma Sayfası (.xlsm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSB() {#getXLSB--}
```
public static FileType getXLSB()
```


Excel İkili Çalışma Sayfası (.xlsb)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTX() {#getXLTX--}
```
public static FileType getXLTX()
```


Excel Açık XML Çalışma Sayfası Şablonu (.xltx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTM() {#getXLTM--}
```
public static FileType getXLTM()
```


Excel Açık XML Makro Etkin Çalışma Sayfası Şablonu (.xltm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLT() {#getXLT--}
```
public static FileType getXLT()
```


Excel Şablonu (.xlt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getCSV() {#getCSV--}
```
public static FileType getCSV()
```


Virgülle Ayrılmış Değerler Dosyası (.csv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTSV() {#getTSV--}
```
public static FileType getTSV()
```


Sekme Ayrılmış Değerler Dosyası (.tsv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTAB() {#getTAB--}
```
public static FileType getTAB()
```


Sekme Ayrılmış Değerler Dosyası (.tab)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODS() {#getODS--}
```
public static FileType getODS()
```


OpenDocument Çalışma Sayfası (.ods)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTS() {#getOTS--}
```
public static FileType getOTS()
```


OpenDocument Çalışma Sayfası Şablonu (.ots)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getNUMBERS() {#getNUMBERS--}
```
public static FileType getNUMBERS()
```


Apple Numbers Çalışma Sayfası (.numbers)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getMD() {#getMD--}
```
public static FileType getMD()
```


Markdown Dokümantasyon Dosyası (.md)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOC() {#getDOC--}
```
public static FileType getDOC()
```


Microsoft Word Belgesi (.doc)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCX() {#getDOCX--}
```
public static FileType getDOCX()
```


Microsoft Word Açık XML Belgesi (.docx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCM() {#getDOCM--}
```
public static FileType getDOCM()
```


Word Açık XML Makro Etkin Belgesi (.docm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOT() {#getDOT--}
```
public static FileType getDOT()
```


Word Belge Şablonu (.dot)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTX() {#getDOTX--}
```
public static FileType getDOTX()
```


Word Açık XML Belge Şablonu (.dotx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTM() {#getDOTM--}
```
public static FileType getDOTM()
```


Word Açık XML Makro Etkin Belge Şablonu (.dotm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getRTF() {#getRTF--}
```
public static FileType getRTF()
```


Zengin Metin Biçimi Dosyası (.rtf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTXT() {#getTXT--}
```
public static FileType getTXT()
```


Düz Metin Dosyası (.txt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODT() {#getODT--}
```
public static FileType getODT()
```


OpenDocument Metin Belgesi (.odt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTT() {#getOTT--}
```
public static FileType getOTT()
```


OpenDocument Belge Şablonu (.ott)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### fromExtension(String extension) {#fromExtension-java.lang.String-}
```
public static FileType fromExtension(String extension)
```


Dosya uzantısını dosya türüne eşler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | uzantı | java.lang.String | Dosya uzantısı (nokta "." dahil). |
|

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - When file type is supported returns it, otherwise returns default  Unknown  file type.

### getSupportedFileTypes() {#getSupportedFileTypes--}
```
public static Iterable<FileType> getSupportedFileTypes()
```


Desteklenen dosya türlerini alır


**Returns:**
java.lang.Iterable<com.groupdocs.redaction.FileType> - Desteklenen dosya türlerinin dizisini döndürür

### equals(FileType other) {#equals-com.groupdocs.redaction.FileType-}
```
public final boolean equals(FileType other)
```


Geçerli olanı belirler
DosyaTürü
belirtilen ile aynı mı
DosyaTürü
nesne.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | other | [FileType](../../com.groupdocs.redaction/filetype) | Geçerli  FileType  nesnesiyle karşılaştırılacak nesne. |
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

eğer

```
obj
```

parametre  FileType  olup geçerli  FileType  nesnesiyle aynı ise; aksi takdirde,

```
false
```


### hashCode() {#hashCode--}
```
public int hashCode()
```


Geçerli olan için karma kodunu döndürür
DosyaTürü
nesne.


**Returns:**
int - Geçerli  FileType  nesnesi için bir karma kodu.

### op_Equality(FileType left, FileType right) {#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Equality(FileType left, FileType right)
```


İki ... olup olmadığını belirler
DosyaTürü
nesneler aynı.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | left | [FileType](../../com.groupdocs.redaction/filetype) | Sol  FileType  nesnesi. |
|
|  | right | [FileType](../../com.groupdocs.redaction/filetype) | Sağ  FileType  nesnesi. |
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

eğer her iki  FileType  nesnesi aynı değilse; aksi takdirde,

```
false
```


### toString() {#toString--}
```
public String toString()
```


Geçerli nesneyi temsil eden bir dize döndürür.


**Returns:**
java.lang.String - Geçerli nesneyi temsil eden bir dize.

