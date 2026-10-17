---
title: "فئة DocumentFormatInstance"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يمثل تنسيقًا محددًا لمستند ويمكن تنفيذه لإضافة أنواع مستند مخصصة."
type: docs
url: /ar/python-net/groupdocs.redaction.integration/documentformatinstance/
is_root: false
weight: 10
---


## DocumentFormatInstance class

يمثل تنسيقًا محددًا لمستند ويمكن تنفيذه لإضافة أنواع مستند مخصصة.

اعرف المزيد

- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

نوع DocumentFormatInstance يكشف عن الأعضاء التالية:

### الطرق
| طريقة | الوصف |
| :- | :- |
| [initialize](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/#config-settings) | يُنشئ مثيل معالج تنسيق المستند. |
| [initialize_document_format_configuration](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize_document_format_configuration/) |  |
| [is_redaction_accepted](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/#description) | يتحقق من تنفيذ [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) ويستدعيه إذا تم تحديده. |
| [is_redaction_accepted_redaction_description](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted_redaction_description/) |  |
| [load](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load/#input) | يقوم بتحميل المستند من تدفق. |
| [load_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_streams/) |  |
| [perform_binary_check](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/#input) | يتحقق مما إذا كان التدفق المعطى يحتوي على مستند مدعوم من قبل هذا المثيل من التنسيق. |
| [perform_binary_check_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_stream/) |  |
| [perform_binary_check_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_streams/) |  |
| [save](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save/#output) | يحفظ المستند إلى تدفق. |
| [save_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_streams/) |  |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/password/) | كلمة المرور للمستندات المحمية بكلمة مرور. |

### مثال

```python
class DummyDocument(DocumentFormatInstance):
    def load(self, output: io.RawIOBase) -> None:
        # تحميل محتوى الملف
        pass

    def save(self, output: io.RawIOBase) -> None:
        # حفظ التغييرات إلى الملف
        pass
```

```python
class MyCustomHandler(DocumentFormatInstance):
    def __init__(self):
        self.my_property = None

    def initialize(self, config: DocumentFormatConfiguration) -> None:
        super().initialize(config)
        if "MyProperty" in config.initialization_data:
            self.my_property = config.initialization_data["MyProperty"]
```

### انظر أيضًا
* module [`groupdocs.redaction.integration`](/redaction/python-net/groupdocs.redaction.integration/)
