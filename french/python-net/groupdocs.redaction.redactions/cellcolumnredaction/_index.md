---
title: "Classe CellColumnRedaction"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Représente un caviardage de texte qui remplace le texte dans un document de feuille de calcul (CSV, Excel, etc.)."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/cellcolumnredaction/
is_root: false
weight: 20
---


## CellColumnRedaction class

Représente un caviardage de texte qui remplace le texte dans un document de feuille de calcul (CSV, Excel, etc.).

- Learn more: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about spreadsheet redactions: https://docs.groupdocs.com/redaction/net/spreadsheet-redactions/

Le type CellColumnRedaction expose les membres suivants :

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/#filter-reg_ex-options) | Initialise une nouvelle CellColumnRedaction. |

### Méthodes
| Méthode | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to/#format_instance) | Applique la rédaction à une instance de format donnée. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to_document_format_instance/) |  |

### Propriétés
| Propriété | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/description/) | La description de la rédaction, contenant son nom et ses paramètres. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/filter/) | Le filtre de colonne et de feuille de calcul. |
| [pattern](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/pattern/) | Le modèle d'expression régulière à correspondre. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | L'instance [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) spécifiant le type de remplacement de texte. (héritée de [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | L'implémentation IOcrConnector utilisée pour extraire le texte du contenu graphique. (héritée de [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Exemple

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import CellColumnRedaction, ReplacementOptions
from groupdocs.redaction.filters import CellFilter

with Redactor("Sales in September.xlsx") as redactor:
    filter = CellFilter(column_index=1, worksheet_name="Customers")
    regex = r"^\w+([-+.']\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*$"
    redactor.apply(CellColumnRedaction(filter, regex, ReplacementOptions("[customer email]")))
    redactor.save()
```

### Voir aussi
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
