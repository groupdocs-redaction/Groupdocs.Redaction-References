---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi instance Redactor baru menggunakan jalur file."
type: docs
url: /id/python-net/groupdocs.redaction/redactor/__init__/
is_root: false
weight: 10
---


## __init__ {#file_path}

Menginisialisasi instance Redactor baru menggunakan jalur file.

```python
def __init__(self, file_path):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| file_path | `str` | Jalur ke file. |

### Contoh

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    # Lakukan operasi redaksi di sini
    pass
```

## __init__ {#document}

Menginisialisasi instance baru dari [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) menggunakan aliran.

```python
def __init__(self, document):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| document | `io.RawIOBase` | Aliran sumber dokumen. |

### Contoh

```python
from groupdocs.redaction import Redactor

def open_from_stream():
    # Buka dokumen sebagai aliran biner
    with open("./sample.pdf", "rb") as stream:
        # Muat dokumen dari aliran
        with Redactor(stream) as redactor:
            # Lakukan redaksi di sini
            pass
```

## __init__ {#file_path-load_options}

Menginisialisasi instance baru dari [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) untuk dokumen yang dilindungi kata sandi menggunakan jalurnya.

```python
def __init__(self, file_path, load_options):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| file_path | `str` | Jalur ke file. |
| load_options | `LoadOptions` | Opsi, termasuk kata sandi. |

### Contoh

```python
from groupdocs.redaction import Redactor

# Muat dokumen yang dilindungi kata sandi dari jalur file
with Redactor("protected.docx") as redactor:
    # Lakukan operasi redaksi di sini
    pass
```

## __init__ {#file_path-load_options-settings}

Menginisialisasi instance Redactor baru untuk dokumen yang dilindungi kata sandi menggunakan jalur dan pengaturannya.

```python
def __init__(self, file_path, load_options, settings):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| file_path | `str` | Jalur ke file. |
| load_options | `LoadOptions` | Opsi yang bergantung pada file, termasuk kata sandi. |
| settings | `RedactorSettings` | Pengaturan default untuk proses redaksi. |

### Contoh

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

## __init__ {#document-load_options}

Menginisialisasi instance Redactor baru untuk dokumen yang dilindungi kata sandi menggunakan aliran.

```python
def __init__(self, document, load_options):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| document | `io.RawIOBase` | Aliran input sumber. |
| load_options | `LoadOptions` | Opsi, termasuk kata sandi. |

### Contoh

```python
from groupdocs.redaction import Redactor, LoadOptions

def open_protected_doc():
    # Buka PDF yang dilindungi sebagai aliran biner
    with open(r"C:\sample.pdf", "rb") as stream:
        # Berikan kata sandi melalui LoadOptions
        load_options = LoadOptions("mypassword")
        # Inisialisasi Redactor dengan aliran dan opsi pemuatan
        with Redactor(stream, load_options) as redactor:
            # Lakukan operasi redaksi di sini
            pass
```

## __init__ {#document-load_options-settings}

Menginisialisasi instance baru dari [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) untuk dokumen yang dilindungi kata sandi menggunakan aliran dan pengaturan.

```python
def __init__(self, document, load_options, settings):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| document | `io.RawIOBase` | Aliran input sumber. |
| load_options | `LoadOptions` | Opsi, termasuk kata sandi. |
| settings | `RedactorSettings` | Pengaturan default untuk proses redaksi. |

### Lihat Juga
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
