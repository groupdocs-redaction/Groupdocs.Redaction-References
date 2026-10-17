---
title: "__init__ yapıcı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "RegexRedaction'ın yeni bir örneğini başlatır."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/regexredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-options}

RegexRedaction'ın yeni bir örneğini başlatır.

```python
def __init__(self, pattern, options):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| pattern | `str` | Arama ve değiştirme için düzenli ifade. |
| options | `ReplacementOptions` | Değiştirme seçenekleri (metinsel, renk). |

### Örnek

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

## __init__ {#regex-options}

Yeni bir RegexRedaction örneğini başlatır.

```python
def __init__(self, regex, options):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Arama ve değiştirme için düzenli ifade. |
| options | `ReplacementOptions` | Değiştirme seçenekleri (metinsel, renk). |

### Örnek

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

### Ayrıca Bakınız
* class [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)
