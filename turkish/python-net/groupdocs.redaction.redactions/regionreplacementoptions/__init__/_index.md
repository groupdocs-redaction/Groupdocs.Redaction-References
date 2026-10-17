---
title: "__init__ yapıcı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Yeni bir RegionReplacementOptions örneği başlatır."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#fill_color-size}

Yeni bir RegionReplacementOptions örneği başlatır.

```python
def __init__(self, fill_color, size):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Alanı doldurmak için renk. |
| size | `System.Drawing.Size` | Doldurulmuş alan boyutu. |

### Örnek

```python
from groupdocs.redaction.redactions import RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

options = RegionReplacementOptions(Color.BLACK, Size(200, 80))
```

## __init__ {#fill_color-font-expected_text}

Verilen metne uygun boyutta yeni bir RegionReplacementOptions sınıfı örneği başlatır.

```python
def __init__(self, fill_color, font, expected_text):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | Alanı doldurmak için renk. |
| font | `System.Drawing.Font` | Beklenen metin yazı tipi. |
| expected_text | `str` | Beklenen metin. |

### Ayrıca Bakınız
* class [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/)
