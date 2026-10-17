---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuw object met standaardinstellingen: rasterizetopdf is False en addsuffix is False."
type: docs
url: /nl/python-net/groupdocs.redaction.options/saveoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initialiseert een nieuw exemplaar met standaardinstellingen: rasterize_to_pdf is False en add_suffix is False.

```python
def __init__(self):
    ...
```

### Voorbeeld

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

Initialiseert een nieuw exemplaar met opgegeven parameters.

```python
def __init__(self, rasterize_to_pdf, suffix):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| rasterize_to_pdf | `bool` | True, als alle pagina's in het document moeten worden geconverteerd naar afbeeldingen en in één PDF‑bestand moeten worden geplaatst. |
| suffix | `str` | Deze tekst wordt toegevoegd aan het einde van de bestandsnaam; indien niet leeg stelt dit ook `add_suffix` in op True. |

### Voorbeeld

```python
from groupdocs.redaction.options import SaveOptions

# Maak opslaan‑opties met standaardinstellingen
options = SaveOptions()
options.add_suffix = True
options.rasterize_to_pdf = True
options.redacted_file_suffix = "redacted"
```

### Zie ook
* class [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/)
