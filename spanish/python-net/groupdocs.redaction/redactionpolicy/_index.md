---
title: "Clase RedactionPolicy"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa una política de saneamiento, que contiene un conjunto de redacciones específicas a aplicar."
type: docs
url: /es/python-net/groupdocs.redaction/redactionpolicy/
is_root: false
weight: 120
---


## RedactionPolicy class

Representa una política de saneamiento, que contiene un conjunto de redacciones específicas a aplicar.

**Learn more**
- More details about policies: https://docs.groupdocs.com/redaction/net/use-redaction-policies/
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/

El tipo RedactionPolicy expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/) | Inicializa una nueva instancia de RedactionPolicy. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/#redactions) | Inicializa una nueva RedactionPolicy con una lista específica de redacciones. |

### Métodos
| Método | Descripción |
| :- | :- |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#file_path) | Carga una RedactionPolicy desde un archivo XML. |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#input) | Carga una instancia de RedactionPolicy desde un flujo que contiene la configuración XML. |
| [load_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_file/) |  |
| [load_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_streams/) |  |
| [load_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_string/) |  |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#file_path) | Guarda la política de redacción en un archivo. |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#output) | Guarda la política de redacción en un flujo. |
| [save_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_file/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_streams/) |  |
| [save_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_string/) |  |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [redactions](/redaction/python-net/groupdocs.redaction/redactionpolicy/redactions/) | La lista de clases derivadas de [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/) totalmente configuradas. |

### Ejemplo

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

# Construye una política reutilizable en memoria
policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])

# Aplica la política a un documento
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Guides
Guías de tareas que usan `RedactionPolicy`:

* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Ver también
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
