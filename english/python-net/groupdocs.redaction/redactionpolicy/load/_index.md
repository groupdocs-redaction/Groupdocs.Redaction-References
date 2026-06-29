---
title: load method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Loads a RedactionPolicy from an XML file."
type: docs
url: /python-net/groupdocs.redaction/redactionpolicy/load/
is_root: false
weight: 1010
---


## load {#file_path}

Loads a RedactionPolicy from an XML file.

```python
def load(cls, file_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | Path to the XML file. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Example

```python
from groupdocs.redaction import RedactionPolicy, Redactor

policy = RedactionPolicy.load("RedactionPolicy.xml")

with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

## load {#input}

Loads a RedactionPolicy instance from a stream containing XML configuration.

```python
def load(cls, input):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| input | `io.RawIOBase` | Stream containing XML configuration. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Example

```python
from groupdocs.redaction import RedactionPolicy, Redactor

# Load the policy from an XML file
with open("policy.xml", "rb") as stream:
    policy = RedactionPolicy.load(stream)

# Apply the policy to a document
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### See Also
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
