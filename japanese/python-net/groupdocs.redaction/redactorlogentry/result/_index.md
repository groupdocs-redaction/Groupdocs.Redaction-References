---
title: "result プロパティ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "DocumentFormatInstance によって返される結果。"
type: docs
url: /ja/python-net/groupdocs.redaction/redactorlogentry/result/
is_root: false
weight: 2020
---


## result property

[`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) が返す結果です。

すべてのメタデータのマスクは各メタデータ項目に個別に適用され、メタデータ項目のマスクが失敗した場合でも、残りのメタデータ項目は更新されます。失敗した、スキップされた（拒否された）メタデータ項目とその理由の一覧は、`ErrorMessage` プロパティの [`RedactorLogEntry.Result`](/redaction/python-net/groupdocs.redaction/redactorlogentry/result/) にあります。

### Definition:
```python
@property
def result(self):
    ...
```

### 関連項目
* class [`RedactorLogEntry`](/redaction/python-net/groupdocs.redaction/redactorlogentry/)
