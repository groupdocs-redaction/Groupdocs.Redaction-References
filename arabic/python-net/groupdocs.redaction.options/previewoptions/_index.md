---
title: "فئة PreviewOptions"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يوفر خيارات لتعيين المتطلبات ومندوبات التدفق لإنشاء المعاينات."
type: docs
url: /ar/python-net/groupdocs.redaction.options/previewoptions/
is_root: false
weight: 70
---


## PreviewOptions class

يوفر خيارات لتعيين المتطلبات ومندوبات التدفق لإنشاء المعاينات.

تسمح الفئة بتحديد صيغة المعاينة، أبعاد الصورة، أرقام الصفحات، والموكّلات التي تنشئ وتفرج اختياريًا عن التدفقات لكل صفحة مُولدة.

يعرض نوع PreviewOptions الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream) | يُنشئ مثيلاً جديدًا من PreviewOptions. سيتم إغلاق تدفق الإخراج بعد الاستخدام. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream-release_page_stream) | يُنشئ مثيلاً جديدًا من PreviewOptions، مما يؤدي إلى إرجاع تدفق الإخراج إلى العميل للاستخدام لاحقًا. |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [create_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/create_page_stream/) | المندوب المسؤول عن إنشاء تدفق الصفحة. |
| [height](/redaction/python-net/groupdocs.redaction.options/previewoptions/height/) | ارتفاع معاينة الصفحة. |
| [page_numbers](/redaction/python-net/groupdocs.redaction.options/previewoptions/page_numbers/) | أرقام الصفحات لتوليد المعاينة. |
| [preview_format](/redaction/python-net/groupdocs.redaction.options/previewoptions/preview_format/) | تنسيق صورة المعاينة. |
| [release_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/release_page_stream/) | المندوب المسؤول عن إكمال معاينة الصفحة. |
| [width](/redaction/python-net/groupdocs.redaction.options/previewoptions/width/) | عرض معاينة الصفحة. |

### مثال

```python
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int):
    # إنشاء ملف لصورة المعاينة للصفحة المحددة
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")  # returns a writable binary stream

preview_options = PreviewOptions(create_page_stream)
preview_options.preview_format = PreviewOptions.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### انظر أيضًا
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
