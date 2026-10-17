---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "ينشئ مثيلاً جديداً من فئة MetadataSearchRedaction، باستخدام القيمة لمطابقة العناصر المحذوفة."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#value_pattern-replacement}

ينشئ مثيلاً جديداً من فئة MetadataSearchRedaction، باستخدام القيمة لمطابقة العناصر المحذوفة.

```python
def __init__(self, value_pattern, replacement):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| value_pattern | `str` | تعبير نمطي للبحث والاستبدال |
| replacement | `str` | استبدال نصي |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    redactor.apply(MetadataSearchRedaction(".*@acme\\.com", "[EMAIL]"))
    redactor.save()
```

## __init__ {#value_pattern-replacement-key_pattern}

ينشئ مثيلاً جديداً من MetadataSearchRedaction، باستخدام اسم العنصر والقيمة لمطابقة العناصر المحذوفة.

```python
def __init__(self, value_pattern, replacement, key_pattern):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| value_pattern | `str` | تعبير نمطي للبحث واستبدال قيمة عنصر البيانات الوصفية. |
| replacement | `str` | استبدال نصي. |
| key_pattern | `str` | تعبير نمطي للبحث واستبدال اسم عنصر البيانات الوصفية. |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    # استبدال أي عنوان بريد إلكتروني موجود في قيم البيانات الوصفية
    redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement}

ينشئ مثيلاً جديداً من فئة MetadataSearchRedaction، باستخدام القيمة لمطابقة العناصر المحذوفة.

```python
def __init__(self, value_regex, replacement):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | تعبير نمطي للبحث والاستبدال. |
| replacement | `str` | استبدال نصي. |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

# إخفاء أي عنوان بريد إلكتروني في البيانات الوصفية
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement-key_regex}

ينشئ مثيلاً جديداً من MetadataSearchRedaction باستخدام اسم العنصر والقيمة لمطابقة العناصر المحذوفة.

```python
def __init__(self, value_regex, replacement, key_regex):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | تعبير نمطي للبحث واستبدال قيمة عنصر البيانات الوصفية. |
| replacement | `str` | استبدال نصي. |
| key_regex | `System.Text.RegularExpressions.Regex` | تعبير نمطي للبحث واستبدال اسم عنصر البيانات الوصفية. |

### مثال

```python
from groupdocs.redaction.redactions import MetadataSearchRedaction
from groupdocs.redaction import Redactor

# إخفاء عناوين البريد الإلكتروني في قيم البيانات الوصفية
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

### انظر أيضًا
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/)
