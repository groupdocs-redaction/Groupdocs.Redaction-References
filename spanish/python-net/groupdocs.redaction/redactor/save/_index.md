---
title: "método save"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Guarda el documento en un archivo con las siguientes opciones: AddSuffix = True, RasterizeToPDF = True."
type: docs
url: /es/python-net/groupdocs.redaction/redactor/save/
is_root: false
weight: 1080
---


## save

Guarda el documento en un archivo con las siguientes opciones: AddSuffix = True, RasterizeToPDF = True.

```python
def save(self):
    ...
```

**Returns:** str: Path to redacted document.

### Ejemplo

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

Guarda el documento en un archivo.

```python
def save(self, save_options):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| save_options | `SaveOptions` | Opciones para añadir sufijo o rasterizar. |

**Returns:** Path to redacted document.

### Ejemplo

```python
from datetime import datetime
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions


def save_in_original_format():
    # Especifique las opciones de redacción
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Cargue el documento que será redactado
    with Redactor("./sample.docx") as redactor:
        # Aplicar la redacción
        redactor.apply(ex_red)

        # Guardar el documento redactado en su formato original con un sufijo de fecha
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

Guarda el documento en un flujo, incluyendo ubicación personalizada.

```python
def save(self, document, rasterization_options):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| document | `io.RawIOBase` | Flujo de destino. |
| rasterization_options | `RasterizationOptions` | Opciones para rasterizar o no y para especificar páginas para la rasterización. |

### Ejemplo

```python
import io
from groupdocs.redaction.options import RasterizationOptions
from groupdocs.redaction import Redactor

with Redactor("document.pptx") as redactor:
    # configurar la rasterización para procesar solo la primera diapositiva
    ro = RasterizationOptions()
    ro.page_index = 0
    ro.page_count = 1

    stream = io.BytesIO()
    redactor.save(stream, ro)

    # el objeto BytesIO ahora contiene el documento guardado
    data = stream.getvalue()
```

### Ver también
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
