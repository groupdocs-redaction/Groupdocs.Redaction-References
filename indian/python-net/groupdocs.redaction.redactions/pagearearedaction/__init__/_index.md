---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "नया PageAreaRedaction उदाहरण प्रारंभ करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#regex-options}

नया PageAreaRedaction उदाहरण प्रारंभ करता है।

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
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(r"\d{3}-\d{2}-\d{4}", ReplacementOptions("[SSN]"))
    )
    redactor.save()
```

## __init__ {#regex-options-image_options}

नया PageAreaRedaction प्रारंभ करता है।

```python
def __init__(self, regex, options, image_options):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | खोज और प्रतिस्थापन के लिए नियमित अभिव्यक्ति। |
| options | `ReplacementOptions` | प्रतिस्थापन विकल्प (पाठ्य, रंग). |
| image_options | `RegionReplacementOptions` | प्रतिस्थापन विकल्प (छवि क्षेत्र). |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

redactor = Redactor("scan.pdf")
redactor.apply(
    PageAreaRedaction(
        r"\d{3}-\d{2}-\d{4}",
        ReplacementOptions("[SSN]"),
        RegionReplacementOptions(Color.BLACK, Size(120, 20))
    )
)
redactor.save()
```

### संबंधित देखें
* class [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/)
