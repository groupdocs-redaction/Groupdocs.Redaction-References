---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise une nouvelle AnnotationRedaction avec un motif regex et un texte de remplacement."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-replacement}

Initialise une nouvelle AnnotationRedaction avec un motif regex et un texte de remplacement.

```python
def __init__(self, pattern, replacement):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| pattern | `str` | Expression régulière à correspondre. |
| replacement | `str` | Remplacement textuel du texte correspondant. |

### Exemple

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Masquez le mot "approved" dans les textes d'annotation
redaction = AnnotationRedaction(r"(?i)approved", "[REVIEW]")
```

## __init__ {#regex-replacement}

Initialise une nouvelle instance de [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/).

```python
def __init__(self, regex, replacement):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Expression régulière à correspondre. |
| replacement | `str` | Remplacement textuel du texte correspondant. |

### Exemple

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# Masquez le mot "approved" (insensible à la casse) et remplacez-le par "[REVIEW]"
redaction = AnnotationRedaction("(?i)approved", "[REVIEW]")
```

### Voir aussi
* class [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/)
