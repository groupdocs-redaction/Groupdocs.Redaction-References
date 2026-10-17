---
title: "result 属性"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "DocumentFormatInstance 返回的 result。"
type: docs
url: /zh/python-net/groupdocs.redaction/redactorlogentry/result/
is_root: false
weight: 2020
---


## result property

由 [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) 返回的结果。

所有元数据脱敏都会分别应用于每个元数据项，即使某个元数据项的脱敏失败，其他元数据项仍会被更新。您可以在 [`RedactorLogEntry.Result`](/redaction/python-net/groupdocs.redaction/redactorlogentry/result/) 的 `ErrorMessage` 属性中找到失败、已跳过（被拒绝）的元数据项列表及其原因。

### Definition:
```python
@property
def result(self):
    ...
```

### 另请参阅
* class [`RedactorLogEntry`](/redaction/python-net/groupdocs.redaction/redactorlogentry/)
