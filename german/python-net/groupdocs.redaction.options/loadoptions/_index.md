---
title: "LoadOptions Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt Optionen bereit, die zum Öffnen einer Datei verwendet werden."
type: docs
url: /de/python-net/groupdocs.redaction.options/loadoptions/
is_root: false
weight: 40
---


## LoadOptions class

Stellt Optionen bereit, die zum Öffnen einer Datei verwendet werden.

Mehr erfahren
- [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
- [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
- [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
- [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

Der LoadOptions Typ stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/) | Initialisiert eine neue Instanz der LoadOptions Klasse. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password) | Initialisiert eine neue Instanz von LoadOptions mit dem angegebenen Passwort. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#pre_rasterize) | Initialisiert eine neue LoadOptions‑Instanz mit dem angegebenen Pre‑Rasterisierungs‑Flag. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password-pre_rasterize) | Initialisiert eine neue LoadOptions‑Instanz mit dem angegebenen Passwort. |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.options/loadoptions/password/) | Das Passwort für passwortgeschützte Dokumente. |
| [pre_rasterize](/redaction/python-net/groupdocs.redaction.options/loadoptions/pre_rasterize/) | Das pre_rasterize‑Flag gibt an, ob die Datei vorgerastert werden soll. |

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Geben Sie die Ladeoptionen mit dem Dokumentenpasswort an
load_opt = LoadOptions("mypassword")

# Definieren Sie eine Redaktion
repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

# Öffnen Sie das passwortgeschützte Dokument
with Redactor("./protected.docx", load_opt) as redactor:
    redactor.apply(ex_red)

    # Speichern Sie das redigierte Dokument
    save_opt = SaveOptions()
    save_opt.add_suffix = True
    result_path = redactor.save(save_opt)
    print(f"Document redacted successfully. Check output in {result_path}.")
```

### Siehe auch
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
