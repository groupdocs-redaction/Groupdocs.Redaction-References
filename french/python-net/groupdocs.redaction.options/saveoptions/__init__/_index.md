---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise une nouvelle instance avec les paramètres par défaut : rasterizetopdf est False et addsuffix est False."
type: docs
url: /fr/python-net/groupdocs.redaction.options/saveoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initialise une nouvelle instance avec les paramètres par défaut : rasterize_to_pdf est False et add_suffix est False.

```python
def __init__(self):
    ...
```

### Exemple

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

Initialise une nouvelle instance avec les paramètres fournis.

```python
def __init__(self, rasterize_to_pdf, suffix):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| rasterize_to_pdf | `bool` | True, si toutes les pages du document doivent être converties en images et placées dans un seul fichier PDF. |
| suffix | `str` | Ce texte sera ajouté à la fin du nom de fichier ; s'il n'est pas vide, il définit également `add_suffix` à True. |

### Exemple

```python
from groupdocs.redaction.options import SaveOptions

# Créer des options de sauvegarde avec les paramètres par défaut
options = SaveOptions()
options.add_suffix = True
options.rasterize_to_pdf = True
options.redacted_file_suffix = "redacted"
```

### Voir aussi
* class [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/)
