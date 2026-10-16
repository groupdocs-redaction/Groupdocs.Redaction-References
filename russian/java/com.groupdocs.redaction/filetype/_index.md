---
title: "FileType"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет тип файла."
type: docs
weight: 11
url: /ru/java/com.groupdocs.redaction/filetype/
---
**Inheritance:**
java.lang.Object
```
public final class FileType
```

Представляет тип файла. Предоставляет методы для получения списка всех типов файлов, поддерживаемых GroupDocs.Redaction, определения типа файла по расширению и т.д.

*** ** * ** ***


**Learn more**

* [Supported Document Formats](../https://docs.groupdocs.com/redaction/java/supported-document-formats/)
* [Get supported file formats](../https://docs.groupdocs.com/redaction/java/get-supported-file-formats/)
* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Методы

| Метод | Описание |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Получает название типа файла, например "Microsoft Word Document". |
|
|  | [getExtension()](#getExtension--) | Получает суффикс имени файла (включая точку "."), например ".doc". |
|
|  | [getUnknown()](#getUnknown--) | Представляет неизвестный тип файла. |
|
|  | [getTIF()](#getTIF--) | Tagged Image File (.tif) |
|
|  | [getTIFF()](#getTIFF--) | Tagged Image File Format (.tiff) |
|
|  | [getJPG()](#getJPG--) | Изображение JPEG (.jpg) |
|
|  | [getJPEG()](#getJPEG--) | Изображение JPEG (.jpeg) |
|
|  | [getPNG()](#getPNG--) | Портативный сетевой графический (.png) |
|
|  | [getGIF()](#getGIF--) | Файл графического формата обмена (.gif) |
|
|  | [getBMP()](#getBMP--) | Файл растрового изображения (.bmp) |
|
|  | [getJP2()](#getJP2--) | Файл основного изображения JPEG 2000 (.jp2) |
|
|  | [getHTM()](#getHTM--) | Файл гипертекстовой разметки (.htm) |
|
|  | [getHTML()](#getHTML--) | Файл гипертекстовой разметки (.html) |
|
|  | [getPDF()](#getPDF--) | Файл формата Portable Document (.pdf) |
|
|  | [getPPT()](#getPPT--) | Презентация PowerPoint (.ppt) |
|
|  | [getPPTX()](#getPPTX--) | Презентация PowerPoint Open XML (.pptx) |
|
|  | [getODP()](#getODP--) | Презентация OpenDocument (.odp) |
|
|  | [getPOTX()](#getPOTX--) | Шаблон презентации PowerPoint Open XML (.potx) |
|
|  | [getPOTM()](#getPOTM--) | Шаблон презентации PowerPoint Open XML с поддержкой макросов (.potm) |
|
|  | [getOTP()](#getOTP--) | Шаблон презентации OpenDocument (.otp) |
|
|  | [getXLS()](#getXLS--) | Электронная таблица Excel (.xls) |
|
|  | [getXLSX()](#getXLSX--) | Электронная таблица Microsoft Excel Open XML (.xlsx) |
|
|  | [getXLSM()](#getXLSM--) | Электронная таблица Excel Open XML с поддержкой макросов (.xlsm) |
|
|  | [getXLSB()](#getXLSB--) | Бинарная электронная таблица Excel (.xlsb) |
|
|  | [getXLTX()](#getXLTX--) | Шаблон электронной таблицы Excel Open XML (.xltx) |
|
|  | [getXLTM()](#getXLTM--) | Шаблон электронной таблицы Excel Open XML с поддержкой макросов (.xltm) |
|
|  | [getXLT()](#getXLT--) | Шаблон электронной таблицы Excel (.xlt) |
|
|  | [getCSV()](#getCSV--) | Файл значений, разделённых запятыми (.csv) |
|
|  | [getTSV()](#getTSV--) | Файл значений, разделённых табуляцией (.tsv) |
|
|  | [getTAB()](#getTAB--) | Файл значений, разделённых табуляцией (.tab) |
|
|  | [getODS()](#getODS--) | Электронная таблица OpenDocument (.ods) |
|
|  | [getOTS()](#getOTS--) | Шаблон электронной таблицы OpenDocument (.ots) |
|
|  | [getNUMBERS()](#getNUMBERS--) | Электронная таблица Apple Numbers (.numbers) |
|
|  | [getMD()](#getMD--) | Файл документации Markdown (.md) |
|
|  | [getDOC()](#getDOC--) | Документ Microsoft Word (.doc) |
|
|  | [getDOCX()](#getDOCX--) | Документ Microsoft Word Open XML (.docx) |
|
|  | [getDOCM()](#getDOCM--) | Документ Microsoft Word Open XML с поддержкой макросов (.docm) |
|
|  | [getDOT()](#getDOT--) | Шаблон документа Word (.dot) |
|
|  | [getDOTX()](#getDOTX--) | Шаблон документа Word Open XML (.dotx) |
|
|  | [getDOTM()](#getDOTM--) | Шаблон документа Word Open XML с поддержкой макросов (.dotm) |
|
|  | [getRTF()](#getRTF--) | Файл Rich Text Format (.rtf) |
|
|  | [getTXT()](#getTXT--) | Текстовый файл (.txt) |
|
|  | [getODT()](#getODT--) | Документ текста OpenDocument (.odt) |
|
|  | [getOTT()](#getOTT--) | Шаблон документа OpenDocument (.ott) |
|
|  | [fromExtension(String extension)](#fromExtension-java.lang.String-) | Сопоставляет расширение файла с типом файла. |
|
|  | [getSupportedFileTypes()](#getSupportedFileTypes--) | Получает поддерживаемые типы файлов |
|
|  | [equals(FileType other)](#equals-com.groupdocs.redaction.FileType-) | Определяет, является ли текущий |
FileType
тем же, что указано
FileType
объект.
|
|  | [equals(Object obj)](#equals-java.lang.Object-) | Определяет, является ли текущий |
FileType
является тем же объектом, что указано.
|
|  | [hashCode()](#hashCode--) | Возвращает код хеша для текущего |
FileType
объект.
|
|  | [op_Equality(FileType left, FileType right)](#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Определяет, являются ли два |
FileType
объекта одинаковыми.
|
|  | [op_Inequality(FileType left, FileType right)](#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Определяет, являются ли два |
FileType
объекты не одинаковы.
|
|  | [toString()](#toString--) | Возвращает строку, представляющую текущий объект. |
|
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


Получает название типа файла, например "Microsoft Word Document".


**Returns:**
java.lang.String - имя типа файла, например "Microsoft Word Document".

### getExtension() {#getExtension--}
```
public final String getExtension()
```


Получает суффикс имени файла (включая точку "."), например ".doc".


**Returns:**
java.lang.String - суффикс имени файла (включая точку "."), например ".doc".

### getUnknown() {#getUnknown--}
```
public static FileType getUnknown()
```


Представляет неизвестный тип файла.


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


Изображение JPEG (.jpg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPEG() {#getJPEG--}
```
public static FileType getJPEG()
```


Изображение JPEG (.jpeg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPNG() {#getPNG--}
```
public static FileType getPNG()
```


Портативный сетевой графический (.png)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getGIF() {#getGIF--}
```
public static FileType getGIF()
```


Файл графического формата обмена (.gif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getBMP() {#getBMP--}
```
public static FileType getBMP()
```


Файл растрового изображения (.bmp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJP2() {#getJP2--}
```
public static FileType getJP2()
```


Файл основного изображения JPEG 2000 (.jp2)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTM() {#getHTM--}
```
public static FileType getHTM()
```


Файл гипертекстовой разметки (.htm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTML() {#getHTML--}
```
public static FileType getHTML()
```


Файл гипертекстовой разметки (.html)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPDF() {#getPDF--}
```
public static FileType getPDF()
```


Файл формата Portable Document (.pdf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPT() {#getPPT--}
```
public static FileType getPPT()
```


Презентация PowerPoint (.ppt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPTX() {#getPPTX--}
```
public static FileType getPPTX()
```


Презентация PowerPoint Open XML (.pptx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODP() {#getODP--}
```
public static FileType getODP()
```


Презентация OpenDocument (.odp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTX() {#getPOTX--}
```
public static FileType getPOTX()
```


Шаблон презентации PowerPoint Open XML (.potx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTM() {#getPOTM--}
```
public static FileType getPOTM()
```


Шаблон презентации PowerPoint Open XML с поддержкой макросов (.potm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTP() {#getOTP--}
```
public static FileType getOTP()
```


Шаблон презентации OpenDocument (.otp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLS() {#getXLS--}
```
public static FileType getXLS()
```


Электронная таблица Excel (.xls)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSX() {#getXLSX--}
```
public static FileType getXLSX()
```


Электронная таблица Microsoft Excel Open XML (.xlsx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSM() {#getXLSM--}
```
public static FileType getXLSM()
```


Электронная таблица Excel Open XML с поддержкой макросов (.xlsm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSB() {#getXLSB--}
```
public static FileType getXLSB()
```


Бинарная электронная таблица Excel (.xlsb)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTX() {#getXLTX--}
```
public static FileType getXLTX()
```


Шаблон электронной таблицы Excel Open XML (.xltx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTM() {#getXLTM--}
```
public static FileType getXLTM()
```


Шаблон электронной таблицы Excel Open XML с поддержкой макросов (.xltm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLT() {#getXLT--}
```
public static FileType getXLT()
```


Шаблон электронной таблицы Excel (.xlt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getCSV() {#getCSV--}
```
public static FileType getCSV()
```


Файл значений, разделённых запятыми (.csv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTSV() {#getTSV--}
```
public static FileType getTSV()
```


Файл значений, разделённых табуляцией (.tsv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTAB() {#getTAB--}
```
public static FileType getTAB()
```


Файл значений, разделённых табуляцией (.tab)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODS() {#getODS--}
```
public static FileType getODS()
```


Электронная таблица OpenDocument (.ods)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTS() {#getOTS--}
```
public static FileType getOTS()
```


Шаблон электронной таблицы OpenDocument (.ots)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getNUMBERS() {#getNUMBERS--}
```
public static FileType getNUMBERS()
```


Электронная таблица Apple Numbers (.numbers)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getMD() {#getMD--}
```
public static FileType getMD()
```


Файл документации Markdown (.md)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOC() {#getDOC--}
```
public static FileType getDOC()
```


Документ Microsoft Word (.doc)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCX() {#getDOCX--}
```
public static FileType getDOCX()
```


Документ Microsoft Word Open XML (.docx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCM() {#getDOCM--}
```
public static FileType getDOCM()
```


Документ Microsoft Word Open XML с поддержкой макросов (.docm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOT() {#getDOT--}
```
public static FileType getDOT()
```


Шаблон документа Word (.dot)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTX() {#getDOTX--}
```
public static FileType getDOTX()
```


Шаблон документа Word Open XML (.dotx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTM() {#getDOTM--}
```
public static FileType getDOTM()
```


Шаблон документа Word Open XML с поддержкой макросов (.dotm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getRTF() {#getRTF--}
```
public static FileType getRTF()
```


Файл Rich Text Format (.rtf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTXT() {#getTXT--}
```
public static FileType getTXT()
```


Текстовый файл (.txt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODT() {#getODT--}
```
public static FileType getODT()
```


Документ текста OpenDocument (.odt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTT() {#getOTT--}
```
public static FileType getOTT()
```


Шаблон документа OpenDocument (.ott)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### fromExtension(String extension) {#fromExtension-java.lang.String-}
```
public static FileType fromExtension(String extension)
```


Сопоставляет расширение файла с типом файла.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | расширение | java.lang.String | Расширение файла (включая точку "."). |
|

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - When file type is supported returns it, otherwise returns default  Unknown  file type.

### getSupportedFileTypes() {#getSupportedFileTypes--}
```
public static Iterable<FileType> getSupportedFileTypes()
```


Получает поддерживаемые типы файлов


**Returns:**
java.lang.Iterable<com.groupdocs.redaction.FileType> - Возвращает последовательность поддерживаемых типов файлов

### equals(FileType other) {#equals-com.groupdocs.redaction.FileType-}
```
public final boolean equals(FileType other)
```


Определяет, является ли текущий
FileType
тем же, что указано
FileType
объект.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | other | [FileType](../../com.groupdocs.redaction/filetype) | Объект для сравнения с текущим  FileType  объектом. |
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

если

```
obj
```

параметр является  FileType  и совпадает с текущим  FileType  объектом; иначе,

```
false
```


### hashCode() {#hashCode--}
```
public int hashCode()
```


Возвращает код хеша для текущего
FileType
объект.


**Returns:**
int - Хеш-код для текущего  FileType  объекта.

### op_Equality(FileType left, FileType right) {#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Equality(FileType left, FileType right)
```


Определяет, являются ли два
FileType
объекта одинаковыми.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | left | [FileType](../../com.groupdocs.redaction/filetype) | Левый  FileType  объект. |
|
|  | right | [FileType](../../com.groupdocs.redaction/filetype) | Правый  FileType  объект. |
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

если оба  FileType  объекта не одинаковы; иначе,

```
false
```


### toString() {#toString--}
```
public String toString()
```


Возвращает строку, представляющую текущий объект.


**Returns:**
java.lang.String - Строка, представляющая текущий объект.

