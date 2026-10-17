---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza una nuova istanza con le impostazioni predefinite: rasterizetopdf è False e addsuffix è False."
type: docs
url: /it/python-net/groupdocs.redaction.options/saveoptions/__init__/
is_root: false
weight: 10
---


## __init__

Inizializza una nuova istanza con le impostazioni predefinite: rasterize_to_pdf è False e add_suffix è False.

```python
def __init__(self):
    ...
```

### Esempio

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

with Redactor("./sample.docx") as redactor:
    redactor.apply(ex_red)
    save_options = SaveOptions()  # defaults: rasterize_to_pdf=False, add_suffix=False
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}.")
```

## __init__ {#rasterize_to_pdf-suffix}

Inizializza una nuova istanza con i parametri forniti.

```python
def __init__(self, rasterize_to_pdf, suffix):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| rasterize_to_pdf | `bool` | True, se tutte le pagine del documento devono essere convertite in immagini e inserite in un unico file PDF. |
| suffix | `str` | Questo testo sarà aggiunto alla fine del nome file; se non è vuoto imposta anche `add_suffix` a True. |

### Esempio

```python
from groupdocs.redaction.options import SaveOptions

# Crea le opzioni di salvataggio con le impostazioni predefinite
options = SaveOptions()
options.add_suffix = True
options.rasterize_to_pdf = True
options.redacted_file_suffix = "redacted"
```

### Vedi anche
* class [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/)
