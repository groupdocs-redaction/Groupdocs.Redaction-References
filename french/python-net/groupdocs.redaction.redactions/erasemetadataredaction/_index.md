---
title: "Classe EraseMetadataRedaction"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Représente un caviardage de métadonnées qui efface toutes les métadonnées ou les métadonnées correspondant à des filtres MetadataFilters spécifiques du document."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/erasemetadataredaction/
is_root: false
weight: 70
---


## EraseMetadataRedaction class

Représente un caviardage de métadonnées qui efface toutes les métadonnées ou les métadonnées correspondant à des filtres MetadataFilters spécifiques du document.

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document metadata redactions: https://docs.groupdocs.com/redaction/net/metadata-redactions/

Le type EraseMetadataRedaction expose les membres suivants :

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/) | Initialise une nouvelle instance de la classe EraseMetadataRedaction, en effaçant toutes les métadonnées. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/#filter) | Initialise une nouvelle instance de EraseMetadataRedaction, en effaçant les métadonnées qui correspondent aux `MetadataFilters` spécifiés. |

### Méthodes
| Méthode | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Applique la rédaction à une instance de format donnée. (hérité de [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (hérité de [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Propriétés
| Propriété | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/description/) | La description de la rédaction et de ses paramètres. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Le filtre utilisé pour sélectionner toutes les métadonnées ou des métadonnées spécifiques, telles que Auteur ou Société. (hérité de [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Exemple

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Effacer toutes les métadonnées
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Effacer uniquement le champ auteur
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Guides
Guides de tâches qui utilisent `EraseMetadataRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Voir aussi
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
