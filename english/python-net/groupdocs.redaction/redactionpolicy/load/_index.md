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

Loads a [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/) from an XML file.

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
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

policy = RedactionPolicy.load("./sample_policy.xml")

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
from pathlib import Path
from groupdocs.redaction import Redactor, RedactionPolicy, RedactionStatus
from groupdocs.redaction.options import SaveOptions

# Load the policy from an XML file
with open("RedactionPolicy.xml", "rb") as stream:
    policy = RedactionPolicy.load(stream)

inbound = Path("inbound")
done, failed = Path("outbound/done"), Path("outbound/failed")
done.mkdir(parents=True, exist_ok=True)
failed.mkdir(parents=True, exist_ok=True)

for file_path in inbound.iterdir():
    if file_path.is_file():
        with Redactor(str(file_path)) as redactor:
            result = redactor.apply(policy)
            target_folder = done if result.status != RedactionStatus.FAILED else failed
            with open(str(target_folder / file_path.name), "wb") as out_stream:
                redactor.save(out_stream, SaveOptions(rasterize_to_pdf=False))  # keep the format
```

### Aliases

These names call `load` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `load_file` | `load_file(file_path)` |
| `load_string` | `load_string(file_path)` |
| `load_stream` | `load_stream(input)` |
| `load_streams` | `load_streams(input)` |

### See Also
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
