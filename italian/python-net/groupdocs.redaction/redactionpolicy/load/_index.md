---
title: "metodo load"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Carica una RedactionPolicy da un file XML."
type: docs
url: /it/python-net/groupdocs.redaction/redactionpolicy/load/
is_root: false
weight: 1010
---


## load {#file_path}

Carica una RedactionPolicy da un file XML.

```python
def load(cls, file_path):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| file_path | `str` | Percorso al file XML. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Esempio

```python
from groupdocs.redaction import RedactionPolicy, Redactor

policy = RedactionPolicy.load("RedactionPolicy.xml")

with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

## load {#input}

Carica un'istanza di RedactionPolicy da uno stream contenente la configurazione XML.

```python
def load(cls, input):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| input | `io.RawIOBase` | Stream contenente la configurazione XML. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Esempio

```python
from groupdocs.redaction import RedactionPolicy, Redactor

# Carica la policy da un file XML
with open("policy.xml", "rb") as stream:
    policy = RedactionPolicy.load(stream)

# Applica la politica a un documento
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Vedi anche
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
