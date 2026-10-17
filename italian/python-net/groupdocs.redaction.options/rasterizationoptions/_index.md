---
title: "Classe RasterizationOptions"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Fornisce opzioni per convertire i file in PDF."
type: docs
url: /it/python-net/groupdocs.redaction.options/rasterizationoptions/
is_root: false
weight: 80
---


## RasterizationOptions class

Fornisce opzioni per convertire i file in PDF.

- More details about saving document as a rasterized PDF: https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/
- More details about rasterization options: https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/

Il tipo RasterizationOptions espone i seguenti membri:

### Costruttori
| Costruttore | Descrizione |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/__init__/) | Inizializza una nuova istanza. |

### Metodi
| Metodo | Descrizione |
| :- | :- |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type) | Registra un'opzione di rasterizzazione avanzata da applicare. |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type-parameters) | Registra un'opzione di rasterizzazione avanzata da applicare. |
| [add_advanced_option_advanced_rasterization_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option_advanced_rasterization_options/) |  |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [compliance](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/compliance/) | Il livello di conformità PDF. |
| [enabled](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/enabled/) | Il flag abilitato indica se tutte le pagine del documento vengono convertite in immagini e inserite in un unico file PDF. Vero per impostazione predefinita; impostalo su False per evitare la rasterizzazione. |
| [has_advanced_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/has_advanced_options/) | L'indicatore è True se sono impostate opzioni avanzate di rasterizzazione. |
| [page_count](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_count/) | Il numero di pagine da convertire in PDF. |
| [page_index](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_index/) | L'indice della prima pagina (basato su 0) da convertire in PDF. |

### Esempio

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

### Vedi anche
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
