---
title: "Método redact"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Aplica redacción personalizada a contenido específico del documento."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
is_root: false
weight: 1010
---


## redact {#context}

Aplica redacción personalizada a contenido específico del documento.

Actualmente, esto solo es compatible con PDF [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/).

Los usuarios pueden definir su propia lógica de redacción, como la redacción basada en IA, que puede ser más avanzada que los métodos simples basados en patrones.

```python
def redact(self, context):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| context | `CustomRedactionContext` | Contiene el contenido del documento que se redactará junto con los metadatos relacionados. |

**Returns:** CustomRedactionResult: Indicates whether the redaction should be applied and the modified content.

### Ver también
* class [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/)
