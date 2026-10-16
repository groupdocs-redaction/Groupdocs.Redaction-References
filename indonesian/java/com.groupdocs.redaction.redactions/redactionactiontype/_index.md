---
title: "RedactionActionType"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili tindakan yang dapat diambil untuk melakukan redaksi."
type: docs
weight: 37
url: /id/java/com.groupdocs.redaction.redactions/redactionactiontype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionActionType extends Enum<RedactionActionType>
```

Mewakili tindakan yang dapat diambil untuk melakukan redaksi.

## Bidang

| Bidang | Deskripsi |
| --- | --- |
|  | [Replacement](#Replacement) | Teks yang disensor diganti dengan teks lain atau ditutupi dengan blok. |
|
|  | [Cleanup](#Cleanup) | Data dihapus, tetapi objek kosong tetap ada dalam dokumen. |
|
|  | [Deletion](#Deletion) | Data dan struktur terkait dihapus dari dokumen. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Replacement {#Replacement}
```
public static final RedactionActionType Replacement
```


Teks yang disensor diganti dengan teks lain atau ditutupi dengan blok.


### Cleanup {#Cleanup}
```
public static final RedactionActionType Cleanup
```


Data dihapus, tetapi objek kosong tetap ada dalam dokumen.


### Deletion {#Deletion}
```
public static final RedactionActionType Deletion
```


Data dan struktur terkait dihapus dari dokumen.


### values() {#values--}
```
public static RedactionActionType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.RedactionActionType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionActionType valueOf(String name)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype)
