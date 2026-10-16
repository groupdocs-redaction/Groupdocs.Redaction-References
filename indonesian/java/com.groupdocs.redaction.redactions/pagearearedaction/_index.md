---
title: "PageAreaRedaction"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili redaksi teks kompleks yang memengaruhi gambar teks dan anotasi dalam area halaman."
type: docs
weight: 23
url: /id/java/com.groupdocs.redaction.redactions/pagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction), [com.groupdocs.redaction.redactions.RegexRedaction](../../com.groupdocs.redaction.redactions/regexredaction)
```
public class PageAreaRedaction extends RegexRedaction
```

Mewakili redaksi tekstual kompleks yang memengaruhi teks, gambar, dan anotasi dalam area halaman.

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](../https://docs.groupdocs.com/redaction/java/use-page-area-redaction/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [PageAreaRedaction(Pattern regex, ReplacementOptions options)](#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Menginisialisasi instance baru dari kelas PageAreaRedaction. |
|
|  | [PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions)](#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Menginisialisasi instance baru dari kelas PageAreaRedaction. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getImageOptions()](#getImageOptions--) | Mendapatkan |
RegionReplacementOptions
opsi dengan parameter warna dan area.
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Menerapkan redaksi pada instance format yang diberikan. |
|
### PageAreaRedaction(Pattern regex, ReplacementOptions options) {#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public PageAreaRedaction(Pattern regex, ReplacementOptions options)
```


Menginisialisasi instance baru dari kelas PageAreaRedaction.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Ekspresi reguler untuk mencari dan mengganti |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Opsi penggantian (teks, warna) |
|

### PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions) {#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions)
```


Menginisialisasi instance baru dari kelas PageAreaRedaction.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Ekspresi reguler untuk mencari dan mengganti |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Opsi penggantian (teks, warna) |
|
|  | imageOptions | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Opsi penggantian (area gambar) |
|

### getImageOptions() {#getImageOptions--}
```
public final RegionReplacementOptions getImageOptions()
```


Mendapatkan
RegionReplacementOptions
opsi dengan parameter warna dan area.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Menerapkan redaksi pada instance format yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Sebuah instance dokumen untuk menerapkan redaksi |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

