---
title: "FileType"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente un type de fichier."
type: docs
weight: 11
url: /fr/java/com.groupdocs.redaction/filetype/
---
**Inheritance:**
java.lang.Object
```
public final class FileType
```

Représente un type de fichier. Fournit des méthodes pour obtenir la liste de tous les types de fichiers pris en charge par GroupDocs.Redaction, détecter le type de fichier par extension, etc.

*** ** * ** ***


**Learn more**

* [Supported Document Formats](../https://docs.groupdocs.com/redaction/java/supported-document-formats/)
* [Get supported file formats](../https://docs.groupdocs.com/redaction/java/get-supported-file-formats/)
* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Obtient le nom du type de fichier, par exemple "Microsoft Word Document". |
|
|  | [getExtension()](#getExtension--) | Obtient le suffixe du nom de fichier (y compris le point "."), par exemple ".doc". |
|
|  | [getUnknown()](#getUnknown--) | Représente un type de fichier inconnu. |
|
|  | [getTIF()](#getTIF--) | Fichier image balisé (.tif) |
|
|  | [getTIFF()](#getTIFF--) | Format de fichier image balisé (.tiff) |
|
|  | [getJPG()](#getJPG--) | Image JPEG (.jpg) |
|
|  | [getJPEG()](#getJPEG--) | Image JPEG (.jpeg) |
|
|  | [getPNG()](#getPNG--) | Graphique Réseau Portable (.png) |
|
|  | [getGIF()](#getGIF--) | Fichier Format d'échange graphique (.gif) |
|
|  | [getBMP()](#getBMP--) | Fichier d'image bitmap (.bmp) |
|
|  | [getJP2()](#getJP2--) | Fichier d'image principale JPEG 2000 (.jp2) |
|
|  | [getHTM()](#getHTM--) | Fichier Langage de balisage hypertexte (.htm) |
|
|  | [getHTML()](#getHTML--) | Fichier Langage de balisage hypertexte (.html) |
|
|  | [getPDF()](#getPDF--) | Fichier Format de document portable (.pdf) |
|
|  | [getPPT()](#getPPT--) | Présentation PowerPoint (.ppt) |
|
|  | [getPPTX()](#getPPTX--) | Présentation PowerPoint Open XML (.pptx) |
|
|  | [getODP()](#getODP--) | Présentation OpenDocument (.odp) |
|
|  | [getPOTX()](#getPOTX--) | Modèle de présentation PowerPoint Open XML (.potx) |
|
|  | [getPOTM()](#getPOTM--) | Modèle de présentation PowerPoint Open XML avec macros (.potm) |
|
|  | [getOTP()](#getOTP--) | Modèle de présentation OpenDocument (.otp) |
|
|  | [getXLS()](#getXLS--) | Feuille de calcul Excel (.xls) |
|
|  | [getXLSX()](#getXLSX--) | Feuille de calcul Microsoft Excel Open XML (.xlsx) |
|
|  | [getXLSM()](#getXLSM--) | Feuille de calcul Excel Open XML avec macros (.xlsm) |
|
|  | [getXLSB()](#getXLSB--) | Feuille de calcul binaire Excel (.xlsb) |
|
|  | [getXLTX()](#getXLTX--) | Modèle de feuille de calcul Excel Open XML (.xltx) |
|
|  | [getXLTM()](#getXLTM--) | Modèle de feuille de calcul Excel Open XML avec macros (.xltm) |
|
|  | [getXLT()](#getXLT--) | Modèle Excel (.xlt) |
|
|  | [getCSV()](#getCSV--) | Fichier de valeurs séparées par des virgules (.csv) |
|
|  | [getTSV()](#getTSV--) | Fichier de valeurs séparées par des tabulations (.tsv) |
|
|  | [getTAB()](#getTAB--) | Fichier de valeurs séparées par des tabulations (.tab) |
|
|  | [getODS()](#getODS--) | Feuille de calcul OpenDocument (.ods) |
|
|  | [getOTS()](#getOTS--) | Modèle de feuille de calcul OpenDocument (.ots) |
|
|  | [getNUMBERS()](#getNUMBERS--) | Feuille de calcul Apple Numbers (.numbers) |
|
|  | [getMD()](#getMD--) | Fichier de documentation Markdown (.md) |
|
|  | [getDOC()](#getDOC--) | Document Microsoft Word (.doc) |
|
|  | [getDOCX()](#getDOCX--) | Document Microsoft Word Open XML (.docx) |
|
|  | [getDOCM()](#getDOCM--) | Document Microsoft Word Open XML avec macros (.docm) |
|
|  | [getDOT()](#getDOT--) | Modèle de document Word (.dot) |
|
|  | [getDOTX()](#getDOTX--) | Modèle de document Microsoft Word Open XML (.dotx) |
|
|  | [getDOTM()](#getDOTM--) | Modèle de document Microsoft Word Open XML avec macros (.dotm) |
|
|  | [getRTF()](#getRTF--) | Fichier Rich Text Format (.rtf) |
|
|  | [getTXT()](#getTXT--) | Fichier texte brut (.txt) |
|
|  | [getODT()](#getODT--) | Document texte OpenDocument (.odt) |
|
|  | [getOTT()](#getOTT--) | Modèle de document OpenDocument (.ott) |
|
|  | [fromExtension(String extension)](#fromExtension-java.lang.String-) | Mappe l'extension de fichier au type de fichier. |
|
|  | [getSupportedFileTypes()](#getSupportedFileTypes--) | Récupère les types de fichiers pris en charge |
|
|  | [equals(FileType other)](#equals-com.groupdocs.redaction.FileType-) | Détermine si le courant |
FileType
est le même que spécifié
FileType
objet.
|
|  | [equals(Object obj)](#equals-java.lang.Object-) | Détermine si le courant |
FileType
est le même que l'objet spécifié.
|
|  | [hashCode()](#hashCode--) | Renvoie le code de hachage pour le courant |
FileType
objet.
|
|  | [op_Equality(FileType left, FileType right)](#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Détermine si deux |
FileType
les objets sont identiques.
|
|  | [op_Inequality(FileType left, FileType right)](#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Détermine si deux |
FileType
les objets ne sont pas identiques.
|
|  | [toString()](#toString--) | Renvoie une chaîne qui représente l'objet courant. |
|
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


Obtient le nom du type de fichier, par exemple "Microsoft Word Document".


**Returns:**
java.lang.String - Nom du type de fichier, par exemple "Microsoft Word Document".

### getExtension() {#getExtension--}
```
public final String getExtension()
```


Obtient le suffixe du nom de fichier (y compris le point "."), par exemple ".doc".


**Returns:**
java.lang.String - Suffixe du nom de fichier (incluant le point "."), par exemple ".doc".

### getUnknown() {#getUnknown--}
```
public static FileType getUnknown()
```


Représente un type de fichier inconnu.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIF() {#getTIF--}
```
public static FileType getTIF()
```


Fichier image balisé (.tif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIFF() {#getTIFF--}
```
public static FileType getTIFF()
```


Format de fichier image balisé (.tiff)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPG() {#getJPG--}
```
public static FileType getJPG()
```


Image JPEG (.jpg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPEG() {#getJPEG--}
```
public static FileType getJPEG()
```


Image JPEG (.jpeg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPNG() {#getPNG--}
```
public static FileType getPNG()
```


Graphique Réseau Portable (.png)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getGIF() {#getGIF--}
```
public static FileType getGIF()
```


Fichier Format d'échange graphique (.gif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getBMP() {#getBMP--}
```
public static FileType getBMP()
```


Fichier d'image bitmap (.bmp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJP2() {#getJP2--}
```
public static FileType getJP2()
```


Fichier d'image principale JPEG 2000 (.jp2)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTM() {#getHTM--}
```
public static FileType getHTM()
```


Fichier Langage de balisage hypertexte (.htm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTML() {#getHTML--}
```
public static FileType getHTML()
```


Fichier Langage de balisage hypertexte (.html)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPDF() {#getPDF--}
```
public static FileType getPDF()
```


Fichier Format de document portable (.pdf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPT() {#getPPT--}
```
public static FileType getPPT()
```


Présentation PowerPoint (.ppt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPTX() {#getPPTX--}
```
public static FileType getPPTX()
```


Présentation PowerPoint Open XML (.pptx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODP() {#getODP--}
```
public static FileType getODP()
```


Présentation OpenDocument (.odp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTX() {#getPOTX--}
```
public static FileType getPOTX()
```


Modèle de présentation PowerPoint Open XML (.potx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTM() {#getPOTM--}
```
public static FileType getPOTM()
```


Modèle de présentation PowerPoint Open XML avec macros (.potm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTP() {#getOTP--}
```
public static FileType getOTP()
```


Modèle de présentation OpenDocument (.otp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLS() {#getXLS--}
```
public static FileType getXLS()
```


Feuille de calcul Excel (.xls)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSX() {#getXLSX--}
```
public static FileType getXLSX()
```


Feuille de calcul Microsoft Excel Open XML (.xlsx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSM() {#getXLSM--}
```
public static FileType getXLSM()
```


Feuille de calcul Excel Open XML avec macros (.xlsm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSB() {#getXLSB--}
```
public static FileType getXLSB()
```


Feuille de calcul binaire Excel (.xlsb)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTX() {#getXLTX--}
```
public static FileType getXLTX()
```


Modèle de feuille de calcul Excel Open XML (.xltx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTM() {#getXLTM--}
```
public static FileType getXLTM()
```


Modèle de feuille de calcul Excel Open XML avec macros (.xltm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLT() {#getXLT--}
```
public static FileType getXLT()
```


Modèle Excel (.xlt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getCSV() {#getCSV--}
```
public static FileType getCSV()
```


Fichier de valeurs séparées par des virgules (.csv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTSV() {#getTSV--}
```
public static FileType getTSV()
```


Fichier de valeurs séparées par des tabulations (.tsv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTAB() {#getTAB--}
```
public static FileType getTAB()
```


Fichier de valeurs séparées par des tabulations (.tab)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODS() {#getODS--}
```
public static FileType getODS()
```


Feuille de calcul OpenDocument (.ods)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTS() {#getOTS--}
```
public static FileType getOTS()
```


Modèle de feuille de calcul OpenDocument (.ots)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getNUMBERS() {#getNUMBERS--}
```
public static FileType getNUMBERS()
```


Feuille de calcul Apple Numbers (.numbers)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getMD() {#getMD--}
```
public static FileType getMD()
```


Fichier de documentation Markdown (.md)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOC() {#getDOC--}
```
public static FileType getDOC()
```


Document Microsoft Word (.doc)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCX() {#getDOCX--}
```
public static FileType getDOCX()
```


Document Microsoft Word Open XML (.docx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCM() {#getDOCM--}
```
public static FileType getDOCM()
```


Document Microsoft Word Open XML avec macros (.docm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOT() {#getDOT--}
```
public static FileType getDOT()
```


Modèle de document Word (.dot)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTX() {#getDOTX--}
```
public static FileType getDOTX()
```


Modèle de document Microsoft Word Open XML (.dotx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTM() {#getDOTM--}
```
public static FileType getDOTM()
```


Modèle de document Microsoft Word Open XML avec macros (.dotm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getRTF() {#getRTF--}
```
public static FileType getRTF()
```


Fichier Rich Text Format (.rtf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTXT() {#getTXT--}
```
public static FileType getTXT()
```


Fichier texte brut (.txt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODT() {#getODT--}
```
public static FileType getODT()
```


Document texte OpenDocument (.odt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTT() {#getOTT--}
```
public static FileType getOTT()
```


Modèle de document OpenDocument (.ott)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### fromExtension(String extension) {#fromExtension-java.lang.String-}
```
public static FileType fromExtension(String extension)
```


Mappe l'extension de fichier au type de fichier.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | extension | java.lang.String | Extension de fichier (incluant le point "."). |
|

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - When file type is supported returns it, otherwise returns default  Unknown  file type.

### getSupportedFileTypes() {#getSupportedFileTypes--}
```
public static Iterable<FileType> getSupportedFileTypes()
```


Récupère les types de fichiers pris en charge


**Returns:**
java.lang.Iterable<com.groupdocs.redaction.FileType> - Retourne la séquence des types de fichiers pris en charge

### equals(FileType other) {#equals-com.groupdocs.redaction.FileType-}
```
public final boolean equals(FileType other)
```


Détermine si le courant
FileType
est le même que spécifié
FileType
objet.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | other | [FileType](../../com.groupdocs.redaction/filetype) | L'objet à comparer avec l'objet  FileType  actuel. |
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

le paramètre est  FileType  et est le même que l'objet  FileType  actuel ; sinon,

```
false
```


### hashCode() {#hashCode--}
```
public int hashCode()
```


Renvoie le code de hachage pour le courant
FileType
objet.


**Returns:**
int - Un code de hachage pour l'objet  FileType  actuel.

### op_Equality(FileType left, FileType right) {#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Equality(FileType left, FileType right)
```


Détermine si deux
FileType
les objets sont identiques.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | left | [FileType](../../com.groupdocs.redaction/filetype) | Objet  FileType  de gauche. |
|
|  | right | [FileType](../../com.groupdocs.redaction/filetype) | Objet  FileType  de droite. |
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

si les deux objets  FileType  ne sont pas identiques ; sinon,

```
false
```


### toString() {#toString--}
```
public String toString()
```


Renvoie une chaîne qui représente l'objet courant.


**Returns:**
java.lang.String - Une chaîne qui représente l'objet actuel.

