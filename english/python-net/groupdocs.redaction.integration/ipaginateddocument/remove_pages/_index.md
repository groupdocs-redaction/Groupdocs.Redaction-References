---
title: remove_pages method
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.integration/ipaginateddocument/remove_pages/
is_root: false
weight: 20
---

## remove_pages {#groupdocs.redaction.redactions.PageSeekOrigin-int-int}

Removes one or multiple pages depending on its start position, offset and count.


### Returns 


Pages removal redaction result


```python
def remove_pages(self, origin, index, count):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| origin | groupdocs.redaction.redactions.PageSeekOrigin | Search origin position, the beginning or the end of the document |
| index | int | Start position index (0-based) |
| count | int | Count of pages to remove |



### See Also
* module [`groupdocs.redaction.integration`](../../)
* class [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument)
