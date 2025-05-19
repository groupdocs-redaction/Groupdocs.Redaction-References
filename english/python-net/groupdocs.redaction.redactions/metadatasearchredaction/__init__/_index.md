---
title: MetadataSearchRedaction constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/
is_root: false
weight: 10
---

## __init__ {#str-str}

Initializes a new instance of MetadataSearchRedaction class, using value to match redacted items.



```python
def __init__(self, value_pattern, replacement):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| value_pattern | str | Regular expression to search and replace |
| replacement | str | Textual replacement |


## __init__ {#str-str-str}

Initializes a new instance of MetadataSearchRedaction class, using item name and value to match redacted items.



```python
def __init__(self, value_pattern, replacement, key_pattern):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| value_pattern | str | Regular expression to search and replace metadata item value |
| replacement | str | Textual replacement |
| key_pattern | str | Regular expression to search and replace metadata item name |



### See Also
* module [`groupdocs.redaction.redactions`](../../)
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction)
