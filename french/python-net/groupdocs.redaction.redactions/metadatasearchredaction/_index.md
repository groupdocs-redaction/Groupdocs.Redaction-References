---
title: "Classe MetadataSearchRedaction"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Représente une rédaction de métadonnées qui recherche et censure les métadonnées en utilisant des expressions régulières, en faisant correspondre les clés et/ou les valeurs."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/metadatasearchredaction/
is_root: false
weight: 140
---


## MetadataSearchRedaction class

Représente une rédaction de métadonnées qui recherche et censure les métadonnées en utilisant des expressions régulières, en faisant correspondre les clés et/ou les valeurs.

- More details about applying redactions: <https://docs.groupdocs.com/redaction/net/redaction-basics/>
- More details about document metadata redactions: <https://docs.groupdocs.com/redaction/net/metadata-redactions/>

Le type MetadataSearchRedaction expose les membres suivants :

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement) | Initialise une nouvelle instance de la classe MetadataSearchRedaction, en utilisant la valeur pour correspondre aux éléments censurés. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement-key_pattern) | Initialise une nouvelle instance de MetadataSearchRedaction, en utilisant le nom de l'élément et la valeur pour correspondre aux éléments censurés. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement) | Initialise une nouvelle instance de la classe MetadataSearchRedaction, en utilisant la valeur pour correspondre aux éléments censurés. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement-key_regex) | Initialise une nouvelle instance de MetadataSearchRedaction en utilisant le nom de l'élément et la valeur pour correspondre aux éléments censurés. |

### Méthodes
| Méthode | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Applique la rédaction à une instance de format donnée. (hérité de [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (hérité de [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Propriétés
| Propriété | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/description/) | La description de la rédaction, contenant son nom et ses paramètres. |
| [key_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/key_expression/) | L'expression régulière pour correspondre au nom (clé) d'un élément de métadonnées. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/replacement/) | La valeur de remplacement textuel. |
| [value_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/value_expression/) | L'expression régulière pour correspondre au texte de valeur d'un élément de métadonnées. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Le filtre utilisé pour sélectionner toutes les métadonnées ou des métadonnées spécifiques, telles que Auteur ou Société. (hérité de [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Exemple

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Censurer toute valeur de métadonnées correspondant au modèle
    redaction = MetadataSearchRedaction("Company Ltd.", "--company--")
    redaction.filter = MetadataFilters.COMPANY
    redactor.apply(redaction)
    redactor.save()
```

### Guides
Guides de tâches qui utilisent `MetadataSearchRedaction`:

* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)

### Voir aussi
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
