---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza una nuova istanza di Redactor utilizzando un percorso file."
type: docs
url: /it/python-net/groupdocs.redaction/redactor/__init__/
is_root: false
weight: 10
---


## __init__ {#file_path}

Inizializza una nuova istanza di Redactor utilizzando un percorso file.

```python
def __init__(self, file_path):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| file_path | `str` | Percorso del file. |

### Esempio

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    # Esegui le operazioni di redazione qui
    pass
```

## __init__ {#document}

Inizializza una nuova istanza di [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) utilizzando uno stream.

```python
def __init__(self, document):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| document | `io.RawIOBase` | Flusso sorgente del documento. |

### Esempio

```python
from groupdocs.redaction import Redactor

def open_from_stream():
    # Apri il documento come stream binario
    with open("./sample.pdf", "rb") as stream:
        # Carica il documento dallo stream
        with Redactor(stream) as redactor:
            # Esegui le redazioni qui
            pass
```

## __init__ {#file_path-load_options}

Inizializza una nuova istanza di [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) per un documento protetto da password utilizzando il suo percorso.

```python
def __init__(self, file_path, load_options):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| file_path | `str` | Percorso del file. |
| load_options | `LoadOptions` | Opzioni, inclusa la password. |

### Esempio

```python
from groupdocs.redaction import Redactor

# Carica un documento protetto da password da un percorso file
with Redactor("protected.docx") as redactor:
    # Esegui le operazioni di redazione qui
    pass
```

## __init__ {#file_path-load_options-settings}

Inizializza una nuova istanza di Redactor per un documento protetto da password utilizzando il suo percorso e le impostazioni.

```python
def __init__(self, file_path, load_options, settings):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| file_path | `str` | Percorso del file. |
| load_options | `LoadOptions` | Opzioni dipendenti dal file, inclusa la password. |
| settings | `RedactorSettings` | Impostazioni predefinite per il processo di redazione. |

### Esempio

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

## __init__ {#document-load_options}

Inizializza una nuova istanza di Redactor per un documento protetto da password utilizzando uno stream.

```python
def __init__(self, document, load_options):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| document | `io.RawIOBase` | Flusso di input sorgente. |
| load_options | `LoadOptions` | Opzioni, inclusa la password. |

### Esempio

```python
from groupdocs.redaction import Redactor, LoadOptions

def open_protected_doc():
    # Apri il PDF protetto come flusso binario
    with open(r"C:\sample.pdf", "rb") as stream:
        # Fornisci la password tramite LoadOptions
        load_options = LoadOptions("mypassword")
        # Inizializza Redactor con il flusso e le opzioni di caricamento
        with Redactor(stream, load_options) as redactor:
            # Esegui le operazioni di redazione qui
            pass
```

## __init__ {#document-load_options-settings}

Inizializza una nuova istanza di [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) per un documento protetto da password utilizzando uno stream e le impostazioni.

```python
def __init__(self, document, load_options, settings):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| document | `io.RawIOBase` | Flusso di input sorgente. |
| load_options | `LoadOptions` | Opzioni, inclusa la password. |
| settings | `RedactorSettings` | Impostazioni predefinite per il processo di redazione. |

### Vedi anche
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
