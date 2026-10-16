---
title: "RedactionResult"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili hasil operasi redaksi."
type: docs
weight: 15
url: /id/java/com.groupdocs.redaction/redactionresult/
---
**Inheritance:**
java.lang.Object
```
public class RedactionResult
```

Mewakili hasil operasi redaksi.

*** ** * ** ***


**Learn more**

* More details about redaction results: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getStatus()](#getStatus--) | Mendapatkan status eksekusi. |
|
|  | [getErrorMessage()](#getErrorMessage--) | Mendapatkan pesan kesalahan untuk diagnostik. |
|
|  | [skipped(String description)](#skipped-java.lang.String-) | Menginisialisasi instance baru dari kelas RedactionResult dengan status Skipped. |
|
|  | [partial(String description)](#partial-java.lang.String-) | Menginisialisasi instance baru dari kelas RedactionResult dengan status PartiallyApplied. |
|
|  | [failed(String description)](#failed-java.lang.String-) | Menginisialisasi instance baru dari kelas RedactionResult dengan status Failed. |
|
|  | [successful()](#successful--) | Menginisialisasi instance baru dari kelas RedactionResult dengan status Applied (berhasil). |
|
### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Mendapatkan status eksekusi.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The execution status.

### getErrorMessage() {#getErrorMessage--}
```
public final String getErrorMessage()
```


Mendapatkan pesan kesalahan untuk diagnostik.


**Returns:**
java.lang.String - Pesan kesalahan untuk diagnostik.

### skipped(String description) {#skipped-java.lang.String-}
```
public static RedactionResult skipped(String description)
```


Menginisialisasi instance baru dari kelas RedactionResult dengan status Skipped.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | deskripsi | java.lang.String | Alasan mengapa operasi dilewati |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Sskipped redaction result

### partial(String description) {#partial-java.lang.String-}
```
public static RedactionResult partial(String description)
```


Menginisialisasi instance baru dari kelas RedactionResult dengan status PartiallyApplied.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | deskripsi | java.lang.String | Alasan mengapa operasi tidak sepenuhnya diterapkan |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Partially applied redaction result

### failed(String description) {#failed-java.lang.String-}
```
public static RedactionResult failed(String description)
```


Menginisialisasi instance baru dari kelas RedactionResult dengan status Failed.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | deskripsi | java.lang.String | Detail kegagalan atau pengecualian |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Failed redaction result

### successful() {#successful--}
```
public static RedactionResult successful()
```


Menginisialisasi instance baru dari kelas RedactionResult dengan status Applied (berhasil).


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Successful redaction result

