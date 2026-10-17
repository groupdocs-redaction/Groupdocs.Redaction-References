---
title: "RemovePageRedaction 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "表示一种从文档中删除页面（幻灯片、工作表等）的编辑。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/removepageredaction/
is_root: false
weight: 250
---


## RemovePageRedaction class

表示一种从文档中删除页面（幻灯片、工作表等）的编辑。

了解更多
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about removing pages: https://docs.groupdocs.com/redaction/net/remove-page-redaction/

RemovePageRedaction 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/#origin-index-count) | 初始化一个新的 RemovePageRedaction。 |

### 方法
| 方法 | 描述 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to/#format_instance) | 将 redaction 应用于给定的格式实例。 |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to_document_format_instance/) |  |

### 属性
| 属性 | 描述 |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/count/) | 要删除的页面数量。 |
| [index](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/index/) | 起始位置索引（从0开始）。 |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/origin/) | 查找参考位置，可为文档的开头或结尾。 |
| [description](/redaction/python-net/groupdocs.redaction/redaction/description/) | 编辑的描述，包含其名称和参数。(继承自 [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)) |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # 从文档末尾计数删除 1 页
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    with Redactor("./test.pdf") as redactor:
        # 应用编辑
        result = redactor.apply(rem_opt)

        # 保存已遮蔽的文档
        so = SaveOptions()
        so.add_suffix = True
        redactor.save(so)
```

### Guides
使用 `RemovePageRedaction` 的任务指南：

* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)

### 另请参阅
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
