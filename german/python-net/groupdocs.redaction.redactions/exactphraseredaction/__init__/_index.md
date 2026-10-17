---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert eine neue Instanz von ExactPhraseRedaction im Modus ohne Groß-/Kleinschreibung."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#search_phrase-options}

Initialisiert eine neue Instanz von ExactPhraseRedaction im Modus ohne Groß-/Kleinschreibung.

```python
def __init__(self, search_phrase, options):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| search_phrase | `str` | Zeichenkette zum Suchen und Ersetzen. |
| options | `ReplacementOptions` | Ersetzungsoptionen (textuell, Farbe). |

### Beispiel

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Ersetze Vorkommen von "John Doe" durch "[CUSTOMER]" (ohne Groß‑ und Kleinschreibung)
redaction = ExactPhraseRedaction("John Doe", ReplacementOptions("[CUSTOMER]"))
```

## __init__ {#search_phrase-is_case_sensitive-options}

Initialisiert eine neue ExactPhraseRedaction-Instanz.

```python
def __init__(self, search_phrase, is_case_sensitive, options):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| search_phrase | `str` | Zeichenkette zum Suchen und Ersetzen. |
| is_case_sensitive | `bool` | True, wenn eine case‑sensitive Suche erforderlich ist. |
| options | `ReplacementOptions` | Ersetzungsoptionen (textuell, Farbe). |

### Beispiel

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Case‑insensitive exakte Phrasen‑Redaktion
redaction = ExactPhraseRedaction("John Doe", False, ReplacementOptions("[CUSTOMER]"))

# Case‑sensitive exakte Phrasen‑Redaktion
redaction_cs = ExactPhraseRedaction("ACME", True, ReplacementOptions("[CO]"))
```

### Siehe auch
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/)
