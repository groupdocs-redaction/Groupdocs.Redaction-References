---
title: "إخفاءات الصور"
linkTitle: "Image redactions"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "توضح هذه المقالة كيفية إخفاء البيانات ذات الطبيعة الحساسة من الصور بمختلف الصيغ مثل JPG و PNG و TIFF وغيرها."
type: docs
url: /ar/python-net/guides/image-redactions/
is_root: false
weight: 60
---


يقدم GroupDocs.Redactions مجموعة من الميزات لإخفاء البيانات ذات الطبيعة الحساسة من الصور بمختلف الصيغ مثل JPG و PNG و TIFF وغيرها. راجع القائمة الكاملة في مقالة [supported document formats]().

يدعم GroupDocs.Redaction طريقتين لإخفاء الصور، كلاً في ملفات صور منفصلة وصور مدمجة:
*   You can put a colored box over a given area, such as header, footer, or an area, where customer's data are expected to appear.
*   You can use any 3-rd party OCR engine to process the image, search it for text and redact sensitive data within the image.   

يتيح GroupDocs.Redaction for Python عبر .NET أيضًا لك تغيير بيانات تعريف الصورة (مثال: تعديل بيانات EXIF لصورة أو العمل كـ "ممحاة EXIF").

## Redact image area

من أجل إخفاء منطقة الصورة، عليك استخدام الفئة [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/).

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_image_area():
    # حدد موضع الزاوية العليا اليسرى للمنطقة التي سيتم إخفاؤها
    sample_point = Point(385, 485)
    # حدد حجم المنطقة التي تحتاج إلى إخفائها
    sample_size = Size(1793, 2069)
    # حدد لون صندوق التعديل
    color = Color.from_argb(255, 220, 20, 60)

    # حدد خيارات الإخفاء
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # حمّل المستند المراد حذفه
    with Redactor("./sample.jpg") as redactor:
        # تطبيق الحجب
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # بشكل افتراضي، يتم حفظ المستند المُعتّم بصيغة PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_image_area()
```

`sample.jpg` هو ملف العينة المستخدم في هذا المثال. انقر [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) لتنزيله.

  
```text
Binary file (PDF, 2.7 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_image_area/sample_redacted.pdf)

إذا تعذر تطبيق الإخفاء على هذا النوع من الملفات، مثل مستند MS Word بدون صور مدمجة، فإن [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) سيكون [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Clean image metadata

يوضح المثال التالي كيفية تعديل بيانات EXIF (مسحها) من صورة أو أي صورة أخرى:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_image_metadata():
    # حدد خيارات الإخفاء لإزالة جميع بيانات تعريف الصورة (مثل EXIF)
    er_opt = EraseMetadataRedaction(MetadataFilters.ALL)

    # حمّل الصورة التي سيتم إخفاؤها
    with Redactor("./sample.jpg") as redactor:
        # تطبيق الحجب
        result = redactor.apply(er_opt)

        # احفظ الصورة المشوهة بجوار ملف المصدر
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_image_metadata()
```

`sample.jpg` هو ملف العينة المستخدم في هذا المثال. انقر [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) لتنزيله.

  
```text
Binary file (JPG, 3.1 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/clean_image_metadata/sample_redacted.jpg)

إذا تعذر تطبيق الإخفاء على هذا النوع من الملفات، مثل صورة BMP، فإن [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) سيكون [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Redact embedded images

يمكنك إخفاء منطقة الصورة داخل جميع أنواع الصور المدمجة داخل مستند.

يوضح المثال التالي كيفية إخفاء جميع الصور المدمجة داخل مستند Microsoft Word:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_embedded_images():
    # حدد موضع الزاوية العليا اليسرى للمنطقة التي سيتم إخفاؤها
    sample_point = Point(516, 311)
    # حدد حجم المنطقة التي تحتاج إلى إخفائها
    sample_size = Size(170, 35)
    # حدد لون صندوق التعديل
    color = Color.from_argb(255, 220, 20, 60)

    # حدد خيارات الإخفاء
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # حمّل المستند المراد حذفه
    with Redactor("./sample.docx") as redactor:
        # طبق الإخفاء على جميع الصور المدمجة
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # بشكل افتراضي، يتم حفظ المستند المُعتّم بصيغة PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_embedded_images()
```

`sample.docx` هو ملف العينة المستخدم في هذا المثال. انقر [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.docx) لتنزيله.

  
```text
Binary file (PDF, 1022 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_embedded_images/sample_redacted.pdf)

إذا تعذر تطبيق الإخفاء على هذا النوع من الملفات، مثل مستند جدول بيانات، فإن [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) سيكون [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Multi-frame images

يمكنك إزالة الإطارات من صورة متعددة الإطارات مع أصل وعدد إطارات محددين. لمزيد من المعلومات راجع مقالة [remove page redactions]().

بعض صيغ الصور، مثل مستندات DjVu، تتطلب [pre-rasterization]() وحفظًا إضافيًا بصيغة PDF.
