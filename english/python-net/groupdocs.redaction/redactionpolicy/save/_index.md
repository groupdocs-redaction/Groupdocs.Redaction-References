---
title: save method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Saves the redaction policy to a file."
type: docs
url: /python-net/groupdocs.redaction/redactionpolicy/save/
is_root: false
weight: 1020
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
    from groupdocs.redaction import RedactionPolicy
    from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

    policy = RedactionPolicy([
        ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
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

### Example

```python
import io
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    ExactPhraseRedaction("confidential", ReplacementOptions("[REDACTED]")),
])

with io.BytesIO() as stream:
    policy.save(stream)
    # The stream now contains the XML representation of the policy
```

### Aliases

These names call `save` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `save_file` | `save_file(file_path)` |
| `save_string` | `save_string(file_path)` |
| `save_stream` | `save_stream(output)` |
| `save_streams` | `save_streams(output)` |

### See Also
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
