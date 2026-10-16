---
title: "ReplacementType"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili jenis penggantian untuk teks yang cocok."
type: docs
weight: 38
url: /id/java/com.groupdocs.redaction.redactions/replacementtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ReplacementType extends Enum<ReplacementType>
```

Mewakili jenis penggantian untuk teks yang cocok.

## Bidang

| Bidang | Deskripsi |
| --- | --- |
|  | [ReplaceString](#ReplaceString) | Mengganti teks yang cocok dengan string lain, misalnya. |
|
|  | [DrawBox](#DrawBox) | Menggambar persegi panjang dengan warna tertentu (Hitam secara default) sebagai pengganti teks yang disensor. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### ReplaceString {#ReplaceString}
```
public static final ReplacementType ReplaceString
```


Mengganti teks yang cocok dengan string lain, misalnya kode pengecualian.


### DrawBox {#DrawBox}
```
public static final ReplacementType DrawBox
```


Menggambar persegi panjang dengan warna tertentu (Hitam secara default) sebagai pengganti teks yang disensor.


### values() {#values--}
```
public static ReplacementType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.ReplacementType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ReplacementType valueOf(String name)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype)
