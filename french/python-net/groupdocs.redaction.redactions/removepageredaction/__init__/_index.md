---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise un nouveau RemovePageRedaction."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#origin-index-count}

Initialise un nouveau RemovePageRedaction.

```python
def __init__(self, origin, index, count):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Chercher la position de référence, le début ou la fin d'un document. |
| index | `int` | Indice de position de départ (index 0). |
| count | `int` | Nombre de pages à supprimer. |

### Exemple

```python
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Supprimer 3 pages à partir de la deuxième page (index de base zéro 1)
redaction = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)
```

### Voir aussi
* class [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/)
