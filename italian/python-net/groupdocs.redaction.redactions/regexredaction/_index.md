---
title: "Classe RegexRedaction"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Rappresenta una redazione di testo che ricerca e sostituisce il testo nel documento corrispondendo all'espressione regolare fornita."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/regexredaction/
is_root: false
weight: 230
---


## RegexRedaction class

Rappresenta una redazione di testo che ricerca e sostituisce il testo nel documento corrispondendo all'espressione regolare fornita.

Per saperne di più

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

Il tipo RegexRedaction espone i seguenti membri:

### Costruttori
| Costruttore | Descrizione |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#pattern-options) | Inizializza una nuova istanza di RegexRedaction. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#regex-options) | Inizializza una nuova istanza di RegexRedaction. |

### Metodi
| Metodo | Descrizione |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to/#format_instance) | Applica la redazione a una data istanza di formato. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to_document_format_instance/) |  |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | La descrizione della redazione, contenente il suo nome e i parametri. |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | Il modello di espressione regolare utilizzato per il matching. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | L'istanza [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) che specifica il tipo di sostituzione del testo. (eredita da [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | L'implementazione IOcrConnector utilizzata per estrarre il testo dal contenuto grafico. (eredita da [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Esempio

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("sample.pdf") as redactor:
    # sostituisci con testo
    redactor.apply(RegexRedaction(r"\d{2}\s*\d{2}[^\d]*\d{6}", ReplacementOptions("[removed]")))
    # sostituisci con rettangolo solido blu
    redactor.apply(RegexRedaction(r"^\d+[,\.]{1}\d+$", ReplacementOptions(Color.BLUE)))
    redactor.save()
```

### Guides
Guide operative che utilizzano `RegexRedaction`:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Vedi anche
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
