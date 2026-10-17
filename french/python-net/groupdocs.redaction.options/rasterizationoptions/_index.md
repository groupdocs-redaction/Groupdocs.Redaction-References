---
title: "Classe RasterizationOptions"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Fournit des options pour convertir des fichiers en PDF."
type: docs
url: /fr/python-net/groupdocs.redaction.options/rasterizationoptions/
is_root: false
weight: 80
---


## RasterizationOptions class

Fournit des options pour convertir des fichiers en PDF.

- More details about saving document as a rasterized PDF: https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/
- More details about rasterization options: https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/

Le type RasterizationOptions expose les membres suivants :

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/__init__/) | Initialise une nouvelle instance. |

### Méthodes
| Méthode | Description |
| :- | :- |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type) | Enregistre une option de rasterisation avancée à appliquer. |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type-parameters) | Enregistre une option de rasterisation avancée à appliquer. |
| [add_advanced_option_advanced_rasterization_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option_advanced_rasterization_options/) |  |

### Propriétés
| Propriété | Description |
| :- | :- |
| [compliance](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/compliance/) | Le niveau de conformité PDF. |
| [enabled](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/enabled/) | Le drapeau activé indique si toutes les pages du document sont converties en images et placées dans un seul fichier PDF. True par défaut ; définissez-le sur False pour éviter la rasterisation. |
| [has_advanced_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/has_advanced_options/) | L'indicateur est True si les options avancées de rasterisation sont définies. |
| [page_count](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_count/) | Le nombre de pages à convertir en PDF. |
| [page_index](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_index/) | L'index de la première page (à partir de 0) à convertir en PDF. |

### Exemple

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

### Voir aussi
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
