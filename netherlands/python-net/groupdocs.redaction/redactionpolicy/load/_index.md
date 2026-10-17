---
title: "load methode"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Laadt een RedactionPolicy vanuit een XML‑bestand."
type: docs
url: /nl/python-net/groupdocs.redaction/redactionpolicy/load/
is_root: false
weight: 1010
---


## load {#file_path}

Laadt een RedactionPolicy vanuit een XML‑bestand.

```python
def load(cls, file_path):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| file_path | `str` | Pad naar het XML‑bestand. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Voorbeeld

```python
from groupdocs.redaction import RedactionPolicy, Redactor

policy = RedactionPolicy.load("RedactionPolicy.xml")

with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

## load {#input}

Laadt een RedactionPolicy‑object vanuit een stream die XML‑configuratie bevat.

```python
def load(cls, input):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| input | `io.RawIOBase` | Stream met XML‑configuratie. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Voorbeeld

```python
from groupdocs.redaction import RedactionPolicy, Redactor

# Laad het beleid vanuit een XML‑bestand
with open("policy.xml", "rb") as stream:
    policy = RedactionPolicy.load(stream)

# Pas het beleid toe op een document
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Zie ook
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
