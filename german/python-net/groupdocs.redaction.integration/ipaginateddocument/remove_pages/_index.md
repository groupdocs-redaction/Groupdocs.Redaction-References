---
title: "remove_pages Methode"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Entfernt eine oder mehrere Seiten abhängig von ihrer Startposition, dem Versatz und der Anzahl."
type: docs
url: /de/python-net/groupdocs.redaction.integration/ipaginateddocument/remove_pages/
is_root: false
weight: 1010
---


## remove_pages {#origin-index-count}

Entfernt eine oder mehrere Seiten abhängig von ihrer Startposition, dem Versatz und der Anzahl.

```python
def remove_pages(self, origin, index, count):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Suchursprungsposition, der Anfang oder das Ende des Dokuments. |
| index | `int` | Startpositionsindex (0-basiert). |
| count | `int` | Anzahl der zu entfernenden Seiten. |

**Returns:** Pages removal redaction result.

### Siehe auch
* class [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/)
