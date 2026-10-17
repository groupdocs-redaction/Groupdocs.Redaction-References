---
title: "Classe DocumentFormatInstance"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Représente un format spécifique d'un document et peut être implémenté pour ajouter des types de documents personnalisés."
type: docs
url: /fr/python-net/groupdocs.redaction.integration/documentformatinstance/
is_root: false
weight: 10
---


## DocumentFormatInstance class

Représente un format spécifique d'un document et peut être implémenté pour ajouter des types de documents personnalisés.

En savoir plus

- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Le type DocumentFormatInstance expose les membres suivants :

### Méthodes
| Méthode | Description |
| :- | :- |
| [initialize](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/#config-settings) | Initialise l'instance du gestionnaire de format de document. |
| [initialize_document_format_configuration](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize_document_format_configuration/) |  |
| [is_redaction_accepted](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/#description) | Vérifie la présence d'une implémentation de [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) et l'appelle, si spécifiée. |
| [is_redaction_accepted_redaction_description](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted_redaction_description/) |  |
| [load](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load/#input) | Charge le document depuis un flux. |
| [load_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_streams/) |  |
| [perform_binary_check](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/#input) | Vérifie si le flux fourni contient un document pris en charge par cette instance de format. |
| [perform_binary_check_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_stream/) |  |
| [perform_binary_check_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_streams/) |  |
| [save](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save/#output) | Enregistre le document dans un flux. |
| [save_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_streams/) |  |

### Propriétés
| Propriété | Description |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/password/) | Le mot de passe pour les documents protégés par mot de passe. |

### Exemple

```python
class DummyDocument(DocumentFormatInstance):
    def load(self, output: io.RawIOBase) -> None:
        # charger le contenu du fichier
        pass

    def save(self, output: io.RawIOBase) -> None:
        # enregistrer les modifications dans le fichier
        pass
```

```python
class MyCustomHandler(DocumentFormatInstance):
    def __init__(self):
        self.my_property = None

    def initialize(self, config: DocumentFormatConfiguration) -> None:
        super().initialize(config)
        if "MyProperty" in config.initialization_data:
            self.my_property = config.initialization_data["MyProperty"]
```

### Voir aussi
* module [`groupdocs.redaction.integration`](/redaction/python-net/groupdocs.redaction.integration/)
