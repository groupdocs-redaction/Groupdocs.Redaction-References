---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny instans av DeleteAnnotationRedaction-klass med inställningar för att ta bort alla annotationer (matchar allt)."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/
is_root: false
weight: 10
---


## __init__

Initierar en ny instans av DeleteAnnotationRedaction-klass med inställningar för att ta bort alla annotationer (matchar allt).

```python
def __init__(self):
    ...
```

### Exempel

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Ta bort alla annotationer
del_red = DeleteAnnotationRedaction()
```

## __init__ {#pattern}

Initierar en ny instans av DeleteAnnotationRedaction-klass som tar bort annotationer som matchar det givna uttrycket.

```python
def __init__(self, pattern):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| pattern | `str` | Reguljärt uttryck. |

### Exempel

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Ta bort annotationer som innehåller ordet "internal" (skiftlägesokänslig)
del_red = DeleteAnnotationRedaction(r"(?i)internal")
```

## __init__ {#regex}

Initierar en ny instans av DeleteAnnotationRedaction-klass som tar bort annotationer som matchar det givna uttrycket.

```python
def __init__(self, regex):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Reguljärt uttryck. |

### Exempel

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Ta bort annotationer vars innehåll matchar regexen (skiftlägesokänslig)
del_red = DeleteAnnotationRedaction("(?i)internal")
```

### Se även
* class [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/)
