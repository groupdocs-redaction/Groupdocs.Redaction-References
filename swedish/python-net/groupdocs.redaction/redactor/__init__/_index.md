---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny Redactor-instans med en filsökväg."
type: docs
url: /sv/python-net/groupdocs.redaction/redactor/__init__/
is_root: false
weight: 10
---


## __init__ {#file_path}

Initierar en ny Redactor-instans med en filsökväg.

```python
def __init__(self, file_path):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| file_path | `str` | Sökväg till filen. |

### Exempel

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    # Utför raderingsoperationer här
    pass
```

## __init__ {#document}

Initierar en ny instans av [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) med en ström.

```python
def __init__(self, document):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| document | `io.RawIOBase` | Källström för dokumentet. |

### Exempel

```python
from groupdocs.redaction import Redactor

def open_from_stream():
    # Öppna dokumentet som en binär ström
    with open("./sample.pdf", "rb") as stream:
        # Läs in dokumentet från strömmen
        with Redactor(stream) as redactor:
            # Utför raderingar här
            pass
```

## __init__ {#file_path-load_options}

Initierar en ny instans av [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) för ett lösenordsskyddat dokument med dess sökväg.

```python
def __init__(self, file_path, load_options):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| file_path | `str` | Sökväg till filen. |
| load_options | `LoadOptions` | Alternativ, inklusive lösenord. |

### Exempel

```python
from groupdocs.redaction import Redactor

# Läs in ett lösenordsskyddat dokument från en filsökväg
with Redactor("protected.docx") as redactor:
    # Utför raderingsoperationer här
    pass
```

## __init__ {#file_path-load_options-settings}

Initierar en ny Redactor-instans för ett lösenordsskyddat dokument med dess sökväg och inställningar.

```python
def __init__(self, file_path, load_options, settings):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| file_path | `str` | Sökväg till fil. |
| load_options | `LoadOptions` | Filberoende alternativ, inklusive lösenord. |
| settings | `RedactorSettings` | Standardinställningar för raderingsprocessen. |

### Exempel

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

## __init__ {#document-load_options}

Initierar en ny Redactor-instans för ett lösenordsskyddat dokument med en ström.

```python
def __init__(self, document, load_options):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| document | `io.RawIOBase` | Källinmatningsström. |
| load_options | `LoadOptions` | Alternativ, inklusive lösenord. |

### Exempel

```python
from groupdocs.redaction import Redactor, LoadOptions

def open_protected_doc():
    # Öppna det skyddade PDF‑dokumentet som en binärström
    with open(r"C:\sample.pdf", "rb") as stream:
        # Ange lösenordet via LoadOptions
        load_options = LoadOptions("mypassword")
        # Initiera Redactor med strömmen och laddningsalternativen
        with Redactor(stream, load_options) as redactor:
            # Utför raderingsoperationer här
            pass
```

## __init__ {#document-load_options-settings}

Initierar en ny instans av [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) för ett lösenordsskyddat dokument med en ström och inställningar.

```python
def __init__(self, document, load_options, settings):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| document | `io.RawIOBase` | Källinmatningsström. |
| load_options | `LoadOptions` | Alternativ, inklusive lösenord. |
| settings | `RedactorSettings` | Standardinställningar för redigeringsprocessen. |

### Se även
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
