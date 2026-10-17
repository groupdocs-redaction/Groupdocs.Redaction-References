---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi CellColumnRedaction baru."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#filter-reg_ex-options}

Menginisialisasi CellColumnRedaction baru.

```python
def __init__(self, filter, reg_ex, options):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| filter | `CellFilter` | Filter kolom dan lembar kerja. |
| reg_ex | `System.Text.RegularExpressions.Regex` | Ekspresi reguler untuk mencari dan mengganti. |
| options | `ReplacementOptions` | Opsi penggantian. |

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import CellColumnRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("spreadsheet.xlsx") as redactor:
    redactor.apply(
        CellColumnRedaction(
            CellFilter(worksheet="Sheet1", column=2),
            r"\bsecret\b",
            ReplacementOptions(Color.BLACK)
        )
    )
    redactor.save()
```

### Lihat Juga
* class [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/)
