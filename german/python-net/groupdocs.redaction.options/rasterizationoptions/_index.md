---
title: "Klasse RasterizationOptions"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt Optionen zum Konvertieren von Dateien in PDF bereit."
type: docs
url: /de/python-net/groupdocs.redaction.options/rasterizationoptions/
is_root: false
weight: 80
---


## RasterizationOptions class

Stellt Optionen zum Konvertieren von Dateien in PDF bereit.

- More details about saving document as a rasterized PDF: https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/
- More details about rasterization options: https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/

Der Typ RasterizationOptions stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/__init__/) | Initialisiert eine neue Instanz. |

### Methoden
| Methode | Beschreibung |
| :- | :- |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type) | Registriert eine erweiterte Rasterisierungsoption zum Anwenden. |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type-parameters) | Registriert eine erweiterte Rasterisierungsoption zum Anwenden. |
| [add_advanced_option_advanced_rasterization_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option_advanced_rasterization_options/) |  |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [compliance](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/compliance/) | Das PDF-Konformitätsniveau. |
| [enabled](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/enabled/) | Das aktivierte Flag gibt an, ob alle Seiten im Dokument in Bilder konvertiert und in einer einzigen PDF-Datei abgelegt werden. Standardmäßig True; auf False setzen, um die Rasterisierung zu vermeiden. |
| [has_advanced_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/has_advanced_options/) | Der Indikator ist True, wenn erweiterte Rasterisierungsoptionen gesetzt sind. |
| [page_count](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_count/) | Die Anzahl der Seiten, die in PDF konvertiert werden sollen. |
| [page_index](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_index/) | Der Index der ersten Seite (0-basiert), die in PDF konvertiert werden soll. |

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import RasterizationOptions, PdfComplianceLevel

with Redactor("SomePresentation.pptx") as redactor:
    ro = RasterizationOptions()
    ro.page_index = 0          # first slide
    ro.page_count = 1
    ro.compliance = PdfComplianceLevel.PdfA1a
    redactor.save("PresentationFirstSlide.pdf", ro)
```

### Siehe auch
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
