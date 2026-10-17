---
title: "classe LoadOptions"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Fornisce opzioni che saranno utilizzate per aprire un file."
type: docs
url: /it/python-net/groupdocs.redaction.options/loadoptions/
is_root: false
weight: 40
---


## LoadOptions class

Fornisce opzioni che saranno utilizzate per aprire un file.

Per saperne di più
- [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
- [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
- [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
- [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

Il tipo LoadOptions espone i seguenti membri:

### Costruttori
| Costruttore | Descrizione |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/) | Inizializza una nuova istanza della classe LoadOptions. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password) | Inizializza una nuova istanza di LoadOptions con la password specificata. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#pre_rasterize) | Inizializza una nuova istanza di LoadOptions con il flag di pre‑rasterizzazione specificato. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password-pre_rasterize) | Inizializza una nuova istanza di LoadOptions con la password specificata. |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.options/loadoptions/password/) | La password per i documenti protetti da password. |
| [pre_rasterize](/redaction/python-net/groupdocs.redaction.options/loadoptions/pre_rasterize/) | Il flag pre_rasterize indica se il file deve essere pre‑rasterizzato. |

### Esempio

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Specifica le opzioni di caricamento con la password del documento
load_opt = LoadOptions("mypassword")

# Definisci una redazione
repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

# Apri il documento protetto da password
with Redactor("./protected.docx", load_opt) as redactor:
    redactor.apply(ex_red)

    # Salva il documento redatto
    save_opt = SaveOptions()
    save_opt.add_suffix = True
    result_path = redactor.save(save_opt)
    print(f"Document redacted successfully. Check output in {result_path}.")
```

### Vedi anche
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
