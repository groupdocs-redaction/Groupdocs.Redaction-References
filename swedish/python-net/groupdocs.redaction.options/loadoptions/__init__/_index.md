---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny instans av LoadOptions-klass."
type: docs
url: /sv/python-net/groupdocs.redaction.options/loadoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initierar en ny instans av LoadOptions-klass.

```python
def __init__(self):
    ...
```

## __init__ {#password}

Initierar en ny instans av LoadOptions med det angivna lösenordet.

```python
def __init__(self, password):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| password | `str` | Lösenord för skyddade filer. |

### Exempel

```python
    from groupdocs.redaction.options import LoadOptions

    # Läs in ett lösenordsskyddat dokument
    load_opt = LoadOptions("mypassword")
    ```

## __init__ {#pre_rasterize}

Initierar en ny LoadOptions-instans med den angivna pre‑rasteriseringsflaggan.

```python
def __init__(self, pre_rasterize):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| pre_rasterize | `bool` | Om True, tvinga rasterisering vid inläsning. |

## __init__ {#password-pre_rasterize}

Initierar en ny LoadOptions-instans med det angivna lösenordet.

Om `pre_rasterize` är True, tvingas rasterisering när dokumentet läses in.

```python
def __init__(self, password, pre_rasterize):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| password | `str` | Lösenord för skyddade filer. |
| pre_rasterize | `bool` | Om True, tvinga rasterisering vid inläsning. |

### Exempel

```python
from groupdocs.redaction.options import LoadOptions

# Läs in ett lösenordsskyddat dokument
load_opt = LoadOptions("mypassword")
```

### Se även
* class [`LoadOptions`](/redaction/python-net/groupdocs.redaction.options/loadoptions/)
