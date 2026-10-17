---
title: "تشويه النص"
linkTitle: "Text redaction"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "توضح هذه المقالة كيف يتيح لك Python redaction API تشويه البيانات الحساسة أو الخاصة بسهولة من مستنداتك. يمكنك تطبيق تشويه النص باستخدام عبارة دقيقة أو تعبير منتظم للوثائق ذات الصيغ المختلفة مثل PDF، DOC، DOCX، PPT، PPTX، XLS، XLSX وغيرها."
type: docs
url: /ar/python-net/guides/text-redactions/
is_root: false
weight: 50
---


يتيح GroupDocs.Redaction تشويه البيانات الحساسة أو الخاصة بسهولة من مستنداتك. أكثر حالات التشويه شيوعًا هي إزالة نص من مستند.

باستخدام GroupDocs.Redaction API يمكنك تطبيق تشويه النص باستخدام عبارة دقيقة أو [تعبير منتظم](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expressions) للوثائق ذات الصيغ المختلفة مثل PDF، DOC، DOCX، PPT، PPTX، XLS، XLSX وغيرها. راجع القائمة الكاملة في مقالة [صيغ المستندات المدعومة]().

## Use exact phrase redaction

في المثال أدناه، نطبق تشويهًا نصيًا، نستبدل العبارة الدقيقة الشخصية "John Doe" بـ "\[personal\]" (أو أي رمز استثناء):

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_exact_phrase():
    # حدد خيارات الإخفاء
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # حمّل المستند المراد حذفه
    with Redactor("./sample.docx") as redactor:
        # تطبيق الحجب
        result = redactor.apply(ex_red)

        # احفظ المستند المُخفى بجوار ملف المصدر
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_exact_phrase()
```

`sample.docx` هو ملف العينة المستخدم في هذا المثال. انقر [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) لتنزيله.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_exact_phrase/sample_redacted.docx)

بشكل افتراضي، البحث عن العبارة الدقيقة غير حساس لحالة الأحرف. للحصول على تعديل حساس لحالة الأحرف، هناك معامل في المُنشئ وخصيصة عامة مقابلة:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_case_sensitive_phrase():
    # تمكين المطابقة الحساسة لحالة الأحرف
    case_sensitive = True

    # حدد خيارات الإخفاء
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", case_sensitive, repl_opt)

    # حمّل المستند المراد حذفه
    with Redactor("./sample.docx") as redactor:
        # تطبيق الحجب
        result = redactor.apply(ex_red)

        # احفظ المستند المُخفى بجوار ملف المصدر
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_case_sensitive_phrase()
```

`sample.docx` هو ملف العينة المستخدم في هذا المثال. انقر [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) لتنزيله.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_case_sensitive_phrase/sample_redacted.docx)

إذا كنت بحاجة إلى صندوق ملون فوق النص المُحذوف، يمكنك استخدام اللون بدلاً من سلسلة الاستبدال. سيقوم التعديل بمسح النص المطابق ووضع مستطيل باللون المحدد مكان النص المُحذوف:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_color_box():
    # حدد لون صندوق التعديل
    color = Color.from_argb(255, 220, 20, 60)

    # حدد خيارات الإخفاء
    repl_opt = ReplacementOptions(color)
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # حمّل المستند المراد حذفه
    with Redactor("./sample.docx") as redactor:
        # تطبيق الحجب
        result = redactor.apply(ex_red)

        # احفظ المستند المُخفى بجوار ملف المصدر
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_color_box()
```

`sample.docx` هو ملف العينة المستخدم في هذا المثال. انقر [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) لتنزيله.

  
```text
Binary file (DOCX, 17 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_color_box/sample_redacted.docx)

قد تحتاج إلى تطبيق التعديل على مستند من اليمين إلى اليسار، مثل العربية أو العبرية. المثال التالي يوضح كيفية تطبيق ExactPhraseRedaction على مستند PDF عربي:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_right_to_left_text():
    # حدد خيارات التعديل باستخدام عبارة عربية
    repl_opt = ReplacementOptions("[test]")
    ex_red = ExactPhraseRedaction("انتقد", repl_opt)

    # حمّل المستند المراد حذفه
    with Redactor("./arabic.pdf") as redactor:
        # تطبيق الحجب
        result = redactor.apply(ex_red)

        # احفظ المستند المُخفى بجوار ملف المصدر
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_right_to_left_text()
```

`arabic.pdf` هو ملف العينة المستخدم في هذا المثال. انقر [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/arabic.pdf) لتنزيله.

  
```text
Binary file (PDF, 23 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_right_to_left_text/arabic_redacted.pdf)

## Use regular expression

خلف الكواليس، تعديل "العبارة الدقيقة" يعمل عبر التعبيرات النمطية، التي تُعد النهج الأساسي للتعديل. في المثال أدناه، نقوم بحذف أي نص يطابق "رقمان، مسافة أو لا شيء، رقمان، مرة أخرى مسافة وستة أرقام" باستخدام صندوق أزرق اللون:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_regex():
    # حدد لون صندوق التعديل
    color = Color.from_argb(255, 220, 20, 60)

    # حدد خيارات الإخفاء
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", repl_opt)

    # حمّل المستند المراد حذفه
    with Redactor("./sample.docx") as redactor:
        # تطبيق الحجب
        result = redactor.apply(reg_red)

        # احفظ المستند المُخفى بجوار ملف المصدر
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_regex()
```

`sample.docx` هو ملف العينة المستخدم في هذا المثال. انقر [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) لتنزيله.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_regex/sample_redacted.docx)

إذا كنت بحاجة إلى تعديل فقرة كاملة، قد تحتاج أيضًا إلى استخدام RegexRedaction. المثال التالي يوضح كيفية تعديل الفقرة بالكامل في مستند PDF:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_whole_paragraph():
    # حدد لون صندوق التعديل
    color = Color.from_argb(255, 220, 20, 60)

    # حدد خيارات التعديل التي تطابق فقرة كاملة
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("(Lorem(\n|.)+?urna)", repl_opt)

    # حمّل المستند المراد حذفه
    with Redactor("./sample.pdf") as redactor:
        # تطبيق الحجب
        result = redactor.apply(reg_red)

        # احفظ المستند المُخفى بجوار ملف المصدر
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_whole_paragraph()
```

`sample.pdf` هو ملف العينة المستخدم في هذا المثال. انقر [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.pdf) لتنزيله.

  
```text
Binary file (PDF, 68 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_whole_paragraph/sample_redacted.pdf)
