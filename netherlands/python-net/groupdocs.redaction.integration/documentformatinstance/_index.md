---
title: "DocumentFormatInstance klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt een specifiek formaat van een document voor en kan worden geïmplementeerd om aangepaste documenttypen toe te voegen."
type: docs
url: /nl/python-net/groupdocs.redaction.integration/documentformatinstance/
is_root: false
weight: 10
---


## DocumentFormatInstance class

Stelt een specifiek formaat van een document voor en kan worden geïmplementeerd om aangepaste documenttypen toe te voegen.

Meer informatie

- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Het type DocumentFormatInstance exposeert de volgende leden:

### Methoden
| Methode | Beschrijving |
| :- | :- |
| [initialize](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/#config-settings) | Initialiseert het exemplaar van de documentformaat-handler. |
| [initialize_document_format_configuration](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize_document_format_configuration/) |  |
| [is_redaction_accepted](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/#description) | Controleert op implementatie van [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) en roept deze aan, indien gespecificeerd. |
| [is_redaction_accepted_redaction_description](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted_redaction_description/) |  |
| [load](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load/#input) | Laadt het document vanuit een stream. |
| [load_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_streams/) |  |
| [perform_binary_check](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/#input) | Controleert of de gegeven stream een document bevat dat door dit formaatexemplaar wordt ondersteund. |
| [perform_binary_check_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_stream/) |  |
| [perform_binary_check_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_streams/) |  |
| [save](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save/#output) | Slaat het document op in een stream. |
| [save_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_streams/) |  |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/password/) | Het wachtwoord voor met wachtwoord beveiligde documenten. |

### Voorbeeld

```python
class DummyDocument(DocumentFormatInstance):
    def load(self, output: io.RawIOBase) -> None:
        # laad bestandsinhoud
        pass

    def save(self, output: io.RawIOBase) -> None:
        # sla wijzigingen op in bestand
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

### Zie ook
* module [`groupdocs.redaction.integration`](/redaction/python-net/groupdocs.redaction.integration/)
