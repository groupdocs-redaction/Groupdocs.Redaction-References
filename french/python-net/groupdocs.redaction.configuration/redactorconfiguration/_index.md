---
title: "Classe RedactorConfiguration"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Fournit l'accès à une liste de formats pris en charge, intégrés et formats personnalisés de l'utilisateur."
type: docs
url: /fr/python-net/groupdocs.redaction.configuration/redactorconfiguration/
is_root: false
weight: 20
---


## RedactorConfiguration class

Fournit l'accès à une liste de formats pris en charge, intégrés et formats personnalisés de l'utilisateur.

En savoir plus :

- More details about GroupDocs.Redaction configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Le type RedactorConfiguration expose les membres suivants :

### Méthodes
| Méthode | Description |
| :- | :- |
| [find_format](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/#file_extension) | Trouve les configurations de format pour une extension de fichier donnée. |
| [find_format_file](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_file/) |  |
| [find_format_string](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_string/) |  |
| [get_instance](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/) | Renvoie une instance singleton avec la configuration par défaut des formats intégrés. |

### Propriétés
| Propriété | Description |
| :- | :- |
| [available_formats](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/available_formats/) | La liste des formats reconnus, voir [`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/). |

### Exemple

```python
# Ajouter un gestionnaire de format utilisateur personnalisé
adobe_photoshop_settings = DocumentFormatConfiguration()
adobe_photoshop_settings.extension_filter = ".psd"
adobe_photoshop_settings.document_type = MyAdobePhotoshopFormatInstance

config = RedactorConfiguration.get_instance()
config.available_formats.add(adobe_photoshop_settings)
```

```python
# Récupérer un gestionnaire de format utilisateur intégré ou personnalisé
config = RedactorConfiguration.get_instance()
format_settings = config.find_format(".psd")
```

### Voir aussi
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
