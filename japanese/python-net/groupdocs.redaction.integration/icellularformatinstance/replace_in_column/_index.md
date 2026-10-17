---
title: "replace_in_column メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "指定された列とワークシート内のすべての一致を、指定された置換文字列で置き換えます。"
type: docs
url: /ja/python-net/groupdocs.redaction.integration/icellularformatinstance/replace_in_column/
is_root: false
weight: 1040
---


## replace_in_column {#regular_expression-replacement-column-sheet}

指定された列とワークシート内のすべての一致を、指定された置換文字列で置き換えます。

```python
def replace_in_column(self, regular_expression, replacement, column, sheet):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | 検索と置換に使用する正規表現。 |
| replacement | `str` | テキスト置換。 |
| column | `int` | 0 ベースの列インデックス。 |
| sheet | `int` | 0 ベースのワークシートインデックス。 |

**Returns:** Replacement result.

## replace_in_column {#regular_expression-replacement-column}

すべてのワークシートの指定された列内のすべての一致を、指定された置換文字列で置き換えます。

```python
def replace_in_column(self, regular_expression, replacement, column):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | 検索と置換に使用する正規表現。 |
| replacement | `str` | テキスト置換。 |
| column | `int` | 0 ベースの列インデックス。 |

**Returns:** Replacement result.

### 関連項目
* class [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/)
