---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise une nouvelle instance de RegexRedaction."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/regexredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-options}

Initialise une nouvelle instance de RegexRedaction.

```python
def __init__(self, pattern, options):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| pattern | `str` | Expression régulière pour rechercher et remplacer. |
| options | `ReplacementOptions` | Options de remplacement (textuel, couleur). |

### Exemple

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

## __init__ {#regex-options}

Initialise une nouvelle instance de RegexRedaction.

```python
def __init__(self, regex, options):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Expression régulière pour rechercher et remplacer. |
| options | `ReplacementOptions` | Options de remplacement (textuel, couleur). |

### Exemple

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

### Voir aussi
* class [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)
