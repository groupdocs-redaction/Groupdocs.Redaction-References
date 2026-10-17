---
title: "LoadOptions klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Biedt opties die worden gebruikt om een bestand te openen."
type: docs
url: /nl/python-net/groupdocs.redaction.options/loadoptions/
is_root: false
weight: 40
---


## LoadOptions class

Biedt opties die worden gebruikt om een bestand te openen.

Meer informatie
- [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
- [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
- [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
- [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

Het LoadOptions-type geeft de volgende leden weer:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/) | Initialiseert een nieuw exemplaar van de LoadOptions-klasse. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password) | Initialiseert een nieuw exemplaar van LoadOptions met het opgegeven wachtwoord. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#pre_rasterize) | Initialiseert een nieuw LoadOptions-exemplaar met de opgegeven pre‑rasterisatie‑vlag. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password-pre_rasterize) | Initialiseert een nieuw LoadOptions-exemplaar met het opgegeven wachtwoord. |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.options/loadoptions/password/) | Het wachtwoord voor met wachtwoord beveiligde documenten. |
| [pre_rasterize](/redaction/python-net/groupdocs.redaction.options/loadoptions/pre_rasterize/) | De pre_rasterize‑vlag geeft aan of het bestand vooraf moet worden gerasterd. |

### Voorbeeld

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Geef de laadopties op met het documentwachtwoord
load_opt = LoadOptions("mypassword")

# Definieer een redactie
repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

# Open het wachtwoord‑beveiligde document
with Redactor("./protected.docx", load_opt) as redactor:
    redactor.apply(ex_red)

    # Sla het geredigeerde document op
    save_opt = SaveOptions()
    save_opt.add_suffix = True
    result_path = redactor.save(save_opt)
    print(f"Document redacted successfully. Check output in {result_path}.")
```

### Zie ook
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
