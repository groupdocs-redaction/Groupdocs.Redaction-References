---
title: "RedactorLogEntry"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili hasil penerapan redaksi."
type: docs
weight: 18
url: /id/java/com.groupdocs.redaction/redactorlogentry/
---
**Inheritance:**
java.lang.Object
```
public class RedactorLogEntry
```

Mewakili hasil penerapan redaksi.

*** ** * ** ***


**Learn more**

* More details about redaction log entries: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [RedactorLogEntry(Redaction redaction, RedactionResult result)](#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-) | Menginisialisasi instance baru dari kelas RedactorLogEntry untuk redaksi. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getResult()](#getResult--) | Mendapatkan hasil, yang dikembalikan oleh |
GroupDocs.Redaction.Integration.DocumentFormatInstance
.
|
|  | [getRedaction()](#getRedaction--) | Mendapatkan referensi ke redaksi dan opsi-opsinya. |
|
### RedactorLogEntry(Redaction redaction, RedactionResult result) {#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-}
```
public RedactorLogEntry(Redaction redaction, RedactionResult result)
```


Menginisialisasi instance baru dari kelas RedactorLogEntry untuk redaksi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Referensi ke redaksi |
|
|  | result | [RedactionResult](../../com.groupdocs.redaction/redactionresult) | Hasil redaksi, dilaporkan oleh penangan format |
|

### getResult() {#getResult--}
```
public final RedactionResult getResult()
```


Mendapatkan hasil, yang dikembalikan oleh
GroupDocs.Redaction.Integration.DocumentFormatInstance
.


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - The result, returned by  GroupDocs.Redaction.Integration.DocumentFormatInstance .

### getRedaction() {#getRedaction--}
```
public final Redaction getRedaction()
```


Mendapatkan referensi ke redaksi dan opsi-opsinya.


**Returns:**
[Redaction](../../com.groupdocs.redaction/redaction) - The reference to redaction and its options.

