---
title: "WordprocessingSaveOptions"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Opsi penyimpanan pengolah kata."
type: docs
weight: 15
url: /id/java/com.groupdocs.redaction.options/wordprocessingsaveoptions/
---
**Inheritance:**
java.lang.Object
```
public class WordprocessingSaveOptions
```

Opsi penyimpanan pengolah kata.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [WordprocessingSaveOptions()](#WordprocessingSaveOptions--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getOoxmlCompliance()](#getOoxmlCompliance--) | Kepatuhan OOXML yang diterapkan saat menyimpan. |
|
| [setOoxmlCompliance(WordProcessingComplianceLevel value)](#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-) |  |
### WordprocessingSaveOptions() {#WordprocessingSaveOptions--}
```
public WordprocessingSaveOptions()
```


### getOoxmlCompliance() {#getOoxmlCompliance--}
```
public final WordProcessingComplianceLevel getOoxmlCompliance()
```


Kepatuhan OOXML yang diterapkan saat menyimpan.  null  mempertahankan tingkat dokumen asli. Strict tidak dapat disimpan sebagai Ecma secara langsung; gunakan Transitional terlebih dahulu.


**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
### setOoxmlCompliance(WordProcessingComplianceLevel value) {#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-}
```
public final void setOoxmlCompliance(WordProcessingComplianceLevel value)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel) |  |

