---
title: Redactor constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction/redactor/__init__/
is_root: false
weight: 10
---

## __init__ {#str}

Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor) class using file path.



```python
def __init__(self, file_path):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_path | str | Path to the file |

### Example 


The following example demonstrates how to open a document for redaction.


## __init__ {#io.RawIOBase}

Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor) class using stream.



```python
def __init__(self, document):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| document | io.RawIOBase | Source stream of the document |

### Example 


The following example demonstrates how to open a document from stream.


## __init__ {#str-groupdocs.redaction.options.LoadOptions}

Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor) class for a password-protected document using its path.



```python
def __init__(self, file_path, load_options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_path | str | Path to file. |
| load_options | groupdocs.redaction.options.LoadOptions | Options, including password. |


## __init__ {#io.RawIOBase-groupdocs.redaction.options.LoadOptions}

Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor) class for a password-protected document using stream.



```python
def __init__(self, document, load_options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| document | io.RawIOBase | Source input stream. |
| load_options | groupdocs.redaction.options.LoadOptions | Options, including password. |

### Example 


The following example demonstrates how to open a password-protected documents using LoadOptions.


## __init__ {#str-groupdocs.redaction.options.LoadOptions-groupdocs.redaction.options.RedactorSettings}

Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor) class for a password-protected document using its path and settings.



```python
def __init__(self, file_path, load_options, settings):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_path | str | Path to file. |
| load_options | groupdocs.redaction.options.LoadOptions | File-dependent options, including password. |
| settings | groupdocs.redaction.options.RedactorSettings | Default settings for redaction process. |


## __init__ {#io.RawIOBase-groupdocs.redaction.options.LoadOptions-groupdocs.redaction.options.RedactorSettings}

Initializes a new instance of [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor) class for a password-protected document using stream and settings.



```python
def __init__(self, document, load_options, settings):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| document | io.RawIOBase | Source input stream. |
| load_options | groupdocs.redaction.options.LoadOptions | Options, including password. |
| settings | groupdocs.redaction.options.RedactorSettings | Default settings for redaction process. |

### Example 


The following example demonstrates how to open a password-protected documents using LoadOptions.



### See Also
* module [`groupdocs.redaction`](../../)
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor)
