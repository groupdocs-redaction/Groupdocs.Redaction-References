---
title: "Klassen RasterizationOptions"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Tillhandahåller alternativ för att konvertera filer till PDF."
type: docs
url: /sv/python-net/groupdocs.redaction.options/rasterizationoptions/
is_root: false
weight: 80
---


## RasterizationOptions class

Tillhandahåller alternativ för att konvertera filer till PDF.

- More details about saving document as a rasterized PDF: https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/
- More details about rasterization options: https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/

Typen RasterizationOptions visar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/__init__/) | Initierar en ny instans. |

### Metoder
| Metod | Beskrivning |
| :- | :- |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type) | Registrerar ett avancerat rasteriseringsalternativ att tillämpa. |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type-parameters) | Registrerar ett avancerat rasteriseringsalternativ att tillämpa. |
| [add_advanced_option_advanced_rasterization_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option_advanced_rasterization_options/) |  |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [compliance](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/compliance/) | PDF‑kompatibilitetsnivån. |
| [enabled](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/enabled/) | Den aktiverade flaggan indikerar om alla sidor i dokumentet konverteras till bilder och placeras i en enda PDF‑fil. True som standard; sätt till False för att undvika rasterisering. |
| [has_advanced_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/has_advanced_options/) | Indikatorn är True om avancerade rasteriseringsalternativ är inställda. |
| [page_count](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_count/) | Antalet sidor som ska konverteras till PDF. |
| [page_index](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_index/) | Indexet för den första sidan (0‑baserat) som ska konverteras till PDF. |

### Exempel

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

### Se även
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
