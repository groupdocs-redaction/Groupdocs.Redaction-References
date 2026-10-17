---
title: "find_format Methode"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Findet Formatkonfigurationen für eine gegebene Dateierweiterung."
type: docs
url: /de/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/
is_root: false
weight: 1010
---


## find_format {#file_extension}

Findet Formatkonfigurationen für eine gegebene Dateierweiterung.

```python
def find_format(self, file_extension):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| file_extension | `str` | Dateierweiterung, Format ist ".ext". |

**Returns:** DocumentFormatConfiguration or None: If found, instance of DocumentFormatConfiguration, None otherwise.

### Beispiel

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Erhalte die Singleton-Konfigurationsinstanz
config = RedactorConfiguration.get_instance()

# Rufe die Formateinstellungen für eine gegebene Erweiterung ab.
settings = config.find_format(".txt")
if settings:
    # Erweitere die Liste der behandelten Erweiterungen, z. B. füge .dump hinzu
    settings.extension_filter = settings.extension_filter + ",.dump"
```

### Siehe auch
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
