---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi instance PageAreaRedaction baru."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#regex-options}

Menginisialisasi instance PageAreaRedaction baru.

```python
def __init__(self, regex, options):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Ekspresi reguler untuk mencari dan mengganti. |
| options | `ReplacementOptions` | Opsi penggantian (teks, warna). |

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(r"\d{3}-\d{2}-\d{4}", ReplacementOptions("[SSN]"))
    )
    redactor.save()
```

## __init__ {#regex-options-image_options}

Menginisialisasi PageAreaRedaction baru.

```python
def __init__(self, regex, options, image_options):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Ekspresi reguler untuk mencari dan mengganti. |
| options | `ReplacementOptions` | Opsi penggantian (teks, warna). |
| image_options | `RegionReplacementOptions` | Opsi penggantian (area gambar). |

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

redactor = Redactor("scan.pdf")
redactor.apply(
    PageAreaRedaction(
        r"\d{3}-\d{2}-\d{4}",
        ReplacementOptions("[SSN]"),
        RegionReplacementOptions(Color.BLACK, Size(120, 20))
    )
)
redactor.save()
```

### Lihat Juga
* class [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/)
