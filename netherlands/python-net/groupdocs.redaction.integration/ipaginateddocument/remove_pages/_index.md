---
title: "remove_pages methode"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Verwijdert één of meerdere pagina's afhankelijk van de startpositie, offset en aantal."
type: docs
url: /nl/python-net/groupdocs.redaction.integration/ipaginateddocument/remove_pages/
is_root: false
weight: 1010
---


## remove_pages {#origin-index-count}

Verwijdert één of meerdere pagina's afhankelijk van de startpositie, offset en aantal.

```python
def remove_pages(self, origin, index, count):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Zoek de oorsprongpositie, het begin of het einde van het document. |
| index | `int` | Startpositie-index (0-gebaseerd). |
| count | `int` | Aantal te verwijderen pagina's. |

**Returns:** Pages removal redaction result.

### Zie ook
* class [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/)
