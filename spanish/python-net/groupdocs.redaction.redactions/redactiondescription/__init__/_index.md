---
title: "Constructor __init__"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Inicializa una nueva instancia de la clase RedactionDescription sin información de reemplazo."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/
is_root: false
weight: 10
---


## __init__ {#redaction_type-action_type-original_text}

Inicializa una nueva instancia de la clase RedactionDescription sin información de reemplazo.

```python
def __init__(self, redaction_type, action_type, original_text):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| redaction_type | `RedactionType` | Tipo de datos que se están redactando. |
| action_type | `RedactionActionType` | Acción a realizar sobre estos datos. |
| original_text | `str` | Texto coincidente, comentario o cuerpo de la anotación. |

## __init__ {#redaction_type-action_type-original_text-replacement}

Inicializa una nueva instancia de la clase RedactionDescription con información de reemplazo.

```python
def __init__(self, redaction_type, action_type, original_text, replacement):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| redaction_type | `RedactionType` | Tipo de datos que se están redactando. |
| action_type | `RedactionActionType` | Acción a realizar sobre estos datos. |
| original_text | `str` | Texto coincidente, comentario o cuerpo de la anotación. |
| replacement | `TextReplacement` | Texto de reemplazo, texto coincidente y su posición dentro de la cadena original. |

## __init__ {#redaction_type-action_type-image_area_replacement-image_details}

Inicializa una nueva RedactionDescription con información de reemplazo de área de imagen.

```python
def __init__(self, redaction_type, action_type, image_area_replacement, image_details):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| redaction_type | `RedactionType` | Tipo de datos que se están redactando. |
| action_type | `RedactionActionType` | Acción a realizar sobre estos datos. |
| image_area_replacement | `RegionReplacementOptions` | Información de reemplazo del área de imagen. |
| image_details | `str` | Descripción textual de la imagen, por defecto es una cadena vacía. |

### Ver también
* class [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/)
