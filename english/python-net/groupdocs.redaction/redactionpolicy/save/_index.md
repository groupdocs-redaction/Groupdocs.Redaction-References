---
title: save method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Saves the redaction policy to a file."
type: docs
url: /python-net/groupdocs.redaction/redactionpolicy/save/
is_root: false
weight: 1060
---


## save {#file_path}

Saves the redaction policy to a file.

```python
def save(self, file_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | Path to file. |

### Example

```python
    policy = RedactionPolicy([
        ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
        RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
    ])
    policy.save("./sample_policy.xml")
    ```

## save {#output}

Saves the redaction policy to a stream.

```python
def save(self, output):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| output | `io.RawIOBase` | Target stream to save the policy. |

**Returns:** None.

### See Also
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
