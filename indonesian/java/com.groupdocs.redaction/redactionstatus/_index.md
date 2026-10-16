---
title: "RedactionStatus"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili status penyelesaian redaksi."
type: docs
weight: 20
url: /id/java/com.groupdocs.redaction/redactionstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionStatus extends Enum<RedactionStatus>
```

Mewakili status penyelesaian redaksi.

## Bidang

| Bidang | Deskripsi |
| --- | --- |
|  | [Applied](#Applied) | Redaksi berhasil diterapkan sepenuhnya dan sukses. |
|
|  | [PartiallyApplied](#PartiallyApplied) | Redaksi hanya diterapkan pada sebagian dari kecocokannya. |
|
|  | [Skipped](#Skipped) | Redaksi dilewati (tidak diterapkan). |
|
|  | [Failed](#Failed) | Redaksi gagal dengan pengecualian. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Applied {#Applied}
```
public static final RedactionStatus Applied
```


Redaksi berhasil diterapkan sepenuhnya dan sukses.


### PartiallyApplied {#PartiallyApplied}
```
public static final RedactionStatus PartiallyApplied
```


Redaksi hanya diterapkan pada sebagian dari kecocokannya.


### Skipped {#Skipped}
```
public static final RedactionStatus Skipped
```


Redaksi dilewati (tidak diterapkan).


### Failed {#Failed}
```
public static final RedactionStatus Failed
```


Redaksi gagal dengan pengecualian.


### values() {#values--}
```
public static RedactionStatus[] values()
```




**Returns:**
com.groupdocs.redaction.RedactionStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionStatus valueOf(String name)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus)
