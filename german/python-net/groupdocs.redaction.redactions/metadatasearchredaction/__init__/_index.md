---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert eine neue Instanz der Klasse MetadataSearchRedaction und verwendet den Wert, um zu redigierende Elemente zu finden."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#value_pattern-replacement}

Initialisiert eine neue Instanz der Klasse MetadataSearchRedaction und verwendet den Wert, um zu redigierende Elemente zu finden.

```python
def __init__(self, value_pattern, replacement):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| value_pattern | `str` | Regulärer Ausdruck zum Suchen und Ersetzen |
| replacement | `str` | Textuelle Ersetzung |

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    redactor.apply(MetadataSearchRedaction(".*@acme\\.com", "[EMAIL]"))
    redactor.save()
```

## __init__ {#value_pattern-replacement-key_pattern}

Initialisiert eine neue Instanz von MetadataSearchRedaction und verwendet den Elementnamen und den Wert, um zu redigierende Elemente zu finden.

```python
def __init__(self, value_pattern, replacement, key_pattern):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| value_pattern | `str` | Regulärer Ausdruck zum Suchen und Ersetzen des Metadaten‑Elementwerts. |
| replacement | `str` | Textuelle Ersetzung. |
| key_pattern | `str` | Regulärer Ausdruck zum Suchen und Ersetzen des Metadaten‑Elementnamens. |

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    # Ersetze jede in Metadatenwerten gefundene E‑Mail‑Adresse
    redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement}

Initialisiert eine neue Instanz der Klasse MetadataSearchRedaction und verwendet den Wert, um zu redigierende Elemente zu finden.

```python
def __init__(self, value_regex, replacement):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Regulärer Ausdruck zum Suchen und Ersetzen. |
| replacement | `str` | Textuelle Ersetzung. |

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

# Redigiere jede E‑Mail‑Adresse in Metadaten
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement-key_regex}

Initialisiert eine neue Instanz von MetadataSearchRedaction, wobei der Elementname und der Wert zum Abgleichen zu redigierender Elemente verwendet werden.

```python
def __init__(self, value_regex, replacement, key_regex):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Regulärer Ausdruck zum Suchen und Ersetzen des Metadaten‑Elementwerts. |
| replacement | `str` | Textuelle Ersetzung. |
| key_regex | `System.Text.RegularExpressions.Regex` | Regulärer Ausdruck zum Suchen und Ersetzen des Metadaten‑Elementnamens. |

### Beispiel

```python
from groupdocs.redaction.redactions import MetadataSearchRedaction
from groupdocs.redaction import Redactor

# Redigiere E‑Mail‑Adressen in Metadatenwerten
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

### Siehe auch
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/)
