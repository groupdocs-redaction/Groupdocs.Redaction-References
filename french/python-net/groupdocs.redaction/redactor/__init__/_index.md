---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise une nouvelle instance de Redactor en utilisant un chemin de fichier."
type: docs
url: /fr/python-net/groupdocs.redaction/redactor/__init__/
is_root: false
weight: 10
---


## __init__ {#file_path}

Initialise une nouvelle instance de Redactor en utilisant un chemin de fichier.

```python
def __init__(self, file_path):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| file_path | `str` | Chemin vers le fichier. |

### Exemple

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    # Effectuez les opérations de redaction ici
    pass
```

## __init__ {#document}

Initialise une nouvelle instance de [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) en utilisant un flux.

```python
def __init__(self, document):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| document | `io.RawIOBase` | Flux source du document. |

### Exemple

```python
from groupdocs.redaction import Redactor

def open_from_stream():
    # Ouvrez le document en tant que flux binaire
    with open("./sample.pdf", "rb") as stream:
        # Chargez le document depuis le flux
        with Redactor(stream) as redactor:
            # Effectuez les redactions ici
            pass
```

## __init__ {#file_path-load_options}

Initialise une nouvelle instance de [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) pour un document protégé par mot de passe en utilisant son chemin.

```python
def __init__(self, file_path, load_options):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| file_path | `str` | Chemin vers le fichier. |
| load_options | `LoadOptions` | Options, y compris le mot de passe. |

### Exemple

```python
from groupdocs.redaction import Redactor

# Chargez un document protégé par mot de passe depuis un chemin de fichier
with Redactor("protected.docx") as redactor:
    # Effectuez les opérations de redaction ici
    pass
```

## __init__ {#file_path-load_options-settings}

Initialise une nouvelle instance de Redactor pour un document protégé par mot de passe en utilisant son chemin et ses paramètres.

```python
def __init__(self, file_path, load_options, settings):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| file_path | `str` | Chemin du fichier. |
| load_options | `LoadOptions` | Options dépendant du fichier, y compris le mot de passe. |
| settings | `RedactorSettings` | Paramètres par défaut pour le processus de redaction. |

### Exemple

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

## __init__ {#document-load_options}

Initialise une nouvelle instance de Redactor pour un document protégé par mot de passe en utilisant un flux.

```python
def __init__(self, document, load_options):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| document | `io.RawIOBase` | Flux d'entrée source. |
| load_options | `LoadOptions` | Options, y compris le mot de passe. |

### Exemple

```python
from groupdocs.redaction import Redactor, LoadOptions

def open_protected_doc():
    # Ouvrez le PDF protégé en tant que flux binaire
    with open(r"C:\sample.pdf", "rb") as stream:
        # Fournissez le mot de passe via LoadOptions
        load_options = LoadOptions("mypassword")
        # Initialisez Redactor avec le flux et les options de chargement
        with Redactor(stream, load_options) as redactor:
            # Effectuez les opérations de redaction ici
            pass
```

## __init__ {#document-load_options-settings}

Initialise une nouvelle instance de [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) pour un document protégé par mot de passe en utilisant un flux et des paramètres.

```python
def __init__(self, document, load_options, settings):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| document | `io.RawIOBase` | Flux d'entrée source. |
| load_options | `LoadOptions` | Options, y compris le mot de passe. |
| settings | `RedactorSettings` | Paramètres par défaut pour le processus de rédaction. |

### Voir aussi
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
