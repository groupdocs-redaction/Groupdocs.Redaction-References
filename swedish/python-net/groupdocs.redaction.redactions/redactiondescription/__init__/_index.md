---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny instans av RedactionDescription-klass utan ersättningsinformation."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/
is_root: false
weight: 10
---


## __init__ {#redaction_type-action_type-original_text}

Initierar en ny instans av RedactionDescription-klass utan ersättningsinformation.

```python
def __init__(self, redaction_type, action_type, original_text):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| redaction_type | `RedactionType` | Typ av data som raderas. |
| action_type | `RedactionActionType` | Åtgärd som ska utföras på dessa data. |
| original_text | `str` | Matchad text, kommentar eller annoteringsinnehåll. |

## __init__ {#redaction_type-action_type-original_text-replacement}

Initierar en ny instans av RedactionDescription-klass med ersättningsinformation.

```python
def __init__(self, redaction_type, action_type, original_text, replacement):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| redaction_type | `RedactionType` | Typ av data som raderas. |
| action_type | `RedactionActionType` | Åtgärd som ska utföras på dessa data. |
| original_text | `str` | Matchad text, kommentar eller annoteringsinnehåll. |
| replacement | `TextReplacement` | Ersättningstext, matchad text och dess position i den ursprungliga strängen. |

## __init__ {#redaction_type-action_type-image_area_replacement-image_details}

Initierar en ny RedactionDescription med ersättningsinformation för bildområde.

```python
def __init__(self, redaction_type, action_type, image_area_replacement, image_details):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| redaction_type | `RedactionType` | Typ av data som raderas. |
| action_type | `RedactionActionType` | Åtgärd som ska utföras på dessa data. |
| image_area_replacement | `RegionReplacementOptions` | Information om ersättning av bildområde. |
| image_details | `str` | Textuell beskrivning av bilden, som standard är den en tom sträng. |

### Se även
* class [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/)
