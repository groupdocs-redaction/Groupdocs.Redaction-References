---
title: "find_format-metod"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Hittar formatkonfigurationer för en given filändelse."
type: docs
url: /sv/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/
is_root: false
weight: 1010
---


## find_format {#file_extension}

Hittar formatkonfigurationer för en given filändelse.

```python
def find_format(self, file_extension):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| file_extension | `str` | Filändelse, formatet är ".ext". |

**Returns:** DocumentFormatConfiguration or None: If found, instance of DocumentFormatConfiguration, None otherwise.

### Exempel

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Hämta singleton-konfigurationsinstansen
config = RedactorConfiguration.get_instance()

# Hämta formatinställningarna för en given ändelse
settings = config.find_format(".txt")
if settings:
    # Utöka listan över hanterade ändelser, t.ex. lägg till .dump
    settings.extension_filter = settings.extension_filter + ",.dump"
```

### Se även
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
