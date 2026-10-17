---
title: "set_license-Methode"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Wenden Sie eine Lizenz auf den aktuellen Prozess an."
type: docs
url: /de/python-net/groupdocs.redaction/license/set_license/
is_root: false
weight: 1010
---


## set_license {#license_source}

Wenden Sie eine Lizenz auf den aktuellen Prozess an.

```python
def set_license(self, license_source):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| license_source |  | Entweder ein String-Pfad zu einer ``.lic``-Datei oder ein lesbares dateiähnliches Objekt, das die Lizenzbytes liefert. Dateiähnliche Eingaben werden in eine temporäre Datei geschrieben, bevor sie an die Bridge übergeben werden. |

| Wirft | Beschreibung |
| :- | :- |
| `TypeError` | Wenn ``license_source`` weder ein String-Pfad noch ein lesbares dateiähnliches Objekt ist. |

### Siehe auch
* class [`License`](/redaction/python-net/groupdocs.redaction/license/)
