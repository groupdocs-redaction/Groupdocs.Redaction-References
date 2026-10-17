---
title: "AnnotationRedaction 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "表示一种编辑，它用给定正则表达式匹配的内容替换注释文本（评论等）。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/annotationredaction/
is_root: false
weight: 10
---


## AnnotationRedaction class

表示一种编辑，它用给定正则表达式匹配的内容替换注释文本（评论等）。

了解更多

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

AnnotationRedaction 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#pattern-replacement) | 使用正则表达式模式和替换文本初始化新的 AnnotationRedaction。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#regex-replacement) | 初始化 [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) 的新实例。 |

### 方法
| 方法 | 描述 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to/#format_instance) | 将 redaction 应用于给定的格式实例。 |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to_document_format_instance/) |  |

### 属性
| 属性 | 描述 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/description/) | 遮蔽的描述，说明遮蔽及其参数。 |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/expression/) | 用于匹配的正则表达式。 |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/replacement/) | 匹配文本的文字替换。 |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import AnnotationRedaction

with Redactor("document.pdf") as redactor:
    redactor.apply(AnnotationRedaction("(?i)approved", "[REVIEW]"))
    redactor.save()
```

### Guides
使用 `AnnotationRedaction` 的任务指南：

* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)

### 另请参阅
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
