---
title: "ReplacementOptions"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili opsi untuk penggantian teks yang cocok."
type: docs
weight: 31
url: /id/java/com.groupdocs.redaction.redactions/replacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class ReplacementOptions
```

Mewakili opsi untuk penggantian teks yang cocok.

*** ** * ** ***


**Learn more**

* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [ReplacementOptions(String replacement)](#ReplacementOptions-java.lang.String-) | Menginisialisasi instance baru dari kelas ReplacementOptions dengan teks pengganti sebagai opsi. |
|
|  | [ReplacementOptions(Color color)](#ReplacementOptions-java.awt.Color-) | Menginisialisasi instance baru dari kelas ReplacementOptions dengan persegi panjang berwarna sebagai opsi. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getActionType()](#getActionType--) | Mendapatkan tindakan penggantian: menggambar kotak atau mengganti teks. |
|
|  | [getReplacement()](#getReplacement--) | Mendapatkan nilai penggantian teks. |
|
|  | [setReplacement(String value)](#setReplacement-java.lang.String-) | Mengatur nilai penggantian teks. |
|
|  | [getBoxColor()](#getBoxColor--) | Mendapatkan warna untuk sebuah |
ReplacementType.DrawBox
opsi (diabaikan jika tidak).
|
|  | [setBoxColor(Color value)](#setBoxColor-java.awt.Color-) | Mengatur warna untuk |
ReplacementType.DrawBox
opsi (diabaikan jika tidak).
|
|  | [getFilters()](#getFilters--) | Mendapatkan array filter untuk diterapkan dengan redaksi ini. |
|
|  | [setFilters(RedactionFilter[] value)](#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---) | Mengatur array filter untuk diterapkan dengan redaksi ini. |
|
|  | [getCustomRedaction()](#getCustomRedaction--) | Mendapatkan penangan redaksi khusus. |
|
|  | [setCustomRedaction(ICustomRedactionHandler value)](#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-) | Mengatur penangan redaksi khusus. |
|
| [fromFilters(RedactionFilter[] filters)](#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---) |  |
### ReplacementOptions(String replacement) {#ReplacementOptions-java.lang.String-}
```
public ReplacementOptions(String replacement)
```


Menginisialisasi instance baru dari kelas ReplacementOptions dengan teks pengganti sebagai opsi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | penggantian | java.lang.String | Penggantian tekstual |
|

### ReplacementOptions(Color color) {#ReplacementOptions-java.awt.Color-}
```
public ReplacementOptions(Color color)
```


Menginisialisasi instance baru dari kelas ReplacementOptions dengan persegi panjang berwarna sebagai opsi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | warna | java.awt.Color | Warna persegi panjang |
|

### getActionType() {#getActionType--}
```
public final ReplacementType getActionType()
```


Mendapatkan tindakan penggantian: menggambar kotak atau mengganti teks.


**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype) - The replacement action: draw box or replace text.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Mendapatkan nilai penggantian teks.


**Returns:**
java.lang.String - Nilai penggantian tekstual.

### setReplacement(String value) {#setReplacement-java.lang.String-}
```
public final void setReplacement(String value)
```


Mengatur nilai penggantian teks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String | Nilai penggantian tekstual. |
|

### getBoxColor() {#getBoxColor--}
```
public final Color getBoxColor()
```


Mendapatkan warna untuk sebuah
ReplacementType.DrawBox
opsi (diabaikan jika tidak).


**Returns:**
java.awt.Color - Warna untuk opsi  ReplacementType.DrawBox  (diabaikan jika tidak).

### setBoxColor(Color value) {#setBoxColor-java.awt.Color-}
```
public final void setBoxColor(Color value)
```


Mengatur warna untuk
ReplacementType.DrawBox
opsi (diabaikan jika tidak).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.awt.Color | Warna untuk opsi  ReplacementType.DrawBox  (diabaikan jika tidak). |
|

### getFilters() {#getFilters--}
```
public final RedactionFilter[] getFilters()
```


Mendapatkan array filter untuk diterapkan dengan redaksi ini.


**Returns:**
com.groupdocs.redaction.redactions.RedactionFilter[] - Array filter untuk diterapkan dengan redaksi ini.

### setFilters(RedactionFilter[] value) {#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public final void setFilters(RedactionFilter[] value)
```


Mengatur array filter untuk diterapkan dengan redaksi ini.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) | Array filter untuk diterapkan dengan redaksi ini. |
|

### getCustomRedaction() {#getCustomRedaction--}
```
public final ICustomRedactionHandler getCustomRedaction()
```


Mendapatkan penangan redaksi khusus. Hanya didukung untuk PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Returns:**
[ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) - An instance of [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler), or  null  if not set.

### setCustomRedaction(ICustomRedactionHandler value) {#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-}
```
public final void setCustomRedaction(ICustomRedactionHandler value)
```


Mengatur penangan redaksi khusus. Hanya didukung untuk PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) | Sebuah instance dari [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler). |
|

### fromFilters(RedactionFilter[] filters) {#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public static ReplacementOptions fromFilters(RedactionFilter[] filters)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filters | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) |  |

**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions)
