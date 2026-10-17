---
title: "__init__ yapıcı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Yeni bir RemovePageRedaction başlatır."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#origin-index-count}

Yeni bir RemovePageRedaction başlatır.

```python
def __init__(self, origin, index, count):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Belgenin başlangıcı ya da sonu olan referans konumunu ara. |
| index | `int` | Başlangıç konumu indeksi (0‑tabanlı). |
| count | `int` | Kaldırılacak sayfa sayısı. |

### Örnek

```python
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# İkinci sayfadan (sıfır‑tabanlı indeks 1) başlayarak 3 sayfa kaldır
redaction = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)
```

### Ayrıca Bakınız
* class [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/)
