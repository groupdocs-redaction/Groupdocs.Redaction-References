---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuwe AnnotationRedaction met een regex-patroon en vervangende tekst."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-replacement}

Initialiseert een nieuwe AnnotationRedaction met een regex-patroon en vervangende tekst.

```python
def __init__(self, pattern, replacement):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| pattern | `str` | Reguliere expressie om te matchen. |
| replacement | `str` | Tekstvervanging voor overeenkomende tekst. |

### Voorbeeld

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Redigeer het woord "approved" in annotatieteksten
redaction = AnnotationRedaction(r"(?i)approved", "[REVIEW]")
```

## __init__ {#regex-replacement}

Initialiseert een nieuw exemplaar van [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/).

```python
def __init__(self, regex, replacement):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Reguliere expressie om te matchen. |
| replacement | `str` | Tekstvervanging voor overeenkomende tekst. |

### Voorbeeld

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Redigeer het woord "approved" (niet‑hoofdlettergevoelig) en vervang het door "[REVIEW]"
redaction = AnnotationRedaction("(?i)approved", "[REVIEW]")
```

### Zie ook
* class [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/)
