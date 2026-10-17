---
title: "RedactorConfiguration-klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Tillhandahåller åtkomst till en lista över stödda format, inbyggda och anpassade användarformat."
type: docs
url: /sv/python-net/groupdocs.redaction.configuration/redactorconfiguration/
is_root: false
weight: 20
---


## RedactorConfiguration class

Tillhandahåller åtkomst till en lista över stödda format, inbyggda och anpassade användarformat.

Läs mer:

- More details about GroupDocs.Redaction configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Typen RedactorConfiguration visar följande medlemmar:

### Metoder
| Metod | Beskrivning |
| :- | :- |
| [find_format](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/#file_extension) | Hittar formatkonfigurationer för en given filändelse. |
| [find_format_file](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_file/) |  |
| [find_format_string](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_string/) |  |
| [get_instance](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/) | Returnerar en singleton-instans med standardkonfigurationen för inbyggda format. |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [available_formats](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/available_formats/) | Listan över erkända format, se [`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/). |

### Exempel

```python
# Lägg till en anpassad användarformat‑hanterare
adobe_photoshop_settings = DocumentFormatConfiguration()
adobe_photoshop_settings.extension_filter = ".psd"
adobe_photoshop_settings.document_type = MyAdobePhotoshopFormatInstance

config = RedactorConfiguration.get_instance()
config.available_formats.add(adobe_photoshop_settings)
```

```python
# Hämta en inbyggd eller anpassad användarformat‑hanterare
config = RedactorConfiguration.get_instance()
format_settings = config.find_format(".psd")
```

### Se även
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
