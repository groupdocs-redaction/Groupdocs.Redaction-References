---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new instance of LoadOptions class."
type: docs
url: /python-net/groupdocs.redaction.options/loadoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new instance of LoadOptions class.

```python
def __init__(self):
    ...
```

## __init__ {#password}

Initializes a new instance of LoadOptions with the specified password.

```python
def __init__(self, password):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| password | `str` | Password for protected files. |

### Example

```python
    from groupdocs.redaction.options import LoadOptions

    # Load a password‑protected document
    load_opt = LoadOptions("mypassword")
    ```

## __init__ {#pre_rasterize}

Initializes a new LoadOptions instance with the specified pre‑rasterization flag.

```python
def __init__(self, pre_rasterize):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| pre_rasterize | `bool` | If True, force rasterization on loading. |

## __init__ {#password-pre_rasterize}

Initializes a new LoadOptions instance with the specified password.

If `pre_rasterize` is True, rasterization is forced when the document is loaded.

```python
def __init__(self, password, pre_rasterize):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| password | `str` | Password for protected files. |
| pre_rasterize | `bool` | If True, force rasterization on loading. |

### Example

```python
from groupdocs.redaction.options import LoadOptions

# Load a password-protected document
load_opt = LoadOptions("mypassword")
```

### See Also
* class [`LoadOptions`](/redaction/python-net/groupdocs.redaction.options/loadoptions/)
