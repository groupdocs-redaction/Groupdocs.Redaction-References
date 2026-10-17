---
title: "remove_pages メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "開始位置、オフセット、カウントに応じて、1ページまたは複数ページを削除します。"
type: docs
url: /ja/python-net/groupdocs.redaction.integration/ipaginateddocument/remove_pages/
is_root: false
weight: 1010
---


## remove_pages {#origin-index-count}

開始位置、オフセット、カウントに応じて、1ページまたは複数ページを削除します。

```python
def remove_pages(self, origin, index, count):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| origin | `PageSeekOrigin` | 検索の起点位置、ドキュメントの先頭または末尾。 |
| index | `int` | 開始位置インデックス（0 ベース）。 |
| count | `int` | 削除するページ数。 |

**Returns:** Pages removal redaction result.

### 関連項目
* class [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/)
