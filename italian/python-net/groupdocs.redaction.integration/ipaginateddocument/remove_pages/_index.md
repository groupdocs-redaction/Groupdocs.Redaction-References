---
title: "metodo remove_pages"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Rimuove una o più pagine a seconda della posizione iniziale, dell'offset e del conteggio."
type: docs
url: /it/python-net/groupdocs.redaction.integration/ipaginateddocument/remove_pages/
is_root: false
weight: 1010
---


## remove_pages {#origin-index-count}

Rimuove una o più pagine a seconda della posizione iniziale, dell'offset e del conteggio.

```python
def remove_pages(self, origin, index, count):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Posizione di origine della ricerca, l'inizio o la fine del documento. |
| index | `int` | Indice della posizione di partenza (basato su zero). |
| count | `int` | Numero di pagine da rimuovere. |

**Returns:** Pages removal redaction result.

### Vedi anche
* class [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/)
