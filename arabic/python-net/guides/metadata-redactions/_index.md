---
title: "إخفاءات البيانات الوصفية"
linkTitle: "Metadata redactions"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "توضح هذه المقالة كيف يسمح Python redaction API لك باستبدال أو إزالة البيانات الوصفية باستخدام الفلاتر أو البحث بالتعبير النمطي."
type: docs
url: /ar/python-net/guides/metadata-redactions/
is_root: false
weight: 70
---


مع GroupDocs.Redaction API يمكنك تطبيق إخفاءات البيانات الوصفية على مستندات بصيغ مختلفة مثل PDF و DOC و DOCX و PPT و PPTX و XLS و XLSX وغيرها. راجع القائمة الكاملة في مقالة [supported document formats]().

توفر GroupDocs.Redactions API مرن يتيح استبدال أو إزالة البيانات الوصفية باستخدام الفلاتر أو البحث بالتعبير النمطي.

## Filter metadata

الوظيفة الأساسية لجميع الإخفاءات، المستمدة من الفئة الأساسية [MetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) هي *metadata filtering* وهي إلزامية لإخفاءات البيانات الوصفية. تستخدم تعدادًا معلمًا [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/)، يحتوي على عناصر لأكثر الإدخالات الوصفية شيوعًا. يمكنك تعيين الفلتر إلى *All*، أو أي تركيبة من البيانات الوصفية. على سبيل المثال، يحدد المثال أدناه الفلتر إلى *Author* و *Manager* و *NameOfApplication* - للإخفاء النصي أو تنظيفها.

```python
# إخفاء مشتق من MetadataRedaction
redaction.filter = MetadataFilters.AUTHOR | MetadataFilters.MANAGER | MetadataFilters.NAME_OF_APPLICATION
```

فيما يلي الجدول مع القائمة الكاملة لعناصر [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/):

| الفلتر | القيمة الرقمية | الوصف |
| --- | --- | --- |
| *None* | 0 | إعداد الفلتر فارغ، لا يطابق أي عناصر وصفية |
| *Author* | 1 | مؤلف المستند |
| *الفئة* | 2 | فئة المستند |
| *تعليقات* | 4 | تعليق المستند |
| *شركة* | 8 | شركة المؤلف |
| *ContentStatus* | 16 | حالة المحتوى |
| *CreatedTime* | 32 | وقت الإنشاء |
| *HyperlinkBase* | 64 | قاعدة الارتباط التشعبي |
| *LastPrinted* | 128 | تاريخ ووقت الطباعة الأخيرة |
| *LastSavedBy* | 256 | آخر حفظ بواسطة المستخدم |
| *LastSavedTime* | 1024 | تاريخ ووقت الحفظ الأخير |
| *NameOfApplication* | 2048 | اسم التطبيق الذي تم إنشاء المستند فيه |
| *Manager* | 4096 | اسم مدير المؤلف |
| *RevisionNumber* | 8192 | رقم المراجعة |
| *Subject* | 16384 | موضوع المستند |
| *Template* | 32768 | اسم قالب المستند |
| *Title* | 65536 | عنوان المستند |
| *TotalEditingTime* | 131072 | إجمالي وقت التحرير |
| *الإصدار* | 262144 | إصدار المستند |
| *الوصف* | 524288 | وصف المستند |
| *الكلمات المفتاحية* | 1048576 | الكلمات المفتاحية للمستند |
| *نوع_المحتوى* | 2097152 | نوع المحتوى |
| *الكل* | 2147483647 | جميع أنواع عناصر البيانات الوصفية |

## Clean metadata

يمكنك استبدال جميع البيانات الوصفية أو بعضها في المستند بقيم فارغة (خالية أو قليلة) باستخدام الفئة [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/) . المثال أدناه يمسح جميع خصائص المستند:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_all_metadata():
    # حدد خيارات الحذف لمسح جميع البيانات الوصفية
    met_red = EraseMetadataRedaction(MetadataFilters.ALL)

    # حمّل المستند المراد حذفه
    with Redactor("./sample.docx") as redactor:
        # تطبيق الحجب
        result = redactor.apply(met_red)

        # احفظ المستند المُخفى بجوار ملف المصدر
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_all_metadata()
```

`sample.docx` هو ملف العينة المستخدم في هذا المثال. انقر على [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) لتنزيله.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/clean_all_metadata/sample_redacted.docx)

يمكنك تحديد [MetadataFilter.All](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) أو استخدام المُنشئ الافتراضي لمسح جميع البيانات الوصفية داخل المستند المحدد، Custom - لمسح جميع إدخالات البيانات الوصفية المخصصة.

## Redact metadata

يمكنك استخدام [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) لإزالة البيانات الحساسة من بيانات المستند الوصفية باستخدام التعابير النمطية. على سبيل المثال، يمكننا إزالة أي إشارة إلى "Company Ltd.":

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction

def redact_metadata():
    # حدد خيارات الحذف: نمط البحث وسلسلة الاستبدال
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # حمّل المستند المراد حذفه
    with Redactor("./sample.docx") as redactor:
        # تطبيق الحجب
        result = redactor.apply(met_red)

        # احفظ المستند المُخفى بجوار ملف المصدر
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata()
```

`sample.docx` هو ملف العينة المستخدم في هذا المثال. انقر على [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) لتنزيله.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata/sample_redacted.docx)

الحجة الأولى هي تعبير نمطي، والثانية هي سلسلة استبدال. يمكنك أيضًا تحديد نطاق الحذف عن طريق تعيين الفلتر، مثلًا إلى [MetadataFilter.Company](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/). - سيترك مطابقة التعابير النمطية غير مُعدلة في جميع عناصر البيانات الوصفية، باستثناء خاصية "Company".

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

def redact_metadata_with_filter():
    # حدد خيارات الحذف: نمط البحث وسلسلة الاستبدال
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # قصر نطاق الحذف على عنصر البيانات الوصفية Company فقط
    met_red.filter = MetadataFilters.COMPANY

    # حمّل المستند المراد حذفه
    with Redactor("./sample.docx") as redactor:
        # تطبيق الحجب
        result = redactor.apply(met_red)

        # احفظ المستند المُخفى بجوار ملف المصدر
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata_with_filter()
```

`sample.docx` هو ملف العينة المستخدم في هذا المثال. انقر على [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) لتنزيله.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata_with_filter/sample_redacted.docx)

## Metadata redaction status

تنطبق جميع عمليات حذف البيانات الوصفية على كل عنصر بيانات وصفية على حدة، وحتى إذا فشل حذف عنصر معين، سيتم تحديث باقي العناصر. يمكنك العثور على قائمة بالعناصر الفاشلة، المتخطاة (المرفوضة) وأسباب ذلك في خاصية [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) لـ [RedactorLogEntry.Result](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).
