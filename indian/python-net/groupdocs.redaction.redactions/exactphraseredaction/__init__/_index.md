---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "केस‑इंसेंसिटिव मोड में ExactPhraseRedaction का एक नया उदाहरण आरंभ करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#search_phrase-options}

केस‑इंसेंसिटिव मोड में ExactPhraseRedaction का एक नया उदाहरण आरंभ करता है।

```python
def __init__(self, search_phrase, options):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| search_phrase | `str` | खोज और प्रतिस्थापन के लिए स्ट्रिंग। |
| options | `ReplacementOptions` | प्रतिस्थापन विकल्प (पाठ्य, रंग). |

### उदाहरण

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# "John Doe" की घटनाओं को "[CUSTOMER]" से बदलें (case‑insensitive)
redaction = ExactPhraseRedaction("John Doe", ReplacementOptions("[CUSTOMER]"))
```

## __init__ {#search_phrase-is_case_sensitive-options}

एक नया ExactPhraseRedaction उदाहरण आरंभ करता है।

```python
def __init__(self, search_phrase, is_case_sensitive, options):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| search_phrase | `str` | खोज और प्रतिस्थापन के लिए स्ट्रिंग। |
| is_case_sensitive | `bool` | यदि case‑sensitive खोज आवश्यक है तो True। |
| options | `ReplacementOptions` | प्रतिस्थापन विकल्प (पाठ्य, रंग). |

### उदाहरण

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Case‑insensitive सटीक वाक्यांश रेडैक्शन
redaction = ExactPhraseRedaction("John Doe", False, ReplacementOptions("[CUSTOMER]"))

# Case‑sensitive सटीक वाक्यांश रेडैक्शन
redaction_cs = ExactPhraseRedaction("ACME", True, ReplacementOptions("[CO]"))
```

### संबंधित देखें
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/)
