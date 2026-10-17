---
title: "redact_annotation メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "ドキュメント内のすべての注釈で一致するテキストを、指定されたオプションで置換します。"
type: docs
url: /ja/python-net/groupdocs.redaction.integration/ifixedformatdocument/redact_annotation/
is_root: false
weight: 1030
---


## redact_annotation {#regular_expression-options}

ドキュメント内のすべての注釈で一致するテキストを、指定されたオプションで置換します。

```python
def redact_annotation(self, regular_expression, options):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | 検索と置換に使用する正規表現。 |
| options | `ReplacementOptions` | 置換オプション。 |

**Returns:** Replacement result.

### 関連項目
* class [`IFixedFormatDocument`](/redaction/python-net/groupdocs.redaction.integration/ifixedformatdocument/)
