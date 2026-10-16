---
title: "RedactionPolicy"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili kebijakan sanitasi yang berisi sekumpulan redaksi spesifik untuk diterapkan."
type: docs
weight: 14
url: /id/java/com.groupdocs.redaction/redactionpolicy/
---
**Inheritance:**
java.lang.Object
```
public class RedactionPolicy
```

Mewakili kebijakan sanitasi, yang berisi sekumpulan redaksi spesifik untuk diterapkan.

*** ** * ** ***


**Learn more**

* More details about policies: [Use of redaction policies](../https://docs.groupdocs.com/redaction/java/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [RedactionPolicy()](#RedactionPolicy--) | Membuat instance baru dari kebijakan Redaction. |
|
|  | [RedactionPolicy(Redaction[] redactions)](#RedactionPolicy-com.groupdocs.redaction.Redaction---) | Membuat instance baru dari kebijakan Redaction dengan daftar redaksi spesifik. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getRedactions()](#getRedactions--) | Mendapatkan array yang sepenuhnya dikonfigurasi |
Redaksi
-derived classes.
|
|  | [load(String filePath)](#load-java.lang.String-) | Memuat instance dari |
RedactionPolicy
dari jalur file.
|
|  | [load(InputStream input)](#load-java.io.InputStream-) | Memuat instance dari |
RedactionPolicy
dari aliran.
|
|  | [save(String filePath)](#save-java.lang.String-) | Menyimpan kebijakan redaksi ke file. |
|
|  | [save(OutputStream output)](#save-java.io.OutputStream-) | Menyimpan kebijakan redaksi ke aliran. |
|
### RedactionPolicy() {#RedactionPolicy--}
```
public RedactionPolicy()
```


Membuat instance baru dari kebijakan Redaction.


### RedactionPolicy(Redaction[] redactions) {#RedactionPolicy-com.groupdocs.redaction.Redaction---}
```
public RedactionPolicy(Redaction[] redactions)
```


Membuat instance baru dari kebijakan Redaction dengan daftar redaksi spesifik.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | Array redaksi untuk kebijakan |
|

### getRedactions() {#getRedactions--}
```
public final Redaction[] getRedactions()
```


Mendapatkan array yang sepenuhnya dikonfigurasi
Redaksi
-derived classes.


**Returns:**
com.groupdocs.redaction.Redaction[] - Array dari kelas turunan Redaction yang sepenuhnya dikonfigurasi.

### load(String filePath) {#load-java.lang.String-}
```
public static RedactionPolicy load(String filePath)
```


Memuat instance dari
RedactionPolicy
dari jalur file.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Jalur ke file XML |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### load(InputStream input) {#load-java.io.InputStream-}
```
public static RedactionPolicy load(InputStream input)
```


Memuat instance dari
RedactionPolicy
dari aliran.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | masukan | java.io.InputStream | Aliran yang berisi konfigurasi XML |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### save(String filePath) {#save-java.lang.String-}
```
public final void save(String filePath)
```


Menyimpan kebijakan redaksi ke file.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Jalur ke file. |
|

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Menyimpan kebijakan redaksi ke aliran.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | keluaran | java.io.OutputStream | Aliran target untuk menyimpan kebijakan |
|

