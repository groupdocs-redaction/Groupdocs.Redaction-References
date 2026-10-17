---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny instans av RegexRedaction."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/regexredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-options}

Initierar en ny instans av RegexRedaction.

```python
def __init__(self, pattern, options):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| pattern | `str` | Reguljärt uttryck för att söka och ersätta. |
| options | `ReplacementOptions` | Ersättningsalternativ (textuell, färg). |

### Exempel

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

## __init__ {#regex-options}

Initierar en ny RegexRedaction-instans.

```python
def __init__(self, regex, options):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Reguljärt uttryck för att söka och ersätta. |
| options | `ReplacementOptions` | Ersättningsalternativ (textuell, färg). |

### Exempel

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

### Se även
* class [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)
