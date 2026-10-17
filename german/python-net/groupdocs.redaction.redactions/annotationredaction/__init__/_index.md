---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert ein neues AnnotationRedaction mit einem Regex‑Muster und Ersatztext."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-replacement}

Initialisiert ein neues AnnotationRedaction mit einem Regex‑Muster und Ersatztext.

```python
def __init__(self, pattern, replacement):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| pattern | `str` | Regulärer Ausdruck zum Übereinstimmen. |
| replacement | `str` | Textueller Ersatz für übereinstimmenden Text. |

### Beispiel

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Zensieren Sie das Wort "approved" in Anmerkungstexten
redaction = AnnotationRedaction(r"(?i)approved", "[REVIEW]")
```

## __init__ {#regex-replacement}

Initialisiert eine neue Instanz von [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/).

```python
def __init__(self, regex, replacement):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Regulärer Ausdruck zum Übereinstimmen. |
| replacement | `str` | Textueller Ersatz für übereinstimmenden Text. |

### Beispiel

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Zensieren Sie das Wort "approved" (Groß‑/Kleinschreibung ignorierend) und ersetzen Sie es durch "[REVIEW]"
redaction = AnnotationRedaction("(?i)approved", "[REVIEW]")
```

### Siehe auch
* class [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/)
