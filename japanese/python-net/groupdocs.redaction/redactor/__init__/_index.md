---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "ファイルパスを使用して新しい Redactor インスタンスを初期化します。"
type: docs
url: /ja/python-net/groupdocs.redaction/redactor/__init__/
is_root: false
weight: 10
---


## __init__ {#file_path}

ファイルパスを使用して新しい Redactor インスタンスを初期化します。

```python
def __init__(self, file_path):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| file_path | `str` | ファイルへのパスです。 |

### 例

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    # ここでレダクション操作を実行します
    pass
```

## __init__ {#document}

ストリームを使用して[`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) の新しいインスタンスを初期化します。

```python
def __init__(self, document):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| document | `io.RawIOBase` | ドキュメントのソース ストリームです。 |

### 例

```python
from groupdocs.redaction import Redactor

def open_from_stream():
    # バイナリストリームとして文書を開く
    with open("./sample.pdf", "rb") as stream:
        # ストリームから文書を読み込む
        with Redactor(stream) as redactor:
            # ここでレダクションを実行します
            pass
```

## __init__ {#file_path-load_options}

パスを使用してパスワード保護されたドキュメント用に[`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) の新しいインスタンスを初期化します。

```python
def __init__(self, file_path, load_options):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| file_path | `str` | ファイルへのパスです。 |
| load_options | `LoadOptions` | オプション（パスワードを含む）。 |

### 例

```python
from groupdocs.redaction import Redactor

# ファイル パスからパスワード保護されたドキュメントを読み込みます
with Redactor("protected.docx") as redactor:
    # ここでレダクション操作を実行します
    pass
```

## __init__ {#file_path-load_options-settings}

パスと設定を使用して、パスワード保護されたドキュメント用の新しい Redactor インスタンスを初期化します。

```python
def __init__(self, file_path, load_options, settings):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| file_path | `str` | ファイルへのパス。 |
| load_options | `LoadOptions` | ファイル依存のオプション（パスワードを含む）。 |
| settings | `RedactorSettings` | レダクション プロセスのデフォルト設定です。 |

### 例

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

## __init__ {#document-load_options}

ストリームを使用して、パスワード保護されたドキュメント用の新しい Redactor インスタンスを初期化します。

```python
def __init__(self, document, load_options):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| document | `io.RawIOBase` | ソース入力ストリームです。 |
| load_options | `LoadOptions` | オプション（パスワードを含む）。 |

### 例

```python
from groupdocs.redaction import Redactor, LoadOptions

def open_protected_doc():
    # 保護された PDF をバイナリ ストリームとして開きます
    with open(r"C:\sample.pdf", "rb") as stream:
        # LoadOptions でパスワードを提供します
        load_options = LoadOptions("mypassword")
        # ストリームとロード オプションで Redactor を初期化します
        with Redactor(stream, load_options) as redactor:
            # ここでレダクション操作を実行します
            pass
```

## __init__ {#document-load_options-settings}

ストリームと設定を使用して、パスワード保護されたドキュメント用に[`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) の新しいインスタンスを初期化します。

```python
def __init__(self, document, load_options, settings):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| document | `io.RawIOBase` | ソース入力ストリームです。 |
| load_options | `LoadOptions` | オプション（パスワードを含む）。 |
| settings | `RedactorSettings` | 赤字処理のデフォルト設定。 |

### 関連項目
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
