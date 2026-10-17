---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva instancia de PreviewOptions."
type: docs
url: /es/python-net/groupdocs.redaction.options/previewoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#create_page_stream}

Inicializa una nueva instancia de PreviewOptions. El flujo de salida se cerrará después de su uso.

```python
def __init__(self, create_page_stream):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Crea un flujo para una vista previa de página específica. |

## __init__ {#create_page_stream-release_page_stream}

Inicializa una nueva instancia de PreviewOptions, haciendo que el flujo de salida se devuelva al cliente para su uso posterior.

```python
def __init__(self, create_page_stream, release_page_stream):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Crea un flujo para una vista previa de página específica. |
| release_page_stream | `ReleasePageStream` | Notifica que la generación de la vista previa de la página ha finalizado y obtiene el flujo de salida. |

### Ver también
* class [`PreviewOptions`](/redaction/python-net/groupdocs.redaction.options/previewoptions/)
