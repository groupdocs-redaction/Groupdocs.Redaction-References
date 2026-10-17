---
title: "méthode load"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Charge un RedactionPolicy à partir d'un fichier XML."
type: docs
url: /fr/python-net/groupdocs.redaction/redactionpolicy/load/
is_root: false
weight: 1010
---


## load {#file_path}

Charge un RedactionPolicy à partir d'un fichier XML.

```python
def load(cls, file_path):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| file_path | `str` | Chemin vers le fichier XML. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Exemple

```python
from groupdocs.redaction import RedactionPolicy, Redactor

policy = RedactionPolicy.load("RedactionPolicy.xml")

with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

## load {#input}

Charge une instance de RedactionPolicy à partir d'un flux contenant la configuration XML.

```python
def load(cls, input):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| input | `io.RawIOBase` | Flux contenant la configuration XML. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Exemple

```python
from groupdocs.redaction import RedactionPolicy, Redactor

# Charger la politique depuis un fichier XML
with open("policy.xml", "rb") as stream:
    policy = RedactionPolicy.load(stream)

# Appliquer la politique à un document
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Voir aussi
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
