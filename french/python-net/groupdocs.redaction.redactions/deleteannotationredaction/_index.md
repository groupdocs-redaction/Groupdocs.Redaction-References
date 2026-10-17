---
title: "Classe DeleteAnnotationRedaction"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Représente un caviardage de texte qui supprime les annotations si le texte correspond à une expression régulière donnée (supprime éventuellement toutes les annotations)."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/deleteannotationredaction/
is_root: false
weight: 60
---


## DeleteAnnotationRedaction class

Représente un caviardage de texte qui supprime les annotations si le texte correspond à une expression régulière donnée (supprime éventuellement toutes les annotations).

En savoir plus

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

Le type DeleteAnnotationRedaction expose les membres suivants :

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/) | Initialise une nouvelle instance de la classe DeleteAnnotationRedaction, avec des paramètres pour supprimer toutes les annotations (correspondant à tout). |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#pattern) | Initialise une nouvelle instance de la classe DeleteAnnotationRedaction, supprimant les annotations correspondant à l’expression donnée. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#regex) | Initialise une nouvelle instance de la classe DeleteAnnotationRedaction, supprimant les annotations correspondant à l’expression donnée. |

### Méthodes
| Méthode | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to/#format_instance) | Applique la rédaction à une instance de format donnée. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to_document_format_instance/) |  |

### Propriétés
| Propriété | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/description/) | La description de la censure, contenant le nom de la censure et les paramètres. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/expression/) | L’expression régulière à correspondre. |

### Exemple

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

with Redactor("document.pdf") as redactor:
    # Supprimer les annotations contenant le mot « internal » (insensible à la casse)
    redactor.apply(DeleteAnnotationRedaction("(?i)internal"))
    redactor.save()
```

### Guides
Guides de tâches qui utilisent `DeleteAnnotationRedaction` :

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Voir aussi
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
