---
title: "Classe PageRangeFilter"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Représente un filtre de rédaction, définissant une plage de pages à l'intérieur d'un document pour appliquer la rédaction."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/pagerangefilter/
is_root: false
weight: 170
---


## PageRangeFilter class

Représente un filtre de rédaction, définissant une plage de pages à l'intérieur d'un document pour appliquer la rédaction.

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

Le type PageRangeFilter expose les membres suivants :

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/__init__/#origin-index-count) | Initialise un nouveau RemovePageRedaction. |

### Propriétés
| Propriété | Description |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/count/) | Le nombre de pages à supprimer. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/index/) | L'index de position de départ (à base zéro). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/origin/) | La position de référence de recherche, soit le début, soit la fin d'un document. |

### Exemple

```python
from groupdocs.redaction.redactions import PageRangeFilter, PageSeekOrigin

# Définissez un filtre qui cible la dernière page et celle qui la précède
page_filter = PageRangeFilter(PageSeekOrigin.END, 0, 1)

# Le filtre peut être combiné avec d'autres filtres, p. ex., PageAreaFilter,
# et transmis à ReplacementOptions.Filters lors de la configuration d'une rédaction.
```

### Voir aussi
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
