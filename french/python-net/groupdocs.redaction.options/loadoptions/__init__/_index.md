---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise une nouvelle instance de la classe LoadOptions."
type: docs
url: /fr/python-net/groupdocs.redaction.options/loadoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initialise une nouvelle instance de la classe LoadOptions.

```python
def __init__(self):
    ...
```

## __init__ {#password}

Initialise une nouvelle instance de LoadOptions avec le mot de passe spécifié.

```python
def __init__(self, password):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| password | `str` | Mot de passe pour les fichiers protégés. |

### Exemple

```python
    from groupdocs.redaction.options import LoadOptions

    # Charger un document protégé par mot de passe
    load_opt = LoadOptions("mypassword")
    ```

## __init__ {#pre_rasterize}

Initialise une nouvelle instance de LoadOptions avec le drapeau de pré‑rasterisation spécifié.

```python
def __init__(self, pre_rasterize):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| pre_rasterize | `bool` | Si True, forcer la rasterisation lors du chargement. |

## __init__ {#password-pre_rasterize}

Initialise une nouvelle instance de LoadOptions avec le mot de passe spécifié.

Si `pre_rasterize` est True, la rasterisation est forcée lorsque le document est chargé.

```python
def __init__(self, password, pre_rasterize):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| password | `str` | Mot de passe pour les fichiers protégés. |
| pre_rasterize | `bool` | Si True, forcer la rasterisation lors du chargement. |

### Exemple

```python
from groupdocs.redaction.options import LoadOptions

# Charger un document protégé par mot de passe
load_opt = LoadOptions("mypassword")
```

### Voir aussi
* class [`LoadOptions`](/redaction/python-net/groupdocs.redaction.options/loadoptions/)
