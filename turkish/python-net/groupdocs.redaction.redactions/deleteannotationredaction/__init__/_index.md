---
title: "__init__ yapıcı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "DeleteAnnotationRedaction sınıfının yeni bir örneğini, tüm ek açıklamaları (her şeyi eşleştiren) silmek için ayarlarla başlatır."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/
is_root: false
weight: 10
---


## __init__

DeleteAnnotationRedaction sınıfının yeni bir örneğini, tüm ek açıklamaları (her şeyi eşleştiren) silmek için ayarlarla başlatır.

```python
def __init__(self):
    ...
```

### Örnek

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Tüm ek açıklamaları sil
del_red = DeleteAnnotationRedaction()
```

## __init__ {#pattern}

DeleteAnnotationRedaction sınıfının yeni bir örneğini, verilen ifadeye uyan ek açıklamaları silerek başlatır.

```python
def __init__(self, pattern):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| pattern | `str` | Düzenli ifade. |

### Örnek

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# "internal" kelimesini içeren ek açıklamaları sil (büyük/küçük harfe duyarsız)
del_red = DeleteAnnotationRedaction(r"(?i)internal")
```

## __init__ {#regex}

DeleteAnnotationRedaction sınıfının yeni bir örneğini, verilen ifadeye uyan ek açıklamaları silerek başlatır.

```python
def __init__(self, regex):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Düzenli ifade. |

### Örnek

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# İçeriği düzenli ifadeye (büyük/küçük harf duyarsız) uyan ek açıklamaları sil
del_red = DeleteAnnotationRedaction("(?i)internal")
```

### Ayrıca Bakınız
* class [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/)
