---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert eine neue Instanz der Klasse RedactionDescription ohne Ersetzungsinformationen."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/
is_root: false
weight: 10
---


## __init__ {#redaction_type-action_type-original_text}

Initialisiert eine neue Instanz der Klasse RedactionDescription ohne Ersetzungsinformationen.

```python
def __init__(self, redaction_type, action_type, original_text):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| redaction_type | `RedactionType` | Typ der zu redigierten Daten. |
| action_type | `RedactionActionType` | Aktion, die an diesen Daten ausgeführt werden soll. |
| original_text | `str` | Gefundener Text, Kommentar oder Anmerkungsinhalt. |

## __init__ {#redaction_type-action_type-original_text-replacement}

Initialisiert eine neue Instanz der Klasse RedactionDescription mit Ersetzungsinformationen.

```python
def __init__(self, redaction_type, action_type, original_text, replacement):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| redaction_type | `RedactionType` | Typ der zu redigierten Daten. |
| action_type | `RedactionActionType` | Aktion, die an diesen Daten ausgeführt werden soll. |
| original_text | `str` | Gefundener Text, Kommentar oder Anmerkungsinhalt. |
| replacement | `TextReplacement` | Ersetzungstext, gefundener Text und dessen Position im Originalstring. |

## __init__ {#redaction_type-action_type-image_area_replacement-image_details}

Initialisiert ein neues RedactionDescription mit Bildbereich-Ersetzungsinformationen.

```python
def __init__(self, redaction_type, action_type, image_area_replacement, image_details):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| redaction_type | `RedactionType` | Typ der zu redigierten Daten. |
| action_type | `RedactionActionType` | Aktion, die an diesen Daten ausgeführt werden soll. |
| image_area_replacement | `RegionReplacementOptions` | Informationen zum Bildbereichs-Ersatz. |
| image_details | `str` | Bildtextbeschreibung, standardmäßig ist sie eine leere Zeichenkette. |

### Siehe auch
* class [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/)
