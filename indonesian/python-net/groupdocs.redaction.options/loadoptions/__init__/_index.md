---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi sebuah instance baru dari kelas LoadOptions."
type: docs
url: /id/python-net/groupdocs.redaction.options/loadoptions/__init__/
is_root: false
weight: 10
---


## __init__

Menginisialisasi sebuah instance baru dari kelas LoadOptions.

```python
def __init__(self):
    ...
```

## __init__ {#password}

Menginisialisasi sebuah instance baru dari LoadOptions dengan kata sandi yang ditentukan.

```python
def __init__(self, password):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| password | `str` | Kata sandi untuk file yang dilindungi. |

### Contoh

```python
    from groupdocs.redaction.options import LoadOptions

    # Muat dokumen yang dilindungi kata sandi
    load_opt = LoadOptions("mypassword")
    ```

## __init__ {#pre_rasterize}

Menginisialisasi sebuah instance LoadOptions baru dengan flag pra‑rasterisasi yang ditentukan.

```python
def __init__(self, pre_rasterize):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| pre_rasterize | `bool` | Jika True, paksa rasterisasi saat memuat. |

## __init__ {#password-pre_rasterize}

Menginisialisasi sebuah instance LoadOptions baru dengan kata sandi yang ditentukan.

Jika `pre_rasterize` adalah True, rasterisasi dipaksa saat dokumen dimuat.

```python
def __init__(self, password, pre_rasterize):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| password | `str` | Kata sandi untuk file yang dilindungi. |
| pre_rasterize | `bool` | Jika True, paksa rasterisasi saat memuat. |

### Contoh

```python
from groupdocs.redaction.options import LoadOptions

# Muat dokumen yang dilindungi kata sandi
load_opt = LoadOptions("mypassword")
```

### Lihat Juga
* class [`LoadOptions`](/redaction/python-net/groupdocs.redaction.options/loadoptions/)
