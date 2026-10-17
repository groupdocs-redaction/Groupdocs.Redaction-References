---
title: "metode save"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menyimpan dokumen ke file dengan opsi berikut: AddSuffix = True, RasterizeToPDF = True."
type: docs
url: /id/python-net/groupdocs.redaction/redactor/save/
is_root: false
weight: 1080
---


## save

Menyimpan dokumen ke file dengan opsi berikut: AddSuffix = True, RasterizeToPDF = True.

```python
def save(self):
    ...
```

**Returns:** str: Path to redacted document.

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("document.docx") as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    options = SaveOptions()
    options.add_suffix = True
    options.rasterize_to_pdf = True
    result_path = redactor.save(options)
    print(f"Saved to {result_path}")
```

## save {#save_options}

Menyimpan dokumen ke file.

```python
def save(self, save_options):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| save_options | `SaveOptions` | Opsi untuk menambahkan akhiran atau meraster. |

**Returns:** Path to redacted document.

### Contoh

```python
from datetime import datetime
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions


def save_in_original_format():
    # Tentukan opsi redaksi
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Muat dokumen yang akan direduksi
    with Redactor("./sample.docx") as redactor:
        # Terapkan penyensoran
        redactor.apply(ex_red)

        # Simpan dokumen yang disensor dalam format aslinya dengan akhiran tanggal
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = datetime.now().strftime("%Y-%m-%d %H-%M-%S")

        result_path = redactor.save(so)
        print(f"Document redacted successfully.\nCheck output in {result_path}.")


if __name__ == "__main__":
    save_in_original_format()
```

## save {#document-rasterization_options}

Menyimpan dokumen ke aliran, termasuk lokasi khusus.

```python
def save(self, document, rasterization_options):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| document | `io.RawIOBase` | Aliran target. |
| rasterization_options | `RasterizationOptions` | Opsi untuk meraster atau tidak serta menentukan halaman untuk rasterisasi. |

### Contoh

```python
import io
from groupdocs.redaction.options import RasterizationOptions
from groupdocs.redaction import Redactor

with Redactor("document.pptx") as redactor:
    # konfigurasikan rasterisasi untuk memproses hanya slide pertama
    ro = RasterizationOptions()
    ro.page_index = 0
    ro.page_count = 1

    stream = io.BytesIO()
    redactor.save(stream, ro)

    # objek BytesIO sekarang berisi dokumen yang disimpan
    data = stream.getvalue()
```

### Lihat Juga
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
