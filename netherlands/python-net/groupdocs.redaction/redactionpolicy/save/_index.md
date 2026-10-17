---
title: "save methode"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Slaat het redactiebeleid op in een bestand."
type: docs
url: /nl/python-net/groupdocs.redaction/redactionpolicy/save/
is_root: false
weight: 1060
---


## save {#file_path}

Slaat het redactiebeleid op in een bestand.

```python
def save(self, file_path):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| file_path | `str` | Pad naar bestand. |

### Voorbeeld

```python
    policy = RedactionPolicy([
        ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
        RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
    ])
    policy.save("./sample_policy.xml")
    ```

## save {#output}

Slaat het redactiebeleid op in een stream.

```python
def save(self, output):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| output | `io.RawIOBase` | Doelstream om het beleid op te slaan. |

**Returns:** None.

### Zie ook
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
