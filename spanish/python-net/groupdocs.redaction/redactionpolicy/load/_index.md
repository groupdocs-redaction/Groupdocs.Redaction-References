---
title: "método load"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Carga una RedactionPolicy desde un archivo XML."
type: docs
url: /es/python-net/groupdocs.redaction/redactionpolicy/load/
is_root: false
weight: 1010
---


## load {#file_path}

Carga una RedactionPolicy desde un archivo XML.

```python
def load(cls, file_path):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| file_path | `str` | Ruta al archivo XML. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Ejemplo

```python
from groupdocs.redaction import RedactionPolicy, Redactor

policy = RedactionPolicy.load("RedactionPolicy.xml")

with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

## load {#input}

Carga una instancia de RedactionPolicy desde un flujo que contiene la configuración XML.

```python
def load(cls, input):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| input | `io.RawIOBase` | Secuencia que contiene la configuración XML. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Ejemplo

```python
from groupdocs.redaction import RedactionPolicy, Redactor

# Cargar la política desde un archivo XML
with open("policy.xml", "rb") as stream:
    policy = RedactionPolicy.load(stream)

# Aplica la política a un documento
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Ver también
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
