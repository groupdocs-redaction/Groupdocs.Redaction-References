---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuw exemplaar van de DeleteAnnotationRedaction‑klasse, met instellingen om alle annotaties te verwijderen (alles matchend)."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/
is_root: false
weight: 10
---


## __init__

Initialiseert een nieuw exemplaar van de DeleteAnnotationRedaction‑klasse, met instellingen om alle annotaties te verwijderen (alles matchend).

```python
def __init__(self):
    ...
```

### Voorbeeld

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Verwijder alle annotaties
del_red = DeleteAnnotationRedaction()
```

## __init__ {#pattern}

Initialiseert een nieuw exemplaar van de DeleteAnnotationRedaction‑klasse, waarbij annotaties worden verwijderd die overeenkomen met de opgegeven expressie.

```python
def __init__(self, pattern):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| pattern | `str` | Reguliere expressie. |

### Voorbeeld

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Verwijder annotaties die het woord "internal" bevatten (niet‑hoofdlettergevoelig)
del_red = DeleteAnnotationRedaction(r"(?i)internal")
```

## __init__ {#regex}

Initialiseert een nieuw exemplaar van de DeleteAnnotationRedaction‑klasse, waarbij annotaties worden verwijderd die overeenkomen met de opgegeven expressie.

```python
def __init__(self, regex):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Reguliere expressie. |

### Voorbeeld

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Verwijder annotaties waarvan de inhoud overeenkomt met de regex (niet‑hoofdlettergevoelig)
del_red = DeleteAnnotationRedaction("(?i)internal")
```

### Zie ook
* class [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/)
