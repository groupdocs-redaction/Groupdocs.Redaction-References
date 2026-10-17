---
title: "metodo redact"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Applica una redazione personalizzata a contenuti specifici del documento."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
is_root: false
weight: 1010
---


## redact {#context}

Applica una redazione personalizzata a contenuti specifici del documento.

Attualmente, questo è supportato solo per PDF [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/).

Gli utenti possono definire la propria logica di redazione, ad esempio la redazione basata su IA, che può essere più avanzata rispetto ai metodi semplici basati su pattern.

```python
def redact(self, context):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| context | `CustomRedactionContext` | Contiene il contenuto del documento da redigere insieme ai relativi metadati. |

**Returns:** CustomRedactionResult: Indicates whether the redaction should be applied and the modified content.

### Vedi anche
* class [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/)
