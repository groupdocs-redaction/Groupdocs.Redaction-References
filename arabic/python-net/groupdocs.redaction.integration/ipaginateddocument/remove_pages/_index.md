---
title: "طريقة remove_pages"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يزيل صفحة واحدة أو عدة صفحات اعتمادًا على موضع البداية والإزاحة والعدد."
type: docs
url: /ar/python-net/groupdocs.redaction.integration/ipaginateddocument/remove_pages/
is_root: false
weight: 1010
---


## remove_pages {#origin-index-count}

يزيل صفحة واحدة أو عدة صفحات اعتمادًا على موضع البداية والإزاحة والعدد.

```python
def remove_pages(self, origin, index, count):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| origin | `PageSeekOrigin` | موضع أصل البحث، بداية أو نهاية المستند. |
| index | `int` | فهرس موضع البداية (بدءًا من الصفر). |
| count | `int` | عدد الصفحات التي سيتم إزالتها. |

**Returns:** Pages removal redaction result.

### انظر أيضًا
* class [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/)
