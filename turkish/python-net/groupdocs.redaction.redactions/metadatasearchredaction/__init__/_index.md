---
title: "__init__ yapıcı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "MetadataSearchRedaction sınıfının yeni bir örneğini, kırpılmış öğeleri eşleştirmek için değer kullanarak başlatır."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#value_pattern-replacement}

MetadataSearchRedaction sınıfının yeni bir örneğini, kırpılmış öğeleri eşleştirmek için değer kullanarak başlatır.

```python
def __init__(self, value_pattern, replacement):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| value_pattern | `str` | Arama ve değiştirme için düzenli ifade |
| replacement | `str` | Metinsel değiştirme |

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    redactor.apply(MetadataSearchRedaction(".*@acme\\.com", "[EMAIL]"))
    redactor.save()
```

## __init__ {#value_pattern-replacement-key_pattern}

MetadataSearchRedaction'ın yeni bir örneğini, kırpılmış öğeleri eşleştirmek için öğe adı ve değer kullanarak başlatır.

```python
def __init__(self, value_pattern, replacement, key_pattern):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| value_pattern | `str` | Üst veri öğesi değerini aramak ve değiştirmek için düzenli ifade. |
| replacement | `str` | Metinsel değiştirme. |
| key_pattern | `str` | Üst veri öğesi adını aramak ve değiştirmek için düzenli ifade. |

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    # Üst veri değerlerinde bulunan tüm e‑posta adreslerini değiştir
    redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement}

MetadataSearchRedaction sınıfının yeni bir örneğini, kırpılmış öğeleri eşleştirmek için değer kullanarak başlatır.

```python
def __init__(self, value_regex, replacement):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Arama ve değiştirme için düzenli ifade. |
| replacement | `str` | Metinsel değiştirme. |

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

# Üst verideki tüm e‑posta adreslerini gizle
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement-key_regex}

MetadataSearchRedaction'ın yeni bir örneğini, kırpılmış öğeleri eşleştirmek için öğe adı ve değer kullanarak başlatır.

```python
def __init__(self, value_regex, replacement, key_regex):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Üst veri öğesi değerini aramak ve değiştirmek için düzenli ifade. |
| replacement | `str` | Metinsel değiştirme. |
| key_regex | `System.Text.RegularExpressions.Regex` | Üst veri öğesi adını aramak ve değiştirmek için düzenli ifade. |

### Örnek

```python
from groupdocs.redaction.redactions import MetadataSearchRedaction
from groupdocs.redaction import Redactor

# Üst veri değerlerindeki e‑posta adreslerini gizle
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

### Ayrıca Bakınız
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/)
