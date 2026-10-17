---
title: "__init__ yapıcı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belirli bir dikdörtgen alanı gizlemek için yeni bir ImageAreaRedaction başlatır."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-options}

Belirli bir dikdörtgen alanı gizlemek için yeni bir ImageAreaRedaction başlatır.

```python
def __init__(self, top_left, options):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Sol üst alan koordinatları. |
| options | `RegionReplacementOptions` | Alan boyutu ve renk. |

### Örnek

```python
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

# Sansürlenecek alanın sol‑üst köşesini tanımla
top_left = Point(385, 485)
# Sansür bölgesinin boyutunu ve rengini tanımla
region_options = RegionReplacementOptions(Color.from_argb(255, 220, 20, 60), Size(1793, 2069))

# Sansür nesnesini oluştur
redaction = ImageAreaRedaction(top_left, region_options)
```

### Ayrıca Bakınız
* class [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/)
