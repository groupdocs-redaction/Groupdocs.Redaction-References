---
title: "Clase LoadOptions"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Proporciona opciones que se usarán para abrir un archivo."
type: docs
url: /es/python-net/groupdocs.redaction.options/loadoptions/
is_root: false
weight: 40
---


## LoadOptions class

Proporciona opciones que se usarán para abrir un archivo.

Aprende más
- [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
- [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
- [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
- [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

El tipo LoadOptions expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/) | Inicializa una nueva instancia de la clase LoadOptions. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password) | Inicializa una nueva instancia de LoadOptions con la contraseña especificada. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#pre_rasterize) | Inicializa una nueva instancia de LoadOptions con el indicador de pre‑rasterización especificado. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password-pre_rasterize) | Inicializa una nueva instancia de LoadOptions con la contraseña especificada. |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.options/loadoptions/password/) | La contraseña para documentos protegidos con contraseña. |
| [pre_rasterize](/redaction/python-net/groupdocs.redaction.options/loadoptions/pre_rasterize/) | El indicador pre_rasterize que indica si el archivo debe ser pre‑rasterizado. |

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Especifique las opciones de carga con la contraseña del documento
load_opt = LoadOptions("mypassword")

# Defina una redacción
repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

# Abra el documento protegido con contraseña
with Redactor("./protected.docx", load_opt) as redactor:
    redactor.apply(ex_red)

    # Guarde el documento redactado
    save_opt = SaveOptions()
    save_opt.add_suffix = True
    result_path = redactor.save(save_opt)
    print(f"Document redacted successfully. Check output in {result_path}.")
```

### Ver también
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
