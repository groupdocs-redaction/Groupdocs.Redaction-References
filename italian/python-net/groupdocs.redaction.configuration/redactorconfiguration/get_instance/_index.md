---
title: "Metodo get_instance"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Restituisce un'istanza singleton con la configurazione predefinita dei formati integrati."
type: docs
url: /it/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/
is_root: false
weight: 1040
---


## get_instance

Restituisce un'istanza singleton con la configurazione predefinita dei formati integrati.

```python
def get_instance(cls):
    ...
```

**Returns:** RedactorConfiguration: Configuration instance.

### Esempio

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Ottieni la configurazione singleton
config = RedactorConfiguration.get_instance()

# Estendi le estensioni supportate per i formati di testo semplice
txt_settings = config.find_format(".txt")
txt_settings.extension_filter += ",.dump"
```

### Vedi anche
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
