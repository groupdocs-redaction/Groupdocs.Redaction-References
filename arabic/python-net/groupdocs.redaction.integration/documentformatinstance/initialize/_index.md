---
title: "طريقة initialize"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يُنشئ مثيل معالج تنسيق المستند."
type: docs
url: /ar/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/
is_root: false
weight: 1010
---


## initialize {#config-settings}

يُنشئ مثيل معالج تنسيق المستند.

```python
def initialize(self, config, settings):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| config | `DocumentFormatConfiguration` | تهيئة التنسيق. |
| settings | `RedactorSettings` | الإعدادات الافتراضية لعملية الحجب. |

**Returns:** None.

### مثال

```python
from groupdocs.redaction.integration import DocumentFormatInstance, DocumentFormatConfiguration, RedactorConfiguration

class MyCustomHandler(DocumentFormatInstance):
    def __init__(self):
        super().__init__()
        self.my_property = None

    def initialize(self, config, settings=None):
        super().initialize(config, settings)
        if "MyProperty" in config.initialization_data:
            self.my_property = config.initialization_data["MyProperty"]

# تسجيل التنسيق المخصص
my_config = DocumentFormatConfiguration()
my_config.extension_filter = ".foo"
my_config.document_type = MyCustomHandler
my_config.initialization_data["MyProperty"] = "bar"

redactor_config = RedactorConfiguration.get_instance()
redactor_config.available_formats.append(my_config)
```

### انظر أيضًا
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
