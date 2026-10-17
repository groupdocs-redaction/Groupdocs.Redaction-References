---
title: "استخدم سياسات الإزالة"
linkTitle: "Use redaction policies"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "تعلم كيفية التعامل. إذا كان لديك سياسة إزالة البيانات الحساسة في الشركة على شكل قائمة من قواعد الإزالة، لا تحتاج إلى تحديدها في الشيفرة الخاصة بك. يمكنك تحديد مستند XML يحتوي على قائمة من عمليات الإزالة المكوّنة مسبقًا."
type: docs
url: /ar/python-net/guides/use-redaction-policies/
is_root: false
weight: 110
---


إذا كان لديك سياسة إزالة البيانات الحساسة في الشركة على شكل قائمة من قواعد الإزالة، لا تحتاج إلى تحديدها في الشيفرة الخاصة بك. يمكنك تحديد مستند XML يحتوي على قائمة من عمليات الإزالة المكوّنة مسبقًا.

فيما يلي مثال على ملف XML لسياسة الإزالة (تطابق خصائص الشيفرة واضح):

**RedactionPolicy.xml**

```xml
<?xml version="1.0" encoding="utf-8"?>  
<redactionPolicy xmlns="http://www.groupdocs.com/redaction">  
  <regexRedaction regularExpression="(dolor)" actionType="ReplaceString" replacement="foobar" />  
  <exactPhraseRedaction searchPhrase="dolor" caseSensitive="true" actionType="DrawBox" color="Red" />   
  
  <eraseMetadataRedaction filter="All" />  
  <metadataSearchRedaction filter="Title, Author" replacement="foobar" valueExpression="(metasearch)" keyExpression="" />  
  
  <annotationRedaction regularExpression="(anno1)" replacement="foobar" />  
  <deleteAnnotationRedaction regularExpression="(anno2)" />  
  
  <imageAreaRedaction pointX="15" pointY="17" width="200" height="10" color="#AA50FC"  />  
  <imageAreaRedaction pointX="110" pointY="120" width="60" height="20" color="Magenta"  />  
</redactionPolicy> 
```
يمكنك استخدام طريقة RedactionPolicy.save() لإنشاء مستندات XML بهذا الهيكل، مع تكوين عمليات الإزالة أثناء التشغيل.

يوضح المثال التالي كيفية حفظ [RedactionPolicy](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionpolicy/) إلى ملف XML.
 

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    ReplacementOptions,
    RegexRedaction,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def create_redaction_policy():
    # حدد لون الإزالة
    color = Color.from_argb(255, 220, 20, 60)

    # قم بتكوين عمليات الإزالة
    redactions = [
        ExactPhraseRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # أنشئ السياسة
    policy = RedactionPolicy(redactions)

    # احفظ سياسة الإزالة إلى ملف XML
    policy.save("./sample_policy.xml")
    print("Redactions policy saved to ./sample_policy.xml")

if __name__ == "__main__":
    create_redaction_policy()
```

  
```text
<?xml version="1.0"?>
<redactionPolicy>
  <exactPhraseRedaction actionType="ReplaceString" replacement="[Product]" searchPhrase="Redaction" />
  <regexRedaction actionType="DrawBox" color="#DC143C" regularExpression="\d{2}\s*\d{2}[^\d]*\d{6}" />
  <deleteAnnotationRedaction regularExpression="[.]*" />
  <eraseMetadataRedaction filter="All" />
</redactionPolicy>
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/create_redaction_policy/sample_policy.xml)

يمكنك الحصول على عدد غير محدود من السياسات حسب الحاجة، وتحميلها لإزالة تغطية مستنداتك.

المثال أدناه يحمل سياسة إخفاء من ملف XML ويطبق كل قاعدة تحتويها على مستند في استدعاء `apply` واحد:

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.options import SaveOptions

def use_redaction_policy():
    # حمّل سياسة الإخفاء من ملف XML
    policy = RedactionPolicy.load("./redaction_policy.xml")

    # حمّل المستند وطبق السياسة بالكامل في استدعاء واحد
    with Redactor("./sample.docx") as redactor:
        redactor.apply(policy)

        # احتفظ بالتنسيق الأصلي وأضف لاحقة إلى اسم الإخراج
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = False
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Redaction policy applied. Output saved to {result_path}.")

if __name__ == "__main__":
    use_redaction_policy()
```

`redaction_policy.xml` هو ملف السياسة المستخدم في هذا المثال. انقر [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/redaction_policy.xml) لتنزيله.

`sample.docx` هو المستند المُخفى في هذا المثال. انقر [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/sample.docx) لتنزيله.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/use_redaction_policy/sample_redacted.docx)
