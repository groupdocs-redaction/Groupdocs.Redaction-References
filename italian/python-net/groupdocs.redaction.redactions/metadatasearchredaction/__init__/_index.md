---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza una nuova istanza della classe MetadataSearchRedaction, utilizzando il valore per corrispondere agli elementi redatti."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#value_pattern-replacement}

Inizializza una nuova istanza della classe MetadataSearchRedaction, utilizzando il valore per corrispondere agli elementi redatti.

```python
def __init__(self, value_pattern, replacement):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| value_pattern | `str` | Espressione regolare per cercare e sostituire |
| replacement | `str` | Sostituzione testuale |

### Esempio

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    redactor.apply(MetadataSearchRedaction(".*@acme\\.com", "[EMAIL]"))
    redactor.save()
```

## __init__ {#value_pattern-replacement-key_pattern}

Inizializza una nuova istanza di MetadataSearchRedaction, utilizzando il nome e il valore dell'elemento per corrispondere agli elementi redatti.

```python
def __init__(self, value_pattern, replacement, key_pattern):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| value_pattern | `str` | Espressione regolare per cercare e sostituire il valore dell'elemento di metadati. |
| replacement | `str` | Sostituzione testuale. |
| key_pattern | `str` | Espressione regolare per cercare e sostituire il nome dell'elemento di metadati. |

### Esempio

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    # Sostituisci qualsiasi indirizzo email trovato nei valori dei metadati
    redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement}

Inizializza una nuova istanza della classe MetadataSearchRedaction, utilizzando il valore per corrispondere agli elementi redatti.

```python
def __init__(self, value_regex, replacement):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Espressione regolare da cercare e sostituire. |
| replacement | `str` | Sostituzione testuale. |

### Esempio

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

# Oscura qualsiasi indirizzo email nei metadati
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement-key_regex}

Inizializza una nuova istanza di MetadataSearchRedaction utilizzando il nome e il valore dell'elemento per corrispondere agli elementi redatti.

```python
def __init__(self, value_regex, replacement, key_regex):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | Espressione regolare per cercare e sostituire il valore dell'elemento di metadati. |
| replacement | `str` | Sostituzione testuale. |
| key_regex | `System.Text.RegularExpressions.Regex` | Espressione regolare per cercare e sostituire il nome dell'elemento di metadati. |

### Esempio

```python
from groupdocs.redaction.redactions import MetadataSearchRedaction
from groupdocs.redaction import Redactor

# Oscura gli indirizzi email nei valori dei metadati
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

### Vedi anche
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/)
