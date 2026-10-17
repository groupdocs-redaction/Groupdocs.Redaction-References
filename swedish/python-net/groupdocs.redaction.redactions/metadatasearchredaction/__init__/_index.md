---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny instans av MetadataSearchRedaction-klassen med värde för att matcha redigerade objekt."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#value_pattern-replacement}

Initierar en ny instans av MetadataSearchRedaction-klassen med värde för att matcha redigerade objekt.

```python
def __init__(self, value_pattern, replacement):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| value_pattern | `str` | Reguljärt uttryck för att söka och ersätta |
| replacement | `str` | Textuell ersättning |

### Exempel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    redactor.apply(MetadataSearchRedaction(".*@acme\\.com", "[EMAIL]"))
    redactor.save()
```

## __init__ {#value_pattern-replacement-key_pattern}

Initierar en ny instans av MetadataSearchRedaction med objektnamn och värde för att matcha redigerade objekt.

```python
def __init__(self, value_pattern, replacement, key_pattern):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| value_pattern | `str` | Reguljärt uttryck för att söka och ersätta metadataobjektets värde. |
| replacement | `str` | Textuell ersättning. |
| key_pattern | `str` | Reguljärt uttryck för att söka och ersätta metadataobjektets namn. |

### Exempel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    # Ersätt alla e‑postadresser som hittas i metadata‑värden
    redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement}

Initierar en ny instans av MetadataSearchRedaction-klassen med värde för att matcha redigerade objekt.

```python
def __init__(self, value_regex, replacement):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Reguljärt uttryck för att söka och ersätta. |
| replacement | `str` | Textuell ersättning. |

### Exempel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

# Maskera alla e‑postadresser i metadata
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement-key_regex}

Initierar en ny instans av MetadataSearchRedaction med objektnamn och värde för att matcha redigerade objekt.

```python
def __init__(self, value_regex, replacement, key_regex):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Reguljärt uttryck för att söka och ersätta metadataobjektets värde. |
| replacement | `str` | Textuell ersättning. |
| key_regex | `System.Text.RegularExpressions.Regex` | Reguljärt uttryck för att söka och ersätta metadataobjektets namn. |

### Exempel

```python
from groupdocs.redaction.redactions import MetadataSearchRedaction
from groupdocs.redaction import Redactor

# Maskera e‑postadresser i metadata‑värden
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

### Se även
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/)
