---
title: "ExactPhraseRedaction"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili penyensoran teks yang menggantikan frasa tepat dalam teks dokumen tanpa memperhatikan huruf besar/kecil secara default."
type: docs
weight: 17
url: /id/java/com.groupdocs.redaction.redactions/exactphraseredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class ExactPhraseRedaction extends TextRedaction
```

Mewakili redaksi teks yang mengganti frasa tepat dalam teks dokumen, tidak sensitif huruf besar/kecil secara default.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />

Contoh berikut menunjukkan melakukan pencarian frasa yang sensitif huruf besar/kecil dan penggantiannya.

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
   // By default, the second parameter, isCaseSensitive = false;
   doc.apply(new ExactPhraseRedaction("John Doe", true, new ReplacementOptions("[personal]")));
   doc.save();
 }
 
``` 
````

The following example demonstrates replacing phrase (case insensitive) with solid red rectangle.

````

try (Redactor redactor = new Redactor("C:\\sample.pdf"))
{
// Secara default, isCaseSensitive = false;
doc.apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(System.Drawing.Color.Red)));
doc.save();
}
 
``` 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Menginisialisasi instance baru dari kelas ExactPhraseRedaction dalam mode tidak sensitif huruf besar/kecil. |
|
|  | [ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-) | Menginisialisasi instance baru dari kelas ExactPhraseRedaction. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getSearchPhrase()](#getSearchPhrase--) | Mendapatkan string untuk mencari dan mengganti. |
|
|  | [isCaseSensitive()](#isCaseSensitive--) | Mendapatkan nilai yang menunjukkan apakah pencarian bersifat peka huruf besar/kecil atau tidak. |
|
|  | [isRightToLeft()](#isRightToLeft--) | Mendapatkan nilai yang menunjukkan apakah teks ini dari kanan ke kiri atau tidak, false secara default. |
|
|  | [setRightToLeft(boolean value)](#setRightToLeft-boolean-) | Mengatur nilai yang menunjukkan apakah teks ini dari kanan ke kiri atau tidak, false secara default. |
|
|  | [getDescription()](#getDescription--) | Mengembalikan string yang menggambarkan redaksi dan parameternya. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Menerapkan redaksi pada instance format yang diberikan. |
|
### ExactPhraseRedaction(String searchPhrase, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)
```


Menginisialisasi instance baru dari kelas ExactPhraseRedaction dalam mode tidak sensitif huruf besar/kecil.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | String untuk mencari dan mengganti |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Opsi penggantian (teks, warna) |
|

### ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)
```


Menginisialisasi instance baru dari kelas ExactPhraseRedaction.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | String untuk mencari dan mengganti |
|
|  | isCaseSensitive | boolean | True jika pencarian peka huruf besar/kecil diperlukan |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Opsi penggantian (teks, warna) |
|

### getSearchPhrase() {#getSearchPhrase--}
```
public final String getSearchPhrase()
```


Mendapatkan string untuk mencari dan mengganti.


**Returns:**
java.lang.String - String untuk mencari dan mengganti.

### isCaseSensitive() {#isCaseSensitive--}
```
public final boolean isCaseSensitive()
```


Mendapatkan nilai yang menunjukkan apakah pencarian bersifat peka huruf besar/kecil atau tidak.


**Returns:**
boolean - Nilai yang menunjukkan apakah pencarian peka huruf besar/kecil atau tidak.

### isRightToLeft() {#isRightToLeft--}
```
public final boolean isRightToLeft()
```


Mendapatkan nilai yang menunjukkan apakah teks ini dari kanan ke kiri atau tidak, false secara default.


**Returns:**
boolean - Nilai yang menunjukkan apakah teks ini dari kanan ke kiri atau tidak, false secara default.

### setRightToLeft(boolean value) {#setRightToLeft-boolean-}
```
public final void setRightToLeft(boolean value)
```


Mengatur nilai yang menunjukkan apakah teks ini dari kanan ke kiri atau tidak, false secara default.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah teks ini dari kanan ke kiri atau tidak, false secara default. |
|

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

