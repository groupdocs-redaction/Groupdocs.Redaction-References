---
title: "PageAreaFilter 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "表示编辑过滤器，设置文档页面内的区域以应用编辑。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/pageareafilter/
is_root: false
weight: 150
---


## PageAreaFilter class

表示编辑过滤器，设置文档页面内的区域以应用编辑。

了解更多

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

PageAreaFilter 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/#top_left-size) | 初始化一个用于遮蔽特定区域的新 PageAreaFilter。 |

### 属性
| 属性 | 描述 |
| :- | :- |
| [rectangle](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/rectangle/) | 页面上的矩形（区域的左上位置和大小）。 |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

with Redactor("doc.pdf") as redactor:
    page = redactor.get_document_info().pages[0]
    area_filter = PageAreaFilter(
        Point(0, int(page.height / 2)),
        Size(page.width, int(page.height / 2))
    )
```

### 另请参阅
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
