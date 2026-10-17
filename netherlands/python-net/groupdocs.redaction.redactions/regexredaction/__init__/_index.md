---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuw exemplaar van RegexRedaction."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/regexredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-options}

Initialiseert een nieuw exemplaar van RegexRedaction.

```python
def __init__(self, pattern, options):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| pattern | `str` | Reguliere expressie om te zoeken en te vervangen. |
| options | `ReplacementOptions` | Vervangingsopties (tekstueel, kleur). |

### Voorbeeld

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

## __init__ {#regex-options}

Initialiseert een nieuw RegexRedaction‑exemplaar.

```python
def __init__(self, regex, options):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Reguliere expressie om te zoeken en te vervangen. |
| options | `ReplacementOptions` | Vervangingsopties (tekstueel, kleur). |

### Voorbeeld

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

### Zie ook
* class [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)
