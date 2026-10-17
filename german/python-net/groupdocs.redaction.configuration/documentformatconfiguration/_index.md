---
title: "DocumentFormatConfiguration Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt eine Typreferenz für von DocumentFormatInstance abgeleitete Klassen und eine Liste unterstützter Dateierweiterungen für eine schnellere Formaterkennung dar."
type: docs
url: /de/python-net/groupdocs.redaction.configuration/documentformatconfiguration/
is_root: false
weight: 10
---


## DocumentFormatConfiguration class

Stellt eine Typreferenz für die von [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)-abgeleitete Klasse und eine Liste unterstützter Dateierweiterungen für eine schnellere Format-Erkennung dar.

Mehr erfahren

- More details about **GroupDocs.Redaction** configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Der DocumentFormatConfiguration-Typ stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/__init__/) | Initialisiert eine neue Instanz von DocumentFormatConfiguration. |

### Methoden
| Methode | Beschreibung |
| :- | :- |
| [supports_extension](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/#file_extension) | Überprüft, ob eine gegebene Dateierweiterung als DocumentType verarbeitet werden kann. |
| [supports_extension_file](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_file/) |  |
| [supports_extension_string](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_string/) |  |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [document_type](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/document_type/) | Der Typ einer Klasse, die von [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) erbt. |
| [extension_filter](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/extension_filter/) | Die kommagetrennte Liste von Dateierweiterungen (z. B. ".pdf"), nicht groß‑/kleinschreibungssensitiv. |
| [initialization_data](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/initialization_data/) | Die für die Initialisierung von [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) erforderlichen Daten. |

### Beispiel

```python
from groupdocs.redaction import DocumentFormatConfiguration

# Erstelle eine benutzerdefinierte Formatkonfiguration
config = DocumentFormatConfiguration()
config.ExtensionFilter = ".psd"
config.DocumentType = MyAdobePhotoshopFormatInstance
```

### Siehe auch
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
