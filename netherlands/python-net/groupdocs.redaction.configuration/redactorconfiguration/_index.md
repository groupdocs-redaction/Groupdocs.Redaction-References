---
title: "RedactorConfiguration klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Biedt toegang tot een lijst met ondersteunde formaten, ingebouwde en aangepaste gebruikersformaten."
type: docs
url: /nl/python-net/groupdocs.redaction.configuration/redactorconfiguration/
is_root: false
weight: 20
---


## RedactorConfiguration class

Biedt toegang tot een lijst met ondersteunde formaten, ingebouwde en aangepaste gebruikersformaten.

Meer informatie:

- More details about GroupDocs.Redaction configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

De RedactorConfiguration type bevat de volgende leden:

### Methoden
| Methode | Beschrijving |
| :- | :- |
| [find_format](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/#file_extension) | Vindt formatconfiguraties voor een gegeven bestandsextensie. |
| [find_format_file](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_file/) |  |
| [find_format_string](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_string/) |  |
| [get_instance](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/) | Retourneert een singleton‑instantie met de standaardconfiguratie van ingebouwde formaten. |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [available_formats](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/available_formats/) | De lijst met herkende formaten, zie [`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/). |

### Voorbeeld

```python
# Voeg een aangepaste gebruikersformaat‑handler toe
adobe_photoshop_settings = DocumentFormatConfiguration()
adobe_photoshop_settings.extension_filter = ".psd"
adobe_photoshop_settings.document_type = MyAdobePhotoshopFormatInstance

config = RedactorConfiguration.get_instance()
config.available_formats.add(adobe_photoshop_settings)
```

```python
# Haal een ingebouwde of aangepaste gebruikersformaat‑handler op
config = RedactorConfiguration.get_instance()
format_settings = config.find_format(".psd")
```

### Zie ook
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
