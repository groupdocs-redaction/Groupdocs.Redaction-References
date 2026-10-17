---
title: "Classe PreviewOptions"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Fornisce opzioni per impostare requisiti e delegati di stream per la generazione dell'anteprima."
type: docs
url: /it/python-net/groupdocs.redaction.options/previewoptions/
is_root: false
weight: 70
---


## PreviewOptions class

Fornisce opzioni per impostare requisiti e delegati di stream per la generazione dell'anteprima.

La classe consente di specificare il formato di anteprima, le dimensioni dell'immagine, i numeri di pagina e i delegati che creano e opzionalmente rilasciano i flussi per ogni pagina generata.

Il tipo PreviewOptions espone i seguenti membri:

### Costruttori
| Costruttore | Descrizione |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream) | Inizializza una nuova istanza di PreviewOptions. Il flusso di output verrà chiuso dopo l'uso. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream-release_page_stream) | Inizializza una nuova istanza di PreviewOptions, facendo sì che il flusso di output venga restituito al client per un uso successivo. |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [create_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/create_page_stream/) | Il delegato per la creazione del flusso della pagina. |
| [height](/redaction/python-net/groupdocs.redaction.options/previewoptions/height/) | L'altezza dell'anteprima della pagina. |
| [page_numbers](/redaction/python-net/groupdocs.redaction.options/previewoptions/page_numbers/) | I numeri di pagina per generare l'anteprima. |
| [preview_format](/redaction/python-net/groupdocs.redaction.options/previewoptions/preview_format/) | Il formato dell'immagine di anteprima. |
| [release_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/release_page_stream/) | Il delegato per il completamento dell'anteprima della pagina. |
| [width](/redaction/python-net/groupdocs.redaction.options/previewoptions/width/) | La larghezza dell'anteprima della pagina. |

### Esempio

```python
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int):
    # Crea un file per l'immagine di anteprima della pagina specificata
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")  # returns a writable binary stream

preview_options = PreviewOptions(create_page_stream)
preview_options.preview_format = PreviewOptions.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### Vedi anche
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
