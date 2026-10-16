---
title: "FileType"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta un tipo di file."
type: docs
weight: 11
url: /it/java/com.groupdocs.redaction/filetype/
---
**Inheritance:**
java.lang.Object
```
public final class FileType
```

Rappresenta un tipo di file. Fornisce metodi per ottenere un elenco di tutti i tipi di file supportati da GroupDocs.Redaction, rilevare il tipo di file per estensione, ecc.

*** ** * ** ***


**Learn more**

* [Supported Document Formats](../https://docs.groupdocs.com/redaction/java/supported-document-formats/)
* [Get supported file formats](../https://docs.groupdocs.com/redaction/java/get-supported-file-formats/)
* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Restituisce il nome del tipo di file, ad esempio "Microsoft Word Document". |
|
|  | [getExtension()](#getExtension--) | Restituisce il suffisso del nome file (incluso il punto "."), ad esempio ".doc". |
|
|  | [getUnknown()](#getUnknown--) | Rappresenta un tipo di file sconosciuto. |
|
|  | [getTIF()](#getTIF--) | Tagged Image File (.tif) |
|
|  | [getTIFF()](#getTIFF--) | Tagged Image File Format (.tiff) |
|
|  | [getJPG()](#getJPG--) | JPEG Immagine (.jpg) |
|
|  | [getJPEG()](#getJPEG--) | JPEG Immagine (.jpeg) |
|
|  | [getPNG()](#getPNG--) | Grafica di Rete Portabile (.png) |
|
|  | [getGIF()](#getGIF--) | File di Formato di Interscambio Grafico (.gif) |
|
|  | [getBMP()](#getBMP--) | File di Immagine Bitmap (.bmp) |
|
|  | [getJP2()](#getJP2--) | File di Immagine Core JPEG 2000 (.jp2) |
|
|  | [getHTM()](#getHTM--) | File di Linguaggio di Marcatura Hypertext (.htm) |
|
|  | [getHTML()](#getHTML--) | File di Linguaggio di Marcatura Hypertext (.html) |
|
|  | [getPDF()](#getPDF--) | File di Formato di Documento Portabile (.pdf) |
|
|  | [getPPT()](#getPPT--) | Presentazione PowerPoint (.ppt) |
|
|  | [getPPTX()](#getPPTX--) | Presentazione PowerPoint Open XML (.pptx) |
|
|  | [getODP()](#getODP--) | Presentazione OpenDocument (.odp) |
|
|  | [getPOTX()](#getPOTX--) | Modello di Presentazione PowerPoint Open XML (.potx) |
|
|  | [getPOTM()](#getPOTM--) | Modello di Presentazione PowerPoint Open XML con Macro (.potm) |
|
|  | [getOTP()](#getOTP--) | Modello di Presentazione OpenDocument (.otp) |
|
|  | [getXLS()](#getXLS--) | Foglio di Calcolo Excel (.xls) |
|
|  | [getXLSX()](#getXLSX--) | Foglio di Calcolo Microsoft Excel Open XML (.xlsx) |
|
|  | [getXLSM()](#getXLSM--) | Foglio di Calcolo Excel Open XML con Macro (.xlsm) |
|
|  | [getXLSB()](#getXLSB--) | Foglio di Calcolo Binario Excel (.xlsb) |
|
|  | [getXLTX()](#getXLTX--) | Modello di Foglio di Calcolo Excel Open XML (.xltx) |
|
|  | [getXLTM()](#getXLTM--) | Modello di Foglio di Calcolo Excel Open XML con Macro (.xltm) |
|
|  | [getXLT()](#getXLT--) | Modello di Excel (.xlt) |
|
|  | [getCSV()](#getCSV--) | File di Valori Separati da Virgola (.csv) |
|
|  | [getTSV()](#getTSV--) | File di Valori Separati da Tabulazione (.tsv) |
|
|  | [getTAB()](#getTAB--) | File di Valori Separati da Tabulazione (.tab) |
|
|  | [getODS()](#getODS--) | Foglio di calcolo OpenDocument (.ods) |
|
|  | [getOTS()](#getOTS--) | Modello di foglio di calcolo OpenDocument (.ots) |
|
|  | [getNUMBERS()](#getNUMBERS--) | Foglio di calcolo Apple Numbers (.numbers) |
|
|  | [getMD()](#getMD--) | File di documentazione Markdown (.md) |
|
|  | [getDOC()](#getDOC--) | Documento Microsoft Word (.doc) |
|
|  | [getDOCX()](#getDOCX--) | Documento Open XML Microsoft Word (.docx) |
|
|  | [getDOCM()](#getDOCM--) | Documento macro abilitato Open XML Word (.docm) |
|
|  | [getDOT()](#getDOT--) | Modello di documento Word (.dot) |
|
|  | [getDOTX()](#getDOTX--) | Modello di documento Open XML Word (.dotx) |
|
|  | [getDOTM()](#getDOTM--) | Modello di documento macro abilitato Open XML Word (.dotm) |
|
|  | [getRTF()](#getRTF--) | File Rich Text Format (.rtf) |
|
|  | [getTXT()](#getTXT--) | File di testo semplice (.txt) |
|
|  | [getODT()](#getODT--) | Documento di testo OpenDocument (.odt) |
|
|  | [getOTT()](#getOTT--) | Modello di documento OpenDocument (.ott) |
|
|  | [fromExtension(String extension)](#fromExtension-java.lang.String-) | Mappa l'estensione del file al tipo di file. |
|
|  | [getSupportedFileTypes()](#getSupportedFileTypes--) | Recupera i tipi di file supportati |
|
|  | [equals(FileType other)](#equals-com.groupdocs.redaction.FileType-) | Determina se l'attuale |
FileType
è lo stesso di quello specificato
FileType
oggetto.
|
|  | [equals(Object obj)](#equals-java.lang.Object-) | Determina se l'attuale |
FileType
è lo stesso dell'oggetto specificato.
|
|  | [hashCode()](#hashCode--) | Restituisce il codice hash per l'attuale |
FileType
oggetto.
|
|  | [op_Equality(FileType left, FileType right)](#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Determina se due |
FileType
gli oggetti sono gli stessi.
|
|  | [op_Inequality(FileType left, FileType right)](#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Determina se due |
FileType
gli oggetti non sono gli stessi.
|
|  | [toString()](#toString--) | Restituisce una stringa che rappresenta l'oggetto corrente. |
|
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


Restituisce il nome del tipo di file, ad esempio "Microsoft Word Document".


**Returns:**
java.lang.String - Nome del tipo di file, ad esempio "Microsoft Word Document".

### getExtension() {#getExtension--}
```
public final String getExtension()
```


Restituisce il suffisso del nome file (incluso il punto "."), ad esempio ".doc".


**Returns:**
java.lang.String - Suffisso del nome file (incluso il punto "."), ad esempio ".doc".

### getUnknown() {#getUnknown--}
```
public static FileType getUnknown()
```


Rappresenta un tipo di file sconosciuto.


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


JPEG Immagine (.jpg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPEG() {#getJPEG--}
```
public static FileType getJPEG()
```


JPEG Immagine (.jpeg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPNG() {#getPNG--}
```
public static FileType getPNG()
```


Grafica di Rete Portabile (.png)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getGIF() {#getGIF--}
```
public static FileType getGIF()
```


File di Formato di Interscambio Grafico (.gif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getBMP() {#getBMP--}
```
public static FileType getBMP()
```


File di Immagine Bitmap (.bmp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJP2() {#getJP2--}
```
public static FileType getJP2()
```


File di Immagine Core JPEG 2000 (.jp2)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTM() {#getHTM--}
```
public static FileType getHTM()
```


File di Linguaggio di Marcatura Hypertext (.htm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTML() {#getHTML--}
```
public static FileType getHTML()
```


File di Linguaggio di Marcatura Hypertext (.html)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPDF() {#getPDF--}
```
public static FileType getPDF()
```


File di Formato di Documento Portabile (.pdf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPT() {#getPPT--}
```
public static FileType getPPT()
```


Presentazione PowerPoint (.ppt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPTX() {#getPPTX--}
```
public static FileType getPPTX()
```


Presentazione PowerPoint Open XML (.pptx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODP() {#getODP--}
```
public static FileType getODP()
```


Presentazione OpenDocument (.odp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTX() {#getPOTX--}
```
public static FileType getPOTX()
```


Modello di Presentazione PowerPoint Open XML (.potx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTM() {#getPOTM--}
```
public static FileType getPOTM()
```


Modello di Presentazione PowerPoint Open XML con Macro (.potm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTP() {#getOTP--}
```
public static FileType getOTP()
```


Modello di Presentazione OpenDocument (.otp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLS() {#getXLS--}
```
public static FileType getXLS()
```


Foglio di Calcolo Excel (.xls)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSX() {#getXLSX--}
```
public static FileType getXLSX()
```


Foglio di Calcolo Microsoft Excel Open XML (.xlsx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSM() {#getXLSM--}
```
public static FileType getXLSM()
```


Foglio di Calcolo Excel Open XML con Macro (.xlsm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSB() {#getXLSB--}
```
public static FileType getXLSB()
```


Foglio di Calcolo Binario Excel (.xlsb)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTX() {#getXLTX--}
```
public static FileType getXLTX()
```


Modello di Foglio di Calcolo Excel Open XML (.xltx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTM() {#getXLTM--}
```
public static FileType getXLTM()
```


Modello di Foglio di Calcolo Excel Open XML con Macro (.xltm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLT() {#getXLT--}
```
public static FileType getXLT()
```


Modello di Excel (.xlt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getCSV() {#getCSV--}
```
public static FileType getCSV()
```


File di Valori Separati da Virgola (.csv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTSV() {#getTSV--}
```
public static FileType getTSV()
```


File di Valori Separati da Tabulazione (.tsv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTAB() {#getTAB--}
```
public static FileType getTAB()
```


File di Valori Separati da Tabulazione (.tab)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODS() {#getODS--}
```
public static FileType getODS()
```


Foglio di calcolo OpenDocument (.ods)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTS() {#getOTS--}
```
public static FileType getOTS()
```


Modello di foglio di calcolo OpenDocument (.ots)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getNUMBERS() {#getNUMBERS--}
```
public static FileType getNUMBERS()
```


Foglio di calcolo Apple Numbers (.numbers)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getMD() {#getMD--}
```
public static FileType getMD()
```


File di documentazione Markdown (.md)


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


Documento Open XML Microsoft Word (.docx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCM() {#getDOCM--}
```
public static FileType getDOCM()
```


Documento macro abilitato Open XML Word (.docm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOT() {#getDOT--}
```
public static FileType getDOT()
```


Modello di documento Word (.dot)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTX() {#getDOTX--}
```
public static FileType getDOTX()
```


Modello di documento Open XML Word (.dotx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTM() {#getDOTM--}
```
public static FileType getDOTM()
```


Modello di documento macro abilitato Open XML Word (.dotm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getRTF() {#getRTF--}
```
public static FileType getRTF()
```


File Rich Text Format (.rtf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTXT() {#getTXT--}
```
public static FileType getTXT()
```


File di testo semplice (.txt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODT() {#getODT--}
```
public static FileType getODT()
```


Documento di testo OpenDocument (.odt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTT() {#getOTT--}
```
public static FileType getOTT()
```


Modello di documento OpenDocument (.ott)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### fromExtension(String extension) {#fromExtension-java.lang.String-}
```
public static FileType fromExtension(String extension)
```


Mappa l'estensione del file al tipo di file.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | estensione | java.lang.String | Estensione del file (incluso il punto "."). |
|

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - When file type is supported returns it, otherwise returns default  Unknown  file type.

### getSupportedFileTypes() {#getSupportedFileTypes--}
```
public static Iterable<FileType> getSupportedFileTypes()
```


Recupera i tipi di file supportati


**Returns:**
java.lang.Iterable<com.groupdocs.redaction.FileType> - Restituisce la sequenza dei tipi di file supportati

### equals(FileType other) {#equals-com.groupdocs.redaction.FileType-}
```
public final boolean equals(FileType other)
```


Determina se l'attuale
FileType
è lo stesso di quello specificato
FileType
oggetto.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | other | [FileType](../../com.groupdocs.redaction/filetype) | L'oggetto da confrontare con l'oggetto FileType corrente. |
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

il parametro è FileType e è lo stesso dell'oggetto FileType corrente; altrimenti,

```
false
```


### hashCode() {#hashCode--}
```
public int hashCode()
```


Restituisce il codice hash per l'attuale
FileType
oggetto.


**Returns:**
int - Un codice hash per l'oggetto FileType corrente.

### op_Equality(FileType left, FileType right) {#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Equality(FileType left, FileType right)
```


Determina se due
FileType
gli oggetti sono gli stessi.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | left | [FileType](../../com.groupdocs.redaction/filetype) | Oggetto FileType sinistro. |
|
|  | right | [FileType](../../com.groupdocs.redaction/filetype) | Oggetto FileType destro. |
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

se entrambi gli oggetti FileType non sono gli stessi; altrimenti,

```
false
```


### toString() {#toString--}
```
public String toString()
```


Restituisce una stringa che rappresenta l'oggetto corrente.


**Returns:**
java.lang.String - Una stringa che rappresenta l'oggetto corrente.

