---
title: "Redactor"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili kelas utama yang mengendalikan proses redaksi dokumen yang memungkinkan membuka, meredaksi, dan menyimpan dokumen."
type: docs
weight: 16
url: /id/java/com.groupdocs.redaction/redactor/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable, [com.groupdocs.redaction.integration.IPreviewable](../../com.groupdocs.redaction.integration/ipreviewable)
```
public final class Redactor implements Closeable, IPreviewable
```

Mewakili kelas utama yang mengontrol proses redaksi dokumen, memungkinkan membuka, meredaksi, dan menyimpan dokumen.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [Redactor(String filePath)](#Redactor-java.lang.String-) | Menginisialisasi sebuah instansi baru dari |
Redactor
kelas menggunakan jalur file.
|
|  | [Redactor(InputStream document)](#Redactor-java.io.InputStream-) | Menginisialisasi sebuah instansi baru dari |
Redactor
kelas menggunakan aliran.
|
|  | [Redactor(String filePath, LoadOptions loadOptions)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-) | Menginisialisasi sebuah instansi baru dari |
Redactor
kelas untuk dokumen yang dilindungi kata sandi menggunakan jalurnya.
|
|  | [Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Menginisialisasi sebuah instansi baru dari |
Redactor
kelas untuk dokumen yang dilindungi kata sandi menggunakan jalurnya dan pengaturan.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-) | Menginisialisasi sebuah instansi baru dari |
Redactor
kelas untuk dokumen yang dilindungi kata sandi menggunakan aliran.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Menginisialisasi sebuah instansi baru dari |
Redactor
kelas untuk dokumen yang dilindungi kata sandi menggunakan aliran dan pengaturan.
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [close()](#close--) | Melepaskan sumber daya. |
|
|  | [apply(Redaction redaction)](#apply-com.groupdocs.redaction.Redaction-) | Menerapkan redaksi pada dokumen. |
|
|  | [apply(Redaction[] redactions)](#apply-com.groupdocs.redaction.Redaction---) | Menerapkan sekumpulan redaksi pada dokumen. |
|
|  | [apply(RedactionPolicy policy)](#apply-com.groupdocs.redaction.RedactionPolicy-) | Menerapkan kebijakan redaksi pada dokumen. |
|
|  | [save()](#save--) | Menyimpan dokumen ke file dengan opsi berikut: AddSuffix = true, RasterizeToPDF = true. |
|
|  | [save(SaveOptions saveOptions)](#save-com.groupdocs.redaction.options.SaveOptions-) | Menyimpan dokumen ke file. |
|
|  | [save(OutputStream document)](#save-java.io.OutputStream-) | Menyimpan dokumen ke aliran. |
|
|  | [save(OutputStream document, SaveOptions saveOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-) | Menyimpan dokumen ke aliran. |
|
|  | [save(OutputStream document, RasterizationOptions rasterizationOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-) | Menyimpan dokumen ke aliran, termasuk lokasi khusus. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.redaction.options.PreviewOptions-) | Menghasilkan gambar pratinjau halaman tertentu dalam format gambar yang diberikan. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | Mendapatkan informasi umum tentang dokumen - ukuran, jumlah halaman, dll. |
|
### Redactor(String filePath) {#Redactor-java.lang.String-}
```
public Redactor(String filePath)
```


Menginisialisasi sebuah instansi baru dari
Redactor
kelas menggunakan jalur file.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Jalur ke file |


Contoh berikut menunjukkan cara membuka dokumen untuk redaksi.

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
     // Here we can use document instance to perform redactions
 }
 
``` 
````

 |

### Redactor(InputStream document) {#Redactor-java.io.InputStream-}
```
public Redactor(InputStream document)
```


Initializes a new instance of 
Redactor
 class using stream.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.InputStream | Source stream of the document


The following example demonstrates how to open a document from stream.

````

try (InputStream stream = new FileInputStream("C:\\sample.pdf"))
{
try (Redactor redactor = new Redactor(stream))
{
// Di sini kita dapat menggunakan instance dokumen untuk melakukan redaksi
}
}
 
``` 
````

|

### Redactor(String filePath, LoadOptions loadOptions) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(String filePath, LoadOptions loadOptions)
```


Menginisialisasi sebuah instansi baru dari
Redactor
kelas untuk dokumen yang dilindungi kata sandi menggunakan jalurnya.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Jalur ke file. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Opsi, termasuk kata sandi. |
|

### Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)
```


Menginisialisasi sebuah instansi baru dari
Redactor
kelas untuk dokumen yang dilindungi kata sandi menggunakan jalurnya dan pengaturan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Jalur ke file. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Opsi yang bergantung pada file, termasuk kata sandi. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Pengaturan default untuk proses redaksi. |
|

### Redactor(InputStream document, LoadOptions loadOptions) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(InputStream document, LoadOptions loadOptions)
```


Menginisialisasi sebuah instansi baru dari
Redactor
kelas untuk dokumen yang dilindungi kata sandi menggunakan aliran.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | dokumen | java.io.InputStream | Aliran input sumber. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Opsi, termasuk kata sandi. |
|

### Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)
```


Menginisialisasi sebuah instansi baru dari
Redactor
kelas untuk dokumen yang dilindungi kata sandi menggunakan aliran dan pengaturan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | dokumen | java.io.InputStream | Aliran input sumber. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Opsi, termasuk kata sandi. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Pengaturan default untuk proses redaksi. |
|

### close() {#close--}
```
public final void close()
```


Melepaskan sumber daya.


### apply(Redaction redaction) {#apply-com.groupdocs.redaction.Redaction-}
```
public final RedactorChangeLog apply(Redaction redaction)
```


Menerapkan redaksi pada dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Sebuah instance dari  Redaction  untuk diterapkan |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(Redaction[] redactions) {#apply-com.groupdocs.redaction.Redaction---}
```
public final RedactorChangeLog apply(Redaction[] redactions)
```


Menerapkan sekumpulan redaksi pada dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | Sebuah array dari redaksi untuk diterapkan |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(RedactionPolicy policy) {#apply-com.groupdocs.redaction.RedactionPolicy-}
```
public final RedactorChangeLog apply(RedactionPolicy policy)
```


Menerapkan kebijakan redaksi pada dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | policy | [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) | Kebijakan redaksi |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### save() {#save--}
```
public final String save()
```


Menyimpan dokumen ke file dengan opsi berikut: AddSuffix = true, RasterizeToPDF = true.


**Returns:**
java.lang.String - Jalur ke dokumen yang disensor

### save(SaveOptions saveOptions) {#save-com.groupdocs.redaction.options.SaveOptions-}
```
public final String save(SaveOptions saveOptions)
```


Menyimpan dokumen ke file.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Opsi untuk menambahkan akhiran atau meraster |
|

**Returns:**
java.lang.String - Jalur ke dokumen yang disensor

### save(OutputStream document) {#save-java.io.OutputStream-}
```
public final void save(OutputStream document)
```


Menyimpan dokumen ke aliran.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | dokumen | java.io.OutputStream | Aliran target |
|

### save(OutputStream document, SaveOptions saveOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-}
```
public final void save(OutputStream document, SaveOptions saveOptions)
```


Menyimpan dokumen ke aliran.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | dokumen | java.io.OutputStream | Aliran target |
|
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Opsi penyimpanan |
|

### save(OutputStream document, RasterizationOptions rasterizationOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-}
```
public final void save(OutputStream document, RasterizationOptions rasterizationOptions)
```


Menyimpan dokumen ke aliran, termasuk lokasi khusus.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | dokumen | java.io.OutputStream | Aliran target |
|
|  | rasterizationOptions | [RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) | Opsi untuk meraster atau tidak dan untuk menentukan halaman untuk rasterisasi |
|

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.redaction.options.PreviewOptions-}
```
public final void generatePreview(PreviewOptions previewOptions)
```


Menghasilkan gambar pratinjau halaman tertentu dalam format gambar yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.redaction.options/previewoptions) | Properti gambar dan pengaturan rentang halaman |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public final IDocumentInfo getDocumentInfo()
```


Mendapatkan informasi umum tentang dokumen - ukuran, jumlah halaman, dll.


**Returns:**
[IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo) - An instance of IDocumentInfo

