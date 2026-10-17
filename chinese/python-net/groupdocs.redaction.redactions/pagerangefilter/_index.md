---
title: "PageRangeFilter 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "表示编辑过滤器，设置文档内部的页码范围以应用编辑。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/pagerangefilter/
is_root: false
weight: 170
---


## PageRangeFilter class

表示编辑过滤器，设置文档内部的页码范围以应用编辑。

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

该 PageRangeFilter 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/__init__/#origin-index-count) | 初始化一个新的 RemovePageRedaction。 |

### 属性
| 属性 | 描述 |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/count/) | 要删除的页面数量。 |
| [index](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/index/) | 起始位置索引（从0开始）。 |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/origin/) | 查找参考位置，可为文档的开头或结尾。 |

### 示例

```python
from groupdocs.redaction.redactions import PageRangeFilter, PageSeekOrigin

# 定义一个针对最后一页及其前一页的过滤器
page_filter = PageRangeFilter(PageSeekOrigin.END, 0, 1)

# 该过滤器可以与其他过滤器组合，例如 PageAreaFilter，
# 并在配置编辑时传递给 ReplacementOptions.Filters。
```

### 另请参阅
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
