---
title: "is_redaction_accepted 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "检查 IRedactionCallback 实现并在指定时调用它。"
type: docs
url: /zh/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/
is_root: false
weight: 1030
---


## is_redaction_accepted {#description}

检查是否实现了[`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/)，如果指定则调用它。

```python
def is_redaction_accepted(self, description):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| description | `RedactionDescription` | 遮盖描述 |

**Returns:** bool: True (by default) if redaction is accepted.

### 另请参阅
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
