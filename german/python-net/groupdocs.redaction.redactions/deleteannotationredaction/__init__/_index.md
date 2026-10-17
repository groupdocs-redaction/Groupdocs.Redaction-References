---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert eine neue Instanz der DeleteAnnotationRedaction‑Klasse mit Einstellungen, um alle Anmerkungen zu löschen (alles passend)."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/
is_root: false
weight: 10
---


## __init__

Initialisiert eine neue Instanz der DeleteAnnotationRedaction‑Klasse mit Einstellungen, um alle Anmerkungen zu löschen (alles passend).

```python
def __init__(self):
    ...
```

### Beispiel

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Alle Anmerkungen löschen
del_red = DeleteAnnotationRedaction()
```

## __init__ {#pattern}

Initialisiert eine neue Instanz der DeleteAnnotationRedaction‑Klasse und löscht Anmerkungen, die dem angegebenen Ausdruck entsprechen.

```python
def __init__(self, pattern):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| pattern | `str` | Regulärer Ausdruck. |

### Beispiel

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Lösche Anmerkungen, die das Wort "internal" enthalten (Groß-/Kleinschreibung ignorierend)
del_red = DeleteAnnotationRedaction(r"(?i)internal")
```

## __init__ {#regex}

Initialisiert eine neue Instanz der DeleteAnnotationRedaction‑Klasse und löscht Anmerkungen, die dem angegebenen Ausdruck entsprechen.

```python
def __init__(self, regex):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | Regulärer Ausdruck. |

### Beispiel

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# Anmerkungen löschen, deren Inhalt dem Regex entspricht (Groß‑/Kleinschreibung ignoriert)
del_red = DeleteAnnotationRedaction("(?i)internal")
```

### Siehe auch
* class [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/)
