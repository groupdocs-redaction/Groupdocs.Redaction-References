---
title: "find_format-methode"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Vindt formatconfiguraties voor een gegeven bestandsextensie."
type: docs
url: /nl/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/
is_root: false
weight: 1010
---


## find_format {#file_extension}

Vindt formatconfiguraties voor een gegeven bestandsextensie.

```python
def find_format(self, file_extension):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| file_extension | `str` | Bestandsextensie, formaat is ".ext". |

**Returns:** DocumentFormatConfiguration or None: If found, instance of DocumentFormatConfiguration, None otherwise.

### Voorbeeld

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Verkrijg de singleton-configuratie-instantie
config = RedactorConfiguration.get_instance()

# Haal de formaatinstellingen op voor een gegeven extensie
settings = config.find_format(".txt")
if settings:
    # Breid de lijst met verwerkte extensies uit, bijv., voeg .dump toe
    settings.extension_filter = settings.extension_filter + ",.dump"
```

### Zie ook
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
