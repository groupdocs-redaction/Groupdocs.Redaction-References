---
title: "redact_annotation メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "ドキュメント内のすべての注釈で一致するテキストを置換します。"
type: docs
url: /ja/python-net/groupdocs.redaction.integration/iannotateddocument/redact_annotation/
is_root: false
weight: 1030
---


## redact_annotation {#regular_expression-replacement}

ドキュメント内のすべての注釈で一致するテキストを置換します。

```python
def redact_annotation(self, regular_expression, replacement):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | 検索と置換に使用する正規表現。 |
| replacement | `str` | テキスト置換。 |

**Returns:** Replacement result.

### 関連項目
* class [`IAnnotatedDocument`](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/)
