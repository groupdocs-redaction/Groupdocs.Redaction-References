---
title: "save 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "将编辑策略保存到文件。"
type: docs
url: /zh/python-net/groupdocs.redaction/redactionpolicy/save/
is_root: false
weight: 1060
---


## save {#file_path}

将编辑策略保存到文件。

```python
def save(self, file_path):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| file_path | `str` | 文件路径。 |

### 示例

```python
    policy = RedactionPolicy([
        ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
        RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
    ])
    policy.save("./sample_policy.xml")
    ```

## save {#output}

将编辑策略保存到流。

```python
def save(self, output):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| output | `io.RawIOBase` | 用于保存策略的目标流。 |

**Returns:** None.

### 另请参阅
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
