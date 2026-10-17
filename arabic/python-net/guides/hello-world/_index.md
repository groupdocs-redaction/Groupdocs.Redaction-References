---
title: "مرحبا، العالم!"
linkTitle: "Hello, World!"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "ابدأ بسرعة مع GroupDocs.Redaction لـ Python عبر .NET عن طريق إنشاء وتشغيل مثال بسيط."
type: docs
url: /ar/python-net/guides/hello-world/
is_root: false
weight: 20
---


## Introduction
غالبًا ما يكون مثال "Hello, World!" هو الخطوة الأولى عند استكشاف GroupDocs.Redaction لـ Python عبر .NET. وهو يعمل كاختبار بسيط لتأكيد أن بيئة التطوير الخاصة بك مُعدة بشكل صحيح وأن المكتبة تعمل كما هو متوقع.

## Overview
يتيح لك GroupDocs.Redaction لـ Python عبر .NET البحث، الإخفاء، وإزالة المعلومات الحساسة من صيغ مستندات مختلفة. مجموعة واسعة من [الصيغ المدعومة](https://docs.groupdocs.com/redaction/python-net/getting-started/supported-document-formats/) تجعلها متعددة الاستخدامات لحالات مختلفة.

## How to redact a document
الخطوات التالية توضح كيفية إخفاء المعلومات الحساسة من مستند باستخدام GroupDocs.Redaction لـ Python عبر .NET:

1. استورد الفئات `groupdocs.redaction` التي تحتاجها.
2. صِف الإخفاء (هنا، عبارة دقيقة لاستبدالها بمربع ملون).
3. أنشئ كائنًا من [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) مع المسار إلى المستند النموذجي.
4. نفّذ الإخفاء.
5. احفظ النتيجة.

## Complete example
المثال أدناه يستبدل كل ظهور لعبارة "John Doe" بمربع أحمر شبه شفاف ويحفظ المستند المَخفِي:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def hello_world():
    # ارسم مربعًا أحمرًا شبه شفاف فوق كل ظهور لـ "John Doe"
    options = ReplacementOptions(Color.from_argb(128, 255, 0, 0))
    redaction = ExactPhraseRedaction("John Doe", options)

    # حمّل المستند، نفّذ الإخفاء، واحفظ النتيجة
    with Redactor("./sample.docx") as redactor:
        redactor.apply(redaction)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Document redacted successfully. Output saved to {result_path}.")

if __name__ == "__main__":
    hello_world()
```

`sample.docx` هو الملف النموذجي المستخدم في هذا المثال. انقر [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/getting-started/hello-world/sample.docx) لتنزيله.

  
```text
Binary file (PDF, 1.0 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/getting-started/hello-world/hello_world/sample_redacted.pdf)

يقوم هذا المثال بتحويل النتيجة إلى ملف PDF باسم `sample_redacted.pdf`، بحيث لا يمكن استعادة المحتوى المَخفِي (`save()` يحول إلى PDF افتراضيًا؛ خيار `redacted_file_suffix` يتحكم فقط في اسم الإخراج). للحفاظ على الصيغة الأصلية بدلاً من ذلك، اضبط `rasterize_to_pdf = False`.

## Additional resources
يشير هذا العرض إلى [نماذج الشيفرة](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET/) الخاصة بـ GroupDocs.Redaction لـ Python عبر .NET.
