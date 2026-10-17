---
title: "LoadOptions klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Tillhandahåller alternativ som kommer att användas för att öppna en fil."
type: docs
url: /sv/python-net/groupdocs.redaction.options/loadoptions/
is_root: false
weight: 40
---


## LoadOptions class

Tillhandahåller alternativ som kommer att användas för att öppna en fil.

Läs mer
- [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
- [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
- [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
- [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

Typen LoadOptions visar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/) | Initierar en ny instans av LoadOptions-klass. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password) | Initierar en ny instans av LoadOptions med det angivna lösenordet. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#pre_rasterize) | Initierar en ny LoadOptions-instans med den angivna pre‑rasteriseringsflaggan. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password-pre_rasterize) | Initierar en ny LoadOptions-instans med det angivna lösenordet. |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.options/loadoptions/password/) | Lösenordet för lösenordsskyddade dokument. |
| [pre_rasterize](/redaction/python-net/groupdocs.redaction.options/loadoptions/pre_rasterize/) | pre_rasterize-flaggan som indikerar om filen ska för‑rasteriseras. |

### Exempel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Ange laddningsalternativen med dokumentets lösenord
load_opt = LoadOptions("mypassword")

# Definiera en redigering
repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

# Öppna det lösenordsskyddade dokumentet
with Redactor("./protected.docx", load_opt) as redactor:
    redactor.apply(ex_red)

    # Spara det redigerade dokumentet
    save_opt = SaveOptions()
    save_opt.add_suffix = True
    result_path = redactor.save(save_opt)
    print(f"Document redacted successfully. Check output in {result_path}.")
```

### Se även
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
