---
title: "classe RedactionPolicy"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Représente une politique de désinfection, contenant un ensemble de censures spécifiques à appliquer."
type: docs
url: /fr/python-net/groupdocs.redaction/redactionpolicy/
is_root: false
weight: 120
---


## RedactionPolicy class

Représente une politique de désinfection, contenant un ensemble de censures spécifiques à appliquer.

**Learn more**
- More details about policies: https://docs.groupdocs.com/redaction/net/use-redaction-policies/
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/

Le type RedactionPolicy expose les membres suivants :

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/) | Initialise une nouvelle instance de RedactionPolicy. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/#redactions) | Initialise un nouveau RedactionPolicy avec une liste spécifique de redactions. |

### Méthodes
| Méthode | Description |
| :- | :- |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#file_path) | Charge un RedactionPolicy à partir d'un fichier XML. |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#input) | Charge une instance de RedactionPolicy à partir d'un flux contenant la configuration XML. |
| [load_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_file/) |  |
| [load_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_streams/) |  |
| [load_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_string/) |  |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#file_path) | Enregistre la politique de rédaction dans un fichier. |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#output) | Enregistre la politique de rédaction dans un flux. |
| [save_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_file/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_streams/) |  |
| [save_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_string/) |  |

### Propriétés
| Propriété | Description |
| :- | :- |
| [redactions](/redaction/python-net/groupdocs.redaction/redactionpolicy/redactions/) | La liste des classes dérivées entièrement configurées [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/). |

### Exemple

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

# Construire une politique réutilisable en mémoire
policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])

# Appliquer la politique à un document
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Guides
Guides de tâches qui utilisent `RedactionPolicy` :

* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Voir aussi
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
