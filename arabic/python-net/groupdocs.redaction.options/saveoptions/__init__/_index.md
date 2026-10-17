---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يُنشئ مثيلًا جديدًا بالإعدادات الافتراضية: rasterizetopdf هو False و addsuffix هو False."
type: docs
url: /ar/python-net/groupdocs.redaction.options/saveoptions/__init__/
is_root: false
weight: 10
---


## __init__

يُنشئ مثيلاً جديدًا بالإعدادات الافتراضية: rasterize_to_pdf هو False و add_suffix هو False.

```python
def __init__(self):
    ...
```

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

with Redactor("./sample.docx") as redactor:
    redactor.apply(ex_red)
    save_options = SaveOptions()  # defaults: rasterize_to_pdf=False, add_suffix=False
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}.")
```

## __init__ {#rasterize_to_pdf-suffix}

يُنشئ مثيلاً جديدًا بالمعلمات المحددة.

```python
def __init__(self, rasterize_to_pdf, suffix):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| rasterize_to_pdf | `bool` | True، إذا كان يجب تحويل جميع صفحات المستند إلى صور ووضعها في ملف PDF واحد. |
| suffix | `str` | سيُضاف هذا النص إلى نهاية اسم الملف؛ إذا لم يكن فارغًا سيضبط أيضًا `add_suffix` إلى True. |

### مثال

```python
from groupdocs.redaction.options import SaveOptions

# إنشاء خيارات الحفظ بالإعدادات الافتراضية
options = SaveOptions()
options.add_suffix = True
options.rasterize_to_pdf = True
options.redacted_file_suffix = "redacted"
```

### انظر أيضًا
* class [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/)
