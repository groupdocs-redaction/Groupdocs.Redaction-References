---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert eine neue Instanz von RegexRedaction."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/regexredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-options}

Initialisiert eine neue Instanz von RegexRedaction.

```python
def __init__(self, pattern, options):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| pattern | `str` | Regulärer Ausdruck zum Suchen und Ersetzen. |
| options | `ReplacementOptions` | Ersetzungsoptionen (textuell, Farbe). |

### Beispiel

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

## __init__ {#regex-options}

Initialisiert eine neue RegexRedaction-Instanz.

```python
def __init__(self, regex, options):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Regulärer Ausdruck zum Suchen und Ersetzen. |
| options | `ReplacementOptions` | Ersetzungsoptionen (textuell, Farbe). |

### Beispiel

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

### Siehe auch
* class [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)
