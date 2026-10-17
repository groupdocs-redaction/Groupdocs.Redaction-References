---
title: "Método find_format"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Busca configuraciones de formato para una extensión de archivo dada."
type: docs
url: /es/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/
is_root: false
weight: 1010
---


## find_format {#file_extension}

Busca configuraciones de formato para una extensión de archivo dada.

```python
def find_format(self, file_extension):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| file_extension | `str` | Extensión de archivo, el formato es ".ext". |

**Returns:** DocumentFormatConfiguration or None: If found, instance of DocumentFormatConfiguration, None otherwise.

### Ejemplo

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Obtener la instancia de configuración singleton
config = RedactorConfiguration.get_instance()

# Recuperar la configuración de formato para una extensión dada
settings = config.find_format(".txt")
if settings:
    # Ampliar la lista de extensiones manejadas, p.ej., agregar .dump
    settings.extension_filter = settings.extension_filter + ",.dump"
```

### Ver también
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
