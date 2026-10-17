---
title: "__init__ Konstruktor"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Initialisiert eine neue PreviewOptions-Instanz."
type: docs
url: /de/python-net/groupdocs.redaction.options/previewoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#create_page_stream}

Initialisiert eine neue PreviewOptions-Instanz. Der Ausgabestream wird nach der Verwendung geschlossen.

```python
def __init__(self, create_page_stream):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Erstellt einen Stream für eine bestimmte Seitenvorschau. |

## __init__ {#create_page_stream-release_page_stream}

Initialisiert eine neue PreviewOptions-Instanz, wodurch der Ausgabestream dem Client für weitere Verwendung zurückgegeben wird.

```python
def __init__(self, create_page_stream, release_page_stream):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Erstellt einen Stream für eine bestimmte Seitenvorschau. |
| release_page_stream | `ReleasePageStream` | Benachrichtigt, dass die Generierung der Seitenvorschau abgeschlossen ist, und gibt den Ausgabestream zurück. |

### Siehe auch
* class [`PreviewOptions`](/redaction/python-net/groupdocs.redaction.options/previewoptions/)
