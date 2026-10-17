---
title: "accept_redaction 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "在对文档应用任何编辑之前触发，允许记录日志或阻止编辑。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/
is_root: false
weight: 1010
---


## accept_redaction {#description}

在对文档应用任何编辑之前触发，允许记录日志或阻止编辑。

```python
def accept_redaction(self, description):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| description | `RedactionDescription` | 包含有关特定匹配类型、条件、文本和位置的信息。 |

**Returns:** bool: True to accept the redaction, False to decline it.

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.redaction.options import LoadOptions, RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

with Redactor("document.docx", LoadOptions(), RedactorSettings(callback=accept)) as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    redactor.save()
```

### 另请参阅
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/)
