---
title: "FileType"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει έναν τύπο αρχείου."
type: docs
weight: 11
url: /el/java/com.groupdocs.redaction/filetype/
---
**Inheritance:**
java.lang.Object
```
public final class FileType
```

Αντιπροσωπεύει έναν τύπο αρχείου. Παρέχει μεθόδους για την απόκτηση λίστας όλων των τύπων αρχείων που υποστηρίζονται από το GroupDocs.Redaction, την ανίχνευση τύπου αρχείου με βάση την επέκταση, κ.λπ.

*** ** * ** ***


**Learn more**

* [Supported Document Formats](../https://docs.groupdocs.com/redaction/java/supported-document-formats/)
* [Get supported file formats](../https://docs.groupdocs.com/redaction/java/get-supported-file-formats/)
* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Λαμβάνει το όνομα του τύπου αρχείου, για παράδειγμα "Microsoft Word Document". |
|
|  | [getExtension()](#getExtension--) | Λαμβάνει το επίθημα του ονόματος αρχείου (συμπεριλαμβανομένου του σημείου "."), για παράδειγμα ".doc". |
|
|  | [getUnknown()](#getUnknown--) | Αντιπροσωπεύει άγνωστο τύπο αρχείου. |
|
|  | [getTIF()](#getTIF--) | Αρχείο Ετικετοποιημένης Εικόνας (.tif) |
|
|  | [getTIFF()](#getTIFF--) | Μορφή Αρχείου Ετικετοποιημένης Εικόνας (.tiff) |
|
|  | [getJPG()](#getJPG--) | JPEG Εικόνα (.jpg) |
|
|  | [getJPEG()](#getJPEG--) | JPEG Εικόνα (.jpeg) |
|
|  | [getPNG()](#getPNG--) | Φορητό Δίκτυο Γραφικό (.png) |
|
|  | [getGIF()](#getGIF--) | Αρχείο Γραφικής Μορφής Ανταλλαγής (.gif) |
|
|  | [getBMP()](#getBMP--) | Αρχείο Εικόνας Bitmap (.bmp) |
|
|  | [getJP2()](#getJP2--) | Αρχείο Κύριας Εικόνας JPEG 2000 (.jp2) |
|
|  | [getHTM()](#getHTM--) | Αρχείο Γλώσσας Σήμανσης Υπερκειμένου (.htm) |
|
|  | [getHTML()](#getHTML--) | Αρχείο Γλώσσας Σήμανσης Υπερκειμένου (.html) |
|
|  | [getPDF()](#getPDF--) | Αρχείο Φορμάτ Φορητού Εγγράφου (.pdf) |
|
|  | [getPPT()](#getPPT--) | Παρουσίαση PowerPoint (.ppt) |
|
|  | [getPPTX()](#getPPTX--) | Παρουσίαση PowerPoint Open XML (.pptx) |
|
|  | [getODP()](#getODP--) | Παρουσίαση OpenDocument (.odp) |
|
|  | [getPOTX()](#getPOTX--) | Πρότυπο Παρουσίασης PowerPoint Open XML (.potx) |
|
|  | [getPOTM()](#getPOTM--) | Πρότυπο Παρουσίασης PowerPoint Open XML με Μακροεντολές (.potm) |
|
|  | [getOTP()](#getOTP--) | Πρότυπο Παρουσίασης OpenDocument (.otp) |
|
|  | [getXLS()](#getXLS--) | Φύλλο Εργασίας Excel (.xls) |
|
|  | [getXLSX()](#getXLSX--) | Φύλλο Εργασίας Microsoft Excel Open XML (.xlsx) |
|
|  | [getXLSM()](#getXLSM--) | Φύλλο Εργασίας Excel Open XML με Μακροεντολές (.xlsm) |
|
|  | [getXLSB()](#getXLSB--) | Δυαδικό Φύλλο Εργασίας Excel (.xlsb) |
|
|  | [getXLTX()](#getXLTX--) | Πρότυπο Φύλλου Εργασίας Excel Open XML (.xltx) |
|
|  | [getXLTM()](#getXLTM--) | Πρότυπο Φύλλου Εργασίας Excel Open XML με Μακροεντολές (.xltm) |
|
|  | [getXLT()](#getXLT--) | Πρότυπο Excel (.xlt) |
|
|  | [getCSV()](#getCSV--) | Αρχείο Τιμών Διαχωρισμένων με Κόμμα (.csv) |
|
|  | [getTSV()](#getTSV--) | Αρχείο Τιμών Διαχωρισμένων με Καρτέλα (.tsv) |
|
|  | [getTAB()](#getTAB--) | Αρχείο Τιμών Διαχωρισμένων με Καρτέλα (.tab) |
|
|  | [getODS()](#getODS--) | Φύλλο εργασίας OpenDocument (.ods) |
|
|  | [getOTS()](#getOTS--) | Πρότυπο φύλλου εργασίας OpenDocument (.ots) |
|
|  | [getNUMBERS()](#getNUMBERS--) | Φύλλο εργασίας Apple Numbers (.numbers) |
|
|  | [getMD()](#getMD--) | Αρχείο τεκμηρίωσης Markdown (.md) |
|
|  | [getDOC()](#getDOC--) | Έγγραφο Microsoft Word (.doc) |
|
|  | [getDOCX()](#getDOCX--) | Έγγραφο Microsoft Word Open XML (.docx) |
|
|  | [getDOCM()](#getDOCM--) | Έγγραφο Word Open XML με μακροεντολές (.docm) |
|
|  | [getDOT()](#getDOT--) | Πρότυπο εγγράφου Word (.dot) |
|
|  | [getDOTX()](#getDOTX--) | Πρότυπο εγγράφου Word Open XML (.dotx) |
|
|  | [getDOTM()](#getDOTM--) | Πρότυπο εγγράφου Word Open XML με μακροεντολές (.dotm) |
|
|  | [getRTF()](#getRTF--) | Αρχείο Rich Text Format (.rtf) |
|
|  | [getTXT()](#getTXT--) | Αρχείο απλού κειμένου (.txt) |
|
|  | [getODT()](#getODT--) | Έγγραφο κειμένου OpenDocument (.odt) |
|
|  | [getOTT()](#getOTT--) | Πρότυπο εγγράφου OpenDocument (.ott) |
|
|  | [fromExtension(String extension)](#fromExtension-java.lang.String-) | Αντιστοιχίζει την επέκταση αρχείου με τον τύπο αρχείου. |
|
|  | [getSupportedFileTypes()](#getSupportedFileTypes--) | Ανακτά τους υποστηριζόμενους τύπους αρχείων |
|
|  | [equals(FileType other)](#equals-com.groupdocs.redaction.FileType-) | Καθορίζει εάν το τρέχον |
FileType
είναι το ίδιο με το καθορισμένο
FileType
αντικείμενο.
|
|  | [equals(Object obj)](#equals-java.lang.Object-) | Καθορίζει εάν το τρέχον |
FileType
είναι το ίδιο με το καθορισμένο αντικείμενο.
|
|  | [hashCode()](#hashCode--) | Επιστρέφει τον κώδικα κατακερματισμού για το τρέχον |
FileType
αντικείμενο.
|
|  | [op_Equality(FileType left, FileType right)](#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Καθορίζει εάν δύο |
FileType
τα αντικείμενα είναι τα ίδια.
|
|  | [op_Inequality(FileType left, FileType right)](#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | Καθορίζει εάν δύο |
FileType
τα αντικείμενα δεν είναι τα ίδια.
|
|  | [toString()](#toString--) | Επιστρέφει μια συμβολοσειρά που αντιπροσωπεύει το τρέχον αντικείμενο. |
|
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


Λαμβάνει το όνομα του τύπου αρχείου, για παράδειγμα "Microsoft Word Document".


**Returns:**
java.lang.String - Όνομα τύπου αρχείου, για παράδειγμα "Microsoft Word Document".

### getExtension() {#getExtension--}
```
public final String getExtension()
```


Λαμβάνει το επίθημα του ονόματος αρχείου (συμπεριλαμβανομένου του σημείου "."), για παράδειγμα ".doc".


**Returns:**
java.lang.String - Κατάληξη ονόματος αρχείου (συμπεριλαμβανομένου του σημείου "."), για παράδειγμα ".doc".

### getUnknown() {#getUnknown--}
```
public static FileType getUnknown()
```


Αντιπροσωπεύει άγνωστο τύπο αρχείου.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIF() {#getTIF--}
```
public static FileType getTIF()
```


Αρχείο Ετικετοποιημένης Εικόνας (.tif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIFF() {#getTIFF--}
```
public static FileType getTIFF()
```


Μορφή Αρχείου Ετικετοποιημένης Εικόνας (.tiff)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPG() {#getJPG--}
```
public static FileType getJPG()
```


JPEG Εικόνα (.jpg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPEG() {#getJPEG--}
```
public static FileType getJPEG()
```


JPEG Εικόνα (.jpeg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPNG() {#getPNG--}
```
public static FileType getPNG()
```


Φορητό Δίκτυο Γραφικό (.png)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getGIF() {#getGIF--}
```
public static FileType getGIF()
```


Αρχείο Γραφικής Μορφής Ανταλλαγής (.gif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getBMP() {#getBMP--}
```
public static FileType getBMP()
```


Αρχείο Εικόνας Bitmap (.bmp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJP2() {#getJP2--}
```
public static FileType getJP2()
```


Αρχείο Κύριας Εικόνας JPEG 2000 (.jp2)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTM() {#getHTM--}
```
public static FileType getHTM()
```


Αρχείο Γλώσσας Σήμανσης Υπερκειμένου (.htm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTML() {#getHTML--}
```
public static FileType getHTML()
```


Αρχείο Γλώσσας Σήμανσης Υπερκειμένου (.html)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPDF() {#getPDF--}
```
public static FileType getPDF()
```


Αρχείο Φορμάτ Φορητού Εγγράφου (.pdf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPT() {#getPPT--}
```
public static FileType getPPT()
```


Παρουσίαση PowerPoint (.ppt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPTX() {#getPPTX--}
```
public static FileType getPPTX()
```


Παρουσίαση PowerPoint Open XML (.pptx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODP() {#getODP--}
```
public static FileType getODP()
```


Παρουσίαση OpenDocument (.odp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTX() {#getPOTX--}
```
public static FileType getPOTX()
```


Πρότυπο Παρουσίασης PowerPoint Open XML (.potx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTM() {#getPOTM--}
```
public static FileType getPOTM()
```


Πρότυπο Παρουσίασης PowerPoint Open XML με Μακροεντολές (.potm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTP() {#getOTP--}
```
public static FileType getOTP()
```


Πρότυπο Παρουσίασης OpenDocument (.otp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLS() {#getXLS--}
```
public static FileType getXLS()
```


Φύλλο Εργασίας Excel (.xls)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSX() {#getXLSX--}
```
public static FileType getXLSX()
```


Φύλλο Εργασίας Microsoft Excel Open XML (.xlsx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSM() {#getXLSM--}
```
public static FileType getXLSM()
```


Φύλλο Εργασίας Excel Open XML με Μακροεντολές (.xlsm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSB() {#getXLSB--}
```
public static FileType getXLSB()
```


Δυαδικό Φύλλο Εργασίας Excel (.xlsb)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTX() {#getXLTX--}
```
public static FileType getXLTX()
```


Πρότυπο Φύλλου Εργασίας Excel Open XML (.xltx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTM() {#getXLTM--}
```
public static FileType getXLTM()
```


Πρότυπο Φύλλου Εργασίας Excel Open XML με Μακροεντολές (.xltm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLT() {#getXLT--}
```
public static FileType getXLT()
```


Πρότυπο Excel (.xlt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getCSV() {#getCSV--}
```
public static FileType getCSV()
```


Αρχείο Τιμών Διαχωρισμένων με Κόμμα (.csv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTSV() {#getTSV--}
```
public static FileType getTSV()
```


Αρχείο Τιμών Διαχωρισμένων με Καρτέλα (.tsv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTAB() {#getTAB--}
```
public static FileType getTAB()
```


Αρχείο Τιμών Διαχωρισμένων με Καρτέλα (.tab)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODS() {#getODS--}
```
public static FileType getODS()
```


Φύλλο εργασίας OpenDocument (.ods)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTS() {#getOTS--}
```
public static FileType getOTS()
```


Πρότυπο φύλλου εργασίας OpenDocument (.ots)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getNUMBERS() {#getNUMBERS--}
```
public static FileType getNUMBERS()
```


Φύλλο εργασίας Apple Numbers (.numbers)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getMD() {#getMD--}
```
public static FileType getMD()
```


Αρχείο τεκμηρίωσης Markdown (.md)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOC() {#getDOC--}
```
public static FileType getDOC()
```


Έγγραφο Microsoft Word (.doc)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCX() {#getDOCX--}
```
public static FileType getDOCX()
```


Έγγραφο Microsoft Word Open XML (.docx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCM() {#getDOCM--}
```
public static FileType getDOCM()
```


Έγγραφο Word Open XML με μακροεντολές (.docm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOT() {#getDOT--}
```
public static FileType getDOT()
```


Πρότυπο εγγράφου Word (.dot)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTX() {#getDOTX--}
```
public static FileType getDOTX()
```


Πρότυπο εγγράφου Word Open XML (.dotx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTM() {#getDOTM--}
```
public static FileType getDOTM()
```


Πρότυπο εγγράφου Word Open XML με μακροεντολές (.dotm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getRTF() {#getRTF--}
```
public static FileType getRTF()
```


Αρχείο Rich Text Format (.rtf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTXT() {#getTXT--}
```
public static FileType getTXT()
```


Αρχείο απλού κειμένου (.txt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODT() {#getODT--}
```
public static FileType getODT()
```


Έγγραφο κειμένου OpenDocument (.odt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTT() {#getOTT--}
```
public static FileType getOTT()
```


Πρότυπο εγγράφου OpenDocument (.ott)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### fromExtension(String extension) {#fromExtension-java.lang.String-}
```
public static FileType fromExtension(String extension)
```


Αντιστοιχίζει την επέκταση αρχείου με τον τύπο αρχείου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | επέκταση | java.lang.String | Επέκταση αρχείου (συμπεριλαμβανομένου του σημείου "."). |
|

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - When file type is supported returns it, otherwise returns default  Unknown  file type.

### getSupportedFileTypes() {#getSupportedFileTypes--}
```
public static Iterable<FileType> getSupportedFileTypes()
```


Ανακτά τους υποστηριζόμενους τύπους αρχείων


**Returns:**
java.lang.Iterable<com.groupdocs.redaction.FileType> - Επιστρέφει τη σειρά των υποστηριζόμενων τύπων αρχείων

### equals(FileType other) {#equals-com.groupdocs.redaction.FileType-}
```
public final boolean equals(FileType other)
```


Καθορίζει εάν το τρέχον
FileType
είναι το ίδιο με το καθορισμένο
FileType
αντικείμενο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | other | [FileType](../../com.groupdocs.redaction/filetype) | Το αντικείμενο προς σύγκριση με το τρέχον  FileType  αντικείμενο. |
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

η παράμετρος είναι  FileType  και είναι η ίδια με το τρέχον  FileType  αντικείμενο· διαφορετικά,

```
false
```


### hashCode() {#hashCode--}
```
public int hashCode()
```


Επιστρέφει τον κώδικα κατακερματισμού για το τρέχον
FileType
αντικείμενο.


**Returns:**
int - Ένας κωδικός κατακερματισμού για το τρέχον  FileType  αντικείμενο.

### op_Equality(FileType left, FileType right) {#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Equality(FileType left, FileType right)
```


Καθορίζει εάν δύο
FileType
τα αντικείμενα είναι τα ίδια.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | left | [FileType](../../com.groupdocs.redaction/filetype) | Αριστερό  FileType  αντικείμενο. |
|
|  | right | [FileType](../../com.groupdocs.redaction/filetype) | Δεξιό  FileType  αντικείμενο. |
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

αν και τα  FileType  αντικείμενα δεν είναι ίδια· διαφορετικά,

```
false
```


### toString() {#toString--}
```
public String toString()
```


Επιστρέφει μια συμβολοσειρά που αντιπροσωπεύει το τρέχον αντικείμενο.


**Returns:**
java.lang.String - Μια συμβολοσειρά που αντιπροσωπεύει το τρέχον αντικείμενο.

