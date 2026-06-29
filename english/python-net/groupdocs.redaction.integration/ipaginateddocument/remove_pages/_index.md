---
title: remove_pages method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Removes one or multiple pages depending on its start position, offset and count."
type: docs
url: /python-net/groupdocs.redaction.integration/ipaginateddocument/remove_pages/
is_root: false
weight: 1010
---


## remove_pages {#origin-index-count}

Removes one or multiple pages depending on its start position, offset and count.

```python
def remove_pages(self, origin, index, count):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Search origin position, the beginning or the end of the document. |
| index | `int` | Start position index (0-based). |
| count | `int` | Count of pages to remove. |

**Returns:** Pages removal redaction result.

### See Also
* class [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/)
