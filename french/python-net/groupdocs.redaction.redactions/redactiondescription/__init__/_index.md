---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise une nouvelle instance de la classe RedactionDescription sans informations de remplacement."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/
is_root: false
weight: 10
---


## __init__ {#redaction_type-action_type-original_text}

Initialise une nouvelle instance de la classe RedactionDescription sans informations de remplacement.

```python
def __init__(self, redaction_type, action_type, original_text):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| redaction_type | `RedactionType` | Type de données à masquer. |
| action_type | `RedactionActionType` | Action à effectuer sur ces données. |
| original_text | `str` | Texte correspondant, commentaire ou corps d'annotation. |

## __init__ {#redaction_type-action_type-original_text-replacement}

Initialise une nouvelle instance de la classe RedactionDescription avec des informations de remplacement.

```python
def __init__(self, redaction_type, action_type, original_text, replacement):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| redaction_type | `RedactionType` | Type de données à masquer. |
| action_type | `RedactionActionType` | Action à effectuer sur ces données. |
| original_text | `str` | Texte correspondant, commentaire ou corps d'annotation. |
| replacement | `TextReplacement` | Texte de remplacement, texte correspondant et sa position dans la chaîne originale. |

## __init__ {#redaction_type-action_type-image_area_replacement-image_details}

Initialise un nouveau RedactionDescription avec des informations de remplacement de zone d'image.

```python
def __init__(self, redaction_type, action_type, image_area_replacement, image_details):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| redaction_type | `RedactionType` | Type de données à masquer. |
| action_type | `RedactionActionType` | Action à effectuer sur ces données. |
| image_area_replacement | `RegionReplacementOptions` | Informations de remplacement de zone d'image. |
| image_details | `str` | Description textuelle de l'image, par défaut c'est une chaîne vide. |

### Voir aussi
* class [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/)
