---
title: "get_instance-methode"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Retourneert een singleton‑instantie met de standaardconfiguratie van ingebouwde formaten."
type: docs
url: /nl/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/
is_root: false
weight: 1040
---


## get_instance

Retourneert een singleton‑instantie met de standaardconfiguratie van ingebouwde formaten.

```python
def get_instance(cls):
    ...
```

**Returns:** RedactorConfiguration: Configuration instance.

### Voorbeeld

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Verkrijg de singleton-configuratie
config = RedactorConfiguration.get_instance()

# Breid ondersteunde extensies uit voor platte-tekstformaten
txt_settings = config.find_format(".txt")
txt_settings.extension_filter += ",.dump"
```

### Zie ook
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
