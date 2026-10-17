---
title: "فئة RasterizationOptions"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يوفر خيارات لتحويل الملفات إلى PDF."
type: docs
url: /ar/python-net/groupdocs.redaction.options/rasterizationoptions/
is_root: false
weight: 80
---


## RasterizationOptions class

يوفر خيارات لتحويل الملفات إلى PDF.

- More details about saving document as a rasterized PDF: https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/
- More details about rasterization options: https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/

نوع RasterizationOptions يعرض الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/__init__/) | يُهيئ نسخة جديدة. |

### الطرق
| طريقة | الوصف |
| :- | :- |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type) | يسجّل خيار تمثيل نقطي متقدم للتطبيق. |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type-parameters) | يسجّل خيار تمثيل نقطي متقدم للتطبيق. |
| [add_advanced_option_advanced_rasterization_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option_advanced_rasterization_options/) |  |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [compliance](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/compliance/) | مستوى توافق PDF. |
| [enabled](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/enabled/) | تشير علامة التمكين إلى ما إذا كانت جميع الصفحات في المستند تُحوَّل إلى صور وتوضع في ملف PDF واحد. القيمة True هي الافتراضية؛ اضبطها إلى False لتجنب التحويل إلى نقطية. |
| [has_advanced_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/has_advanced_options/) | المؤشر هو True إذا تم تعيين خيارات التحويل إلى نقطية المتقدمة. |
| [page_count](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_count/) | عدد الصفحات التي سيتم تحويلها إلى PDF. |
| [page_index](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_index/) | فهرس الصفحة الأولى (بدءًا من 0) للتحويل إلى PDF. |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import RasterizationOptions, PdfComplianceLevel

with Redactor("SomePresentation.pptx") as redactor:
    ro = RasterizationOptions()
    ro.page_index = 0          # first slide
    ro.page_count = 1
    ro.compliance = PdfComplianceLevel.PdfA1a
    redactor.save("PresentationFirstSlide.pdf", ro)
```

### انظر أيضًا
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
