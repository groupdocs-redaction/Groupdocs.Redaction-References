---
title: "DocumentFormatConfiguration klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt een type‑referentie voor een van DocumentFormatInstance afgeleide klasse en een lijst met ondersteunde bestandsextensies voor snellere formatdetectie."
type: docs
url: /nl/python-net/groupdocs.redaction.configuration/documentformatconfiguration/
is_root: false
weight: 10
---


## DocumentFormatConfiguration class

Stelt een type‑referentie voor de van [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)-afgeleide klasse en een lijst met ondersteunde bestandsextensies voor snellere detectie van formaten.

Meer informatie

- More details about **GroupDocs.Redaction** configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

De DocumentFormatConfiguration type bevat de volgende leden:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/__init__/) | Initialiseert een nieuw exemplaar van DocumentFormatConfiguration. |

### Methoden
| Methode | Beschrijving |
| :- | :- |
| [supports_extension](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/#file_extension) | Controleert of een gegeven bestandsextensie kan worden verwerkt als DocumentType. |
| [supports_extension_file](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_file/) |  |
| [supports_extension_string](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_string/) |  |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [document_type](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/document_type/) | Het type van een klasse die erft van [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |
| [extension_filter](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/extension_filter/) | De door komma's gescheiden lijst van bestandsextensies (bijvoorbeeld ".pdf"), hoofdletterongevoelig. |
| [initialization_data](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/initialization_data/) | De gegevens die nodig zijn voor de initialisatie van [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |

### Voorbeeld

```python
from groupdocs.redaction import DocumentFormatConfiguration

# Maak een aangepaste formaatconfiguratie
config = DocumentFormatConfiguration()
config.ExtensionFilter = ".psd"
config.DocumentType = MyAdobePhotoshopFormatInstance
```

### Zie ook
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
