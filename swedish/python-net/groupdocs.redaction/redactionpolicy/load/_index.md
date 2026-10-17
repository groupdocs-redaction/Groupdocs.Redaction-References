---
title: "load metod"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Läser in en RedactionPolicy från en XML‑fil."
type: docs
url: /sv/python-net/groupdocs.redaction/redactionpolicy/load/
is_root: false
weight: 1010
---


## load {#file_path}

Läser in en RedactionPolicy från en XML‑fil.

```python
def load(cls, file_path):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| file_path | `str` | Sökväg till XML‑filen. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Exempel

```python
from groupdocs.redaction import RedactionPolicy, Redactor

policy = RedactionPolicy.load("RedactionPolicy.xml")

with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

## load {#input}

Läser in en RedactionPolicy‑instans från en ström som innehåller XML‑konfiguration.

```python
def load(cls, input):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| input | `io.RawIOBase` | Ström som innehåller XML‑konfiguration. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Exempel

```python
from groupdocs.redaction import RedactionPolicy, Redactor

# Läs in policyn från en XML‑fil
with open("policy.xml", "rb") as stream:
    policy = RedactionPolicy.load(stream)

# Applicera policyn på ett dokument
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Se även
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
