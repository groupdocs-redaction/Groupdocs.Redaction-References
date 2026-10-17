---
title: "Classe RedactorConfiguration"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Fornisce l'accesso a un elenco di formati supportati, sia incorporati che personalizzati dall'utente."
type: docs
url: /it/python-net/groupdocs.redaction.configuration/redactorconfiguration/
is_root: false
weight: 20
---


## RedactorConfiguration class

Fornisce l'accesso a un elenco di formati supportati, sia incorporati che personalizzati dall'utente.

Per saperne di più:

- More details about GroupDocs.Redaction configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Il tipo RedactorConfiguration espone i seguenti membri:

### Metodi
| Metodo | Descrizione |
| :- | :- |
| [find_format](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/#file_extension) | Trova le configurazioni di formato per una data estensione di file. |
| [find_format_file](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_file/) |  |
| [find_format_string](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_string/) |  |
| [get_instance](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/) | Restituisce un'istanza singleton con la configurazione predefinita dei formati integrati. |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [available_formats](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/available_formats/) | L'elenco dei formati riconosciuti, vedi [`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/). |

### Esempio

```python
# Aggiungi un gestore di formato utente personalizzato
adobe_photoshop_settings = DocumentFormatConfiguration()
adobe_photoshop_settings.extension_filter = ".psd"
adobe_photoshop_settings.document_type = MyAdobePhotoshopFormatInstance

config = RedactorConfiguration.get_instance()
config.available_formats.add(adobe_photoshop_settings)
```

```python
# Recupera un gestore di formato utente integrato o personalizzato
config = RedactorConfiguration.get_instance()
format_settings = config.find_format(".psd")
```

### Vedi anche
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
