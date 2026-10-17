---
title: "metode replace_in_column"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mengganti semua kecocokan dengan pengganti yang diberikan pada kolom dan lembar kerja yang ditentukan."
type: docs
url: /id/python-net/groupdocs.redaction.integration/icellularformatinstance/replace_in_column/
is_root: false
weight: 1040
---


## replace_in_column {#regular_expression-replacement-column-sheet}

Mengganti semua kecocokan dengan pengganti yang diberikan pada kolom dan lembar kerja yang ditentukan.

```python
def replace_in_column(self, regular_expression, replacement, column, sheet):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Ekspresi reguler untuk mencari dan mengganti. |
| replacement | `str` | Penggantian teks. |
| column | `int` | Indeks kolom berbasis nol. |
| sheet | `int` | Indeks lembar kerja berbasis nol. |

**Returns:** Replacement result.

## replace_in_column {#regular_expression-replacement-column}

Mengganti semua kecocokan dengan pengganti yang diberikan pada kolom yang ditentukan di semua lembar kerja.

```python
def replace_in_column(self, regular_expression, replacement, column):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Ekspresi reguler untuk mencari dan mengganti. |
| replacement | `str` | Penggantian teks. |
| column | `int` | Indeks kolom berbasis nol. |

**Returns:** Replacement result.

### Lihat Juga
* class [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/)
