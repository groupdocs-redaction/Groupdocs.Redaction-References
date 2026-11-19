---
title: perform_binary_check method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Checks if the given stream contains a document supported by this format instance."
type: docs
url: /python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/
is_root: false
weight: 1040
---


## perform_binary_check {#input}

Checks if the given stream contains a document supported by this format instance.

```python
def perform_binary_check(self, input):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| input | `io.RawIOBase` | Document content stream. |

**Returns:** bool: True if the document can be loaded by this format instance, False otherwise.

### Aliases

These names call `perform_binary_check` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `perform_binary_check_stream` | `perform_binary_check_stream(input)` |
| `perform_binary_check_streams` | `perform_binary_check_streams(input)` |

### See Also
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
