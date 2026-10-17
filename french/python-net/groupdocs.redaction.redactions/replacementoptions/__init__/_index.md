---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise une nouvelle instance de ReplacementOptions avec le texte de remplacement spécifié."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#replacement}

Initialise une nouvelle instance de ReplacementOptions avec le texte de remplacement spécifié.

```python
def __init__(self, replacement):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| replacement | `str` | Remplacement textuel. |

### Exemple

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Remplacer le texte correspondant par "[REDACTED]"
options = ReplacementOptions("[REDACTED]")
```

## __init__ {#color}

Initialise une nouvelle instance de la classe ReplacementOptions avec un rectangle coloré comme option.

```python
def __init__(self, color):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| color | `System.Drawing.Color` | Couleur du rectangle. |

### Voir aussi
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)
