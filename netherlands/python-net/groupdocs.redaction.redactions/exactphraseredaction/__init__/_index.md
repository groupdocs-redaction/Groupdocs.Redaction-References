---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuw exemplaar van ExactPhraseRedaction in hoofdletterongevoelige modus."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#search_phrase-options}

Initialiseert een nieuw exemplaar van ExactPhraseRedaction in hoofdletterongevoelige modus.

```python
def __init__(self, search_phrase, options):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| search_phrase | `str` | String om te zoeken en te vervangen. |
| options | `ReplacementOptions` | Vervangingsopties (tekstueel, kleur). |

### Voorbeeld

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Vervang voorkomens van "John Doe" door "[CUSTOMER]" (niet-hoofdlettergevoelig)
redaction = ExactPhraseRedaction("John Doe", ReplacementOptions("[CUSTOMER]"))
```

## __init__ {#search_phrase-is_case_sensitive-options}

Initialiseert een nieuw ExactPhraseRedaction exemplaar.

```python
def __init__(self, search_phrase, is_case_sensitive, options):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| search_phrase | `str` | String om te zoeken en te vervangen. |
| is_case_sensitive | `bool` | True als hoofdlettergevoelige zoekopdracht vereist is. |
| options | `ReplacementOptions` | Vervangingsopties (tekstueel, kleur). |

### Voorbeeld

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Niet-hoofdlettergevoelige exacte frase redactie
redaction = ExactPhraseRedaction("John Doe", False, ReplacementOptions("[CUSTOMER]"))

# Hoofdlettergevoelige exacte frase redactie
redaction_cs = ExactPhraseRedaction("ACME", True, ReplacementOptions("[CO]"))
```

### Zie ook
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/)
