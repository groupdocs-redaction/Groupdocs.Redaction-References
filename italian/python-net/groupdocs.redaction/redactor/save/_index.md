---
title: "metodo save"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Salva il documento su un file con le seguenti opzioni: AddSuffix = True, RasterizeToPDF = True."
type: docs
url: /it/python-net/groupdocs.redaction/redactor/save/
is_root: false
weight: 1080
---


## save

Salva il documento su un file con le seguenti opzioni: AddSuffix = True, RasterizeToPDF = True.

```python
def save(self):
    ...
```

**Returns:** str: Path to redacted document.

### Esempio

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("document.docx") as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    options = SaveOptions()
    options.add_suffix = True
    options.rasterize_to_pdf = True
    result_path = redactor.save(options)
    print(f"Saved to {result_path}")
```

## save {#save_options}

Salva il documento su un file.

```python
def save(self, save_options):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| save_options | `SaveOptions` | Opzioni per aggiungere il suffisso o rasterizzare. |

**Returns:** Path to redacted document.

### Esempio

```python
from datetime import datetime
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions


def save_in_original_format():
    # Specifica le opzioni di redazione
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Carica il documento da redigere
    with Redactor("./sample.docx") as redactor:
        # Applica la redazione
        redactor.apply(ex_red)

        # Salva il documento redatto nel suo formato originale con un suffisso data
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = datetime.now().strftime("%Y-%m-%d %H-%M-%S")

        result_path = redactor.save(so)
        print(f"Document redacted successfully.\nCheck output in {result_path}.")


if __name__ == "__main__":
    save_in_original_format()
```

## save {#document-rasterization_options}

Salva il documento su uno stream, includendo una posizione personalizzata.

```python
def save(self, document, rasterization_options):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| document | `io.RawIOBase` | Flusso di destinazione. |
| rasterization_options | `RasterizationOptions` | Opzioni per rasterizzare o meno e per specificare le pagine da rasterizzare. |

### Esempio

```python
import io
from groupdocs.redaction.options import RasterizationOptions
from groupdocs.redaction import Redactor

with Redactor("document.pptx") as redactor:
    # configura la rasterizzazione per elaborare solo la prima diapositiva
    ro = RasterizationOptions()
    ro.page_index = 0
    ro.page_count = 1

    stream = io.BytesIO()
    redactor.save(stream, ro)

    # l'oggetto BytesIO ora contiene il documento salvato
    data = stream.getvalue()
```

### Vedi anche
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
