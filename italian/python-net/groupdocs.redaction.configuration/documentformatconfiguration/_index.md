---
title: "Classe DocumentFormatConfiguration"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Rappresenta un riferimento di tipo per la classe derivata da DocumentFormatInstance e un elenco di estensioni di file supportate per una rilevazione del formato più veloce."
type: docs
url: /it/python-net/groupdocs.redaction.configuration/documentformatconfiguration/
is_root: false
weight: 10
---


## DocumentFormatConfiguration class

Rappresenta un riferimento di tipo per la classe derivata da [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) e un elenco di estensioni di file supportate per una più rapida rilevazione del formato.

Per saperne di più

- More details about **GroupDocs.Redaction** configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Il tipo DocumentFormatConfiguration espone i seguenti membri:

### Costruttori
| Costruttore | Descrizione |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/__init__/) | Inizializza una nuova istanza di DocumentFormatConfiguration. |

### Metodi
| Metodo | Descrizione |
| :- | :- |
| [supports_extension](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/#file_extension) | Verifica se un’estensione di file fornita può essere gestita come DocumentType. |
| [supports_extension_file](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_file/) |  |
| [supports_extension_string](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_string/) |  |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [document_type](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/document_type/) | Il tipo di una classe che eredita da [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |
| [extension_filter](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/extension_filter/) | L'elenco delimitato da virgole delle estensioni di file (ad esempio ".pdf"), senza distinzione tra maiuscole e minuscole. |
| [initialization_data](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/initialization_data/) | I dati richiesti per l'inizializzazione di [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |

### Esempio

```python
from groupdocs.redaction import DocumentFormatConfiguration

# Crea una configurazione di formato personalizzata
config = DocumentFormatConfiguration()
config.ExtensionFilter = ".psd"
config.DocumentType = MyAdobePhotoshopFormatInstance
```

### Vedi anche
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
