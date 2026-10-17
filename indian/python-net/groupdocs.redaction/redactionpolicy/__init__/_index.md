---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक नया RedactionPolicy इंस्टेंस प्रारंभ करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction/redactionpolicy/__init__/
is_root: false
weight: 10
---


## __init__

एक नया RedactionPolicy इंस्टेंस प्रारंभ करता है।

```python
def __init__(self):
    ...
```

### उदाहरण

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

## __init__ {#redactions}

विशिष्ट रेडैक्शन सूची के साथ एक नया RedactionPolicy प्रारंभ करता है।

```python
def __init__(self, redactions):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| redactions | `list[Redaction]` | नीति के लिए redactions की एक एरे। |

### उदाहरण

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

### संबंधित देखें
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
