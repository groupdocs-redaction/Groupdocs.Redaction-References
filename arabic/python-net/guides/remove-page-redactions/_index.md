---
title: "إزالة تشويهات الصفحات"
linkTitle: "Remove page redactions"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "توضح هذه المقالة كيفية إزالة الصفحات التي تحتوي على بيانات حساسة من مستندات PDF والعروض التقديمية وجداول البيانات الخاصة بك."
type: docs
url: /ar/python-net/guides/remove-page-redactions/
is_root: false
weight: 100
---


يتيح GroupDocs.Redaction إزالة الصفحات بسهولة من مستندات PDF، والشرائح من العروض التقديمية، وأوراق العمل من مستندات جداول البيانات.

باستخدام GroupDocs.Redaction API يمكنك إزالة الصفحات عن طريق تحديد نطاق الصفحات بناءً على موقعها النسبي (البداية أو النهاية)، والفهرس الصفري، وعدد الصفحات المراد إزالتها. في الوقت الحالي، الصيغ المدعومة هي: PDF، العروض التقديمية (Microsoft PowerPoint، OpenOffice Presentations)، مستندات معالجة النصوص (Microsoft Word، OpenOffice Texts، ملفات النص الغني)، جداول البيانات (Microsoft Excel، OpenOffice Spreadsheets، إلخ) والصور متعددة الإطارات.

## Remove page range

في المثال أدناه، نقوم بإزالة الصفحات الثانية والثالثة والرابعة من المستند، إذا كان المستند يحتوي على عدد كافٍ من الصفحات:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_page_range():
    # حمّل المستند المراد حذفه
    with Redactor("./multipage_sample.pdf") as redactor:
        # الحصول على معلومات المستند
        doc_info = redactor.get_document_info()

        # يتطلب ما لا يقل عن 4 صفحات
        if doc_info.page_count > 3:
            # إزالة 3 صفحات بدءًا من الصفحة الثانية (الفهرس الصفري 1)
            rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)

            # تطبيق الحجب
            result = redactor.apply(rem_opt)

            # احفظ المستند المُخفى بجوار ملف المصدر
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_page_range()
```

`multipage_sample.pdf` هو ملف العينة المستخدم في هذا المثال. انقر [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) لتنزيله.

## Remove last page

في بعض الحالات قد تحتاج إلى حذف الصفحة الأخيرة أو عدد من الصفحات، بغض النظر عن عدد الصفحات الموجودة.

يوضح المثال التالي كيفية إزالة الصفحة الأخيرة من مستند:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # إزالة صفحة واحدة محسوبة من نهاية المستند
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    # حمّل المستند المراد حذفه
    with Redactor("./multipage_sample.pdf") as redactor:
        # الحصول على معلومات المستند
        doc_info = redactor.get_document_info()

        # يتطلب ما لا يقل عن صفحتين حتى لا يبقى المستند فارغًا
        if doc_info.page_count > 1:
            # تطبيق الحجب
            result = redactor.apply(rem_opt)

            # احفظ المستند المُخفى بجوار ملف المصدر
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_last_page()
```

`multipage_sample.pdf` هو ملف العينة المستخدم في هذا المثال. انقر [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) لتنزيله.

  
```text
Binary file (PDF, 190 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_last_page/multipage_sample_redacted.pdf)

## Remove frame from image

في حالة صورة متعددة الإطارات قد تحتاج إلى حذف عدد من الإطارات (المعالجة كـ "صفحات").

يوضح المثال التالي كيفية إزالة 3 إطارات من صورة GIF متحركة:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_frame_from_image():
    # إزالة الإطارات بدءًا من الإطار الثالث (الفهرس الصفري 2)
    rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 2, 5)

    # تحميل صورة متعددة الإطارات لتشويهها
    with Redactor("./sample.gif") as redactor:
        # الحصول على معلومات المستند
        doc_info = redactor.get_document_info()

        # يتطلب ما لا يقل عن 7 إطارات
        if doc_info.page_count >= 7:
            # تطبيق الحجب
            result = redactor.apply(rem_opt)

            # احفظ الصورة المشوهة بجوار ملف المصدر
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_frame_from_image()
```

`sample.gif` هو ملف العينة المستخدم في هذا المثال. انقر [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/sample.gif) لتنزيله.

  
```text
Binary file (GIF, 704 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_frame_from_image/sample_redacted.gif)
