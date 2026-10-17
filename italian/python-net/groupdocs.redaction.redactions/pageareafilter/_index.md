---
title: "Classe PageAreaFilter"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Rappresenta un filtro di redazione, impostando un'area all'interno di una pagina di un documento per applicare la redazione."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/pageareafilter/
is_root: false
weight: 150
---


## PageAreaFilter class

Rappresenta un filtro di redazione, impostando un'area all'interno di una pagina di un documento per applicare la redazione.

Per saperne di più

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

Il tipo PageAreaFilter espone i seguenti membri:

### Costruttori
| Costruttore | Descrizione |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/#top_left-size) | Inizializza un nuovo PageAreaFilter per redigere un'area specifica. |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [rectangle](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/rectangle/) | Il rettangolo (posizione in alto a sinistra e dimensioni dell'area) su una pagina. |

### Esempio

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

with Redactor("doc.pdf") as redactor:
    page = redactor.get_document_info().pages[0]
    area_filter = PageAreaFilter(
        Point(0, int(page.height / 2)),
        Size(page.width, int(page.height / 2))
    )
```

### Vedi anche
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
