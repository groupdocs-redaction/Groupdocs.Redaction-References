---
title: "remove_pages metod"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Tar bort en eller flera sidor beroende på dess startposition, offset och antal."
type: docs
url: /sv/python-net/groupdocs.redaction.integration/ipaginateddocument/remove_pages/
is_root: false
weight: 1010
---


## remove_pages {#origin-index-count}

Tar bort en eller flera sidor beroende på dess startposition, offset och antal.

```python
def remove_pages(self, origin, index, count):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Sök ursprungsposition, början eller slutet av dokumentet. |
| index | `int` | Startpositionsindex (0-baserat). |
| count | `int` | Antal sidor att ta bort. |

**Returns:** Pages removal redaction result.

### Se även
* class [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/)
