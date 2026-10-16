---
title: "RedactionDescription"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili informasi aksi perubahan tunggal yang dilakukan selama proses redaksi."
type: docs
weight: 25
url: /id/java/com.groupdocs.redaction.redactions/redactiondescription/
---
**Inheritance:**
java.lang.Object
```
public class RedactionDescription
```

Mewakili informasi aksi perubahan tunggal yang dilakukan selama proses redaksi.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-) | Menginisialisasi instance baru dari kelas RedactionDescription tanpa informasi penggantian. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-) | Menginisialisasi instance baru dari kelas RedactionDescription dengan informasi penggantian. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-) | Menginisialisasi instance baru dari kelas RedactionDescription dengan informasi penggantian area gambar. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getRedactionType()](#getRedactionType--) | Mendapatkan tipe data dokumen - teks, metadata, atau anotasi. |
|
|  | [getActionType()](#getActionType--) | Mendapatkan operasi redaksi: penggantian, pembersihan, atau penghapusan. |
|
|  | [getOriginalText()](#getOriginalText--) | Mendapatkan teks yang cocok, jika ada ekspresi yang diberikan. |
|
|  | [getReplacement()](#getReplacement--) | Mendapatkan informasi penggantian, dapat bernilai null. |
|
|  | [getImageAreaReplacement()](#getImageAreaReplacement--) | Mendapatkan informasi penggantian untuk redaksi area gambar, mengembalikan null untuk redaksi teks. |
|
|  | [getDetails()](#getDetails--) | Mendapatkan informasi detail opsional untuk item yang sedang di-redact. |
|
|  | [setDetails(String value)](#setDetails-java.lang.String-) | Mengatur informasi detail opsional untuk item yang sedang di-redact. |
|
### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)
```


Menginisialisasi instance baru dari kelas RedactionDescription tanpa informasi penggantian.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | redactionType | int | Jenis data yang di-redact |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Tindakan yang akan dilakukan pada data ini |
|
|  | originalText | java.lang.String | Teks yang cocok, komentar, atau isi anotasi |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)
```


Menginisialisasi instance baru dari kelas RedactionDescription dengan informasi penggantian.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | redactionType | int | Jenis data yang di-redact |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Tindakan yang akan dilakukan pada data ini |
|
|  | originalText | java.lang.String | Teks yang cocok, komentar, atau isi anotasi |
|
|  | replacement | [TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) | Teks pengganti, teks yang cocok, dan posisinya dalam string asli |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)
```


Menginisialisasi instance baru dari kelas RedactionDescription dengan informasi penggantian area gambar.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | redactionType | int | Jenis data yang di-redact |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Tindakan yang akan dilakukan pada data ini |
|
|  | imageAreaReplacement | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Informasi penggantian area gambar |
|
|  | imageDetails | java.lang.String | Deskripsi teks gambar, secara default adalah String.Empty |
|

### getRedactionType() {#getRedactionType--}
```
public final int getRedactionType()
```


Mendapatkan tipe data dokumen - teks, metadata, atau anotasi.


**Returns:**
int - Jenis data dokumen - teks, metadata, atau anotasi.

### getActionType() {#getActionType--}
```
public final RedactionActionType getActionType()
```


Mendapatkan operasi redaksi: penggantian, pembersihan, atau penghapusan.


**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) - The redaction operation: replacement, cleanup or deletion.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Mendapatkan teks yang cocok, jika ada ekspresi yang diberikan.


**Returns:**
java.lang.String - Teks yang cocok, jika ada ekspresi yang diberikan.

### getReplacement() {#getReplacement--}
```
public final TextReplacement getReplacement()
```


Mendapatkan informasi penggantian, dapat bernilai null.


**Returns:**
[TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) - The replacement information, can be null.

### getImageAreaReplacement() {#getImageAreaReplacement--}
```
public final RegionReplacementOptions getImageAreaReplacement()
```


Mendapatkan informasi penggantian untuk redaksi area gambar, mengembalikan null untuk redaksi teks.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The replacement information for image area redactions, returns null for textual redactions.

### getDetails() {#getDetails--}
```
public final String getDetails()
```


Mendapatkan informasi detail opsional untuk item yang sedang di-redact.


**Returns:**
java.lang.String - Informasi detail opsional untuk item yang sedang di-redact.

### setDetails(String value) {#setDetails-java.lang.String-}
```
public final void setDetails(String value)
```


Mengatur informasi detail opsional untuk item yang sedang di-redact.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String | Informasi detail opsional untuk item yang sedang di-redact. |
|

