---
title: "get_instance-metod"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Returnerar en singleton-instans med standardkonfigurationen för inbyggda format."
type: docs
url: /sv/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/
is_root: false
weight: 1040
---


## get_instance

Returnerar en singleton-instans med standardkonfigurationen för inbyggda format.

```python
def get_instance(cls):
    ...
```

**Returns:** RedactorConfiguration: Configuration instance.

### Exempel

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Hämta singleton-konfigurationen
config = RedactorConfiguration.get_instance()

# Utöka stödda ändelser för rena textformat
txt_settings = config.find_format(".txt")
txt_settings.extension_filter += ",.dump"
```

### Se även
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
