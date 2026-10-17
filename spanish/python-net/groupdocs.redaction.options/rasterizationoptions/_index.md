---
title: "Clase RasterizationOptions"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Proporciona opciones para convertir archivos a PDF."
type: docs
url: /es/python-net/groupdocs.redaction.options/rasterizationoptions/
is_root: false
weight: 80
---


## RasterizationOptions class

Proporciona opciones para convertir archivos a PDF.

- More details about saving document as a rasterized PDF: https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/
- More details about rasterization options: https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/

El tipo RasterizationOptions expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/__init__/) | Inicializa una nueva instancia. |

### Métodos
| Método | Descripción |
| :- | :- |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type) | Registra una opción de rasterización avanzada para aplicar. |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type-parameters) | Registra una opción de rasterización avanzada para aplicar. |
| [add_advanced_option_advanced_rasterization_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option_advanced_rasterization_options/) |  |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [compliance](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/compliance/) | El nivel de cumplimiento PDF. |
| [enabled](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/enabled/) | La bandera habilitada indica si todas las páginas del documento se convierten en imágenes y se colocan en un único archivo PDF. Verdadero por defecto; establecer en Falso para evitar la rasterización. |
| [has_advanced_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/has_advanced_options/) | El indicador es True si se establecen opciones avanzadas de rasterización. |
| [page_count](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_count/) | El número de páginas a convertir en PDF. |
| [page_index](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_index/) | El índice de la primera página (basado en 0) para convertir en PDF. |

### Ejemplo

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

### Ver también
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
