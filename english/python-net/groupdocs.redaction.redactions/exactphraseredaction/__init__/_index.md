---
title: ExactPhraseRedaction constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/
is_root: false
weight: 10
---

## __init__ {#str-groupdocs.redaction.redactions.ReplacementOptions}

Initializes a new instance of ExactPhraseRedaction class in case insensitive mode.



```python
def __init__(self, search_phrase, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| search_phrase | str | String to search and replace |
| options | [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions) | Replacement options (textual, color) |


## __init__ {#str-bool-groupdocs.redaction.redactions.ReplacementOptions}

Initializes a new instance of ExactPhraseRedaction class.



```python
def __init__(self, search_phrase, is_case_sensitive, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| search_phrase | str | String to search and replace |
| is_case_sensitive | bool | True if case sensitive search is required |
| options | [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions) | Replacement options (textual, color) |



### See Also
* module [`groupdocs.redaction.redactions`](../../)
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction)
