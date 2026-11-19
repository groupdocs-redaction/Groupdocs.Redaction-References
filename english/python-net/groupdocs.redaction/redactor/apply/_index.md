---
title: apply method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Applies a redaction to the document."
type: docs
url: /python-net/groupdocs.redaction/redactor/apply/
is_root: false
weight: 1010
---


## apply {#redaction}

Applies a redaction to the document.

```python
def apply(self, redaction):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| redaction | `Redaction` | An instance of `Redaction` to apply. |

**Returns:** RedactorChangeLog: Success or failure and error message in this case.

### Example

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("./sample.docx") as redactor:
    repl_opt = ReplacementOptions("[personal]")
    redaction = ExactPhraseRedaction("Emily Johnson", repl_opt)
    result = redactor.apply(redaction)

    if result.status != RedactionStatus.FAILED:
        redactor.save()
```

## apply {#redactions}

Applies a set of redactions to the document.

```python
def apply(self, redactions):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| redactions | `list[Redaction]` | An array of redactions to apply. |

**Returns:** RedactorChangeLog: Indicates success or failure and contains an error message if applicable.

### Example

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("document.docx") as redactor:
    redaction = ExactPhraseRedaction("confidential", ReplacementOptions("[REDACTED]"))
    result = redactor.apply([redaction])
    if result.status != RedactionStatus.FAILED:
        redactor.save()
```

## apply {#policy}

Applies a redaction policy to the document.

```python
def apply(self, policy):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| policy | `RedactionPolicy` | Redaction policy to apply. |

**Returns:** RedactorChangeLog: Contains the status of the operation and an error message if the operation failed.

### Example

```python
import os
from groupdocs.redaction import Redactor, RedactionPolicy, RedactionStatus
from groupdocs.redaction.options import SaveOptions

policy = RedactionPolicy.load("RedactionPolicy.xml")
for folder in ("outbound/done", "outbound/failed"):
    os.makedirs(folder, exist_ok=True)

for file_name in os.listdir("inbound"):
    with Redactor(os.path.join("inbound", file_name)) as redactor:
        result = redactor.apply(policy)
        target_dir = "outbound/done" if result.status != RedactionStatus.FAILED else "outbound/failed"
        with open(os.path.join(target_dir, file_name), "wb") as output:
            redactor.save(output, SaveOptions(rasterize_to_pdf=False))  # keep the format
```

### Aliases

These names call `apply` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `apply_redaction` | `apply_redaction(redaction)`<br>`apply_redaction(redactions)` |
| `apply_redaction_policy` | `apply_redaction_policy(policy)` |

### See Also
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
