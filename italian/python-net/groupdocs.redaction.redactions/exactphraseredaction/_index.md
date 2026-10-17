---
title: "classe ExactPhraseRedaction"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Rappresenta una redazione testuale che sostituisce una frase esatta nel testo del documento, senza distinzione tra maiuscole e minuscole per impostazione predefinita."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/exactphraseredaction/
is_root: false
weight: 80
---


## ExactPhraseRedaction class

Rappresenta una redazione testuale che sostituisce una frase esatta nel testo del documento, senza distinzione tra maiuscole e minuscole per impostazione predefinita.

Per saperne di più:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/

Il tipo ExactPhraseRedaction espone i seguenti membri:

### Costruttori
| Costruttore | Descrizione |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-options) | Inizializza una nuova istanza di ExactPhraseRedaction in modalità non sensibile al maiuscolo/minuscolo. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-is_case_sensitive-options) | Inizializza una nuova istanza di ExactPhraseRedaction. |

### Metodi
| Metodo | Descrizione |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to/#format_instance) | Applica la redazione a una data istanza di formato. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to_document_format_instance/) |  |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/description/) | La descrizione della redazione, contenente il nome della redazione e i parametri. |
| [is_case_sensitive](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_case_sensitive/) | Il valore che indica se la ricerca è sensibile al maiuscolo/minuscolo. |
| [is_right_to_left](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_right_to_left/) | Il flag di direzione del testo che indica se il testo è da destra a sinistra. Il valore predefinito è False. |
| [search_phrase](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/search_phrase/) | La stringa da cercare e sostituire. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | L'istanza [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) che specifica il tipo di sostituzione del testo. (eredita da [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | L'implementazione IOcrConnector utilizzata per estrarre il testo dal contenuto grafico. (eredita da [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Esempio

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("sample.pdf") as redactor:
    # sostituzione sensibile al maiuscolo/minuscolo
    redactor.apply(ExactPhraseRedaction("John Doe", True, ReplacementOptions("[personal]")))
    redactor.save()
```

### Guides
Guide operative che utilizzano `ExactPhraseRedaction`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Vedi anche
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
