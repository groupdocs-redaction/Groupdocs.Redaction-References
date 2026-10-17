---
title: "redact メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "特定のドキュメント コンテンツにカスタム削除を適用します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
is_root: false
weight: 1010
---


## redact {#context}

特定のドキュメント コンテンツにカスタム削除を適用します。

現在、これは PDF のみでサポートされています [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/).

ユーザーは独自の赤字化ロジック（例として AI ベースの赤字化）を定義でき、単純なパターンベースの手法よりも高度になる可能性があります。

```python
def redact(self, context):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| context | `CustomRedactionContext` | 赤字化対象の文書コンテンツと関連メタデータを含みます。 |

**Returns:** CustomRedactionResult: Indicates whether the redaction should be applied and the modified content.

### 関連項目
* class [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/)
