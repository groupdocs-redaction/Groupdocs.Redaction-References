---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuw exemplaar van de MetadataSearchRedaction klasse, met een waarde om te matchen met geredigeerde items."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#value_pattern-replacement}

Initialiseert een nieuw exemplaar van de MetadataSearchRedaction klasse, met een waarde om te matchen met geredigeerde items.

```python
def __init__(self, value_pattern, replacement):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| value_pattern | `str` | Reguliere expressie om te zoeken en te vervangen |
| replacement | `str` | Tekstuele vervanging |

### Voorbeeld

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    redactor.apply(MetadataSearchRedaction(".*@acme\\.com", "[EMAIL]"))
    redactor.save()
```

## __init__ {#value_pattern-replacement-key_pattern}

Initialiseert een nieuw exemplaar van MetadataSearchRedaction, met itemnaam en waarde om te matchen met geredigeerde items.

```python
def __init__(self, value_pattern, replacement, key_pattern):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| value_pattern | `str` | Reguliere expressie om de waarde van een metagegevensitem te zoeken en te vervangen. |
| replacement | `str` | Tekstvervanging. |
| key_pattern | `str` | Reguliere expressie om de naam van een metagegevensitem te zoeken en te vervangen. |

### Voorbeeld

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    # Vervang elk e‑mailadres dat in metagegevenswaarden wordt gevonden
    redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement}

Initialiseert een nieuw exemplaar van de MetadataSearchRedaction klasse, met een waarde om te matchen met geredigeerde items.

```python
def __init__(self, value_regex, replacement):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Reguliere expressie om te zoeken en te vervangen. |
| replacement | `str` | Tekstvervanging. |

### Voorbeeld

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

# Redigeer elk e‑mailadres in metagegevens
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement-key_regex}

Initialiseert een nieuw exemplaar van MetadataSearchRedaction met itemnaam en waarde om te matchen met geredigeerde items.

```python
def __init__(self, value_regex, replacement, key_regex):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Reguliere expressie om de waarde van een metagegevensitem te zoeken en te vervangen. |
| replacement | `str` | Tekstvervanging. |
| key_regex | `System.Text.RegularExpressions.Regex` | Reguliere expressie om de naam van een metagegevensitem te zoeken en te vervangen. |

### Voorbeeld

```python
from groupdocs.redaction.redactions import MetadataSearchRedaction
from groupdocs.redaction import Redactor

# Redigeer e‑mailadressen in metagegevenswaarden
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

### Zie ook
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/)
