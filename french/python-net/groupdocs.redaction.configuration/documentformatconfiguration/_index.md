---
title: "Classe DocumentFormatConfiguration"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Représente une référence de type pour la classe dérivée de DocumentFormatInstance et une liste d'extensions de fichier prises en charge pour une détection de format plus rapide."
type: docs
url: /fr/python-net/groupdocs.redaction.configuration/documentformatconfiguration/
is_root: false
weight: 10
---


## DocumentFormatConfiguration class

Représente une référence de type pour la classe dérivée de [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) et une liste d'extensions de fichiers prises en charge pour une détection de format plus rapide.

En savoir plus

- More details about **GroupDocs.Redaction** configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Le type DocumentFormatConfiguration expose les membres suivants :

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/__init__/) | Initialise une nouvelle instance de DocumentFormatConfiguration. |

### Méthodes
| Méthode | Description |
| :- | :- |
| [supports_extension](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/#file_extension) | Vérifie si une extension de fichier donnée peut être gérée en tant que DocumentType. |
| [supports_extension_file](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_file/) |  |
| [supports_extension_string](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_string/) |  |

### Propriétés
| Propriété | Description |
| :- | :- |
| [document_type](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/document_type/) | Le type d’une classe héritant de [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |
| [extension_filter](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/extension_filter/) | La liste d’extensions de fichiers séparées par des virgules (par exemple ".pdf"), insensible à la casse. |
| [initialization_data](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/initialization_data/) | Les données requises pour l’initialisation de [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |

### Exemple

```python
from groupdocs.redaction import DocumentFormatConfiguration

# Créer une configuration de format personnalisée
config = DocumentFormatConfiguration()
config.ExtensionFilter = ".psd"
config.DocumentType = MyAdobePhotoshopFormatInstance
```

### Voir aussi
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
