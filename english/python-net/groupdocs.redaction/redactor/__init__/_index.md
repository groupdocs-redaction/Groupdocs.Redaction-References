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

Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) using a stream.

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

def open_from_stream():
    # Open the document as a binary stream
    with open("./sample.pdf", "rb") as stream:
        # Load the document from the stream
        with Redactor(stream) as redactor:
            # Perform redactions here
            pass
```

## __init__ {#file_path-load_options}

Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) for a password‑protected document using its path.

```python
def __init__(self, file_path, load_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | Path to the file. |
| load_options | `LoadOptions` | Options, including password. |

### Example

```python
from groupdocs.redaction import Redactor

# Load a password‑protected document from a file path
with Redactor("protected.docx") as redactor:
    # Perform redaction operations here
    pass
```

## __init__ {#file_path-load_options-settings}

Initializes a new Redactor instance for a password‑protected document using its path and settings.

```python
def __init__(self, file_path, load_options, settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | Path to file. |
| load_options | `LoadOptions` | File‑dependent options, including password. |
| settings | `RedactorSettings` | Default settings for redaction process. |

### Example

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

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
from groupdocs.redaction import Redactor, LoadOptions

def open_protected_doc():
    # Open the protected PDF as a binary stream
    with open(r"C:\sample.pdf", "rb") as stream:
        # Provide the password via LoadOptions
        load_options = LoadOptions("mypassword")
        # Initialize Redactor with the stream and load options
        with Redactor(stream, load_options) as redactor:
            # Perform redaction operations here
            pass
```

## __init__ {#document-load_options-settings}

Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) for a password‑protected document using a stream and settings.

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
