---
title: "Classe RegionReplacementOptions"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Rappresenta i parametri di colore e area per la sostituzione di una regione immagine."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/regionreplacementoptions/
is_root: false
weight: 240
---


## RegionReplacementOptions class

Rappresenta i parametri di colore e area per la sostituzione di una regione immagine.

Per saperne di più:
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

Il tipo RegionReplacementOptions espone i seguenti membri:

### Costruttori
| Costruttore | Descrizione |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-size) | Inizializza una nuova istanza di RegionReplacementOptions. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-font-expected_text) | Inizializza una nuova istanza della classe RegionReplacementOptions la cui dimensione corrisponde al testo fornito. |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [fill_color](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/fill_color/) | Il colore usato per riempire l'area redatta. |
| [size](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/size/) | La larghezza e l'altezza del rettangolo. |

### Esempio

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

with Redactor("test.jpg") as redactor:
    # Definisci la posizione in alto‑a‑sinistra dell'area da sostituire
    point = Point(516, 311)
    # Definisci la dimensione dell'area da sostituire
    size = Size(170, 35)
    # Usa un rettangolo nero solido come sostituzione
    repl_opt = RegionReplacementOptions(Color.BLACK, size)
    redaction = ImageAreaRedaction(point, repl_opt)

    result = redactor.apply(redaction)
    if result.status != redactor.RedactionStatus.FAILED:
        redactor.save()
```

### Guides
Guide operative che utilizzano `RegionReplacementOptions`:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### Vedi anche
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
