---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny instans med standardinställningar: rasterizetopdf är False och addsuffix är False."
type: docs
url: /sv/python-net/groupdocs.redaction.options/saveoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initierar en ny instans med standardinställningar: rasterize_to_pdf är False och add_suffix är False.

```python
def __init__(self):
    ...
```

### Exempel

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

Initierar en ny instans med angivna parametrar.

```python
def __init__(self, rasterize_to_pdf, suffix):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| rasterize_to_pdf | `bool` | Sant, om alla sidor i dokumentet måste konverteras till bilder och placeras i en enda PDF-fil. |
| suffix | `str` | Denna text kommer att läggas till i slutet av filnamnet; om den inte är tom sätter den också `add_suffix` till True. |

### Exempel

```python
from groupdocs.redaction.options import SaveOptions

# Skapa sparaalternativ med standardinställningar
options = SaveOptions()
options.add_suffix = True
options.rasterize_to_pdf = True
options.redacted_file_suffix = "redacted"
```

### Se även
* class [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/)
