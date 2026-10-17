---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "新しい PreviewOptions インスタンスを初期化します。"
type: docs
url: /ja/python-net/groupdocs.redaction.options/previewoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#create_page_stream}

新しい PreviewOptions インスタンスを初期化します。出力ストリームは使用後に閉じられます。

```python
def __init__(self, create_page_stream):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | 特定のページプレビュー用のストリームを作成します。 |

## __init__ {#create_page_stream-release_page_stream}

新しい PreviewOptions インスタンスを初期化し、出力ストリームがクライアントに返され、さらに使用できるようにします。

```python
def __init__(self, create_page_stream, release_page_stream):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | 特定のページプレビュー用のストリームを作成します。 |
| release_page_stream | `ReleasePageStream` | ページプレビューの生成が完了したことを通知し、出力ストリームを取得します。 |

### 関連項目
* class [`PreviewOptions`](/redaction/python-net/groupdocs.redaction.options/previewoptions/)
