---
title: "Classe ReplacementOptions"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Rappresenta le opzioni per la sostituzione del testo corrispondente."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/replacementoptions/
is_root: false
weight: 260
---


## ReplacementOptions class

Rappresenta le opzioni per la sostituzione del testo corrispondente.

Per saperne di più

- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

Il tipo ReplacementOptions espone i seguenti membri:

### Costruttori
| Costruttore | Descrizione |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#replacement) | Inizializza una nuova istanza di ReplacementOptions con il testo di sostituzione specificato. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#color) | Inizializza una nuova istanza della classe ReplacementOptions con un rettangolo colorato come opzione. |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/action_type/) | L'azione di sostituzione: disegnare un riquadro o sostituire il testo. |
| [box_color](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_color/) | Il colore per l'opzione `ReplacementType.draw_box` (ignorato altrimenti). |
| [custom_redaction](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/custom_redaction/) | Il gestore di redazione personalizzato che consente agli utenti di definire la propria logica di redazione. |
| [filters](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/filters/) | L'array di filtri da applicare con questa redazione. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/replacement/) | Il valore di sostituzione testuale. |

### Esempio

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Sostituisci il testo corrispondente con il segnaposto "[X]"
repl_opt = ReplacementOptions("[X]")
```

### Guides
Guide operative che utilizzano `ReplacementOptions`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Vedi anche
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
