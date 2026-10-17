---
title: "generate_preview メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "指定された画像形式で特定のページのプレビュー画像を生成します。"
type: docs
url: /ja/python-net/groupdocs.redaction.integration/ipreviewable/generate_preview/
is_root: false
weight: 1010
---


## generate_preview {#preview_options}

指定された画像形式で特定のページのプレビュー画像を生成します。

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

with Redactor("document.pdf") as redactor:
    options = PreviewOptions(
        format=PreviewFormats.PNG,
        start_page=1,
        end_page=5,
        create_page_stream=lambda page: open(f"page_{page}.png", "wb")
    )
    redactor.generate_preview(options)
```

### 関連項目
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
