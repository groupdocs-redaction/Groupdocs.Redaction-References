---
title: "RegexRedaction"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili redaksi teks yang mencari dan mengganti teks dalam dokumen dengan mencocokkan ekspresi reguler yang diberikan."
type: docs
weight: 28
url: /id/java/com.groupdocs.redaction.redactions/regexredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class RegexRedaction extends TextRedaction
```

Mewakili redaksi teks yang mencari dan mengganti teks dalam dokumen dengan mencocokkan ekspresi reguler yang diberikan.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [RegexRedaction(String pattern, ReplacementOptions options)](#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Menginisialisasi sebuah instance baru dari kelas RegexRedaction. |
|
|  | [RegexRedaction(Pattern regex, ReplacementOptions options)](#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Menginisialisasi sebuah instance baru dari kelas RegexRedaction. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getRegularExpression()](#getRegularExpression--) | Mendapatkan ekspresi reguler untuk dicocokkan. |
|
|  | [getDescription()](#getDescription--) | Mengembalikan string yang menggambarkan redaksi dan parameternya. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Menerapkan redaksi pada instance format yang diberikan. |
|
### RegexRedaction(String pattern, ReplacementOptions options) {#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(String pattern, ReplacementOptions options)
```


Menginisialisasi sebuah instance baru dari kelas RegexRedaction.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pola | java.lang.String | Ekspresi reguler untuk mencari dan mengganti |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Opsi penggantian (teks, warna) |
|

### RegexRedaction(Pattern regex, ReplacementOptions options) {#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(Pattern regex, ReplacementOptions options)
```


Menginisialisasi sebuah instance baru dari kelas RegexRedaction.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Ekspresi reguler untuk mencari dan mengganti |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Opsi penggantian (teks, warna) |
|

### getRegularExpression() {#getRegularExpression--}
```
public final Pattern getRegularExpression()
```


Mendapatkan ekspresi reguler untuk dicocokkan.


**Returns:**
java.util.regex.Pattern - Ekspresi reguler untuk dicocokkan.

### getDescription() {#getDescription--}
```
public String getDescription()
```


Mengembalikan string yang menggambarkan redaksi dan parameternya.


**Returns:**
java.lang.String - Teks, yang berisi nama redaksi dan parameter.

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

