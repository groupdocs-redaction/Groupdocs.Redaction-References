---
title: "save metod"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Sparar redigeringspolicyn till en fil."
type: docs
url: /sv/python-net/groupdocs.redaction/redactionpolicy/save/
is_root: false
weight: 1060
---


## save {#file_path}

Sparar redigeringspolicyn till en fil.

```python
def save(self, file_path):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| file_path | `str` | Sökväg till fil. |

### Exempel

```python
    policy = RedactionPolicy([
        ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
        RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
    ])
    policy.save("./sample_policy.xml")
    ```

## save {#output}

Sparar redigeringspolicyn till en ström.

```python
def save(self, output):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| output | `io.RawIOBase` | Målsström för att spara policyn. |

**Returns:** None.

### Se även
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
