---
title: "Classe PageAreaFilter"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Représente un filtre de rédaction, définissant une zone à l'intérieur d'une page d'un document pour appliquer la rédaction."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/pageareafilter/
is_root: false
weight: 150
---


## PageAreaFilter class

Représente un filtre de rédaction, définissant une zone à l'intérieur d'une page d'un document pour appliquer la rédaction.

En savoir plus

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

Le type PageAreaFilter expose les membres suivants :

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/#top_left-size) | Initialise un nouveau PageAreaFilter pour masquer une zone spécifique. |

### Propriétés
| Propriété | Description |
| :- | :- |
| [rectangle](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/rectangle/) | Le rectangle (position en haut à gauche et taille de la zone) sur une page. |

### Exemple

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

with Redactor("doc.pdf") as redactor:
    page = redactor.get_document_info().pages[0]
    area_filter = PageAreaFilter(
        Point(0, int(page.height / 2)),
        Size(page.width, int(page.height / 2))
    )
```

### Voir aussi
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
