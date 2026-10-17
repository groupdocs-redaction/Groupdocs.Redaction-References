---
title: "Classe DeleteAnnotationRedaction"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Rappresenta una redazione testuale che elimina le annotazioni se il testo corrisponde a una determinata espressione regolare (opzionalmente elimina tutte le annotazioni)."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/deleteannotationredaction/
is_root: false
weight: 60
---


## DeleteAnnotationRedaction class

Rappresenta una redazione testuale che elimina le annotazioni se il testo corrisponde a una determinata espressione regolare (opzionalmente elimina tutte le annotazioni).

Per saperne di più

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

Il tipo DeleteAnnotationRedaction espone i seguenti membri:

### Costruttori
| Costruttore | Descrizione |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/) | Inizializza una nuova istanza della classe DeleteAnnotationRedaction, con impostazioni per eliminare tutte le annotazioni (corrispondenti a tutto). |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#pattern) | Inizializza una nuova istanza della classe DeleteAnnotationRedaction, eliminando le annotazioni che corrispondono all'espressione fornita. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#regex) | Inizializza una nuova istanza della classe DeleteAnnotationRedaction, eliminando le annotazioni che corrispondono all'espressione fornita. |

### Metodi
| Metodo | Descrizione |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to/#format_instance) | Applica la redazione a una data istanza di formato. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to_document_format_instance/) |  |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/description/) | La descrizione della redazione, contenente il nome della redazione e i parametri. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/expression/) | L'espressione regolare da corrispondere. |

### Esempio

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

with Redactor("document.pdf") as redactor:
    # Elimina le annotazioni contenenti la parola "internal" (senza distinzione tra maiuscole e minuscole)
    redactor.apply(DeleteAnnotationRedaction("(?i)internal"))
    redactor.save()
```

### Guides
Guide operative che utilizzano `DeleteAnnotationRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Vedi anche
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
