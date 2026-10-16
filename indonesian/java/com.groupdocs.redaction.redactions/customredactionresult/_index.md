---
title: "CustomRedactionResult"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili hasil yang dikembalikan oleh ."
type: docs
weight: 14
url: /id/java/com.groupdocs.redaction.redactions/customredactionresult/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionResult
```

Mewakili hasil yang dikembalikan oleh [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [CustomRedactionResult()](#CustomRedactionResult--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getApply()](#getApply--) | Mendapatkan nilai yang menunjukkan apakah penggantian harus diterapkan. |
|
|  | [setApply(boolean value)](#setApply-boolean-) | Mengatur nilai yang menunjukkan apakah penggantian harus diterapkan. |
|
|  | [getText()](#getText--) | Mendapatkan teks pengganti yang digunakan ketika #getApply().getApply() adalah |
true
.
|
|  | [setText(String value)](#setText-java.lang.String-) | Mengatur teks pengganti yang digunakan ketika #getApply().getApply() adalah |
true
.
|
### CustomRedactionResult() {#CustomRedactionResult--}
```
public CustomRedactionResult()
```


### getApply() {#getApply--}
```
public final boolean getApply()
```


Mendapatkan nilai yang menunjukkan apakah penggantian harus diterapkan.


**Returns:**
boolean -  true  untuk mengganti teks yang cocok dengan #getText().getText(); jika tidak,  false .

### setApply(boolean value) {#setApply-boolean-}
```
public final void setApply(boolean value)
```


Mengatur nilai yang menunjukkan apakah penggantian harus diterapkan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | true  untuk menerapkan penggantian; jika tidak,  false . |
|

### getText() {#getText--}
```
public final String getText()
```


Mendapatkan teks pengganti yang digunakan ketika #getApply().getApply() adalah
true
.


**Returns:**
java.lang.String - Teks pengganti.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Mengatur teks pengganti yang digunakan ketika #getApply().getApply() adalah
true
.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String | Teks pengganti. |
|

