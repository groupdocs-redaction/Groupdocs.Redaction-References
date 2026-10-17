---
title: "Classe PageRangeFilter"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Rappresenta un filtro di redazione, impostando l'intervallo di pagine all'interno di un documento per applicare la redazione."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/pagerangefilter/
is_root: false
weight: 170
---


## PageRangeFilter class

Rappresenta un filtro di redazione, impostando l'intervallo di pagine all'interno di un documento per applicare la redazione.

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

Il tipo PageRangeFilter espone i seguenti membri:

### Costruttori
| Costruttore | Descrizione |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/__init__/#origin-index-count) | Inizializza un nuovo RemovePageRedaction. |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/count/) | Il numero di pagine da rimuovere. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/index/) | L'indice di posizione iniziale (basato su zero). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/origin/) | La posizione di riferimento di ricerca, sia l'inizio che la fine di un documento. |

### Esempio

```python
from groupdocs.redaction.redactions import PageRangeFilter, PageSeekOrigin

# Definisci un filtro che mira all'ultima pagina e a quella precedente.
page_filter = PageRangeFilter(PageSeekOrigin.END, 0, 1)

# Il filtro può essere combinato con altri filtri, ad es., PageAreaFilter,
# e passato a ReplacementOptions.Filters durante la configurazione di una redazione.
```

### Vedi anche
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
