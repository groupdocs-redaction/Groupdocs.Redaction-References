---
title: "Método get_instance"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Devuelve una instancia singleton con la configuración predeterminada de los formatos incorporados."
type: docs
url: /es/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/
is_root: false
weight: 1040
---


## get_instance

Devuelve una instancia singleton con la configuración predeterminada de los formatos incorporados.

```python
def get_instance(cls):
    ...
```

**Returns:** RedactorConfiguration: Configuration instance.

### Ejemplo

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Obtener la configuración singleton
config = RedactorConfiguration.get_instance()

# Ampliar las extensiones compatibles para formatos de texto plano
txt_settings = config.find_format(".txt")
txt_settings.extension_filter += ",.dump"
```

### Ver también
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
