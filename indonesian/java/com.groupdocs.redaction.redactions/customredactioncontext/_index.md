---
title: "CustomRedactionContext"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Menyediakan data masukan untuk ."
type: docs
weight: 13
url: /id/java/com.groupdocs.redaction.redactions/customredactioncontext/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionContext
```

Menyediakan data masukan untuk [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [CustomRedactionContext()](#CustomRedactionContext--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Mendapatkan nomor halaman dari fragmen yang cocok, bila tersedia. |
|
|  | [setPageNumber(int value)](#setPageNumber-int-) | Mengatur nomor halaman dari fragmen yang cocok. |
|
|  | [getText()](#getText--) | Mendapatkan teks yang cocok untuk redaksi. |
|
|  | [setText(String value)](#setText-java.lang.String-) | Mengatur teks yang cocok untuk redaksi. |
|
### CustomRedactionContext() {#CustomRedactionContext--}
```
public CustomRedactionContext()
```


### getPageNumber() {#getPageNumber--}
```
public final int getPageNumber()
```


Mendapatkan nomor halaman dari fragmen yang cocok, bila tersedia.


**Returns:**
int - Nomor halaman, atau nilai spesifik format jika halaman tidak diketahui.

### setPageNumber(int value) {#setPageNumber-int-}
```
public final void setPageNumber(int value)
```


Mengatur nomor halaman dari fragmen yang cocok.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Nomor halaman. |
|

### getText() {#getText--}
```
public final String getText()
```


Mendapatkan teks yang cocok untuk redaksi.


**Returns:**
java.lang.String - Teks yang cocok.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Mengatur teks yang cocok untuk redaksi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String | Teks yang cocok. |
|

