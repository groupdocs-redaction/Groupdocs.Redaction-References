---
title: "Speichermethode"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Speichert die Redaktionsrichtlinie in einer Datei."
type: docs
url: /de/python-net/groupdocs.redaction/redactionpolicy/save/
is_root: false
weight: 1060
---


## save {#file_path}

Speichert die Redaktionsrichtlinie in einer Datei.

```python
def save(self, file_path):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| file_path | `str` | Pfad zur Datei. |

### Beispiel

```python
    policy = RedactionPolicy([
        ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
        RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
    ])
    policy.save("./sample_policy.xml")
    ```

## save {#output}

Speichert die Redaktionsrichtlinie in einen Stream.

```python
def save(self, output):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| output | `io.RawIOBase` | Ziel-Stream zum Speichern der Richtlinie. |

**Returns:** None.

### Siehe auch
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
