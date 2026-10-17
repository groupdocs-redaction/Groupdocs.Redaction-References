---
title: "__init__ konstruktor"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Initierar en ny PreviewOptions-instans."
type: docs
url: /sv/python-net/groupdocs.redaction.options/previewoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#create_page_stream}

Initierar en ny PreviewOptions-instans. Utdataströmmen kommer att stängas efter användning.

```python
def __init__(self, create_page_stream):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Skapar en ström för en specifik sidoförhandsgranskning. |

## __init__ {#create_page_stream-release_page_stream}

Initierar en ny PreviewOptions-instans, vilket gör att utdataströmmen returneras till klienten för vidare användning.

```python
def __init__(self, create_page_stream, release_page_stream):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Skapar en ström för en specifik sidoförhandsgranskning. |
| release_page_stream | `ReleasePageStream` | Meddelar att genereringen av sidoförhandsgranskning är klar och hämtar utdataström. |

### Se även
* class [`PreviewOptions`](/redaction/python-net/groupdocs.redaction.options/previewoptions/)
