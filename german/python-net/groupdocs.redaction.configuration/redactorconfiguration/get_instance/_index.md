---
title: "get_instance Methode"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Gibt eine Singleton-Instanz mit der Standardkonfiguration der integrierten Formate zurück."
type: docs
url: /de/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/
is_root: false
weight: 1040
---


## get_instance

Gibt eine Singleton-Instanz mit der Standardkonfiguration der integrierten Formate zurück.

```python
def get_instance(cls):
    ...
```

**Returns:** RedactorConfiguration: Configuration instance.

### Beispiel

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Erhalte die Singleton-Konfiguration
config = RedactorConfiguration.get_instance()

# Erweitere unterstützte Erweiterungen für Klartextformate
txt_settings = config.find_format(".txt")
txt_settings.extension_filter += ",.dump"
```

### Siehe auch
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
