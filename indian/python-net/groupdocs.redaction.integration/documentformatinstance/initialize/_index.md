---
title: "initialize मेथड"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "दस्तावेज़ फ़ॉर्मेट हैंडलर उदाहरण को प्रारंभ करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/
is_root: false
weight: 1010
---


## initialize {#config-settings}

दस्तावेज़ फ़ॉर्मेट हैंडलर उदाहरण को प्रारंभ करता है।

```python
def initialize(self, config, settings):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| config | `DocumentFormatConfiguration` | फ़ॉर्मेट कॉन्फ़िगरेशन। |
| settings | `RedactorSettings` | रेडैक्शन प्रक्रिया के लिए डिफ़ॉल्ट सेटिंग्स। |

**Returns:** None.

### उदाहरण

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

# कस्टम फ़ॉर्मेट को रजिस्टर करें
my_config = DocumentFormatConfiguration()
my_config.extension_filter = ".foo"
my_config.document_type = MyCustomHandler
my_config.initialization_data["MyProperty"] = "bar"

redactor_config = RedactorConfiguration.get_instance()
redactor_config.available_formats.append(my_config)
```

### संबंधित देखें
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
