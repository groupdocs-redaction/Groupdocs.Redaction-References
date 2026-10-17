---
title: "metode initialize"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi instance penangan format dokumen."
type: docs
url: /id/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/
is_root: false
weight: 1010
---


## initialize {#config-settings}

Menginisialisasi instance penangan format dokumen.

```python
def initialize(self, config, settings):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| config | `DocumentFormatConfiguration` | Konfigurasi format. |
| settings | `RedactorSettings` | Pengaturan default untuk proses redaksi. |

**Returns:** None.

### Contoh

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

# Daftarkan format khusus
my_config = DocumentFormatConfiguration()
my_config.extension_filter = ".foo"
my_config.document_type = MyCustomHandler
my_config.initialization_data["MyProperty"] = "bar"

redactor_config = RedactorConfiguration.get_instance()
redactor_config.available_formats.append(my_config)
```

### Lihat Juga
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
