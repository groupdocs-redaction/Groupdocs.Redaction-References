---
title: "PreviewOptions クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "プレビュー生成のための要件とストリーム デリゲートを設定するオプションを提供します。"
type: docs
url: /ja/python-net/groupdocs.redaction.options/previewoptions/
is_root: false
weight: 70
---


## PreviewOptions class

プレビュー生成のための要件とストリーム デリゲートを設定するオプションを提供します。

このクラスは、プレビュー形式、画像サイズ、ページ番号を指定し、各生成ページのストリームを作成し、必要に応じて解放するデリゲートを設定できます。

PreviewOptions 型は次のメンバーを公開します:

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream) | 新しい PreviewOptions インスタンスを初期化します。出力ストリームは使用後に閉じられます。 |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream-release_page_stream) | 新しい PreviewOptions インスタンスを初期化し、出力ストリームがクライアントに返され、さらに使用できるようにします。 |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [create_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/create_page_stream/) | ページストリーム作成デリゲートです。 |
| [height](/redaction/python-net/groupdocs.redaction.options/previewoptions/height/) | ページプレビューの高さです。 |
| [page_numbers](/redaction/python-net/groupdocs.redaction.options/previewoptions/page_numbers/) | プレビューを生成するページ番号です。 |
| [preview_format](/redaction/python-net/groupdocs.redaction.options/previewoptions/preview_format/) | プレビュー画像の形式です。 |
| [release_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/release_page_stream/) | ページプレビュー完了デリゲートです。 |
| [width](/redaction/python-net/groupdocs.redaction.options/previewoptions/width/) | ページプレビューの幅です。 |

### 例

```python
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int):
    # 指定されたページのプレビュー画像用ファイルを作成します
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")  # returns a writable binary stream

preview_options = PreviewOptions(create_page_stream)
preview_options.preview_format = PreviewOptions.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### 関連項目
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
