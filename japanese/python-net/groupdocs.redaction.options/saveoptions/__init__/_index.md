---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "デフォルト設定で新しいインスタンスを初期化します：rasterizetopdf は False、addsuffix は False です。"
type: docs
url: /ja/python-net/groupdocs.redaction.options/saveoptions/__init__/
is_root: false
weight: 10
---


## __init__

デフォルト設定で新しいインスタンスを初期化します：rasterize_to_pdf は False、add_suffix は False です。

```python
def __init__(self):
    ...
```

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

with Redactor("./sample.docx") as redactor:
    redactor.apply(ex_red)
    save_options = SaveOptions()  # defaults: rasterize_to_pdf=False, add_suffix=False
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}.")
```

## __init__ {#rasterize_to_pdf-suffix}

指定されたパラメータで新しいインスタンスを初期化します。

```python
def __init__(self, rasterize_to_pdf, suffix):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| rasterize_to_pdf | `bool` | 文書内のすべてのページを画像に変換し、単一の PDF ファイルにまとめる必要がある場合は True です。 |
| suffix | `str` | このテキストはファイル名の末尾に追加されます。空でない場合は `add_suffix` も True に設定されます。 |

### 例

```python
from groupdocs.redaction.options import SaveOptions

# デフォルト設定で保存オプションを作成します
options = SaveOptions()
options.add_suffix = True
options.rasterize_to_pdf = True
options.redacted_file_suffix = "redacted"
```

### 関連項目
* class [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/)
