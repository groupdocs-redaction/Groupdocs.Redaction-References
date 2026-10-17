---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης LoadOptions."
type: docs
url: /el/python-net/groupdocs.redaction.options/loadoptions/__init__/
is_root: false
weight: 10
---


## __init__

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης LoadOptions.

```python
def __init__(self):
    ...
```

## __init__ {#password}

Αρχικοποιεί ένα νέο στιγμιότυπο του LoadOptions με τον καθορισμένο κωδικό πρόσβασης.

```python
def __init__(self, password):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| password | `str` | Κωδικός πρόσβασης για προστατευμένα αρχεία. |

### Παράδειγμα

```python
    from groupdocs.redaction.options import LoadOptions

    # Φόρτωση εγγράφου προστατευμένου με κωδικό πρόσβασης
    load_opt = LoadOptions("mypassword")
    ```

## __init__ {#pre_rasterize}

Αρχικοποιεί ένα νέο στιγμιότυπο LoadOptions με τη συγκεκριμένη σημαία προ‑απεικόνισης.

```python
def __init__(self, pre_rasterize):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| pre_rasterize | `bool` | Αν True, εξαναγκάστε την αποτύπωση κατά τη φόρτωση. |

## __init__ {#password-pre_rasterize}

Αρχικοποιεί ένα νέο στιγμιότυπο LoadOptions με τον καθορισμένο κωδικό πρόσβασης.

Αν `pre_rasterize` είναι True, η αποτύπωση εξαναγκάζεται όταν το έγγραφο φορτώνεται.

```python
def __init__(self, password, pre_rasterize):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| password | `str` | Κωδικός πρόσβασης για προστατευμένα αρχεία. |
| pre_rasterize | `bool` | Αν True, εξαναγκάστε την αποτύπωση κατά τη φόρτωση. |

### Παράδειγμα

```python
from groupdocs.redaction.options import LoadOptions

# Φόρτωση εγγράφου προστατευμένου με κωδικό πρόσβασης
load_opt = LoadOptions("mypassword")
```

### Δείτε επίσης
* class [`LoadOptions`](/redaction/python-net/groupdocs.redaction.options/loadoptions/)
