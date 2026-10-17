---
title: "Classe DocumentFormatInstance"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Rappresenta un formato specifico di un documento e può essere implementato per aggiungere tipi di documento personalizzati."
type: docs
url: /it/python-net/groupdocs.redaction.integration/documentformatinstance/
is_root: false
weight: 10
---


## DocumentFormatInstance class

Rappresenta un formato specifico di un documento e può essere implementato per aggiungere tipi di documento personalizzati.

Per saperne di più

- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Il tipo DocumentFormatInstance espone i seguenti membri:

### Metodi
| Metodo | Descrizione |
| :- | :- |
| [initialize](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/#config-settings) | Inizializza l'istanza del gestore del formato documento. |
| [initialize_document_format_configuration](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize_document_format_configuration/) |  |
| [is_redaction_accepted](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/#description) | Verifica la presenza di un'implementazione di [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) e la invoca, se specificata. |
| [is_redaction_accepted_redaction_description](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted_redaction_description/) |  |
| [load](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load/#input) | Carica il documento da uno stream. |
| [load_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_streams/) |  |
| [perform_binary_check](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/#input) | Verifica se lo stream fornito contiene un documento supportato da questa istanza di formato. |
| [perform_binary_check_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_stream/) |  |
| [perform_binary_check_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_streams/) |  |
| [save](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save/#output) | Salva il documento su uno stream. |
| [save_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_streams/) |  |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/password/) | La password per i documenti protetti da password. |

### Esempio

```python
class DummyDocument(DocumentFormatInstance):
    def load(self, output: io.RawIOBase) -> None:
        # carica il contenuto del file
        pass

    def save(self, output: io.RawIOBase) -> None:
        # salva le modifiche nel file
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

### Vedi anche
* module [`groupdocs.redaction.integration`](/redaction/python-net/groupdocs.redaction.integration/)
