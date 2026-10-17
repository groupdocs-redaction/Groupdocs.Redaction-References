---
title: "LoadOptions فئة"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يوفر خيارات سيتم استخدامها لفتح ملف."
type: docs
url: /ar/python-net/groupdocs.redaction.options/loadoptions/
is_root: false
weight: 40
---


## LoadOptions class

يوفر خيارات سيتم استخدامها لفتح ملف.

اعرف المزيد
- [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
- [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
- [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
- [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

نوع LoadOptions يعرض الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/) | يُهيئ مثلاً جديداً من فئة LoadOptions. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password) | يُهيئ مثلاً جديداً من LoadOptions باستخدام كلمة المرور المحددة. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#pre_rasterize) | يُهيئ مثلاً جديداً من LoadOptions مع العلامة المحددة للتمهيد المسبق للتصوير النقطي. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password-pre_rasterize) | يُهيئ مثلاً جديداً من LoadOptions مع كلمة المرور المحددة. |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.options/loadoptions/password/) | كلمة المرور للمستندات المحمية بكلمة مرور. |
| [pre_rasterize](/redaction/python-net/groupdocs.redaction.options/loadoptions/pre_rasterize/) | علامة pre_rasterize التي تشير إلى ما إذا كان يجب تمهيد الملف مسبقاً. |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# حدد خيارات التحميل باستخدام كلمة مرور المستند
load_opt = LoadOptions("mypassword")

# حدد حذفًا
repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

# افتح المستند المحمي بكلمة مرور
with Redactor("./protected.docx", load_opt) as redactor:
    redactor.apply(ex_red)

    # احفظ المستند المحذوف
    save_opt = SaveOptions()
    save_opt.add_suffix = True
    result_path = redactor.save(save_opt)
    print(f"Document redacted successfully. Check output in {result_path}.")
```

### انظر أيضًا
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
