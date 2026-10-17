---
title: "Classe ReplacementOptions"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Représente les options pour le remplacement du texte correspondant."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/replacementoptions/
is_root: false
weight: 260
---


## ReplacementOptions class

Représente les options pour le remplacement du texte correspondant.

En savoir plus

- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

Le type ReplacementOptions expose les membres suivants :

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#replacement) | Initialise une nouvelle instance de ReplacementOptions avec le texte de remplacement spécifié. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#color) | Initialise une nouvelle instance de la classe ReplacementOptions avec un rectangle coloré comme option. |

### Propriétés
| Propriété | Description |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/action_type/) | L'action de remplacement : dessiner une boîte ou remplacer le texte. |
| [box_color](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_color/) | La couleur pour l'option `ReplacementType.draw_box` (ignorée sinon). |
| [custom_redaction](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/custom_redaction/) | Le gestionnaire de rédaction personnalisé qui permet aux utilisateurs de définir leur propre logique de rédaction. |
| [filters](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/filters/) | Le tableau de filtres à appliquer avec cette rédaction. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/replacement/) | La valeur de remplacement textuel. |

### Exemple

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Remplacer le texte correspondant par le texte de substitution "[X]"
repl_opt = ReplacementOptions("[X]")
```

### Guides
Guides de tâches utilisant `ReplacementOptions` :

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Voir aussi
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
