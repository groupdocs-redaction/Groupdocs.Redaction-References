---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva instancia con la configuración predeterminada: rasterizetopdf es False y addsuffix es False."
type: docs
url: /es/python-net/groupdocs.redaction.options/saveoptions/__init__/
is_root: false
weight: 10
---


## __init__

Inicializa una nueva instancia con la configuración predeterminada: rasterize_to_pdf es False y add_suffix es False.

```python
def __init__(self):
    ...
```

### Ejemplo

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

Inicializa una nueva instancia con los parámetros proporcionados.

```python
def __init__(self, rasterize_to_pdf, suffix):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| rasterize_to_pdf | `bool` | True, si todas las páginas del documento deben convertirse en imágenes y colocarse en un solo archivo PDF. |
| suffix | `str` | Este texto se añadirá al final del nombre del archivo; si no está vacío también establece `add_suffix` a True. |

### Ejemplo

```python
from groupdocs.redaction.options import SaveOptions

# Crear opciones de guardado con la configuración predeterminada
options = SaveOptions()
options.add_suffix = True
options.rasterize_to_pdf = True
options.redacted_file_suffix = "redacted"
```

### Ver también
* class [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/)
