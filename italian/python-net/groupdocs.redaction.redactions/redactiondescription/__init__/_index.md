---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza una nuova istanza della classe RedactionDescription senza informazioni di sostituzione."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/
is_root: false
weight: 10
---


## __init__ {#redaction_type-action_type-original_text}

Inizializza una nuova istanza della classe RedactionDescription senza informazioni di sostituzione.

```python
def __init__(self, redaction_type, action_type, original_text):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| redaction_type | `RedactionType` | Tipo di dati da censurare. |
| action_type | `RedactionActionType` | Azione da eseguire su questi dati. |
| original_text | `str` | Testo corrispondente, commento o corpo dell'annotazione. |

## __init__ {#redaction_type-action_type-original_text-replacement}

Inizializza una nuova istanza della classe RedactionDescription con informazioni di sostituzione.

```python
def __init__(self, redaction_type, action_type, original_text, replacement):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| redaction_type | `RedactionType` | Tipo di dati da censurare. |
| action_type | `RedactionActionType` | Azione da eseguire su questi dati. |
| original_text | `str` | Testo corrispondente, commento o corpo dell'annotazione. |
| replacement | `TextReplacement` | Testo di sostituzione, testo corrispondente e la sua posizione nella stringa originale. |

## __init__ {#redaction_type-action_type-image_area_replacement-image_details}

Inizializza un nuovo RedactionDescription con informazioni di sostituzione dell'area immagine.

```python
def __init__(self, redaction_type, action_type, image_area_replacement, image_details):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| redaction_type | `RedactionType` | Tipo di dati da censurare. |
| action_type | `RedactionActionType` | Azione da eseguire su questi dati. |
| image_area_replacement | `RegionReplacementOptions` | Informazioni sulla sostituzione dell'area immagine. |
| image_details | `str` | Descrizione testuale dell'immagine, per impostazione predefinita è una stringa vuota. |

### Vedi anche
* class [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/)
