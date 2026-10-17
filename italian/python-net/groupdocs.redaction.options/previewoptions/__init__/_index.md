---
title: "costruttore __init__"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizializza una nuova istanza di PreviewOptions."
type: docs
url: /it/python-net/groupdocs.redaction.options/previewoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#create_page_stream}

Inizializza una nuova istanza di PreviewOptions. Il flusso di output verrà chiuso dopo l'uso.

```python
def __init__(self, create_page_stream):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Crea uno stream per un'anteprima di pagina specifica. |

## __init__ {#create_page_stream-release_page_stream}

Inizializza una nuova istanza di PreviewOptions, facendo sì che il flusso di output venga restituito al client per un uso successivo.

```python
def __init__(self, create_page_stream, release_page_stream):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Crea uno stream per un'anteprima di pagina specifica. |
| release_page_stream | `ReleasePageStream` | Notifica che la generazione dell'anteprima di pagina è completata e ottiene lo stream di output. |

### Vedi anche
* class [`PreviewOptions`](/redaction/python-net/groupdocs.redaction.options/previewoptions/)
