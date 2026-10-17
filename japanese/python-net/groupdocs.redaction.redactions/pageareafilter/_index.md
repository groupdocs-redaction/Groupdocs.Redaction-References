---
title: "PageAreaFilter クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "ドキュメントのページ内の領域を設定し、赤字を適用する赤字フィルターを表します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/pageareafilter/
is_root: false
weight: 150
---


## PageAreaFilter class

ドキュメントのページ内の領域を設定し、赤字を適用する赤字フィルターを表します。

詳細を見る

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

PageAreaFilter 型は次のメンバーを公開します:

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/#top_left-size) | 特定の領域を編集するための新しい PageAreaFilter を初期化します。 |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [rectangle](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/rectangle/) | ページ上の矩形（領域の左上位置とサイズ）。 |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

with Redactor("doc.pdf") as redactor:
    page = redactor.get_document_info().pages[0]
    area_filter = PageAreaFilter(
        Point(0, int(page.height / 2)),
        Size(page.width, int(page.height / 2))
    )
```

### 関連項目
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
