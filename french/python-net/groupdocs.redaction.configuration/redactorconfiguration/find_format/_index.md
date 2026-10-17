---
title: "méthode find_format"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Trouve les configurations de format pour une extension de fichier donnée."
type: docs
url: /fr/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/
is_root: false
weight: 1010
---


## find_format {#file_extension}

Trouve les configurations de format pour une extension de fichier donnée.

```python
def find_format(self, file_extension):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| file_extension | `str` | Extension de fichier, le format est ".ext". |

**Returns:** DocumentFormatConfiguration or None: If found, instance of DocumentFormatConfiguration, None otherwise.

### Exemple

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Obtenir l'instance de configuration singleton
config = RedactorConfiguration.get_instance()

# Récupérer les paramètres de format pour une extension donnée
settings = config.find_format(".txt")
if settings:
    # Étendre la liste des extensions gérées, p. ex., ajouter .dump
    settings.extension_filter = settings.extension_filter + ",.dump"
```

### Voir aussi
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
