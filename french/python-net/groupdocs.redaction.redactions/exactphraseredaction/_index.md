---
title: "Classe ExactPhraseRedaction"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Représente un caviardage de texte qui remplace une phrase exacte dans le texte du document, insensible à la casse par défaut."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/exactphraseredaction/
is_root: false
weight: 80
---


## ExactPhraseRedaction class

Représente un caviardage de texte qui remplace une phrase exacte dans le texte du document, insensible à la casse par défaut.

En savoir plus :
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/

Le type ExactPhraseRedaction expose les membres suivants:

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-options) | Initialise une nouvelle instance de ExactPhraseRedaction en mode insensible à la casse. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-is_case_sensitive-options) | Initialise une nouvelle instance de ExactPhraseRedaction. |

### Méthodes
| Méthode | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to/#format_instance) | Applique la rédaction à une instance de format donnée. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to_document_format_instance/) |  |

### Propriétés
| Propriété | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/description/) | La description de la censure, contenant le nom de la censure et les paramètres. |
| [is_case_sensitive](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_case_sensitive/) | La valeur indiquant si la recherche est sensible à la casse. |
| [is_right_to_left](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_right_to_left/) | Le drapeau de direction du texte indiquant si le texte est de droite à gauche. La valeur par défaut est False. |
| [search_phrase](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/search_phrase/) | La chaîne à rechercher et remplacer. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | L'instance [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) spécifiant le type de remplacement de texte. (héritée de [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | L'implémentation IOcrConnector utilisée pour extraire le texte du contenu graphique. (héritée de [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Exemple

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("sample.pdf") as redactor:
    # remplacement sensible à la casse
    redactor.apply(ExactPhraseRedaction("John Doe", True, ReplacementOptions("[personal]")))
    redactor.save()
```

### Guides
Guides de tâches qui utilisent `ExactPhraseRedaction`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Voir aussi
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
