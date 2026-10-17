---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuwe Redactor-instantie met een bestandspad."
type: docs
url: /nl/python-net/groupdocs.redaction/redactor/__init__/
is_root: false
weight: 10
---


## __init__ {#file_path}

Initialiseert een nieuwe Redactor-instantie met een bestandspad.

```python
def __init__(self, file_path):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| file_path | `str` | Pad naar het bestand. |

### Voorbeeld

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    # Voer hier redactie‑operaties uit
    pass
```

## __init__ {#document}

Initialiseert een nieuwe instantie van [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) met een stream.

```python
def __init__(self, document):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| document | `io.RawIOBase` | Bronstroom van het document. |

### Voorbeeld

```python
from groupdocs.redaction import Redactor

def open_from_stream():
    # Open het document als een binaire stream
    with open("./sample.pdf", "rb") as stream:
        # Laad het document vanuit de stream
        with Redactor(stream) as redactor:
            # Voer hier redacties uit
            pass
```

## __init__ {#file_path-load_options}

Initialiseert een nieuwe instantie van [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) voor een wachtwoord‑beveiligd document met het pad.

```python
def __init__(self, file_path, load_options):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| file_path | `str` | Pad naar het bestand. |
| load_options | `LoadOptions` | Opties, inclusief wachtwoord. |

### Voorbeeld

```python
from groupdocs.redaction import Redactor

# Laad een met wachtwoord beveiligd document vanaf een bestandspad
with Redactor("protected.docx") as redactor:
    # Voer hier redactie‑operaties uit
    pass
```

## __init__ {#file_path-load_options-settings}

Initialiseert een nieuwe Redactor-instantie voor een wachtwoord‑beveiligd document met het pad en instellingen.

```python
def __init__(self, file_path, load_options, settings):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| file_path | `str` | Pad naar bestand. |
| load_options | `LoadOptions` | Bestand‑afhankelijke opties, inclusief wachtwoord. |
| settings | `RedactorSettings` | Standaardinstellingen voor het redactieproces. |

### Voorbeeld

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

## __init__ {#document-load_options}

Initialiseert een nieuwe Redactor-instantie voor een wachtwoord‑beveiligd document met een stream.

```python
def __init__(self, document, load_options):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| document | `io.RawIOBase` | Bron‑invoerstroom. |
| load_options | `LoadOptions` | Opties, inclusief wachtwoord. |

### Voorbeeld

```python
from groupdocs.redaction import Redactor, LoadOptions

def open_protected_doc():
    # Open de beveiligde PDF als een binaire stroom
    with open(r"C:\sample.pdf", "rb") as stream:
        # Geef het wachtwoord op via LoadOptions
        load_options = LoadOptions("mypassword")
        # Initialiseer Redactor met de stroom en laadopties
        with Redactor(stream, load_options) as redactor:
            # Voer hier redactie‑operaties uit
            pass
```

## __init__ {#document-load_options-settings}

Initialiseert een nieuwe instantie van [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) voor een wachtwoord‑beveiligd document met een stream en instellingen.

```python
def __init__(self, document, load_options, settings):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| document | `io.RawIOBase` | Bron‑invoerstroom. |
| load_options | `LoadOptions` | Opties, inclusief wachtwoord. |
| settings | `RedactorSettings` | Standaardinstellingen voor het redactieproces. |

### Zie ook
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
