---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva instancia de Redactor usando una ruta de archivo."
type: docs
url: /es/python-net/groupdocs.redaction/redactor/__init__/
is_root: false
weight: 10
---


## __init__ {#file_path}

Inicializa una nueva instancia de Redactor usando una ruta de archivo.

```python
def __init__(self, file_path):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| file_path | `str` | Ruta al archivo. |

### Ejemplo

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    # Realice operaciones de redacción aquí
    pass
```

## __init__ {#document}

Inicializa una nueva instancia de [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) usando un flujo.

```python
def __init__(self, document):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| document | `io.RawIOBase` | Flujo de origen del documento. |

### Ejemplo

```python
from groupdocs.redaction import Redactor

def open_from_stream():
    # Abrir el documento como un flujo binario
    with open("./sample.pdf", "rb") as stream:
        # Cargar el documento desde el flujo
        with Redactor(stream) as redactor:
            # Realice redacciones aquí
            pass
```

## __init__ {#file_path-load_options}

Inicializa una nueva instancia de [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) para un documento protegido con contraseña usando su ruta.

```python
def __init__(self, file_path, load_options):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| file_path | `str` | Ruta al archivo. |
| load_options | `LoadOptions` | Opciones, incluida la contraseña. |

### Ejemplo

```python
from groupdocs.redaction import Redactor

# Cargue un documento protegido con contraseña desde una ruta de archivo
with Redactor("protected.docx") as redactor:
    # Realice operaciones de redacción aquí
    pass
```

## __init__ {#file_path-load_options-settings}

Inicializa una nueva instancia de Redactor para un documento protegido con contraseña usando su ruta y configuraciones.

```python
def __init__(self, file_path, load_options, settings):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| file_path | `str` | Ruta al archivo. |
| load_options | `LoadOptions` | Opciones dependientes del archivo, incluida la contraseña. |
| settings | `RedactorSettings` | Configuración predeterminada para el proceso de redacción. |

### Ejemplo

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

## __init__ {#document-load_options}

Inicializa una nueva instancia de Redactor para un documento protegido con contraseña usando un flujo.

```python
def __init__(self, document, load_options):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| document | `io.RawIOBase` | Flujo de entrada de origen. |
| load_options | `LoadOptions` | Opciones, incluida la contraseña. |

### Ejemplo

```python
from groupdocs.redaction import Redactor, LoadOptions

def open_protected_doc():
    # Abra el PDF protegido como un flujo binario
    with open(r"C:\sample.pdf", "rb") as stream:
        # Proporcione la contraseña a través de LoadOptions
        load_options = LoadOptions("mypassword")
        # Inicialice Redactor con el flujo y las opciones de carga
        with Redactor(stream, load_options) as redactor:
            # Realice operaciones de redacción aquí
            pass
```

## __init__ {#document-load_options-settings}

Inicializa una nueva instancia de [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) para un documento protegido con contraseña usando un flujo y configuraciones.

```python
def __init__(self, document, load_options, settings):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| document | `io.RawIOBase` | Flujo de entrada de origen. |
| load_options | `LoadOptions` | Opciones, incluida la contraseña. |
| settings | `RedactorSettings` | Configuraciones predeterminadas para el proceso de redacción. |

### Ver también
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
