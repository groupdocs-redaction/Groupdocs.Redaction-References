---
title: "أساسيات التعديل"
linkTitle: "Redaction basics"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "توضح هذه المقالة كيف يمكن لمطوري بايثون تطبيق تعديل البيانات الوصفية، الصور، التعليقات والنص في مستنداتهم. يتم دعم مجموعة واسعة من صيغ المستندات، مثل PDF، DOC، DOCX، PPT، PPTX، XLS، XLSX وغيرها."
type: docs
url: /ar/python-net/guides/redaction-basics/
is_root: false
weight: 40
---


يدعم GroupDocs.Redaction مجموعة فعّالة من ميزات تعديل المستندات. يتيح تطبيق التعديلات على [نص](), [بيانات وصفية](), [تعليقات](), [صور]().

يتم دعم مجموعة واسعة من صيغ المستندات، مثل: PDF، DOC، DOCX، PPT، PPTX، XLS، XLSX وغيرها. راجع القائمة الكاملة للصيغ المدعومة في مقالة [صيغ المستندات المدعومة]().

## Redaction types

يأتي GroupDocs.Redaction مع الأنواع التالية من التعديلات:

| النوع | الوصف | الفئات |
| --- | --- | --- |
| [Text]() | Replaces or hides with color block a portion of text within document body | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) |
| [Metadata]() | Replace metadata values with empty ones or redacts metadata texts | [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/), [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) |
| [Annotations]() | Deletes annotations from document or redacts its texts | [DeleteAnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/), [AnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) |
| [Images]() | Replaces specific area of an image with a colored box | [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) |
| [Pages]() | Removes specific range of pages (slides, worksheets, etc.) | [RemovePageRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) |

## Apply redaction

تطبيق التعتيم على مستند يتم عبر طريقة [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) . نتيجةً لذلك، ستحصل على كائن [RedactorChangeLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/) يحتوي على سجل لكل تعتيم تم تطبيقه. يحتوي السجل على إشارة إلى كائن [Redacton](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redaction/) بما في ذلك خياراته، حالة العملية (انظر أدناه) والوصف النصي عند الحاجة. إذا فشل تعتيم واحد على الأقل، سترى [Status == RedactionStatus.Failed](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/):

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def apply_redaction():
    # حدد خيارات الإخفاء
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # حمّل المستند المراد حذفه
    with Redactor("./sample.docx") as redactor:
        # تطبيق الحجب
        result = redactor.apply(ex_red)

        if result.status != RedactionStatus.FAILED:
            # احفظ المستند المُخفى بجوار ملف المصدر
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    apply_redaction()
```

`sample.docx` هو الملف النموذجي المستخدم في هذا المثال. انقر على [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) لتنزيله.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_redaction/sample_redacted.docx)

جميع الحالات الممكنة لتعداد [RedactionStatus](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) مدرجة في هذا الجدول:

| الحالة | الوصف | الأسباب المحتملة |
| --- | --- | --- |
| *Applied* | تم تطبيق التعتيم بالكامل وبنجاح | تم تطبيق جميع العمليات داخل عملية التعتيم بنجاح |
| *PartiallyApplied* | تم تطبيق التعتيم فقط على جزء من مطابقاته | 1) تم تجاوز حدود التجربة للاستبدالات2) تم رفض تغيير واحد على الأقل من قبل المستخدم |
| *Skipped* | تم تخطي التعتيم (لم يتم تطبيقه) | 1) تم تجاوز حدود التجربة للتعتيمات2) لا يمكن تطبيق التعتيم على هذا النوع من المستندات3) تم رفض جميع الاستبدالات من قبل المستخدم ولم تُجرى أي تغييرات |
| *Failed* | فشل التعتيم مع استثناء | حدث استثناء أثناء عملية التعتيم |

للحصول على معلومات تفصيلية، يجب التنقل عبر سجلات التعتيم في [RedactorChangeLog.RedactionLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/redaction_log/) والتحقق من خاصية [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) لأي عنصر بحالة غير *Applied*:

```python
result = redactor.apply(redaction)
if result.status != RedactionStatus.FAILED:
    # بشكل افتراضي، يتم حفظ المستند المُعتّم بصيغة PDF
    save_options = SaveOptions()
    save_options.add_suffix = True
    save_options.rasterize_to_pdf = True
    save_options.redacted_file_suffix = "redacted"
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}")
else:
    # تفريغ جميع التعتيمات الفاشلة أو المتخطاة
    print("Redaction failed!")
    for log_entry in result.redaction_log:
        if log_entry.result.status != RedactionStatus.APPLIED:
            print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")
```

## Apply multiple redactions

يمكنك تطبيق عددٍ غير محدود من التعتيمات حسب الحاجة في استدعاء واحد لطريقة [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) ، حيث أن النسخة المتعددة للوظيفة تقبل مصفوفة من التعتيمات وسياسة التعتيم. في هذه الحالة، سيتم تطبيق التعتيمات بالترتيب نفسه الذي تظهر به في المصفوفة. كبديل لتحديد مجموعات التعتيم في الشيفرة الخاصة بك، يمكنك إنشاء ملف XML يحتوي على سياسة التعتيم، كما هو موضح في [here]().

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    RegexRedaction,
    ReplacementOptions,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def apply_multiple_redactions():
    # حدد لون صندوق التعديل
    color = Color.from_argb(255, 220, 20, 60)

    # قدّم قائمة بالتعتيمات لتطبيقها بالترتيب
    redaction_list = [
        ExactPhraseRedaction("John Doe", ReplacementOptions("[Client]")),
        RegexRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # حمّل المستند المراد حذفه
    with Redactor("./sample.docx") as redactor:
        # تطبيق قائمة الإخفاءات
        result = redactor.apply(redaction_list)

        if result.status != RedactionStatus.FAILED:
            # بشكل افتراضي، يتم حفظ المستند المُعتّم بصيغة PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)
        else:
            # تفريغ جميع التعتيمات الفاشلة أو المتخطاة
            print("Redaction failed!")
            for log_entry in result.redaction_log:
                if log_entry.result.status != RedactionStatus.APPLIED:
                    print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")

if __name__ == "__main__":
    apply_multiple_redactions()
```

`sample.docx` هو الملف النموذجي المستخدم في هذا المثال. انقر على [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) لتنزيله.

  
```text
Binary file (PDF, 1.2 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_multiple_redactions/sample_redacted.pdf)
