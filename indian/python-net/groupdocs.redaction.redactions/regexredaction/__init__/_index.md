---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "RegexRedaction का एक नया उदाहरण प्रारंभ करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/regexredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-options}

RegexRedaction का एक नया उदाहरण प्रारंभ करता है।

```python
def __init__(self, pattern, options):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| pattern | `str` | खोज और प्रतिस्थापन के लिए नियमित अभिव्यक्ति। |
| options | `ReplacementOptions` | प्रतिस्थापन विकल्प (पाठ्य, रंग). |

### उदाहरण

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

## __init__ {#regex-options}

एक नया RegexRedaction उदाहरण प्रारंभ करता है।

```python
def __init__(self, regex, options):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | खोज और प्रतिस्थापन के लिए नियमित अभिव्यक्ति। |
| options | `ReplacementOptions` | प्रतिस्थापन विकल्प (पाठ्य, रंग). |

### उदाहरण

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

### संबंधित देखें
* class [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)
