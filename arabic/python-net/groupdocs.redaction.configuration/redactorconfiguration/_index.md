---
title: "الفئة RedactorConfiguration"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يوفر وصولًا إلى قائمة الصيغ المدعومة، الصيغ المدمجة وصيغ المستخدم المخصصة."
type: docs
url: /ar/python-net/groupdocs.redaction.configuration/redactorconfiguration/
is_root: false
weight: 20
---


## RedactorConfiguration class

يوفر وصولًا إلى قائمة الصيغ المدعومة، الصيغ المدمجة وصيغ المستخدم المخصصة.

المزيد:

- More details about GroupDocs.Redaction configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

يعرض نوع RedactorConfiguration الأعضاء التالية:

### الطرق
| طريقة | الوصف |
| :- | :- |
| [find_format](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/#file_extension) | يبحث عن تكوينات الصيغ لامتداد ملف معين. |
| [find_format_file](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_file/) |  |
| [find_format_string](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_string/) |  |
| [get_instance](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/) | يعيد مثيلًا وحيدًا مع التكوين الافتراضي للصيغ المدمجة. |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [available_formats](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/available_formats/) | قائمة الصيغ المعترف بها، انظر [`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/). |

### مثال

```python
# أضف معالج صيغة مخصص للمستخدم
adobe_photoshop_settings = DocumentFormatConfiguration()
adobe_photoshop_settings.extension_filter = ".psd"
adobe_photoshop_settings.document_type = MyAdobePhotoshopFormatInstance

config = RedactorConfiguration.get_instance()
config.available_formats.add(adobe_photoshop_settings)
```

```python
# استرجع معالج صيغة مدمج أو مخصص للمستخدم
config = RedactorConfiguration.get_instance()
format_settings = config.find_format(".psd")
```

### انظر أيضًا
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
