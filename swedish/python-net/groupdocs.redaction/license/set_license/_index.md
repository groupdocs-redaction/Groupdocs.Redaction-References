---
title: "set_license‑metod"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Applicera en licens på den aktuella processen."
type: docs
url: /sv/python-net/groupdocs.redaction/license/set_license/
is_root: false
weight: 1010
---


## set_license {#license_source}

Applicera en licens på den aktuella processen.

```python
def set_license(self, license_source):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| license_source |  | Antingen en strängväg till en ``.lic``-fil eller ett läsbart fil‑liknande objekt som returnerar licensbytarna. Fil‑liknande inmatningar skrivs till en temporär fil innan de skickas till bryggan. |

| Uppstår | Beskrivning |
| :- | :- |
| `TypeError` | Om ``license_source`` varken är en strängväg eller ett läsbart fil‑liknande objekt. |

### Se även
* class [`License`](/redaction/python-net/groupdocs.redaction/license/)
