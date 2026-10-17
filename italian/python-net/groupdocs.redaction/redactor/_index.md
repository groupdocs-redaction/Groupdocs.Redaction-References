---
title: "Classe Redactor"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Rappresenta la classe principale che controlla il processo di redazione dei documenti, consentendo di aprire, redigere e salvare i documenti."
type: docs
url: /it/python-net/groupdocs.redaction/redactor/
is_root: false
weight: 150
---


## Redactor class

Rappresenta la classe principale che controlla il processo di redazione dei documenti, consentendo di aprire, redigere e salvare i documenti.

Per saperne di più
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More advanced redaction topics: https://docs.groupdocs.com/redaction/net/advanced-usage/

Il tipo Redactor espone i seguenti membri:

### Costruttori
| Costruttore | Descrizione |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path) | Inizializza una nuova istanza di Redactor utilizzando un percorso file. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document) | Inizializza una nuova istanza di [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) utilizzando uno stream. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options) | Inizializza una nuova istanza di [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) per un documento protetto da password utilizzando il suo percorso. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options-settings) | Inizializza una nuova istanza di Redactor per un documento protetto da password utilizzando il suo percorso e le impostazioni. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options) | Inizializza una nuova istanza di Redactor per un documento protetto da password utilizzando uno stream. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options-settings) | Inizializza una nuova istanza di [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) per un documento protetto da password utilizzando uno stream e le impostazioni. |

### Metodi
| Metodo | Descrizione |
| :- | :- |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redaction) | Applica una redazione al documento. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redactions) | Applica un insieme di redazioni al documento. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#policy) | Applica una politica di redazione al documento. |
| [apply_redaction](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction/) |  |
| [apply_redaction_policy](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction_policy/) |  |
| [dispose](/redaction/python-net/groupdocs.redaction/redactor/dispose/) | Rilascia le risorse. |
| [generate_preview](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#preview_options) | Genera immagini di anteprima di pagine specifiche in un formato immagine specificato. |
| [generate_preview_preview_options](/redaction/python-net/groupdocs.redaction/redactor/generate_preview_preview_options/) |  |
| [get_document_info](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/) | Recupera le informazioni generali sul documento, come dimensione e numero di pagine. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/) | Salva il documento su un file con le seguenti opzioni: AddSuffix = True, RasterizeToPDF = True. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#save_options) | Salva il documento su un file. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#document-rasterization_options) | Salva il documento su uno stream, includendo una posizione personalizzata. |
| [save_save_options](/redaction/python-net/groupdocs.redaction/redactor/save_save_options/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactor/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactor/save_streams/) |  |

### Esempio

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Apri un documento e rimuovi la prima pagina
with Redactor("document.pdf") as redactor:
    redactor.apply(RemovePageRedaction(PageSeekOrigin.BEGIN, 0, 1))
    redactor.save()
```

### Guides
Guide operative che utilizzano `Redactor`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [Get file info](/redaction/python-net/guides/get-file-info/)

### Vedi anche
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
