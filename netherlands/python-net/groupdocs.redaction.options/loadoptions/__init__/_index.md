---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuw exemplaar van de LoadOptions-klasse."
type: docs
url: /nl/python-net/groupdocs.redaction.options/loadoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initialiseert een nieuw exemplaar van de LoadOptions-klasse.

```python
def __init__(self):
    ...
```

## __init__ {#password}

Initialiseert een nieuw exemplaar van LoadOptions met het opgegeven wachtwoord.

```python
def __init__(self, password):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| password | `str` | Wachtwoord voor beveiligde bestanden. |

### Voorbeeld

```python
    from groupdocs.redaction.options import LoadOptions

    # Laad een wachtwoord‑beveiligd document
    load_opt = LoadOptions("mypassword")
    ```

## __init__ {#pre_rasterize}

Initialiseert een nieuw LoadOptions-exemplaar met de opgegeven pre‑rasterisatie‑vlag.

```python
def __init__(self, pre_rasterize):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| pre_rasterize | `bool` | Als True, forceer rasteren bij het laden. |

## __init__ {#password-pre_rasterize}

Initialiseert een nieuw LoadOptions-exemplaar met het opgegeven wachtwoord.

Als `pre_rasterize` True is, wordt rasteren afgedwongen wanneer het document wordt geladen.

```python
def __init__(self, password, pre_rasterize):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| password | `str` | Wachtwoord voor beveiligde bestanden. |
| pre_rasterize | `bool` | Als True, forceer rasteren bij het laden. |

### Voorbeeld

```python
from groupdocs.redaction.options import LoadOptions

# Laad een wachtwoord‑beveiligd document
load_opt = LoadOptions("mypassword")
```

### Zie ook
* class [`LoadOptions`](/redaction/python-net/groupdocs.redaction.options/loadoptions/)
