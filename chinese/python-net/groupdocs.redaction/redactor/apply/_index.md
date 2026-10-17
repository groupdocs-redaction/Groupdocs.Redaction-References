---
title: "应用方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "对文档应用一次编辑。"
type: docs
url: /zh/python-net/groupdocs.redaction/redactor/apply/
is_root: false
weight: 1010
---


## apply {#redaction}

对文档应用一次编辑。

```python
def apply(self, redaction):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| redaction | `Redaction` | 要应用的 `Redaction` 实例。 |

**Returns:** RedactorChangeLog: Indicates success or failure and includes an error message when the operation fails.

### 示例

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

def apply_redaction():
    # 定义用于替换 SSN 模式的 redaction
    ssn_redaction = RegexRedaction(r"\b\d{3}-\d{2}-\d{4}\b", ReplacementOptions("[ssn]"))

    # 加载文档并应用 redaction
    with Redactor("./test.docx") as redactor:
        result = redactor.apply(ssn_redaction)

        if result.status != RedactionStatus.FAILED:
            redactor.save()
```

## apply {#redactions}

对文档应用一组编辑。

```python
def apply(self, redactions):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| redactions | `list[Redaction]` | 要应用的 redaction 数组。 |

**Returns:** RedactorChangeLog: Indicates success or failure and contains an error message if applicable.

### 示例

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    RegexRedaction,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataSearchRedaction,
    ReplacementOptions,
)
from groupdocs.redaction.metadata import MetadataFilter

redaction_list = [
    ExactPhraseRedaction("ClientName", ReplacementOptions("[client]")),
    ExactPhraseRedaction("ClientAddress", ReplacementOptions("[address]")),
    RegexRedaction(r"\d{3}-\d{2}-\d{4}", ReplacementOptions("[ssn]")),
    RegexRedaction(r"\d{16}", ReplacementOptions("[card]")),
    DeleteAnnotationRedaction(r"(?im:(use|show|describe))"),
    EraseMetadataRedaction(MetadataFilter.Author),
    MetadataSearchRedaction("CompanyName", "--company--"),
]

with Redactor("./test.docx") as redactor:
    result = redactor.apply(redaction_list)
    if result.status != RedactionStatus.FAILED:
        redactor.save()
```

## apply {#policy}

对文档应用编辑策略。

```python
def apply(self, policy):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| policy | `RedactionPolicy` | Redaction 策略。 |

**Returns:** `RedactorChangeLog`: Indicates success or failure and contains an error message if the operation failed.

### 示例

```python
import os
from groupdocs.redaction import Redactor, RedactionPolicy, RedactionStatus
from groupdocs.redaction.options import RasterizationOptions

policy = RedactionPolicy.load("RedactionPolicy.xml")
for file_name in os.listdir(r"C:\Inbound"):
    file_path = os.path.join(r"C:\Inbound", file_name)
    with Redactor(file_path) as redactor:
        result = redactor.apply(policy)
        out_folder = (
            r"C:\Outbound\Done"
            if result.status != RedactionStatus.FAILED
            else r"C:\Outbound\Failed"
        )
        out_path = os.path.join(out_folder, file_name)
        with open(out_path, "r+b") as stream:
            redactor.save(stream, RasterizationOptions(enabled=False))
```

### 另请参阅
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
