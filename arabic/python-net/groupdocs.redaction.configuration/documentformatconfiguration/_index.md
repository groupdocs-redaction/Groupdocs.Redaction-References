---
title: "الفئة DocumentFormatConfiguration"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يمثل مرجع نوع لفئة مشتقة من DocumentFormatInstance وقائمة بامتدادات الملفات المدعومة لتسريع اكتشاف الصيغ."
type: docs
url: /ar/python-net/groupdocs.redaction.configuration/documentformatconfiguration/
is_root: false
weight: 10
---


## DocumentFormatConfiguration class

يمثل مرجع نوع لفئة مشتقة من [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) وقائمة بامتدادات الملفات المدعومة لتسريع اكتشاف الصيغة.

اعرف المزيد

- More details about **GroupDocs.Redaction** configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

يعرض نوع DocumentFormatConfiguration الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/__init__/) | يُنشئ مثيلًا جديدًا من DocumentFormatConfiguration. |

### الطرق
| طريقة | الوصف |
| :- | :- |
| [supports_extension](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/#file_extension) | يتحقق مما إذا كان امتداد الملف المحدد يمكن معالجته كـ DocumentType. |
| [supports_extension_file](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_file/) |  |
| [supports_extension_string](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_string/) |  |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [document_type](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/document_type/) | نوع الفئة التي ترث من [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |
| [extension_filter](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/extension_filter/) | قائمة الامتدادات المفصولة بفواصل (على سبيل المثال ".pdf")، غير حساسة لحالة الأحرف. |
| [initialization_data](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/initialization_data/) | البيانات المطلوبة لتهيئة [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |

### مثال

```python
from groupdocs.redaction import DocumentFormatConfiguration

# إنشاء تكوين تنسيق مخصص
config = DocumentFormatConfiguration()
config.ExtensionFilter = ".psd"
config.DocumentType = MyAdobePhotoshopFormatInstance
```

### انظر أيضًا
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
