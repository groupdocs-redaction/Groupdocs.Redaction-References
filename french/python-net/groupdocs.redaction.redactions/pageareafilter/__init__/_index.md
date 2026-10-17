---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise un nouveau PageAreaFilter pour masquer une zone spécifique."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-size}

Initialise un nouveau PageAreaFilter pour masquer une zone spécifique.

```python
def __init__(self, top_left, size):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | Coordonnées de la zone en haut à gauche. |
| size | `System.Drawing.Size` | Taille et couleur de la zone. |

### Exemple

```python
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

point = Point(0, 100)
size = Size(200, 150)
filter = PageAreaFilter(point, size)
```

### Voir aussi
* class [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/)
