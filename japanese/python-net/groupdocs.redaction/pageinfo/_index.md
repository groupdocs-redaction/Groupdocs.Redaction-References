---
title: "PageInfo クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "簡潔なページ情報を表します。"
type: docs
url: /ja/python-net/groupdocs.redaction/pageinfo/
is_root: false
weight: 90
---


## PageInfo class

簡潔なページ情報を表します。

詳しく読む：
- https://docs.groupdocs.com/redaction/net/get-file-info/

PageInfo 型は次のメンバーを公開します:

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/pageinfo/__init__/) |  |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [height](/redaction/python-net/groupdocs.redaction/pageinfo/height/) | ページの高さです。 |
| [page_number](/redaction/python-net/groupdocs.redaction/pageinfo/page_number/) | ページ番号です。 |
| [width](/redaction/python-net/groupdocs.redaction/pageinfo/width/) | ページの幅です。 |

### 例

```python
from groupdocs.redaction import Redactor

try:
    with Redactor(r"C:\Temp\testfile.doc") as red:
        doc_info = red.get_document_info()
        print(f"Document size: {doc_info.size}")
        print(f"Document format: {doc_info.file_type.file_format}")
        print(f"Document contains {doc_info.page_count} pages")
        for page in doc_info.pages:
            print(f"Page {page.page_number} size is {page.width}x{page.height}")
except GroupDocs.Redaction.Exceptions.PasswordRequiredException:
    print("You are trying to access document which is password protected. Please, set the password.")
except GroupDocs.Redaction.Exceptions.IncorrectPasswordException:
    print("The provided password is not valid.")
```

### 関連項目
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
