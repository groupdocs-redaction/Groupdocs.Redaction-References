---
title: "DocumentFormatConfiguration-klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Representerar en typreferens för en DocumentFormatInstance‑avledd klass och en lista över stödjade filändelser för snabbare formatdetektering."
type: docs
url: /sv/python-net/groupdocs.redaction.configuration/documentformatconfiguration/
is_root: false
weight: 10
---


## DocumentFormatConfiguration class

Representerar en typreferens för [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)-avledd klass och en lista över stödda filändelser för snabbare formatdetektering.

Läs mer

- More details about **GroupDocs.Redaction** configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Typen DocumentFormatConfiguration visar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/__init__/) | Initierar en ny instans av DocumentFormatConfiguration. |

### Metoder
| Metod | Beskrivning |
| :- | :- |
| [supports_extension](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/#file_extension) | Kontrollerar om en given filändelse kan hanteras som DocumentType. |
| [supports_extension_file](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_file/) |  |
| [supports_extension_string](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_string/) |  |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [document_type](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/document_type/) | Typen av en klass som ärver från [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |
| [extension_filter](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/extension_filter/) | Den kommaseparerade listan med filändelser (till exempel ".pdf"), skiftlägesokänslig. |
| [initialization_data](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/initialization_data/) | Data som krävs för initiering av [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/). |

### Exempel

```python
from groupdocs.redaction import DocumentFormatConfiguration

# Skapa en anpassad formatkonfiguration
config = DocumentFormatConfiguration()
config.ExtensionFilter = ".psd"
config.DocumentType = MyAdobePhotoshopFormatInstance
```

### Se även
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
