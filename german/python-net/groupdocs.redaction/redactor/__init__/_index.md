---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert eine neue Redactor-Instanz mittels eines Dateipfads."
type: docs
url: /de/python-net/groupdocs.redaction/redactor/__init__/
is_root: false
weight: 10
---


## __init__ {#file_path}

Initialisiert eine neue Redactor-Instanz mittels eines Dateipfads.

```python
def __init__(self, file_path):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| file_path | `str` | Pfad zur Datei. |

### Beispiel

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    # Führen Sie hier Redaktionsvorgänge aus
    pass
```

## __init__ {#document}

Initialisiert eine neue Instanz von [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) mittels eines Streams.

```python
def __init__(self, document):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| document | `io.RawIOBase` | Quellstream des Dokuments. |

### Beispiel

```python
from groupdocs.redaction import Redactor

def open_from_stream():
    # Öffnen Sie das Dokument als Binär-Stream
    with open("./sample.pdf", "rb") as stream:
        # Laden Sie das Dokument aus dem Stream
        with Redactor(stream) as redactor:
            # Führen Sie hier Redaktionen aus
            pass
```

## __init__ {#file_path-load_options}

Initialisiert eine neue Instanz von [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) für ein passwortgeschütztes Dokument mittels seines Pfads.

```python
def __init__(self, file_path, load_options):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| file_path | `str` | Pfad zur Datei. |
| load_options | `LoadOptions` | Optionen, einschließlich Passwort. |

### Beispiel

```python
from groupdocs.redaction import Redactor

# Laden Sie ein passwortgeschütztes Dokument von einem Dateipfad
with Redactor("protected.docx") as redactor:
    # Führen Sie hier Redaktionsvorgänge aus
    pass
```

## __init__ {#file_path-load_options-settings}

Initialisiert eine neue Redactor-Instanz für ein passwortgeschütztes Dokument mittels seines Pfads und seiner Einstellungen.

```python
def __init__(self, file_path, load_options, settings):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| file_path | `str` | Pfad zur Datei. |
| load_options | `LoadOptions` | Dateiabhängige Optionen, einschließlich Passwort. |
| settings | `RedactorSettings` | Standardeinstellungen für den Redaktionsprozess. |

### Beispiel

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

## __init__ {#document-load_options}

Initialisiert eine neue Redactor-Instanz für ein passwortgeschütztes Dokument mittels eines Streams.

```python
def __init__(self, document, load_options):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| document | `io.RawIOBase` | Quell‑Eingabestream. |
| load_options | `LoadOptions` | Optionen, einschließlich Passwort. |

### Beispiel

```python
from groupdocs.redaction import Redactor, LoadOptions

def open_protected_doc():
    # Öffnen Sie das geschützte PDF als Binärstream
    with open(r"C:\sample.pdf", "rb") as stream:
        # Geben Sie das Passwort über LoadOptions an
        load_options = LoadOptions("mypassword")
        # Initialisieren Sie Redactor mit dem Stream und den Ladeoptionen
        with Redactor(stream, load_options) as redactor:
            # Führen Sie hier Redaktionsvorgänge aus
            pass
```

## __init__ {#document-load_options-settings}

Initialisiert eine neue Instanz von [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) für ein passwortgeschütztes Dokument mittels eines Streams und Einstellungen.

```python
def __init__(self, document, load_options, settings):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| document | `io.RawIOBase` | Quell‑Eingabestream. |
| load_options | `LoadOptions` | Optionen, einschließlich Passwort. |
| settings | `RedactorSettings` | Standardeinstellungen für den Redaktionsprozess. |

### Siehe auch
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
