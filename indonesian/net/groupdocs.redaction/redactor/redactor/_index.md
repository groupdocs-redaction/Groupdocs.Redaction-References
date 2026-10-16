---
title: "Redactor"
second_title: "Referensi API GroupDocs.Redaction untuk .NET"
description: "Menginisialisasi sebuah instance baru dari kelas Redactorgroupdocs.redaction/redactor menggunakan jalur file."
type: docs
weight: 10
url: /id/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Menginisialisasi sebuah instance baru dari kelas [`Redactor`](../../redactor) menggunakan jalur file.

```csharp
public Redactor(string filePath)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | String | Jalur ke file |

### Contoh

Contoh berikut menunjukkan cara membuka dokumen untuk redaksi.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // Di sini kita dapat menggunakan instance dokumen untuk melakukan redaksi
}
```

### Lihat Juga

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Menginisialisasi sebuah instance baru dari kelas [`Redactor`](../../redactor) menggunakan aliran.

```csharp
public Redactor(Stream document)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dokumen | Stream | Aliran sumber dokumen |

### Contoh

Contoh berikut menunjukkan cara membuka dokumen dari aliran.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Di sini kita dapat menggunakan instance dokumen untuk melakukan redaksi
    }
}
```

### Lihat Juga

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Menginisialisasi sebuah instance baru dari kelas [`Redactor`](../../redactor) untuk dokumen yang dilindungi kata sandi menggunakan jalurnya.

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | String | Jalur ke file. |
| loadOptions | LoadOptions | Opsi, termasuk kata sandi. |

### Lihat Juga

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Menginisialisasi sebuah instance baru dari kelas [`Redactor`](../../redactor) untuk dokumen yang dilindungi kata sandi menggunakan jalurnya dan pengaturan.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | String | Jalur ke file. |
| loadOptions | LoadOptions | Opsi tergantung file, termasuk kata sandi. |
| settings | RedactorSettings | Pengaturan default untuk proses redaksi. |

### Lihat Juga

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Menginisialisasi sebuah instance baru dari kelas [`Redactor`](../../redactor) untuk dokumen yang dilindungi kata sandi menggunakan aliran.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dokumen | Stream | Aliran input sumber. |
| loadOptions | LoadOptions | Opsi, termasuk kata sandi. |

### Contoh

Contoh berikut menunjukkan cara membuka dokumen yang dilindungi kata sandi menggunakan LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Di sini kita dapat menggunakan instance dokumen untuk melakukan redaksi
}
```

### Lihat Juga

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Menginisialisasi instance baru dari kelas [`Redactor`](../../redactor) untuk dokumen yang dilindungi kata sandi menggunakan stream dan pengaturan.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dokumen | Stream | Aliran input sumber. |
| loadOptions | LoadOptions | Opsi, termasuk kata sandi. |
| settings | RedactorSettings | Pengaturan default untuk proses redaksi. |

### Contoh

Contoh berikut menunjukkan cara membuka dokumen yang dilindungi kata sandi menggunakan LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Di sini kita dapat menggunakan instance dokumen untuk melakukan redaksi
}
```

### Lihat Juga

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
