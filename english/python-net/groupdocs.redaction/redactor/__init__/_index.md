---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new Redactor instance using a file path."
type: docs
url: /python-net/groupdocs.redaction/redactor/__init__/
is_root: false
weight: 10
---


## __init__ {#file_path}

Initializes a new Redactor instance using a file path.

```python
def __init__(self, file_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | Path to the file. |

### Example

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    # Perform redaction operations here
    pass
```

## __init__ {#document}

Initializes a new Redactor instance using a document stream.

```python
def __init__(self, document):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document | `io.RawIOBase` | Source stream of the document. |

### Example

```python
from groupdocs.redaction import Redactor

with open("./sample.docx", "rb") as stream:
    # Load the document from the stream
    with Redactor(stream) as redactor:
        # Perform redaction operations here
        pass
```

## __init__ {#file_path-load_options}

Initializes a new Redactor instance for a password-protected document using its path.

```python
def __init__(self, file_path, load_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | Path to file. |
| load_options | `LoadOptions` | Options, including password. |

## __init__ {#file_path-load_options-settings}

Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) for a password‑protected document using its path and settings.

```python
def __init__(self, file_path, load_options, settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | Path to file. |
| load_options | `LoadOptions` | File-dependent options, including password. |
| settings | `RedactorSettings` | Default settings for redaction process. |

## __init__ {#document-load_options}

Initializes a new Redactor instance for a password‑protected document using a stream.

```python
def __init__(self, document, load_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document | `io.RawIOBase` | Source input stream. |
| load_options | `LoadOptions` | Options, including password. |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions

def open_protected():
    load_options = LoadOptions("mypassword")
    with open("./sample.pdf", "rb") as stream:
        with Redactor(stream, load_options) as redactor:
            # Perform redactions here
            pass
```

## __init__ {#document-load_options-settings}

Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) for a password‑protected document using a stream and optional settings.

```python
def __init__(self, document, load_options, settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document | `io.RawIOBase` | Source input stream. |
| load_options | `LoadOptions` | Options, including password. |
| settings | `RedactorSettings` | Default settings for the redaction process. |

### See Also
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
