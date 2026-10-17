---
title: "remove_pages 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "根据起始位置、偏移量和计数删除一个或多个页面。"
type: docs
url: /zh/python-net/groupdocs.redaction.integration/ipaginateddocument/remove_pages/
is_root: false
weight: 1010
---


## remove_pages {#origin-index-count}

根据起始位置、偏移量和计数删除一个或多个页面。

```python
def remove_pages(self, origin, index, count):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| origin | `PageSeekOrigin` | 搜索起始位置，文档的开头或结尾。 |
| index | `int` | 起始位置索引（从 0 开始）。 |
| count | `int` | 要删除的页数。 |

**Returns:** Pages removal redaction result.

### 另请参阅
* class [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/)
