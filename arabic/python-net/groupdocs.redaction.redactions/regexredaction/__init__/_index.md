---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "ينشئ مثيلاً جديدًا من RegexRedaction."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/regexredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-options}

ينشئ مثيلاً جديدًا من RegexRedaction.

```python
def __init__(self, pattern, options):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| pattern | `str` | تعبير نمطي للبحث والاستبدال. |
| options | `ReplacementOptions` | خيارات الاستبدال (نصية، لون). |

### مثال

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

## __init__ {#regex-options}

ينشئ مثيلاً جديدًا من RegexRedaction.

```python
def __init__(self, regex, options):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | تعبير نمطي للبحث والاستبدال. |
| options | `ReplacementOptions` | خيارات الاستبدال (نصية، لون). |

### مثال

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

### انظر أيضًا
* class [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)
