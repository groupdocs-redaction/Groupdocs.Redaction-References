---
title: "スプレッドシートのレダクション"
linkTitle: "Spreadsheet redactions"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "この記事では、Python のレダクション API が XLS、XLSX、ODS などのスプレッドシート形式から機密またはプライベートなデータをマスクできる方法を示します。"
type: docs
url: /ja/python-net/guides/spreadsheet-redactions/
is_root: false
weight: 90
---


GroupDocs.Redaction は、XLS、XLSX、ODS などのスプレッドシート形式から機密またはプライベートなデータをマスクできます。完全なリストは [サポートされているドキュメント形式]() 記事をご覧ください。

## Redact spreadsheet content

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_spreadsheet_content():
    # レダクションオプションを指定する
    repl_opt = ReplacementOptions("-redacted-")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # マスク対象のスプレッドシートを読み込む
    with Redactor("./sample.xlsx") as redactor:
        # 赤字化を適用します
        result = redactor.apply(ex_red)

        # マスクしたドキュメントを元ファイルの隣に保存する
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_spreadsheet_content()
```

`sample.xlsx` はこの例で使用されるサンプルファイルです。ダウンロードするには [ここ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/spreadsheet-redactions/sample.xlsx) をクリックしてください。

  
```text
Binary file (XLSX, 15 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/spreadsheet-redactions/redact_spreadsheet_content/sample_redacted.xlsx)
