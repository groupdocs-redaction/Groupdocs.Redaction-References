---
title: "Classe RemovePageRedaction"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Représente une rédaction qui supprime une page (diapositive, feuille de calcul, etc.) d'un document."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/removepageredaction/
is_root: false
weight: 250
---


## RemovePageRedaction class

Représente une rédaction qui supprime une page (diapositive, feuille de calcul, etc.) d'un document.

En savoir plus
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about removing pages: https://docs.groupdocs.com/redaction/net/remove-page-redaction/

Le type RemovePageRedaction expose les membres suivants:

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/#origin-index-count) | Initialise un nouveau RemovePageRedaction. |

### Méthodes
| Méthode | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to/#format_instance) | Applique la rédaction à une instance de format donnée. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to_document_format_instance/) |  |

### Propriétés
| Propriété | Description |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/count/) | Le nombre de pages à supprimer. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/index/) | L'index de position de départ (à base zéro). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/origin/) | La position de référence de recherche, soit le début, soit la fin d'un document. |
| [description](/redaction/python-net/groupdocs.redaction/redaction/description/) | La description de la rédaction, contenant son nom et ses paramètres. (hérité de [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)) |

### Exemple

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Supprimer 1 page en comptant depuis la fin du document
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    with Redactor("./test.pdf") as redactor:
        # Appliquer le masquage
        result = redactor.apply(rem_opt)

        # Enregistrer le document rédigé
        so = SaveOptions()
        so.add_suffix = True
        redactor.save(so)
```

### Guides
Guides de tâches qui utilisent `RemovePageRedaction`:

* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)

### Voir aussi
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
