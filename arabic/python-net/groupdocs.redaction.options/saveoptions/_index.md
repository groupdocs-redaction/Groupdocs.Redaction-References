---
title: "الصنف SaveOptions"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يوفر خيارات لتغيير اسم ملف الإخراج و/أو تحويل المستند إلى PDF قائم على الصور (التصوير النقطي)."
type: docs
url: /ar/python-net/groupdocs.redaction.options/saveoptions/
is_root: false
weight: 110
---


## SaveOptions class

يوفر خيارات لتغيير اسم ملف الإخراج و/أو تحويل المستند إلى PDF قائم على الصور (التصوير النقطي).

المزيد:
- [Save with default options](https://docs.groupdocs.com/redaction/net/save-with-default-options/)
- [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
- [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)
- [Save in original format](https://docs.groupdocs.com/redaction/net/save-in-original-format/)
- [Save overwriting original file](https://docs.groupdocs.com/redaction/net/save-overwriting-original-file/)
- [Save to stream](https://docs.groupdocs.com/redaction/net/save-to-stream/)

يعرض نوع SaveOptions الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/) | يُنشئ مثيلاً جديدًا بالإعدادات الافتراضية: rasterize_to_pdf هو False و add_suffix هو False. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/#rasterize_to_pdf-suffix) | يُنشئ مثيلاً جديدًا بالمعلمات المحددة. |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [add_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/add_suffix/) | خاصية add_suffix تشير إلى ما إذا كان يجب تغيير اسم الملف قبل الحفظ. القيمة الافتراضية هي False. |
| [rasterization](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterization/) | إعدادات التحويل إلى نقطية. |
| [rasterize_to_pdf](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterize_to_pdf/) | العلم الذي يحدد ما إذا كانت جميع صفحات المستند تُحوَّل إلى صور وتُدمج في ملف PDF واحد. |
| [redacted_file_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/redacted_file_suffix/) | اللاحقة المخصصة لاسم ملف الإخراج. إذا لم يتم تحديدها، يتم استخدام الثابت [`SaveOptions.SaveSuffix`](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/). |

### الحقول
| حقل | الوصف |
| :- | :- |
| [SAVE_SUFFIX](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/) | يمثل قيمة اللاحقة الافتراضية، وهي "Redacted". |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def save_with_default_options():
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    with Redactor("./sample.docx") as redactor:
        redactor.apply(ex_red)

        # احفظ المستند بالخيارات الافتراضية (تحويل إلى PDF وإضافة لاحقة)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"

        result_path = redactor.save(save_options)
        print(f"Document redacted successfully. Check output in {result_path}.")
```

### Guides
أدلة المهام التي تستخدم `SaveOptions`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### انظر أيضًا
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
