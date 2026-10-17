---
title: "RedactorConfiguration Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Bietet Zugriff auf eine Liste unterstützter Formate, integrierter und benutzerdefinierter Formate."
type: docs
url: /de/python-net/groupdocs.redaction.configuration/redactorconfiguration/
is_root: false
weight: 20
---


## RedactorConfiguration class

Bietet Zugriff auf eine Liste unterstützter Formate, integrierter und benutzerdefinierter Formate.

Mehr erfahren:

- More details about GroupDocs.Redaction configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Der RedactorConfiguration-Typ stellt die folgenden Mitglieder bereit:

### Methoden
| Methode | Beschreibung |
| :- | :- |
| [find_format](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/#file_extension) | Findet Formatkonfigurationen für eine gegebene Dateierweiterung. |
| [find_format_file](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_file/) |  |
| [find_format_string](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_string/) |  |
| [get_instance](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/) | Gibt eine Singleton-Instanz mit der Standardkonfiguration der integrierten Formate zurück. |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [available_formats](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/available_formats/) | Die Liste der erkannten Formate, siehe [`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/). |

### Beispiel

```python
# Fügen Sie einen benutzerdefinierten Format-Handler hinzu
adobe_photoshop_settings = DocumentFormatConfiguration()
adobe_photoshop_settings.extension_filter = ".psd"
adobe_photoshop_settings.document_type = MyAdobePhotoshopFormatInstance

config = RedactorConfiguration.get_instance()
config.available_formats.add(adobe_photoshop_settings)
```

```python
# Rufen Sie einen integrierten oder benutzerdefinierten Format-Handler ab
config = RedactorConfiguration.get_instance()
format_settings = config.find_format(".psd")
```

### Siehe auch
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
