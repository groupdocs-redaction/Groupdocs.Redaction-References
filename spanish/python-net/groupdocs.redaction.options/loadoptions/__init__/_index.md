---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva instancia de la clase LoadOptions."
type: docs
url: /es/python-net/groupdocs.redaction.options/loadoptions/__init__/
is_root: false
weight: 10
---


## __init__

Inicializa una nueva instancia de la clase LoadOptions.

```python
def __init__(self):
    ...
```

## __init__ {#password}

Inicializa una nueva instancia de LoadOptions con la contraseña especificada.

```python
def __init__(self, password):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| password | `str` | Contraseña para archivos protegidos. |

### Ejemplo

```python
    from groupdocs.redaction.options import LoadOptions

    # Cargar un documento protegido con contraseña
    load_opt = LoadOptions("mypassword")
    ```

## __init__ {#pre_rasterize}

Inicializa una nueva instancia de LoadOptions con el indicador de pre‑rasterización especificado.

```python
def __init__(self, pre_rasterize):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| pre_rasterize | `bool` | Si es True, forzar la rasterización al cargar. |

## __init__ {#password-pre_rasterize}

Inicializa una nueva instancia de LoadOptions con la contraseña especificada.

Si `pre_rasterize` es True, la rasterización se fuerza cuando se carga el documento.

```python
def __init__(self, password, pre_rasterize):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| password | `str` | Contraseña para archivos protegidos. |
| pre_rasterize | `bool` | Si es True, forzar la rasterización al cargar. |

### Ejemplo

```python
from groupdocs.redaction.options import LoadOptions

# Cargar un documento protegido con contraseña
load_opt = LoadOptions("mypassword")
```

### Ver también
* class [`LoadOptions`](/redaction/python-net/groupdocs.redaction.options/loadoptions/)
