---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise une nouvelle instance de la classe DeleteAnnotationRedaction, avec des paramètres pour supprimer toutes les annotations (correspondant à tout)."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/
is_root: false
weight: 10
---


## __init__

Initialise une nouvelle instance de la classe DeleteAnnotationRedaction, avec des paramètres pour supprimer toutes les annotations (correspondant à tout).

```python
def __init__(self):
    ...
```

### Exemple

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Supprimer toutes les annotations
del_red = DeleteAnnotationRedaction()
```

## __init__ {#pattern}

Initialise une nouvelle instance de la classe DeleteAnnotationRedaction, supprimant les annotations correspondant à l’expression donnée.

```python
def __init__(self, pattern):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| pattern | `str` | Expression régulière. |

### Exemple

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Supprimer les annotations contenant le mot « internal » (insensible à la casse)
del_red = DeleteAnnotationRedaction(r"(?i)internal")
```

## __init__ {#regex}

Initialise une nouvelle instance de la classe DeleteAnnotationRedaction, supprimant les annotations correspondant à l’expression donnée.

```python
def __init__(self, regex):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Expression régulière. |

### Exemple

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Supprimer les annotations dont le contenu correspond à l'expression régulière (insensible à la casse)
del_red = DeleteAnnotationRedaction("(?i)internal")
```

### Voir aussi
* class [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/)
