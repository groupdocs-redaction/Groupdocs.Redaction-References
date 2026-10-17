---
title: "load 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "从 XML 文件加载 RedactionPolicy。"
type: docs
url: /zh/python-net/groupdocs.redaction/redactionpolicy/load/
is_root: false
weight: 1010
---


## load {#file_path}

从 XML 文件加载 RedactionPolicy。

```python
def load(cls, file_path):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| file_path | `str` | XML 文件的路径。 |

**Returns:** RedactionPolicy: The loaded redaction policy.

### 示例

```python
from groupdocs.redaction import RedactionPolicy, Redactor

policy = RedactionPolicy.load("RedactionPolicy.xml")

with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

## load {#input}

从包含 XML 配置的流加载 RedactionPolicy 实例。

```python
def load(cls, input):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| input | `io.RawIOBase` | 包含 XML 配置的流。 |

**Returns:** RedactionPolicy: The loaded redaction policy.

### 示例

```python
from groupdocs.redaction import RedactionPolicy, Redactor

# 从 XML 文件加载策略
with open("policy.xml", "rb") as stream:
    policy = RedactionPolicy.load(stream)

# 将策略应用于文档
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### 另请参阅
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
