---
title: "méthode get_instance"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Renvoie une instance singleton avec la configuration par défaut des formats intégrés."
type: docs
url: /fr/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/
is_root: false
weight: 1040
---


## get_instance

Renvoie une instance singleton avec la configuration par défaut des formats intégrés.

```python
def get_instance(cls):
    ...
```

**Returns:** RedactorConfiguration: Configuration instance.

### Exemple

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Obtenir la configuration singleton
config = RedactorConfiguration.get_instance()

# Étendre les extensions prises en charge pour les formats texte brut
txt_settings = config.find_format(".txt")
txt_settings.extension_filter += ",.dump"
```

### Voir aussi
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
