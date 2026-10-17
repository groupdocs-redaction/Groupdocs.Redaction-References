---
title: "فئة Redactor"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يمثل الفئة الرئيسية التي تتحكم في عملية إخفاء المستند، مما يسمح بفتح المستندات وإخفائها وحفظها."
type: docs
url: /ar/python-net/groupdocs.redaction/redactor/
is_root: false
weight: 150
---


## Redactor class

يمثل الفئة الرئيسية التي تتحكم في عملية إخفاء المستند، مما يسمح بفتح المستندات وإخفائها وحفظها.

اعرف المزيد
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More advanced redaction topics: https://docs.groupdocs.com/redaction/net/advanced-usage/

نوع Redactor يكشف عن الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path) | ينشئ مثيلًا جديدًا من Redactor باستخدام مسار ملف. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document) | ينشئ مثيلًا جديدًا من [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) باستخدام تدفق. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options) | ينشئ مثيلًا جديدًا من [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) لمستند محمي بكلمة مرور باستخدام مساره. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options-settings) | ينشئ مثيلًا جديدًا من Redactor لمستند محمي بكلمة مرور باستخدام مساره والإعدادات. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options) | ينشئ مثيلًا جديدًا من Redactor لمستند محمي بكلمة مرور باستخدام تدفق. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options-settings) | ينشئ مثيلًا جديدًا من [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) لمستند محمي بكلمة مرور باستخدام تدفق وإعدادات. |

### الطرق
| طريقة | الوصف |
| :- | :- |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redaction) | يطبق حذفًا على المستند. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redactions) | يطبق مجموعة من عمليات الحذف على المستند. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#policy) | يطبق سياسة حذف على المستند. |
| [apply_redaction](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction/) |  |
| [apply_redaction_policy](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction_policy/) |  |
| [dispose](/redaction/python-net/groupdocs.redaction/redactor/dispose/) | يطلق الموارد. |
| [generate_preview](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#preview_options) | ينشئ صور معاينة لصفحات محددة بصيغة صورة معينة. |
| [generate_preview_preview_options](/redaction/python-net/groupdocs.redaction/redactor/generate_preview_preview_options/) |  |
| [get_document_info](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/) | يسترجع المعلومات العامة حول المستند، مثل الحجم وعدد الصفحات. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/) | يحفظ المستند إلى ملف مع الخيارات التالية: AddSuffix = True, RasterizeToPDF = True. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#save_options) | يحفظ المستند إلى ملف. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#document-rasterization_options) | يحفظ المستند إلى تدفق، بما في ذلك الموقع المخصص. |
| [save_save_options](/redaction/python-net/groupdocs.redaction/redactor/save_save_options/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactor/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactor/save_streams/) |  |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# افتح مستندًا وأزل الصفحة الأولى
with Redactor("document.pdf") as redactor:
    redactor.apply(RemovePageRedaction(PageSeekOrigin.BEGIN, 0, 1))
    redactor.save()
```

### Guides
دلائل المهام التي تستخدم `Redactor`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [Get file info](/redaction/python-net/guides/get-file-info/)

### انظر أيضًا
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
