---
title: "Redaksi"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili kelas abstrak dasar untuk semua tipe redaksi."
type: docs
weight: 13
url: /id/java/com.groupdocs.redaction/redaction/
---
**Inheritance:**
java.lang.Object
```
public abstract class Redaction
```

Mewakili kelas abstrak dasar untuk semua tipe redaksi.

*** ** * ** ***


**Learn more**

* More details about redaction types: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Redaction()](#Redaction--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getDescription()](#getDescription--) | Mengembalikan string yang menggambarkan redaksi dan parameternya. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Menerapkan redaksi pada instance format yang diberikan. |
|
### Redaction() {#Redaction--}
```
public Redaction()
```


### getDescription() {#getDescription--}
```
public String getDescription()
```


Mengembalikan string yang menggambarkan redaksi dan parameternya.


**Returns:**
java.lang.String - Teks, yang berisi nama redaksi dan parameter.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public abstract RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Menerapkan redaksi pada instance format yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Sebuah instance dokumen untuk menerapkan redaksi |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

