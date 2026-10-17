---
title: "__init__ yapıcı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belirtilen değiştirme metniyle ReplacementOptions'ın yeni bir örneğini başlatır."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#replacement}

Belirtilen değiştirme metniyle ReplacementOptions'ın yeni bir örneğini başlatır.

```python
def __init__(self, replacement):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| replacement | `str` | Metinsel değiştirme. |

### Örnek

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Eşleşen metni "[REDACTED]" ile değiştir
options = ReplacementOptions("[REDACTED]")
```

## __init__ {#color}

Renkli dikdörtgeni seçenek olarak kullanarak ReplacementOptions sınıfının yeni bir örneğini başlatır.

```python
def __init__(self, color):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| color | `System.Drawing.Color` | Dikdörtgen rengi. |

### Ayrıca Bakınız
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)
