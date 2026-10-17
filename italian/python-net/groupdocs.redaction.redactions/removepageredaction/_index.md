---
title: "classe RemovePageRedaction"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Rappresenta una redazione che rimuove una pagina (diapositiva, foglio di lavoro, ecc.) da un documento."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/removepageredaction/
is_root: false
weight: 250
---


## RemovePageRedaction class

Rappresenta una redazione che rimuove una pagina (diapositiva, foglio di lavoro, ecc.) da un documento.

Per saperne di più
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about removing pages: https://docs.groupdocs.com/redaction/net/remove-page-redaction/

Il tipo RemovePageRedaction espone i seguenti membri:

### Costruttori
| Costruttore | Descrizione |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/#origin-index-count) | Inizializza un nuovo RemovePageRedaction. |

### Metodi
| Metodo | Descrizione |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to/#format_instance) | Applica la redazione a una data istanza di formato. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to_document_format_instance/) |  |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/count/) | Il numero di pagine da rimuovere. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/index/) | L'indice di posizione iniziale (basato su zero). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/origin/) | La posizione di riferimento di ricerca, sia l'inizio che la fine di un documento. |
| [description](/redaction/python-net/groupdocs.redaction/redaction/description/) | La descrizione della redazione, contenente il suo nome e i parametri. (eredita da [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)) |

### Esempio

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Rimuovi 1 pagina contando dalla fine del documento
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    with Redactor("./test.pdf") as redactor:
        # Applica la redazione
        result = redactor.apply(rem_opt)

        # Salva il documento redatto
        so = SaveOptions()
        so.add_suffix = True
        redactor.save(so)
```

### Guides
Guide operative che utilizzano `RemovePageRedaction`:

* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)

### Vedi anche
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
