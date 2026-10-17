---
title: "إخفاءات التعليقات التوضيحية"
linkTitle: "Annotation redactions"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "توضح هذه المقالة تنفيذ إخفاء التعليقات التوضيحية للمستندات بصيغ مختلفة مثل PDF، DOC، DOCX، PPT، PPTX، XLS، XLSX وغيرها."
type: docs
url: /ar/python-net/guides/annotation-redactions/
is_root: false
weight: 80
---


باستخدام واجهة برمجة تطبيقات GroupDocs.Redaction يمكنك تطبيق إخفاءات التعليقات التوضيحية للمستندات بصيغ مختلفة مثل PDF، DOC، DOCX، PPT، PPTX، XLS، XLSX وغيرها. راجع القائمة الكاملة في مقالة [الصيغ المدعومة]().

توفر GroupDocs.Redactions واجهة برمجة تطبيقات مرنة تسمح بإزالة البيانات الحساسة من نص التعليق التوضيحي، أو إزالة التعليقات التوضيحية بالكامل باستخدام تعبير عادي.

## Remove annotations (comments etc)

يمكنك استخدام GroupDocs.Redaction لإزالة جميع التعليقات أو تعليقات محددة وغيرها من التعليقات التوضيحية من المستند. على سبيل المثال، يمكننا إزالة جميع التعليقات التي تحتوي على نصوص مثل "use"، "show" أو "describe" في محتواها:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

def remove_all_annotations():
    # حدد خيارات الإخفاء لحذف التعليقات التوضيحية التي تطابق النمط
    a_red = DeleteAnnotationRedaction("(?im:(use|show|describe))")

    # حمّل المستند المراد حذفه
    with Redactor("./annotated.xlsx") as redactor:
        # تطبيق الحجب
        result = redactor.apply(a_red)

        # احفظ المستند المُخفى بجوار ملف المصدر
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    remove_all_annotations()
```

`annotated.xlsx` هو الملف النموذجي المستخدم في هذا المثال. انقر [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) لتنزيله.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/remove_all_annotations/annotated_redacted.xlsx)

يمكنك استخدام المُنشئ بدون أي معاملات لإزالة جميع التعليقات التوضيحية داخل المستند.

## Redact annotations

بدلاً من إزالة جميع التعليقات أو تعليقات محددة، يمكنك إزالة البيانات الحساسة من نص التعليق. على سبيل المثال، يمكننا إزالة جميع الإشارات إلى "John" في المستند المعطى، مثل:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import AnnotationRedaction

def redact_annotations():
    # حدد خيارات الحذف: نمط البحث وسلسلة الاستبدال
    a_red = AnnotationRedaction("(?im:john)", "[redacted]")

    # حمّل المستند المراد حذفه
    with Redactor("./annotated.xlsx") as redactor:
        # تطبيق الحجب
        result = redactor.apply(a_red)

        # احفظ المستند المُخفى بجوار ملف المصدر
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_annotations()
```

`annotated.xlsx` هو الملف النموذجي المستخدم في هذا المثال. انقر [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) لتنزيله.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/redact_annotations/annotated_redacted.xlsx)
