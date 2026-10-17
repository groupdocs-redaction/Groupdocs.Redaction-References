---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise une nouvelle instance de ExactPhraseRedaction en mode insensible à la casse."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#search_phrase-options}

Initialise une nouvelle instance de ExactPhraseRedaction en mode insensible à la casse.

```python
def __init__(self, search_phrase, options):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| search_phrase | `str` | Chaîne à rechercher et remplacer. |
| options | `ReplacementOptions` | Options de remplacement (textuel, couleur). |

### Exemple

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Remplacer les occurrences de "John Doe" par "[CUSTOMER]" (insensible à la casse)
redaction = ExactPhraseRedaction("John Doe", ReplacementOptions("[CUSTOMER]"))
```

## __init__ {#search_phrase-is_case_sensitive-options}

Initialise une nouvelle instance de ExactPhraseRedaction.

```python
def __init__(self, search_phrase, is_case_sensitive, options):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| search_phrase | `str` | Chaîne à rechercher et remplacer. |
| is_case_sensitive | `bool` | Vrai si une recherche sensible à la casse est requise. |
| options | `ReplacementOptions` | Options de remplacement (textuel, couleur). |

### Exemple

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Masquage de phrase exacte insensible à la casse
redaction = ExactPhraseRedaction("John Doe", False, ReplacementOptions("[CUSTOMER]"))

# Masquage de phrase exacte sensible à la casse
redaction_cs = ExactPhraseRedaction("ACME", True, ReplacementOptions("[CO]"))
```

### Voir aussi
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/)
