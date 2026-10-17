---
title: "RasterizationOptions klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Biedt opties voor het converteren van bestanden naar PDF."
type: docs
url: /nl/python-net/groupdocs.redaction.options/rasterizationoptions/
is_root: false
weight: 80
---


## RasterizationOptions class

Biedt opties voor het converteren van bestanden naar PDF.

- More details about saving document as a rasterized PDF: https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/
- More details about rasterization options: https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/

Het type RasterizationOptions bevat de volgende leden:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/__init__/) | Initialiseert een nieuw exemplaar. |

### Methoden
| Methode | Beschrijving |
| :- | :- |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type) | Registreert een geavanceerde rasterisatie-optie om toe te passen. |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type-parameters) | Registreert een geavanceerde rasterisatie-optie om toe te passen. |
| [add_advanced_option_advanced_rasterization_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option_advanced_rasterization_options/) |  |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [compliance](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/compliance/) | Het PDF-complianceniveau. |
| [enabled](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/enabled/) | De ingeschakelde vlag geeft aan of alle pagina's in het document worden geconverteerd naar afbeeldingen en in één PDF-bestand worden geplaatst. True standaard; stel in op False om rasterisatie te vermijden. |
| [has_advanced_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/has_advanced_options/) | De indicator is True als geavanceerde rasterisatie-opties zijn ingesteld. |
| [page_count](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_count/) | Het aantal pagina's dat naar PDF moet worden geconverteerd. |
| [page_index](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_index/) | De index van de eerste pagina (0-gebaseerd) die naar PDF moet worden geconverteerd. |

### Voorbeeld

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

### Zie ook
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
