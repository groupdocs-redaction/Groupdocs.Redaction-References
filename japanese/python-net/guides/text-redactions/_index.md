---
title: "テキストのレダクション"
linkTitle: "Text redaction"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "この記事では、Python のレダクション API が文書から機密またはプライベートなデータを簡単にレダクションできる方法を説明します。PDF、DOC、DOCX、PPT、PPTX、XLS、XLSX などのさまざまな形式の文書に対して、正確なフレーズまたは正規表現を使用してテキストレダクションを適用できます。"
type: docs
url: /ja/python-net/guides/text-redactions/
is_root: false
weight: 50
---


GroupDocs.Redaction を使用すると、文書から機密またはプライベートなデータを簡単にレダクションできます。最も一般的なレダクションケースは、文書からテキストを削除することです。

GroupDocs.Redaction API を使用すると、PDF、DOC、DOCX、PPT、PPTX、XLS、XLSX などのさまざまな形式の文書に対して、正確なフレーズまたは [regular expression](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expressions) を使用してテキストレダクションを適用できます。完全なリストは [supported document formats]() 記事をご覧ください。

## Use exact phrase redaction

以下の例では、テキストレダクションを適用し、個人の正確なフレーズ "John Doe" を "\\[personal\\]"（または任意の免除コード）に置き換えます。

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_exact_phrase():
    # レダクションオプションを指定する
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # レダクト対象のドキュメントをロードします
    with Redactor("./sample.docx") as redactor:
        # 赤字化を適用します
        result = redactor.apply(ex_red)

        # マスクしたドキュメントを元ファイルの隣に保存する
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_exact_phrase()
```

`sample.docx` はこの例で使用されるサンプルファイルです。クリック [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) してダウンロードしてください。

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_exact_phrase/sample_redacted.docx)

デフォルトでは、正確なフレーズの検索は大文字と小文字を区別しません。大文字小文字を区別する赤字化を行う場合、コンストラクタのパラメータと対応するパブリックプロパティがあります：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_case_sensitive_phrase():
    # 大文字小文字を区別したマッチングを有効にする
    case_sensitive = True

    # レダクションオプションを指定する
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", case_sensitive, repl_opt)

    # レダクト対象のドキュメントをロードします
    with Redactor("./sample.docx") as redactor:
        # 赤字化を適用します
        result = redactor.apply(ex_red)

        # マスクしたドキュメントを元ファイルの隣に保存する
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_case_sensitive_phrase()
```

`sample.docx` はこの例で使用されるサンプルファイルです。クリック [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) してダウンロードしてください。

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_case_sensitive_phrase/sample_redacted.docx)

赤字化されたテキストの上にカラーのボックスが必要な場合、置換文字列の代わりに color を使用できます。赤字化は一致したテキストを削除し、指定した色の矩形を赤字化されたテキストの位置に配置します：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_color_box():
    # 赤字化ボックスの色を定義する
    color = Color.from_argb(255, 220, 20, 60)

    # レダクションオプションを指定する
    repl_opt = ReplacementOptions(color)
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # レダクト対象のドキュメントをロードします
    with Redactor("./sample.docx") as redactor:
        # 赤字化を適用します
        result = redactor.apply(ex_red)

        # マスクしたドキュメントを元ファイルの隣に保存する
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_color_box()
```

`sample.docx` はこの例で使用されるサンプルファイルです。クリック [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) してダウンロードしてください。

  
```text
Binary file (DOCX, 17 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_color_box/sample_redacted.docx)

アラビア語やヘブライ語など、右から左へ書く文書に赤字化を適用する必要があるかもしれません。以下の例は、Arabic PDF ドキュメントに ExactPhraseRedaction を適用する方法を示しています：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_right_to_left_text():
    # アラビア語のフレーズで赤字化オプションを指定する
    repl_opt = ReplacementOptions("[test]")
    ex_red = ExactPhraseRedaction("انتقد", repl_opt)

    # レダクト対象のドキュメントをロードします
    with Redactor("./arabic.pdf") as redactor:
        # 赤字化を適用します
        result = redactor.apply(ex_red)

        # マスクしたドキュメントを元ファイルの隣に保存する
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_right_to_left_text()
```

`arabic.pdf` はこの例で使用されるサンプルファイルです。[here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/arabic.pdf) をクリックしてダウンロードしてください。

  
```text
Binary file (PDF, 23 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_right_to_left_text/arabic_redacted.pdf)

## Use regular expression

内部では,"exact phrase" 赤字化は正規表現を使用して動作し、これは赤字化の基本的なアプローチです。以下の例では,"2 桁、スペースまたはなし、2 桁、再びスペース、6 桁" に一致する任意のテキストを青色のボックスで赤字化します：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_regex():
    # 赤字化ボックスの色を定義する
    color = Color.from_argb(255, 220, 20, 60)

    # レダクションオプションを指定する
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", repl_opt)

    # レダクト対象のドキュメントをロードします
    with Redactor("./sample.docx") as redactor:
        # 赤字化を適用します
        result = redactor.apply(reg_red)

        # マスクしたドキュメントを元ファイルの隣に保存する
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_regex()
```

`sample.docx` はこの例で使用されるサンプルファイルです。クリック [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) してダウンロードしてください。

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_regex/sample_redacted.docx)

段落全体を赤字化する必要がある場合は、RegexRedaction を使用する必要があります。以下の例は、PDF ドキュメント内の段落全体を赤字化する方法を示しています：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_whole_paragraph():
    # 赤字化ボックスの色を定義する
    color = Color.from_argb(255, 220, 20, 60)

    # 段落全体に一致する赤字化オプションを指定する
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("(Lorem(\n|.)+?urna)", repl_opt)

    # レダクト対象のドキュメントをロードします
    with Redactor("./sample.pdf") as redactor:
        # 赤字化を適用します
        result = redactor.apply(reg_red)

        # マスクしたドキュメントを元ファイルの隣に保存する
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_whole_paragraph()
```

`sample.pdf` はこの例で使用されるサンプルファイルです。[here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.pdf) をクリックしてダウンロードしてください。

  
```text
Binary file (PDF, 68 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_whole_paragraph/sample_redacted.pdf)
