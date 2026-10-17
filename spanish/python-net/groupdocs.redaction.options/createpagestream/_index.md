---
title: "Clase CreatePageStream"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa un método que devuelve un flujo para escribir datos de vista previa de la página."
type: docs
url: /es/python-net/groupdocs.redaction.options/createpagestream/
is_root: false
weight: 20
---


## CreatePageStream class

Representa un método que devuelve un flujo para escribir datos de vista previa de la página.

El tipo CreatePageStream expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/createpagestream/__init__/#object-method) |  |

### Métodos
| Método | Descripción |
| :- | :- |
| [begin_invoke](/redaction/python-net/groupdocs.redaction.options/createpagestream/begin_invoke/#page_number-callback-object) |  |
| [begin_invoke_int32](/redaction/python-net/groupdocs.redaction.options/createpagestream/begin_invoke_int32/) |  |
| [end_invoke](/redaction/python-net/groupdocs.redaction.options/createpagestream/end_invoke/#result) |  |
| [end_invoke_iasync_result](/redaction/python-net/groupdocs.redaction.options/createpagestream/end_invoke_iasync_result/) |  |
| [invoke](/redaction/python-net/groupdocs.redaction.options/createpagestream/invoke/#page_number) |  |
| [invoke_int32](/redaction/python-net/groupdocs.redaction.options/createpagestream/invoke_int32/) |  |

### Ejemplo

```python
import os
import io
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int) -> io.RawIOBase:
    page_path = os.path.join(r"C:\Temp", f"page_{page_number}.png")
    return open(page_path, "wb")

preview_options = PreviewOptions(create_page_stream)
preview_options.preview_format = PreviewOptions.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor(r"C:\Temp\SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### Ver también
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
