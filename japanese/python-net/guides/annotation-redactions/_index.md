---
title: "注釈の編集"
linkTitle: "Annotation redactions"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "この記事では、PDF、DOC、DOCX、PPT、PPTX、XLS、XLSX など、さまざまな形式の文書に対する注釈編集の実装方法を示します。"
type: docs
url: /ja/python-net/guides/annotation-redactions/
is_root: false
weight: 80
---


GroupDocs.Redaction API を使用すると、PDF、DOC、DOCX、PPT、PPTX、XLS、XLSX など、さまざまな形式の文書に対して注釈編集を適用できます。完全な一覧は[サポートされている文書形式]()の記事をご覧ください。

GroupDocs.Redactions は柔軟な API を提供し、注釈テキストから機密データを削除したり、正規表現で注釈を完全に削除したりできます。

## Remove annotations (comments etc)

GroupDocs.Redaction を使用して、文書からすべてまたは特定のコメントやその他の注釈を削除できます。例えば、本文に「use」「show」「describe」などのテキストを含むすべてのコメントを削除できます。

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

def remove_all_annotations():
    # パターンに一致する注釈を削除するための編集オプションを指定します
    a_red = DeleteAnnotationRedaction("(?im:(use|show|describe))")

    # レダクト対象のドキュメントをロードします
    with Redactor("./annotated.xlsx") as redactor:
        # 赤字化を適用します
        result = redactor.apply(a_red)

        # マスクしたドキュメントを元ファイルの隣に保存する
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    remove_all_annotations()
```

`annotated.xlsx` はこの例で使用されるサンプルファイルです。[ここをクリック](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx)してダウンロードしてください。

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/remove_all_annotations/annotated_redacted.xlsx)

引数なしのコンストラクタを使用して、文書内のすべての注釈を削除できます。

## Redact annotations

すべてまたは特定のアノテーションを削除する代わりに、アノテーションテキストから機密データを削除できます。例えば、対象のドキュメント内の「John」のすべての言及を削除することができます。例:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import AnnotationRedaction

def redact_annotations():
    # レダクションオプションを指定してください：検索パターンと置換文字列
    a_red = AnnotationRedaction("(?im:john)", "[redacted]")

    # レダクト対象のドキュメントをロードします
    with Redactor("./annotated.xlsx") as redactor:
        # 赤字化を適用します
        result = redactor.apply(a_red)

        # マスクしたドキュメントを元ファイルの隣に保存する
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_annotations()
```

`annotated.xlsx` はこの例で使用されるサンプルファイルです。[ここをクリック](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx)してダウンロードしてください。

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/redact_annotations/annotated_redacted.xlsx)
