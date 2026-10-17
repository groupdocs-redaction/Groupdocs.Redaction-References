---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert eine neue Instanz der LoadOptions Klasse."
type: docs
url: /de/python-net/groupdocs.redaction.options/loadoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initialisiert eine neue Instanz der LoadOptions Klasse.

```python
def __init__(self):
    ...
```

## __init__ {#password}

Initialisiert eine neue Instanz von LoadOptions mit dem angegebenen Passwort.

```python
def __init__(self, password):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| password | `str` | Passwort für geschützte Dateien. |

### Beispiel

```python
    from groupdocs.redaction.options import LoadOptions

    # Lade ein passwortgeschütztes Dokument
    load_opt = LoadOptions("mypassword")
    ```

## __init__ {#pre_rasterize}

Initialisiert eine neue LoadOptions‑Instanz mit dem angegebenen Pre‑Rasterisierungs‑Flag.

```python
def __init__(self, pre_rasterize):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| pre_rasterize | `bool` | Wenn True, Rasterisierung beim Laden erzwingen. |

## __init__ {#password-pre_rasterize}

Initialisiert eine neue LoadOptions‑Instanz mit dem angegebenen Passwort.

Wenn `pre_rasterize` True ist, wird die Rasterisierung erzwungen, wenn das Dokument geladen wird.

```python
def __init__(self, password, pre_rasterize):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| password | `str` | Passwort für geschützte Dateien. |
| pre_rasterize | `bool` | Wenn True, Rasterisierung beim Laden erzwingen. |

### Beispiel

```python
from groupdocs.redaction.options import LoadOptions

# Lade ein passwortgeschütztes Dokument
load_opt = LoadOptions("mypassword")
```

### Siehe auch
* class [`LoadOptions`](/redaction/python-net/groupdocs.redaction.options/loadoptions/)
