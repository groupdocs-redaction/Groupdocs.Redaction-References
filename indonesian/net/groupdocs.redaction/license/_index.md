---
title: License
second_title: GroupDocs.Redaction untuk Referensi .NET API
description: Menyediakan metode untuk menerapkan lisensi.
type: docs
weight: 260
url: /id/net/groupdocs.redaction/license/
---
## License class

Menyediakan metode untuk menerapkan lisensi.

```csharp
public class License
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [License](license)() | Menginisialisasi turunan dari kelas Lisensi. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [SetLicense](../../groupdocs.redaction/license/setlicense#setlicense)(Stream) | Menetapkan lisensi GroupDocs.Redaction dari aliran. |
| [SetLicense](../../groupdocs.redaction/license/setlicense#setlicense_1)(string) | Menetapkan lisensi GroupDocs.Redaction dari jalur file. |

### Perkataan

**Belajarlah lagi**

* Lebih lanjut tentang lisensi: [FAQ Lisensi GroupDocs](https://purchase.groupdocs.com/faqs/licensing)
* Lebih lanjut tentang**GroupDocs.Redaction** lisensi: [Batasan Evaluasi dan Perizinan](https://docs.groupdocs.com/redaction/net/evaluation-limitations-and-licensing/)

### Contoh

Contoh berikut menunjukkan cara menyetel lisensi untuk GroupDocs.Redaction.

```csharp
GroupDocs.Redaction.License license = new GroupDocs.Redaction.License();
// sebagai alternatif, Anda dapat menggunakan aliran:
license.SetLicense(licensePath);
```

### Lihat juga

* ruang nama [GroupDocs.Redaction](../../groupdocs.redaction)
* perakitan [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
