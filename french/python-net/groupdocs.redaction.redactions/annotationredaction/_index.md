---
title: "Classe AnnotationRedaction"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Représente un caviardage qui remplace le texte des annotations (commentaires, etc.) correspondant à une expression régulière donnée."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/annotationredaction/
is_root: false
weight: 10
---


## AnnotationRedaction class

Représente un caviardage qui remplace le texte des annotations (commentaires, etc.) correspondant à une expression régulière donnée.

En savoir plus

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

Le type AnnotationRedaction expose les membres suivants :

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#pattern-replacement) | Initialise une nouvelle AnnotationRedaction avec un motif regex et un texte de remplacement. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#regex-replacement) | Initialise une nouvelle instance de [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/). |

### Méthodes
| Méthode | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to/#format_instance) | Applique la rédaction à une instance de format donnée. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to_document_format_instance/) |  |

### Propriétés
| Propriété | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/description/) | La description de la redaction, décrivant la redaction et ses paramètres. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/expression/) | L’expression régulière à correspondre. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/replacement/) | Le remplacement textuel pour le texte correspondant. |

### Exemple

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import AnnotationRedaction

with Redactor("document.pdf") as redactor:
    redactor.apply(AnnotationRedaction("(?i)approved", "[REVIEW]"))
    redactor.save()
```

### Guides
Guides de tâches qui utilisent `AnnotationRedaction` :

* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)

### Voir aussi
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
