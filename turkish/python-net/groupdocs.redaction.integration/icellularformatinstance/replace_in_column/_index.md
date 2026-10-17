---
title: "replace_in_column yöntemi"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belirtilen sütun ve çalışma sayfasındaki tüm eşleşmeleri verilen bir değiştirme ile değiştirir."
type: docs
url: /tr/python-net/groupdocs.redaction.integration/icellularformatinstance/replace_in_column/
is_root: false
weight: 1040
---


## replace_in_column {#regular_expression-replacement-column-sheet}

Belirtilen sütun ve çalışma sayfasındaki tüm eşleşmeleri verilen bir değiştirme ile değiştirir.

```python
def replace_in_column(self, regular_expression, replacement, column, sheet):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Arama ve değiştirme için düzenli ifade. |
| replacement | `str` | Metinsel değiştirme. |
| column | `int` | Sıfır tabanlı sütun indeksi. |
| sheet | `int` | Sıfır tabanlı çalışma sayfası indeksi. |

**Returns:** Replacement result.

## replace_in_column {#regular_expression-replacement-column}

Tüm çalışma sayfalarındaki belirtilen sütunda tüm eşleşmeleri verilen bir değiştirme ile değiştirir.

```python
def replace_in_column(self, regular_expression, replacement, column):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Arama ve değiştirme için düzenli ifade. |
| replacement | `str` | Metinsel değiştirme. |
| column | `int` | Sıfır tabanlı sütun indeksi. |

**Returns:** Replacement result.

### Ayrıca Bakınız
* class [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/)
