---
title: Redactor
second_title: GroupDocs.Redaction untuk Referensi .NET API
description: Menginisialisasi instance baru dariRedactorgroupdocs.redaction/redactor kelas menggunakan file path.
type: docs
weight: 10
url: /id/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Menginisialisasi instance baru dari[`Redactor`](../../redactor) kelas menggunakan file path.

```csharp
public Redactor(string filePath)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| filePath | String | Jalur ke file |

### Contoh

Contoh berikut menunjukkan cara membuka dokumen untuk redaksi.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // Di sini kita bisa menggunakan document instance untuk melakukan redaksi
}
```

### Lihat juga

* class [Redactor](../../redactor)
* ruang nama [GroupDocs.Redaction](../../redactor)
* perakitan [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Menginisialisasi instance baru dari[`Redactor`](../../redactor) kelas menggunakan stream.

```csharp
public Redactor(Stream document)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| document | Stream | Aliran sumber dokumen |

### Contoh

Contoh berikut menunjukkan cara membuka dokumen dari stream.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Di sini kita bisa menggunakan document instance untuk melakukan redaksi
    }
}
```

### Lihat juga

* class [Redactor](../../redactor)
* ruang nama [GroupDocs.Redaction](../../redactor)
* perakitan [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Menginisialisasi instance baru dari[`Redactor`](../../redactor) kelas untuk dokumen yang dilindungi kata sandi menggunakan jalurnya.

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| filePath | String | Jalur ke file. |
| loadOptions | LoadOptions | Opsi, termasuk kata sandi. |

### Lihat juga

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* ruang nama [GroupDocs.Redaction](../../redactor)
* perakitan [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Menginisialisasi instance baru dari[`Redactor`](../../redactor) kelas untuk dokumen yang dilindungi kata sandi menggunakan jalur dan pengaturannya.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| filePath | String | Jalur ke file. |
| loadOptions | LoadOptions | Opsi yang bergantung pada file, termasuk kata sandi. |
| settings | RedactorSettings | Pengaturan default untuk proses redaksi. |

### Lihat juga

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* ruang nama [GroupDocs.Redaction](../../redactor)
* perakitan [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Menginisialisasi instance baru dari[`Redactor`](../../redactor) kelas untuk dokumen yang dilindungi kata sandi menggunakan stream.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| document | Stream | Aliran masukan sumber. |
| loadOptions | LoadOptions | Opsi, termasuk kata sandi. |

### Contoh

Contoh berikut menunjukkan cara membuka dokumen yang dilindungi kata sandi menggunakan LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Di sini kita bisa menggunakan document instance untuk melakukan redaksi
}
```

### Lihat juga

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* ruang nama [GroupDocs.Redaction](../../redactor)
* perakitan [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Menginisialisasi instance baru dari[`Redactor`](../../redactor)kelas untuk dokumen yang dilindungi kata sandi menggunakan aliran dan pengaturan.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| document | Stream | Aliran masukan sumber. |
| loadOptions | LoadOptions | Opsi, termasuk kata sandi. |
| settings | RedactorSettings | Pengaturan default untuk proses redaksi. |

### Contoh

Contoh berikut menunjukkan cara membuka dokumen yang dilindungi kata sandi menggunakan LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Di sini kita bisa menggunakan document instance untuk melakukan redaksi
}
```

### Lihat juga

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* ruang nama [GroupDocs.Redaction](../../redactor)
* perakitan [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
