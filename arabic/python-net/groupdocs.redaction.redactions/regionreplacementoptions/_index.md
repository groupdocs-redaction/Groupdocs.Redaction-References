---
title: "الفئة RegionReplacementOptions"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يمثل معلمات اللون والمنطقة لاستبدال جزء من الصورة."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/regionreplacementoptions/
is_root: false
weight: 240
---


## RegionReplacementOptions class

يمثل معلمات اللون والمنطقة لاستبدال جزء من الصورة.

المزيد:
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

يعرض نوع RegionReplacementOptions الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-size) | يُنشئ مثيلًا جديدًا من RegionReplacementOptions. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-font-expected_text) | يُنشئ مثيلًا جديدًا من الفئة RegionReplacementOptions بحيث يتطابق حجمه مع النص المعطى. |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [fill_color](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/fill_color/) | اللون المستخدم لملء المنطقة المحوّرة. |
| [size](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/size/) | عرض وارتفاع المستطيل. |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

with Redactor("test.jpg") as redactor:
    # حدد موضع الزاوية العليا اليسرى للمنطقة التي سيتم استبدالها
    point = Point(516, 311)
    # حدد حجم المنطقة التي سيتم استبدالها
    size = Size(170, 35)
    # استخدم مستطيلًا أسودًا صلبًا كبديل
    repl_opt = RegionReplacementOptions(Color.BLACK, size)
    redaction = ImageAreaRedaction(point, repl_opt)

    result = redactor.apply(redaction)
    if result.status != redactor.RedactionStatus.FAILED:
        redactor.save()
```

### Guides
أدلة المهام التي تستخدم `RegionReplacementOptions`:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### انظر أيضًا
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
