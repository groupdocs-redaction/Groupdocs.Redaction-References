---
title: "__init__ yapıcı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "LoadOptions sınıfının yeni bir örneğini başlatır."
type: docs
url: /tr/python-net/groupdocs.redaction.options/loadoptions/__init__/
is_root: false
weight: 10
---


## __init__

LoadOptions sınıfının yeni bir örneğini başlatır.

```python
def __init__(self):
    ...
```

## __init__ {#password}

Belirtilen şifre ile LoadOptions'ın yeni bir örneğini başlatır.

```python
def __init__(self, password):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| password | `str` | Korunan dosyalar için parola. |

### Örnek

```python
    from groupdocs.redaction.options import LoadOptions

    # Parola korumalı bir belgeyi yükle
    load_opt = LoadOptions("mypassword")
    ```

## __init__ {#pre_rasterize}

Belirtilen ön‑tarama bayrağı ile yeni bir LoadOptions örneğini başlatır.

```python
def __init__(self, pre_rasterize):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| pre_rasterize | `bool` | True ise, yükleme sırasında rasterleştirmeyi zorla. |

## __init__ {#password-pre_rasterize}

Belirtilen şifre ile yeni bir LoadOptions örneğini başlatır.

Eğer `pre_rasterize` True ise, belge yüklendiğinde rasterleştirme zorlanır.

```python
def __init__(self, password, pre_rasterize):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| password | `str` | Korunan dosyalar için parola. |
| pre_rasterize | `bool` | True ise, yükleme sırasında rasterleştirmeyi zorla. |

### Örnek

```python
from groupdocs.redaction.options import LoadOptions

# Parola korumalı bir belgeyi yükle
load_opt = LoadOptions("mypassword")
```

### Ayrıca Bakınız
* class [`LoadOptions`](/redaction/python-net/groupdocs.redaction.options/loadoptions/)
