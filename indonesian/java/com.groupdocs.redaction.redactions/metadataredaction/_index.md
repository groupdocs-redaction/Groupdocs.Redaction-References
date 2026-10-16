---
title: "MetadataRedaction"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili kelas abstrak dasar untuk redaksi metadata dokumen."
type: docs
weight: 20
url: /id/java/com.groupdocs.redaction.redactions/metadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class MetadataRedaction extends Redaction
```

Mewakili kelas abstrak dasar untuk redaksi metadata dokumen.

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Metadata redactions](../https://docs.groupdocs.com/redaction/java/metadata-redactions/)

<br />


## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getFilter()](#getFilter--) | Mendapatkan filter, yang digunakan untuk memilih semua atau metadata tertentu, misalnya Author atau Company. |
|
|  | [setFilter(int value)](#setFilter-int-) | Menetapkan filter, yang digunakan untuk memilih semua atau metadata tertentu, misalnya Author atau Company. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Menerapkan redaksi pada instance format yang diberikan. |
|
### getFilter() {#getFilter--}
```
public final int getFilter()
```


Mendapatkan filter, yang digunakan untuk memilih semua atau metadata tertentu, misalnya Author atau Company.


**Returns:**
int - Filter, yang digunakan untuk memilih semua atau metadata tertentu, misalnya Author atau Company.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Menetapkan filter, yang digunakan untuk memilih semua atau metadata tertentu, misalnya Author atau Company.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Filter, yang digunakan untuk memilih semua atau metadata tertentu, misalnya Author atau Company. |
|

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

