---
title: RedactionDescription constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.redactions/redactiondescription/__init__/
is_root: false
weight: 10
---

## __init__ {#groupdocs.redaction.redactions.RedactionType-groupdocs.redaction.redactions.RedactionActionType-str}

Initializes a new instance of RedactionDescription class without replacement information.



```python
def __init__(self, redaction_type, action_type, original_text):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| redaction_type | [`RedactionType`](/redaction/python-net/groupdocs.redaction.redactions/redactiontype) | Type of data being redacted |
| action_type | [`RedactionActionType`](/redaction/python-net/groupdocs.redaction.redactions/redactionactiontype) | Action to be performed on these data |
| original_text | str | Matched text, comment or annotation body |


## __init__ {#groupdocs.redaction.redactions.RedactionType-groupdocs.redaction.redactions.RedactionActionType-str-groupdocs.redaction.redactions.TextReplacement}

Initializes a new instance of RedactionDescription class with replacement information.



```python
def __init__(self, redaction_type, action_type, original_text, replacement):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| redaction_type | [`RedactionType`](/redaction/python-net/groupdocs.redaction.redactions/redactiontype) | Type of data being redacted |
| action_type | [`RedactionActionType`](/redaction/python-net/groupdocs.redaction.redactions/redactionactiontype) | Action to be performed on these data |
| original_text | str | Matched text, comment or annotation body |
| replacement | [`TextReplacement`](/redaction/python-net/groupdocs.redaction.redactions/textreplacement) | Replacement text, matched text and its position within original string |


## __init__ {#groupdocs.redaction.redactions.RedactionType-groupdocs.redaction.redactions.RedactionActionType-groupdocs.redaction.redactions.RegionReplacementOptions-str}

Initializes a new instance of RedactionDescription class with image area replacement information.



```python
def __init__(self, redaction_type, action_type, image_area_replacement, image_details):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| redaction_type | [`RedactionType`](/redaction/python-net/groupdocs.redaction.redactions/redactiontype) | Type of data being redacted |
| action_type | [`RedactionActionType`](/redaction/python-net/groupdocs.redaction.redactions/redactionactiontype) | Action to be performed on these data |
| image_area_replacement | [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions) | Image area replacement information |
| image_details | str | Image textual description, by default it is String.Empty |



### See Also
* module [`groupdocs.redaction.redactions`](../../)
* class [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription)
