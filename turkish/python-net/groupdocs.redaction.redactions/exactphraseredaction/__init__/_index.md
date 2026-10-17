---
title: "__init__ yapıcı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Büyük/küçük harfe duyarsız modda yeni bir ExactPhraseRedaction örneği başlatır."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#search_phrase-options}

Büyük/küçük harfe duyarsız modda yeni bir ExactPhraseRedaction örneği başlatır.

```python
def __init__(self, search_phrase, options):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| search_phrase | `str` | Aranacak ve değiştirilecek dize. |
| options | `ReplacementOptions` | Değiştirme seçenekleri (metinsel, renk). |

### Örnek

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# "John Doe" ifadelerini "[CUSTOMER]" ile değiştir (büyük/küçük harfe duyarsız)
redaction = ExactPhraseRedaction("John Doe", ReplacementOptions("[CUSTOMER]"))
```

## __init__ {#search_phrase-is_case_sensitive-options}

Yeni bir ExactPhraseRedaction örneği başlatır.

```python
def __init__(self, search_phrase, is_case_sensitive, options):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| search_phrase | `str` | Aranacak ve değiştirilecek dize. |
| is_case_sensitive | `bool` | Büyük/küçük harfe duyarlı arama gerekiyorsa True. |
| options | `ReplacementOptions` | Değiştirme seçenekleri (metinsel, renk). |

### Örnek

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Büyük/küçük harfe duyarsız tam ifade gizleme
redaction = ExactPhraseRedaction("John Doe", False, ReplacementOptions("[CUSTOMER]"))

# Büyük/küçük harfe duyarlı tam ifade gizleme
redaction_cs = ExactPhraseRedaction("ACME", True, ReplacementOptions("[CO]"))
```

### Ayrıca Bakınız
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/)
