---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक नया CellColumnRedaction आरंभ करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#filter-reg_ex-options}

एक नया CellColumnRedaction आरंभ करता है।

```python
def __init__(self, filter, reg_ex, options):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| filter | `CellFilter` | कॉलम और वर्कशीट फ़िल्टर। |
| reg_ex | `System.Text.RegularExpressions.Regex` | खोज और प्रतिस्थापन के लिए नियमित अभिव्यक्ति। |
| options | `ReplacementOptions` | प्रतिस्थापन विकल्प। |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import CellColumnRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("spreadsheet.xlsx") as redactor:
    redactor.apply(
        CellColumnRedaction(
            CellFilter(worksheet="Sheet1", column=2),
            r"\bsecret\b",
            ReplacementOptions(Color.BLACK)
        )
    )
    redactor.save()
```

### संबंधित देखें
* class [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/)
