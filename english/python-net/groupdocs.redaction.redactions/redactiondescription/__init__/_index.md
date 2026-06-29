---
title: __init__ constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Initializes a new instance of RedactionDescription class without replacement information."
type: docs
url: /python-net/groupdocs.redaction.redactions/redactiondescription/__init__/
is_root: false
weight: 10
---


## __init__ {#redaction_type-action_type-original_text}

Initializes a new instance of RedactionDescription class without replacement information.

```python
def __init__(self, redaction_type, action_type, original_text):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| redaction_type | `RedactionType` | Type of data being redacted. |
| action_type | `RedactionActionType` | Action to be performed on these data. |
| original_text | `str` | Matched text, comment or annotation body. |

## __init__ {#redaction_type-action_type-original_text-replacement}

Initializes a new instance of RedactionDescription class with replacement information.

```python
def __init__(self, redaction_type, action_type, original_text, replacement):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| redaction_type | `RedactionType` | Type of data being redacted. |
| action_type | `RedactionActionType` | Action to be performed on these data. |
| original_text | `str` | Matched text, comment or annotation body. |
| replacement | `TextReplacement` | Replacement text, matched text and its position within original string. |

## __init__ {#redaction_type-action_type-image_area_replacement-image_details}

Initializes a new RedactionDescription with image area replacement information.

```python
def __init__(self, redaction_type, action_type, image_area_replacement, image_details):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| redaction_type | `RedactionType` | Type of data being redacted. |
| action_type | `RedactionActionType` | Action to be performed on these data. |
| image_area_replacement | `RegionReplacementOptions` | Image area replacement information. |
| image_details | `str` | Image textual description, by default it is an empty string. |

### See Also
* class [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/)
