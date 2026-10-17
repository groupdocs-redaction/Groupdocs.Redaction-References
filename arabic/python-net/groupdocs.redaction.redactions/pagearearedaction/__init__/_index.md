---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يُنشئ كائن PageAreaRedaction جديد."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#regex-options}

يُنشئ كائن PageAreaRedaction جديد.

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
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(r"\d{3}-\d{2}-\d{4}", ReplacementOptions("[SSN]"))
    )
    redactor.save()
```

## __init__ {#regex-options-image_options}

يُنشئ PageAreaRedaction جديدًا.

```python
def __init__(self, regex, options, image_options):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | تعبير نمطي للبحث والاستبدال. |
| options | `ReplacementOptions` | خيارات الاستبدال (نصية، لون). |
| image_options | `RegionReplacementOptions` | خيارات الاستبدال (منطقة الصورة). |

### مثال

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

### انظر أيضًا
* class [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/)
