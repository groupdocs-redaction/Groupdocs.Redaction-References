---
title: "فئة MetadataSearchRedaction"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يمثل إزالة بيانات تعريف تبحث وتزيل بيانات التعريف باستخدام التعابير النمطية، مع مطابقة المفاتيح و/أو القيم."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/metadatasearchredaction/
is_root: false
weight: 140
---


## MetadataSearchRedaction class

يمثل إزالة بيانات تعريف تبحث وتزيل بيانات التعريف باستخدام التعابير النمطية، مع مطابقة المفاتيح و/أو القيم.

- More details about applying redactions: <https://docs.groupdocs.com/redaction/net/redaction-basics/>
- More details about document metadata redactions: <https://docs.groupdocs.com/redaction/net/metadata-redactions/>

يعرض نوع MetadataSearchRedaction الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement) | ينشئ مثيلاً جديداً من فئة MetadataSearchRedaction، باستخدام القيمة لمطابقة العناصر المحذوفة. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement-key_pattern) | ينشئ مثيلاً جديداً من MetadataSearchRedaction، باستخدام اسم العنصر والقيمة لمطابقة العناصر المحذوفة. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement) | ينشئ مثيلاً جديداً من فئة MetadataSearchRedaction، باستخدام القيمة لمطابقة العناصر المحذوفة. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement-key_regex) | ينشئ مثيلاً جديداً من MetadataSearchRedaction باستخدام اسم العنصر والقيمة لمطابقة العناصر المحذوفة. |

### الطرق
| طريقة | الوصف |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | يطبق الحذف على مثيل تنسيق معين. (موروث من [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (موروث من [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/description/) | وصف Redaction، يحتوي على اسمه ومعاماته. |
| [key_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/key_expression/) | التعبير النمطي لمطابقة اسم (المفتاح) عنصر البيانات الوصفية. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/replacement/) | قيمة الاستبدال النصي. |
| [value_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/value_expression/) | التعبير النمطي لمطابقة نص القيمة لعنصر البيانات الوصفية. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | المرشح المستخدم لاختيار جميع البيانات الوصفية أو بعضها، مثل المؤلف أو الشركة. (موروث من [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # إخفاء أي قيمة بيانات وصفية تطابق النمط
    redaction = MetadataSearchRedaction("Company Ltd.", "--company--")
    redaction.filter = MetadataFilters.COMPANY
    redactor.apply(redaction)
    redactor.save()
```

### Guides
دليل المهام الذي يستخدم `MetadataSearchRedaction`:

* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)

### انظر أيضًا
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
