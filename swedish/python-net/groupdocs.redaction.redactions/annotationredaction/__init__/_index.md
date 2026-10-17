---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny AnnotationRedaction med ett regex-mönster och ersättningstext."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-replacement}

Initierar en ny AnnotationRedaction med ett regex-mönster och ersättningstext.

```python
def __init__(self, pattern, replacement):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| pattern | `str` | Reguljärt uttryck att matcha. |
| replacement | `str` | Textuell ersättning för matchad text. |

### Exempel

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Rensa ordet "approved" i annoteringstexter
redaction = AnnotationRedaction(r"(?i)approved", "[REVIEW]")
```

## __init__ {#regex-replacement}

Initierar en ny instans av [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/).

```python
def __init__(self, regex, replacement):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Reguljärt uttryck att matcha. |
| replacement | `str` | Textuell ersättning för matchad text. |

### Exempel

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Rensa ordet "approved" (skiftlägesokänslig) och ersätt det med "[REVIEW]"
redaction = AnnotationRedaction("(?i)approved", "[REVIEW]")
```

### Se även
* class [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/)
