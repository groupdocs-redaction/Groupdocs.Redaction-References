---
title: "__init__ constructeur"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Initialise une nouvelle instance de PreviewOptions."
type: docs
url: /fr/python-net/groupdocs.redaction.options/previewoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#create_page_stream}

Initialise une nouvelle instance de PreviewOptions. Le flux de sortie sera fermé après utilisation.

```python
def __init__(self, create_page_stream):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Crée un flux pour un aperçu de page spécifique. |

## __init__ {#create_page_stream-release_page_stream}

Initialise une nouvelle instance de PreviewOptions, faisant en sorte que le flux de sortie soit renvoyé au client pour une utilisation ultérieure.

```python
def __init__(self, create_page_stream, release_page_stream):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Crée un flux pour un aperçu de page spécifique. |
| release_page_stream | `ReleasePageStream` | Notifie que la génération de l'aperçu de page est terminée et récupère le flux de sortie. |

### Voir aussi
* class [`PreviewOptions`](/redaction/python-net/groupdocs.redaction.options/previewoptions/)
