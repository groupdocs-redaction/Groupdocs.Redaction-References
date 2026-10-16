---
title: "FileType"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa un tipo de archivo."
type: docs
weight: 11
url: /es/java/com.groupdocs.redaction/filetype/
---
**Inheritance:**
java.lang.Object
```
public final class FileType
```

Representa un tipo de archivo. Proporciona métodos para obtener una lista de todos los tipos de archivo compatibles con GroupDocs.Redaction, detectar el tipo de archivo por extensión, etc.

*** ** * ** ***


**Learn more**

* [Supported Document Formats](../https://docs.groupdocs.com/redaction/java/supported-document-formats/)
* [Get supported file formats](../https://docs.groupdocs.com/redaction/java/get-supported-file-formats/)
* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Métodos

| Método | Descripción |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Obtiene el nombre del tipo de archivo, por ejemplo "Microsoft Word Document". |
|
|  | [getExtension()](#getExtension--) | Obtiene el sufijo del nombre de archivo (incluyendo el punto "."), por ejemplo ".doc". |
|
|  | [getUnknown()](#getUnknown--) | Representa un tipo de archivo desconocido. |
|
|  | [getTIF()](#getTIF--) | Archivo de Imagen Etiquetado (.tif) |
|
|  | [getTIFF()](#getTIFF--) | Formato de Archivo de Imagen Etiquetado (.tiff) |
|
|  | [getJPG()](#getJPG--) | Imagen JPEG (.jpg) |
|
|  | [getJPEG()](#getJPEG--) | Imagen JPEG (.jpeg) |
|
|  | [getPNG()](#getPNG--) | Gráfico de Red Portátil (.png) |
|
|  | [getGIF()](#getGIF--) | Archivo de Formato de Intercambio Gráfico (.gif) |
|
|  | [getBMP()](#getBMP--) | Archivo de Imagen Bitmap (.bmp) |
|
|  | [getJP2()](#getJP2--) | Archivo de Imagen Central JPEG 2000 (.jp2) |
|
|  | [getHTM()](#getHTM--) | Archivo de Lenguaje de Marcado de Hipertexto (.htm) |
|
|  | [getHTML()](#getHTML--) | Archivo de Lenguaje de Marcado de Hipertexto (.html) |
|
|  | [getPDF()](#getPDF--) | Archivo de Formato de Documento Portátil (.pdf) |
|
|  | [getPPT()](#getPPT--) | Presentación de PowerPoint (.ppt) |
|
|  | [getPPTX()](#getPPTX--) | Presentación Open XML de PowerPoint (.pptx) |
|
|  | [getODP()](#getODP--) | Presentación OpenDocument (.odp) |
|
|  | [getPOTX()](#getPOTX--) | Plantilla de Presentación Open XML de PowerPoint (.potx) |
|
|  | [getPOTM()](#getPOTM--) | Plantilla de Presentación Open XML con Macros de PowerPoint (.potm) |
|
|  | [getOTP()](#getOTP--) | Plantilla de Presentación OpenDocument (.otp) |
|
|  | [getXLS()](#getXLS--) | Hoja de cálculo Excel (.xls) |
|
|  | [getXLSX()](#getXLSX--) | Hoja de cálculo Open XML de Microsoft Excel (.xlsx) |
|
|  | [getXLSM()](#getXLSM--) | Hoja de cálculo Open XML con Macros de Excel (.xlsm) |
|
|  | [getXLSB()](#getXLSB--) | Hoja de cálculo binaria de Excel (.xlsb) |
|
|  | [getXLTX()](#getXLTX--) | Plantilla de Hoja de cálculo Open XML de Excel (.xltx) |
|
|  | [getXLTM()](#getXLTM--) | Plantilla de Hoja de cálculo Open XML con Macros de Excel (.xltm) |
|
|  | [getXLT()](#getXLT--) | Plantilla de Excel (.xlt) |
|
|  | [getCSV()](#getCSV--) | Archivo de Valores Separados por Comas (.csv) |
|
|  | [getTSV()](#getTSV--) | Archivo de Valores Separados por Tabulaciones (.tsv) |
|
|  | [getTAB()](#getTAB--) | Archivo de Valores Separados por Tabulaciones (.tab) |
|
|  | [getODS()](#getODS--) | Hoja de cálculo OpenDocument (.ods) |
|
|  | [getOTS()](#getOTS--) | Plantilla de hoja de cálculo OpenDocument (.ots) |
|
|  | [getNUMBERS()](#getNUMBERS--) | Hoja de cálculo Apple Numbers (.numbers) |
|
|  | [getMD()](#getMD--) | Archivo de documentación Markdown (.md) |
|
|  | [getDOC()](#getDOC--) | Documento Microsoft Word (.doc) |
|
|  | [getDOCX()](#getDOCX--) | Documento Open XML de Microsoft Word (.docx) |
|
|  | [getDOCM()](#getDOCM--) | Documento con macros Open XML de Word (.docm) |
|
|  | [getDOT()](#getDOT--) | Plantilla de documento Word (.dot) |
|
|  | [getDOTX()](#getDOTX--) | Plantilla de documento Open XML de Word (.dotx) |
|
|  | [getDOTM()](#getDOTM--) | Plantilla de documento con macros Open XML de Word (.dotm) |
|
|  | [getRTF()](#getRTF--) | Archivo Rich Text Format (.rtf) |
|
|  | [getTXT()](#getTXT--) | Archivo de texto plano (.txt) |
|
|  | [getODT()](#getODT--) | Documento de texto OpenDocument (.odt) |
|
|  | [getOTT()](#getOTT--) | Plantilla de documento OpenDocument (.ott) |
|
|  | [fromExtension(String extension)](#fromExtension-java.lang.String-) | Mapea la extensión de archivo al tipo de archivo. |
|
|  | [getSupportedFileTypes()](#getSupportedFileTypes--) | Recupera los tipos de archivo compatibles |
|
|  | [equals(FileType other)](#equals-com.groupdocs.redaction.FileType-) | Determina si el actual |
FileType
es el mismo que el especificado
FileType
objeto.
|
|  | [equals(Object obj)](#equals-java.lang.Object-) | Determina si el actual |
FileType
es el mismo que el objeto especificado.
|
|  | [hashCode()](#hashCode--) | Devuelve el código hash del actual |
FileType
objeto.
|
|  | [op_Equality(FileType left, FileType right)](#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Determina si dos |
FileType
objetos son iguales.
|
|  | [op_Inequality(FileType left, FileType right)](#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Determina si dos |
FileType
objetos no son iguales.
|
|  | [toString()](#toString--) | Devuelve una cadena que representa el objeto actual. |
|
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


Obtiene el nombre del tipo de archivo, por ejemplo "Microsoft Word Document".


**Returns:**
java.lang.String - Nombre del tipo de archivo, por ejemplo "Microsoft Word Document".

### getExtension() {#getExtension--}
```
public final String getExtension()
```


Obtiene el sufijo del nombre de archivo (incluyendo el punto "."), por ejemplo ".doc".


**Returns:**
java.lang.String - Sufijo del nombre de archivo (incluyendo el punto "."), por ejemplo ".doc".

### getUnknown() {#getUnknown--}
```
public static FileType getUnknown()
```


Representa un tipo de archivo desconocido.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIF() {#getTIF--}
```
public static FileType getTIF()
```


Archivo de Imagen Etiquetado (.tif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIFF() {#getTIFF--}
```
public static FileType getTIFF()
```


Formato de Archivo de Imagen Etiquetado (.tiff)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPG() {#getJPG--}
```
public static FileType getJPG()
```


Imagen JPEG (.jpg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPEG() {#getJPEG--}
```
public static FileType getJPEG()
```


Imagen JPEG (.jpeg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPNG() {#getPNG--}
```
public static FileType getPNG()
```


Gráfico de Red Portátil (.png)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getGIF() {#getGIF--}
```
public static FileType getGIF()
```


Archivo de Formato de Intercambio Gráfico (.gif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getBMP() {#getBMP--}
```
public static FileType getBMP()
```


Archivo de Imagen Bitmap (.bmp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJP2() {#getJP2--}
```
public static FileType getJP2()
```


Archivo de Imagen Central JPEG 2000 (.jp2)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTM() {#getHTM--}
```
public static FileType getHTM()
```


Archivo de Lenguaje de Marcado de Hipertexto (.htm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTML() {#getHTML--}
```
public static FileType getHTML()
```


Archivo de Lenguaje de Marcado de Hipertexto (.html)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPDF() {#getPDF--}
```
public static FileType getPDF()
```


Archivo de Formato de Documento Portátil (.pdf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPT() {#getPPT--}
```
public static FileType getPPT()
```


Presentación de PowerPoint (.ppt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPTX() {#getPPTX--}
```
public static FileType getPPTX()
```


Presentación Open XML de PowerPoint (.pptx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODP() {#getODP--}
```
public static FileType getODP()
```


Presentación OpenDocument (.odp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTX() {#getPOTX--}
```
public static FileType getPOTX()
```


Plantilla de Presentación Open XML de PowerPoint (.potx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTM() {#getPOTM--}
```
public static FileType getPOTM()
```


Plantilla de Presentación Open XML con Macros de PowerPoint (.potm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTP() {#getOTP--}
```
public static FileType getOTP()
```


Plantilla de Presentación OpenDocument (.otp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLS() {#getXLS--}
```
public static FileType getXLS()
```


Hoja de cálculo Excel (.xls)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSX() {#getXLSX--}
```
public static FileType getXLSX()
```


Hoja de cálculo Open XML de Microsoft Excel (.xlsx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSM() {#getXLSM--}
```
public static FileType getXLSM()
```


Hoja de cálculo Open XML con Macros de Excel (.xlsm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSB() {#getXLSB--}
```
public static FileType getXLSB()
```


Hoja de cálculo binaria de Excel (.xlsb)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTX() {#getXLTX--}
```
public static FileType getXLTX()
```


Plantilla de Hoja de cálculo Open XML de Excel (.xltx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTM() {#getXLTM--}
```
public static FileType getXLTM()
```


Plantilla de Hoja de cálculo Open XML con Macros de Excel (.xltm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLT() {#getXLT--}
```
public static FileType getXLT()
```


Plantilla de Excel (.xlt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getCSV() {#getCSV--}
```
public static FileType getCSV()
```


Archivo de Valores Separados por Comas (.csv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTSV() {#getTSV--}
```
public static FileType getTSV()
```


Archivo de Valores Separados por Tabulaciones (.tsv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTAB() {#getTAB--}
```
public static FileType getTAB()
```


Archivo de Valores Separados por Tabulaciones (.tab)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODS() {#getODS--}
```
public static FileType getODS()
```


Hoja de cálculo OpenDocument (.ods)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTS() {#getOTS--}
```
public static FileType getOTS()
```


Plantilla de hoja de cálculo OpenDocument (.ots)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getNUMBERS() {#getNUMBERS--}
```
public static FileType getNUMBERS()
```


Hoja de cálculo Apple Numbers (.numbers)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getMD() {#getMD--}
```
public static FileType getMD()
```


Archivo de documentación Markdown (.md)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOC() {#getDOC--}
```
public static FileType getDOC()
```


Documento Microsoft Word (.doc)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCX() {#getDOCX--}
```
public static FileType getDOCX()
```


Documento Open XML de Microsoft Word (.docx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCM() {#getDOCM--}
```
public static FileType getDOCM()
```


Documento con macros Open XML de Word (.docm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOT() {#getDOT--}
```
public static FileType getDOT()
```


Plantilla de documento Word (.dot)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTX() {#getDOTX--}
```
public static FileType getDOTX()
```


Plantilla de documento Open XML de Word (.dotx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTM() {#getDOTM--}
```
public static FileType getDOTM()
```


Plantilla de documento con macros Open XML de Word (.dotm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getRTF() {#getRTF--}
```
public static FileType getRTF()
```


Archivo Rich Text Format (.rtf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTXT() {#getTXT--}
```
public static FileType getTXT()
```


Archivo de texto plano (.txt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODT() {#getODT--}
```
public static FileType getODT()
```


Documento de texto OpenDocument (.odt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTT() {#getOTT--}
```
public static FileType getOTT()
```


Plantilla de documento OpenDocument (.ott)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### fromExtension(String extension) {#fromExtension-java.lang.String-}
```
public static FileType fromExtension(String extension)
```


Mapea la extensión de archivo al tipo de archivo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | extensión | java.lang.String | Extensión de archivo (incluyendo el punto "."). |
|

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - When file type is supported returns it, otherwise returns default  Unknown  file type.

### getSupportedFileTypes() {#getSupportedFileTypes--}
```
public static Iterable<FileType> getSupportedFileTypes()
```


Recupera los tipos de archivo compatibles


**Returns:**
java.lang.Iterable<com.groupdocs.redaction.FileType> - Devuelve la secuencia de tipos de archivo compatibles

### equals(FileType other) {#equals-com.groupdocs.redaction.FileType-}
```
public final boolean equals(FileType other)
```


Determina si el actual
FileType
es el mismo que el especificado
FileType
objeto.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | other | [FileType](../../com.groupdocs.redaction/filetype) | El objeto para comparar con el objeto  FileType  actual. |
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

si

```
obj
```

el parámetro es  FileType  y es el mismo que el objeto  FileType  actual; de lo contrario,

```
false
```


### hashCode() {#hashCode--}
```
public int hashCode()
```


Devuelve el código hash del actual
FileType
objeto.


**Returns:**
int - Un código hash para el objeto  FileType  actual.

### op_Equality(FileType left, FileType right) {#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Equality(FileType left, FileType right)
```


Determina si dos
FileType
objetos son iguales.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | left | [FileType](../../com.groupdocs.redaction/filetype) | Objeto  FileType  izquierdo. |
|
|  | right | [FileType](../../com.groupdocs.redaction/filetype) | Objeto  FileType  derecho. |
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

si ambos objetos  FileType  no son iguales; de lo contrario,

```
false
```


### toString() {#toString--}
```
public String toString()
```


Devuelve una cadena que representa el objeto actual.


**Returns:**
java.lang.String - Una cadena que representa el objeto actual.

