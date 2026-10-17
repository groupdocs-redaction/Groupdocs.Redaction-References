---
title: "__init__ yapıcı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Bir regex deseni ve değiştirme metni ile yeni bir AnnotationRedaction başlatır."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-replacement}

Bir regex deseni ve değiştirme metni ile yeni bir AnnotationRedaction başlatır.

```python
def __init__(self, pattern, replacement):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| pattern | `str` | Eşleşecek düzenli ifade. |
| replacement | `str` | Eşleşen metin için metinsel değiştirme. |

### Örnek

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Açıklama metinlerinde "approved" kelimesini sansürle
redaction = AnnotationRedaction(r"(?i)approved", "[REVIEW]")
```

## __init__ {#regex-replacement}

Yeni bir [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) örneği başlatır.

```python
def __init__(self, regex, replacement):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Eşleşecek düzenli ifade. |
| replacement | `str` | Eşleşen metin için metinsel değiştirme. |

### Örnek

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# "approved" kelimesini (büyük‑küçük harfe duyarsız) sansürle ve "[REVIEW]" ile değiştir
redaction = AnnotationRedaction("(?i)approved", "[REVIEW]")
```

### Ayrıca Bakınız
* class [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/)
