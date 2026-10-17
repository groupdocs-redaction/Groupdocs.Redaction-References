---
title: "initialize μέθοδος"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί την παρουσία του χειριστή μορφής εγγράφου."
type: docs
url: /el/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/
is_root: false
weight: 1010
---


## initialize {#config-settings}

Αρχικοποιεί την παρουσία του χειριστή μορφής εγγράφου.

```python
def initialize(self, config, settings):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| config | `DocumentFormatConfiguration` | Διαμόρφωση μορφής. |
| settings | `RedactorSettings` | Προεπιλεγμένες ρυθμίσεις για τη διαδικασία επεξεργασίας. |

**Returns:** None.

### Παράδειγμα

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

# Καταχωρίστε το προσαρμοσμένο μορφότυπο
my_config = DocumentFormatConfiguration()
my_config.extension_filter = ".foo"
my_config.document_type = MyCustomHandler
my_config.initialization_data["MyProperty"] = "bar"

redactor_config = RedactorConfiguration.get_instance()
redactor_config.available_formats.append(my_config)
```

### Δείτε επίσης
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
