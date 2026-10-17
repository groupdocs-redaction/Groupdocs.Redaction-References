---
title: "PageRangeFilter クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "ドキュメント内のページ範囲を設定し、赤字を適用する赤字フィルターを表します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/pagerangefilter/
is_root: false
weight: 170
---


## PageRangeFilter class

ドキュメント内のページ範囲を設定し、赤字を適用する赤字フィルターを表します。

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

PageRangeFilter 型は次のメンバーを公開します:

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/__init__/#origin-index-count) | 新しい RemovePageRedaction を初期化します。 |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/count/) | 削除するページ数です。 |
| [index](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/index/) | 開始位置インデックス（0 ベース）です。 |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/origin/) | シーク参照位置で、ドキュメントの先頭または末尾のいずれかです。 |

### 例

```python
from groupdocs.redaction.redactions import PageRangeFilter, PageSeekOrigin

# 最後のページとその前のページを対象とするフィルタを定義します
page_filter = PageRangeFilter(PageSeekOrigin.END, 0, 1)

# このフィルタは他のフィルタと組み合わせることができます。例: PageAreaFilter、
# リダクションを構成する際に ReplacementOptions.Filters に渡されます。
```

### 関連項目
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
