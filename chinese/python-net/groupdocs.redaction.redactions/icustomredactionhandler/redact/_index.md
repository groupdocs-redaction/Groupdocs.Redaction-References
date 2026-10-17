---
title: "脱敏方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "对特定文档内容应用自定义编辑。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
is_root: false
weight: 1010
---


## redact {#context}

对特定文档内容应用自定义编辑。

目前，仅在 PDF 中支持 [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/)。

用户可以定义自己的脱敏逻辑，例如基于 AI 的脱敏，这可能比简单的基于模式的方法更高级。

```python
def redact(self, context):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| context | `CustomRedactionContext` | 包含要脱敏的文档内容以及相关元数据。 |

**Returns:** CustomRedactionResult: Indicates whether the redaction should be applied and the modified content.

### 另请参阅
* class [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/)
