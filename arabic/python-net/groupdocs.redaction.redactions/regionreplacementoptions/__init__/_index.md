---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يُنشئ مثيلًا جديدًا من RegionReplacementOptions."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#fill_color-size}

يُنشئ مثيلًا جديدًا من RegionReplacementOptions.

```python
def __init__(self, fill_color, size):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | اللون لملء المنطقة. |
| size | `System.Drawing.Size` | حجم المنطقة المملوءة. |

### مثال

```python
from groupdocs.redaction.redactions import RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

options = RegionReplacementOptions(Color.BLACK, Size(200, 80))
```

## __init__ {#fill_color-font-expected_text}

يُنشئ مثيلًا جديدًا من الفئة RegionReplacementOptions بحيث يتطابق حجمه مع النص المعطى.

```python
def __init__(self, fill_color, font, expected_text):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | اللون لملء المنطقة. |
| font | `System.Drawing.Font` | خط النص المتوقع. |
| expected_text | `str` | النص المتوقع. |

### انظر أيضًا
* class [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/)
