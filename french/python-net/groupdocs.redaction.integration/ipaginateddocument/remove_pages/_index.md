---
title: "méthode remove_pages"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Supprime une ou plusieurs pages en fonction de sa position de départ, de son décalage et de son nombre."
type: docs
url: /fr/python-net/groupdocs.redaction.integration/ipaginateddocument/remove_pages/
is_root: false
weight: 1010
---


## remove_pages {#origin-index-count}

Supprime une ou plusieurs pages en fonction de sa position de départ, de son décalage et de son nombre.

```python
def remove_pages(self, origin, index, count):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Position d'origine de recherche, le début ou la fin du document. |
| index | `int` | Indice de position de départ (base 0). |
| count | `int` | Nombre de pages à supprimer. |

**Returns:** Pages removal redaction result.

### Voir aussi
* class [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/)
