---
title: "DocumentFormatInstance Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt ein bestimmtes Format eines Dokuments dar und kann implementiert werden, um benutzerdefinierte Dokumenttypen hinzuzufügen."
type: docs
url: /de/python-net/groupdocs.redaction.integration/documentformatinstance/
is_root: false
weight: 10
---


## DocumentFormatInstance class

Stellt ein bestimmtes Format eines Dokuments dar und kann implementiert werden, um benutzerdefinierte Dokumenttypen hinzuzufügen.

Mehr erfahren

- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Der Typ DocumentFormatInstance stellt die folgenden Mitglieder bereit:

### Methoden
| Methode | Beschreibung |
| :- | :- |
| [initialize](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/#config-settings) | Initialisiert die Instanz des Dokumentformat-Handlers. |
| [initialize_document_format_configuration](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize_document_format_configuration/) |  |
| [is_redaction_accepted](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/#description) | Prüft auf eine Implementierung von [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) und ruft sie auf, falls angegeben. |
| [is_redaction_accepted_redaction_description](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted_redaction_description/) |  |
| [load](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load/#input) | Lädt das Dokument aus einem Stream. |
| [load_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_streams/) |  |
| [perform_binary_check](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/#input) | Prüft, ob der gegebene Stream ein von dieser Formatinstanz unterstütztes Dokument enthält. |
| [perform_binary_check_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_stream/) |  |
| [perform_binary_check_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_streams/) |  |
| [save](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save/#output) | Speichert das Dokument in einen Stream. |
| [save_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_streams/) |  |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/password/) | Das Passwort für passwortgeschützte Dokumente. |

### Beispiel

```python
class DummyDocument(DocumentFormatInstance):
    def load(self, output: io.RawIOBase) -> None:
        # Dateiinhalt laden
        pass

    def save(self, output: io.RawIOBase) -> None:
        # Änderungen in Datei speichern
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

### Siehe auch
* module [`groupdocs.redaction.integration`](/redaction/python-net/groupdocs.redaction.integration/)
