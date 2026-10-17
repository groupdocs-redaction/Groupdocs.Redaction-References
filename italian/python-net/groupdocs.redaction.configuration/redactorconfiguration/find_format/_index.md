---
title: "Metodo find_format"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Trova le configurazioni di formato per una data estensione di file."
type: docs
url: /it/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/
is_root: false
weight: 1010
---


## find_format {#file_extension}

Trova le configurazioni di formato per una data estensione di file.

```python
def find_format(self, file_extension):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| file_extension | `str` | Estensione file, il formato è ".ext". |

**Returns:** DocumentFormatConfiguration or None: If found, instance of DocumentFormatConfiguration, None otherwise.

### Esempio

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Ottieni l'istanza di configurazione singleton
config = RedactorConfiguration.get_instance()

# Recupera le impostazioni di formato per una determinata estensione
settings = config.find_format(".txt")
if settings:
    # Estendi l'elenco delle estensioni gestite, ad es., aggiungi .dump
    settings.extension_filter = settings.extension_filter + ",.dump"
```

### Vedi anche
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
