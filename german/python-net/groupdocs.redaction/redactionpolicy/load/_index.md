---
title: "load Methode"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Lädt eine RedactionPolicy aus einer XML-Datei."
type: docs
url: /de/python-net/groupdocs.redaction/redactionpolicy/load/
is_root: false
weight: 1010
---


## load {#file_path}

Lädt eine RedactionPolicy aus einer XML-Datei.

```python
def load(cls, file_path):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| file_path | `str` | Pfad zur XML‑Datei. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Beispiel

```python
from groupdocs.redaction import RedactionPolicy, Redactor

policy = RedactionPolicy.load("RedactionPolicy.xml")

with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

## load {#input}

Lädt eine RedactionPolicy-Instanz aus einem Stream, der XML-Konfiguration enthält.

```python
def load(cls, input):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| input | `io.RawIOBase` | Stream, der XML‑Konfiguration enthält. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Beispiel

```python
from groupdocs.redaction import RedactionPolicy, Redactor

# Lade die Richtlinie aus einer XML‑Datei
with open("policy.xml", "rb") as stream:
    policy = RedactionPolicy.load(stream)

# Wende die Richtlinie auf ein Dokument an
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Siehe auch
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
