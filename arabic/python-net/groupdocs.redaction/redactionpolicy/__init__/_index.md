---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "ينشئ مثيلًا جديدًا من RedactionPolicy."
type: docs
url: /ar/python-net/groupdocs.redaction/redactionpolicy/__init__/
is_root: false
weight: 10
---


## __init__

ينشئ مثيلًا جديدًا من RedactionPolicy.

```python
def __init__(self):
    ...
```

### مثال

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

## __init__ {#redactions}

ينشئ RedactionPolicy جديدًا بقائمة محددة من عمليات الحجب.

```python
def __init__(self, redactions):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| redactions | `list[Redaction]` | مصفوفة من redactions للسياسة. |

### مثال

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

### انظر أيضًا
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
