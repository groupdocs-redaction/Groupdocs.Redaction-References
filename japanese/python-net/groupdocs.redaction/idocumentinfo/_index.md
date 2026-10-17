---
title: "IDocumentInfo クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "基本的なドキュメント情報を取得するために必要なメソッドを提供します。"
type: docs
url: /ja/python-net/groupdocs.redaction/idocumentinfo/
is_root: false
weight: 50
---


## IDocumentInfo class

基本的なドキュメント情報を取得するために必要なメソッドを提供します。

詳細はこちら: ファイル情報の取得 (https://docs.groupdocs.com/redaction/net/get-file-info/)。

IDocumentInfo 型は次のメンバーを公開します：

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [file_type](/redaction/python-net/groupdocs.redaction/idocumentinfo/file_type/) | ファイル形式の説明です。 |
| [page_count](/redaction/python-net/groupdocs.redaction/idocumentinfo/page_count/) | 総ページ数です。 |
| [pages](/redaction/python-net/groupdocs.redaction/idocumentinfo/pages/) | ページ情報を表す [`PageInfo`](/redaction/python-net/groupdocs.redaction/pageinfo/) オブジェクトのリストです。 |
| [size](/redaction/python-net/groupdocs.redaction/idocumentinfo/size/) | ドキュメントのサイズ（バイト単位）です。 |

### 例

```python
from groupdocs.redaction import Redactor

with Redactor("document.pdf") as redactor:
    info = redactor.get_document_info()
    print(info.file_type.file_format, info.page_count, info.size)
    for page in info.pages:
        print(f"Page {page.page_number} size is {page.width}x{page.height}")
```

### 関連項目
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
