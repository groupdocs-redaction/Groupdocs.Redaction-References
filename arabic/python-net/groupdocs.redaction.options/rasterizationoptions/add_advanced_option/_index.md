---
title: "طريقة add_advanced_option"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يسجّل خيار تمثيل نقطي متقدم للتطبيق."
type: docs
url: /ar/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/
is_root: false
weight: 1010
---


## add_advanced_option {#option_type}

يسجّل خيار تمثيل نقطي متقدم للتطبيق.

```python
def add_advanced_option(self, option_type):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | يوفر معلومات حول نوع التأثير المحدد (تدرج رمادي، حد، إلخ). |

### مثال

```python
from groupdocs.redaction.options import SaveOptions, AdvancedRasterizationOptions

so = SaveOptions()
so.rasterization.enabled = True
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.NOISE)
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)
```

## add_advanced_option {#option_type-parameters}

يسجّل خيار تمثيل نقطي متقدم للتطبيق.

```python
def add_advanced_option(self, option_type, parameters):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | يوفر معلومات حول نوع التأثير المحدد (تدرج رمادي، حد، إلخ). |
| parameters | `dict[str, str]` | معلمات التأثير المحدد، مثل زاوية الدوران. |

### مثال

```python
from groupdocs.redaction.options import RasterizationOptions, AdvancedRasterizationOptions

ro = RasterizationOptions()
ro.enabled = True
# تطبيق التأثيرات المدمجة
ro.add_advanced_option(AdvancedRasterizationOptions.NOISE)
ro.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)

# تطبيق تأثير بإعدادات مخصصة، مثل حد بسمك 10 وحدات
ro.add_advanced_option(
    AdvancedRasterizationOptions.BORDER,
    {"border": "10"}
)
```

### انظر أيضًا
* class [`RasterizationOptions`](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/)
