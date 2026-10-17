---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny instans av ExactPhraseRedaction i läge utan hänsyn till skiftläge."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#search_phrase-options}

Initierar en ny instans av ExactPhraseRedaction i läge utan hänsyn till skiftläge.

```python
def __init__(self, search_phrase, options):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| search_phrase | `str` | Sträng att söka och ersätta. |
| options | `ReplacementOptions` | Ersättningsalternativ (textuell, färg). |

### Exempel

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Ersätt förekomster av "John Doe" med "[CUSTOMER]" (skiftlägesokänslig)
redaction = ExactPhraseRedaction("John Doe", ReplacementOptions("[CUSTOMER]"))
```

## __init__ {#search_phrase-is_case_sensitive-options}

Initierar en ny ExactPhraseRedaction-instans.

```python
def __init__(self, search_phrase, is_case_sensitive, options):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| search_phrase | `str` | Sträng att söka och ersätta. |
| is_case_sensitive | `bool` | Sant om skiftlägeskänslig sökning krävs. |
| options | `ReplacementOptions` | Ersättningsalternativ (textuell, färg). |

### Exempel

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Skiftlägesokänslig exakt frasrensning
redaction = ExactPhraseRedaction("John Doe", False, ReplacementOptions("[CUSTOMER]"))

# Skiftlägeskänslig exakt frasrensning
redaction_cs = ExactPhraseRedaction("ACME", True, ReplacementOptions("[CO]"))
```

### Se även
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/)
