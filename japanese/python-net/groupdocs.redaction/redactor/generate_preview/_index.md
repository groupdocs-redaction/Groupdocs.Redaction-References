---
title: "generate_preview メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "指定された画像形式で特定のページのプレビュー画像を生成します。"
type: docs
url: /ja/python-net/groupdocs.redaction/redactor/generate_preview/
is_root: false
weight: 1050
---


## generate_preview {#preview_options}

指定された画像形式で特定のページのプレビュー画像を生成します。

プレビューは `preview_options` で定義された設定に従って生成されます。設定には画像形式、サイズ、ページ範囲、ページストリームの作成と解放のコールバックが含まれます。

```python
def generate_preview(self, preview_options):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| preview_options | `PreviewOptions` | 画像プロパティとページ範囲の設定。 |

### 例

```python
from groupdocs.redaction import Redactor, PreviewOptions, PreviewFormats

def create_page_stream(page_number):
    # 指定されたページのプレビュー画像用の書き込み可能なファイルストリームを返します。
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")

def release_page_stream(page_number, page_stream):
    # プレビュー画像が書き込まれた後に呼び出されます。
    page_stream.close()

preview_options = PreviewOptions(
    create_page_stream=create_page_stream,
    release_page_stream=release_page_stream,
)
preview_options.preview_format = PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### 関連項目
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
