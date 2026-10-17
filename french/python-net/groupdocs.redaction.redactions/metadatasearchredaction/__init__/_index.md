---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise une nouvelle instance de la classe MetadataSearchRedaction, en utilisant la valeur pour correspondre aux éléments censurés."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#value_pattern-replacement}

Initialise une nouvelle instance de la classe MetadataSearchRedaction, en utilisant la valeur pour correspondre aux éléments censurés.

```python
def __init__(self, value_pattern, replacement):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| value_pattern | `str` | Expression régulière pour rechercher et remplacer |
| replacement | `str` | Remplacement textuel |

### Exemple

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    redactor.apply(MetadataSearchRedaction(".*@acme\\.com", "[EMAIL]"))
    redactor.save()
```

## __init__ {#value_pattern-replacement-key_pattern}

Initialise une nouvelle instance de MetadataSearchRedaction, en utilisant le nom de l'élément et la valeur pour correspondre aux éléments censurés.

```python
def __init__(self, value_pattern, replacement, key_pattern):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| value_pattern | `str` | Expression régulière pour rechercher et remplacer la valeur d'un élément de métadonnées. |
| replacement | `str` | Remplacement textuel. |
| key_pattern | `str` | Expression régulière pour rechercher et remplacer le nom d'un élément de métadonnées. |

### Exemple

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    # Remplacer toute adresse e‑mail trouvée dans les valeurs de métadonnées
    redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement}

Initialise une nouvelle instance de la classe MetadataSearchRedaction, en utilisant la valeur pour correspondre aux éléments censurés.

```python
def __init__(self, value_regex, replacement):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Expression régulière pour rechercher et remplacer. |
| replacement | `str` | Remplacement textuel. |

### Exemple

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

# Masquer toute adresse e‑mail dans les métadonnées
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement-key_regex}

Initialise une nouvelle instance de MetadataSearchRedaction en utilisant le nom de l'élément et la valeur pour correspondre aux éléments censurés.

```python
def __init__(self, value_regex, replacement, key_regex):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Expression régulière pour rechercher et remplacer la valeur d'un élément de métadonnées. |
| replacement | `str` | Remplacement textuel. |
| key_regex | `System.Text.RegularExpressions.Regex` | Expression régulière pour rechercher et remplacer le nom d'un élément de métadonnées. |

### Exemple

```python
from groupdocs.redaction.redactions import MetadataSearchRedaction
from groupdocs.redaction import Redactor

# Masquer les adresses e‑mail dans les valeurs de métadonnées
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

### Voir aussi
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/)
