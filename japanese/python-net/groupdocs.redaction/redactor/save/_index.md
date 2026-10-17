---
title: "save メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "次のオプションでドキュメントをファイルに保存します：AddSuffix = True、RasterizeToPDF = True。"
type: docs
url: /ja/python-net/groupdocs.redaction/redactor/save/
is_root: false
weight: 1080
---


## save

次のオプションでドキュメントをファイルに保存します：AddSuffix = True、RasterizeToPDF = True。

```python
def save(self):
    ...
```

**Returns:** str: Path to redacted document.

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("document.docx") as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    options = SaveOptions()
    options.add_suffix = True
    options.rasterize_to_pdf = True
    result_path = redactor.save(options)
    print(f"Saved to {result_path}")
```

## save {#save_options}

ドキュメントをファイルに保存します。

```python
def save(self, save_options):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| save_options | `SaveOptions` | サフィックスを追加するかラスタライズするオプションです。 |

**Returns:** Path to redacted document.

### 例

```python
from datetime import datetime
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions


def save_in_original_format():
    # レダクションオプションを指定する
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # レダクト対象のドキュメントをロードします
    with Redactor("./sample.docx") as redactor:
        # 赤字化を適用します
        redactor.apply(ex_red)

        # 日付サフィックスを付けて、元の形式で編集済みドキュメントを保存します
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = datetime.now().strftime("%Y-%m-%d %H-%M-%S")

        result_path = redactor.save(so)
        print(f"Document redacted successfully.\nCheck output in {result_path}.")


if __name__ == "__main__":
    save_in_original_format()
```

## save {#document-rasterization_options}

カスタムロケーションを含めて、ドキュメントをストリームに保存します。

```python
def save(self, document, rasterization_options):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| document | `io.RawIOBase` | 対象ストリーム。 |
| rasterization_options | `RasterizationOptions` | ラスタライズするかしないか、ラスタライズ対象のページを指定するオプションです。 |

### 例

```python
import io
from groupdocs.redaction.options import RasterizationOptions
from groupdocs.redaction import Redactor

with Redactor("document.pptx") as redactor:
    # 最初のスライドのみを処理するようにラスタライズを構成します
    ro = RasterizationOptions()
    ro.page_index = 0
    ro.page_count = 1

    stream = io.BytesIO()
    redactor.save(stream, ro)

    # BytesIO オブジェクトに保存されたドキュメントが含まれています
    data = stream.getvalue()
```

### 関連項目
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
