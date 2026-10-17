---
title: "こんにちは、世界！"
linkTitle: "Hello, World!"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "簡単なサンプルを作成して実行することで、GroupDocs.Redaction for Python via .NET をすぐに始めましょう。"
type: docs
url: /ja/python-net/guides/hello-world/
is_root: false
weight: 20
---


## Introduction
「Hello, World!」のサンプルは、GroupDocs.Redaction for Python via .NET を試す際の最初のステップになることが多いです。開発環境が正しく設定され、ライブラリが期待通りに動作していることを確認するシンプルなテストとして役立ちます。

## Overview
GroupDocs.Redaction for Python via .NET を使用すると、さまざまな文書形式から機密情報を検索、編集、削除できます。幅広い[サポート形式](https://docs.groupdocs.com/redaction/python-net/getting-started/supported-document-formats/)に対応しているため、さまざまなユースケースで柔軟に利用できます。

## How to redact a document
以下の手順は、GroupDocs.Redaction for Python via .NET を使用して文書から機密情報を編集する方法を示しています。

1. 必要な `groupdocs.redaction` クラスをインポートします。
2. 編集内容を記述します（ここでは、特定のフレーズをカラー ボックスで置き換えます）。
3. サンプル文書へのパスを指定して、[`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) のインスタンスを作成します。
4. 編集を適用します。
5. 結果を保存します。

## Complete example
以下の例では、フレーズ"John Doe"のすべての出現箇所を半透明の赤いボックスで置き換え、編集された文書を保存します。

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def hello_world():
    # 「John Doe」のすべての出現箇所に半透明の赤いボックスを描画します
    options = ReplacementOptions(Color.from_argb(128, 255, 0, 0))
    redaction = ExactPhraseRedaction("John Doe", options)

    # 文書を読み込み、編集を適用し、結果を保存します
    with Redactor("./sample.docx") as redactor:
        redactor.apply(redaction)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Document redacted successfully. Output saved to {result_path}.")

if __name__ == "__main__":
    hello_world()
```

`sample.docx` はこの例で使用されるサンプルファイルです。[ここをクリック](https://docs.groupdocs.com/redaction/python-net/_sample_files/getting-started/hello-world/sample.docx)してダウンロードしてください。

  
```text
Binary file (PDF, 1.0 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/getting-started/hello-world/hello_world/sample_redacted.pdf)

この例では、結果を `sample_redacted.pdf` という名前の PDF にラスタライズするため、編集された内容は復元できません（`save()` はデフォルトで PDF にラスタライズします；`redacted_file_suffix` オプションは出力名を制御するだけです）。元の形式を保持したい場合は、`rasterize_to_pdf = False` を設定してください。

## Additional resources
このデモは、GroupDocs.Redaction for Python via .NET の[コードサンプル](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET/)を参照しています。
