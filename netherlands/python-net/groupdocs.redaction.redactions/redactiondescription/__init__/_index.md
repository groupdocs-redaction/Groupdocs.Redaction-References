---
title: "__init__-constructor"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Initialiseert een nieuw exemplaar van de RedactionDescription klasse zonder vervangingsinformatie."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/
is_root: false
weight: 10
---


## __init__ {#redaction_type-action_type-original_text}

Initialiseert een nieuw exemplaar van de RedactionDescription klasse zonder vervangingsinformatie.

```python
def __init__(self, redaction_type, action_type, original_text):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| redaction_type | `RedactionType` | Type gegevens die worden geredigeerd. |
| action_type | `RedactionActionType` | Actie die op deze gegevens moet worden uitgevoerd. |
| original_text | `str` | Gevonden tekst, commentaar of annotatie‑inhoud. |

## __init__ {#redaction_type-action_type-original_text-replacement}

Initialiseert een nieuw exemplaar van de RedactionDescription klasse met vervangingsinformatie.

```python
def __init__(self, redaction_type, action_type, original_text, replacement):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| redaction_type | `RedactionType` | Type gegevens die worden geredigeerd. |
| action_type | `RedactionActionType` | Actie die op deze gegevens moet worden uitgevoerd. |
| original_text | `str` | Gevonden tekst, commentaar of annotatie‑inhoud. |
| replacement | `TextReplacement` | Vervangende tekst, gevonden tekst en de positie ervan binnen de oorspronkelijke tekenreeks. |

## __init__ {#redaction_type-action_type-image_area_replacement-image_details}

Initialiseert een nieuwe RedactionDescription met vervangingsinformatie voor een afbeeldingsgebied.

```python
def __init__(self, redaction_type, action_type, image_area_replacement, image_details):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| redaction_type | `RedactionType` | Type gegevens die worden geredigeerd. |
| action_type | `RedactionActionType` | Actie die op deze gegevens moet worden uitgevoerd. |
| image_area_replacement | `RegionReplacementOptions` | Informatie over vervanging van afbeeldingsgebied. |
| image_details | `str` | Tekstuele beschrijving van de afbeelding, standaard is dit een lege tekenreeks. |

### Zie ook
* class [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/)
