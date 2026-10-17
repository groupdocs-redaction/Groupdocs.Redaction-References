---
title: "الفئة EraseMetadataRedaction"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يمثل حجبًا للبيانات الوصفية يمحو جميع البيانات الوصفية أو تلك المتطابقة مع فلاتر MetadataFilters المحددة من المستند."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/erasemetadataredaction/
is_root: false
weight: 70
---


## EraseMetadataRedaction class

يمثل حجبًا للبيانات الوصفية يمحو جميع البيانات الوصفية أو تلك المتطابقة مع فلاتر MetadataFilters المحددة من المستند.

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document metadata redactions: https://docs.groupdocs.com/redaction/net/metadata-redactions/

يعرض نوع EraseMetadataRedaction الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/) | ينشئ مثيلًا جديدًا من الفئة EraseMetadataRedaction، مما يمسح جميع البيانات الوصفية. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/#filter) | يُنشئ مثيلاً جديدًا من EraseMetadataRedaction، يمسح البيانات الوصفية التي تطابق `MetadataFilters` المحددة. |

### الطرق
| طريقة | الوصف |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | يطبق الحذف على مثيل تنسيق معين. (موروث من [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (موروث من [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/description/) | وصف الحذف ومعامِلاته. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | المرشح المستخدم لاختيار جميع البيانات الوصفية أو بعضها، مثل المؤلف أو الشركة. (موروث من [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # مسح جميع البيانات الوصفية
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # مسح حقل المؤلف فقط
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Guides
أدلة المهام التي تستخدم `EraseMetadataRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### انظر أيضًا
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
