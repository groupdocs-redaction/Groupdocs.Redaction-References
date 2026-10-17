---
title: "perform_binary_check メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "指定されたストリームがこの形式インスタンスでサポートされるドキュメントを含んでいるか確認します。"
type: docs
url: /ja/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/
is_root: false
weight: 1080
---


## perform_binary_check {#input}

指定されたストリームがこの形式インスタンスでサポートされるドキュメントを含んでいるか確認します。

```python
def perform_binary_check(self, input):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| input | `io.RawIOBase` | ドキュメントコンテンツのストリーム。 |

**Returns:** bool: True if the document can be loaded by this format instance, False otherwise.

### 関連項目
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
