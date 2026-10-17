---
title: "赤字化の基本"
linkTitle: "Redaction basics"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "この記事では、Python 開発者がドキュメントにメタデータ、画像、注釈、テキストの赤字化を適用する方法を示します。PDF、DOC、DOCX、PPT、PPTX、XLS、XLSX など、幅広いドキュメント形式がサポートされています。"
type: docs
url: /ja/python-net/guides/redaction-basics/
is_root: false
weight: 40
---


GroupDocs.Redaction は効果的なドキュメント赤字化機能のセットをサポートしています。[text](), [metadata](), [annotations](), [images]() に対する赤字化を適用できます。

PDF、DOC、DOCX、PPT、PPTX、XLS、XLSX など、幅広いドキュメント形式がサポートされています。完全なサポート形式一覧は [supported document formats]() 記事をご覧ください。

## Redaction types

GroupDocs.Redaction には以下の赤字化タイプが用意されています：

| タイプ | 説明 | クラス |
| --- | --- | --- |
| [Text]() | Replaces or hides with color block a portion of text within document body | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/)、[RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) |
| [Metadata]() | Replace metadata values with empty ones or redacts metadata texts | [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/)、[MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) |
| [Annotations]() | Deletes annotations from document or redacts its texts | [DeleteAnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/), [AnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) |
| [Images]() | Replaces specific area of an image with a colored box | [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) |
| [Pages]() | Removes specific range of pages (slides, worksheets, etc.) | [RemovePageRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) |

## Apply redaction

ドキュメントへのレダクションの適用は [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) メソッドを使用して行われます。結果として、各レダクションが適用されたログエントリを含む [RedactorChangeLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/) インスタンスが取得されます。エントリには、オプションや操作のステータス（以下参照）、必要に応じたテキスト説明を含む [Redacton](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redaction/) インスタンスへの参照が含まれます。少なくとも1つのレダクションが失敗した場合、[Status == RedactionStatus.Failed](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) が表示されます:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def apply_redaction():
    # レダクションオプションを指定する
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # レダクト対象のドキュメントをロードします
    with Redactor("./sample.docx") as redactor:
        # 赤字化を適用します
        result = redactor.apply(ex_red)

        if result.status != RedactionStatus.FAILED:
            # マスクしたドキュメントを元ファイルの隣に保存する
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    apply_redaction()
```

`sample.docx` はこの例で使用されているサンプルファイルです。ダウンロードするには [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) をクリックしてください。

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_redaction/sample_redacted.docx)

この表には、[RedactionStatus](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) 列挙体のすべての可能なステータスが一覧表示されています。

| ステータス | 説明 | 考えられる理由 |
| --- | --- | --- |
| *適用済み* | レダクションは完全に、かつ正常に適用されました | レダクションプロセス内のすべての操作が正常に適用されました |
| *部分的に適用* | レダクションは一致項目の一部にのみ適用されました | 1) 置換の試用制限を超えました2) ユーザーによって少なくとも1つの変更が拒否されました |
| *スキップ* | レダクションはスキップされました（適用されません） | 1) レダクションの試用制限を超えました2) この種類のドキュメントにはレダクションを適用できません3) すべての置換がユーザーにより拒否され、変更は行われませんでした |
| *失敗* | レダクションは例外により失敗しました | レダクション処理中に例外が発生しました |

詳細情報を取得するには、[RedactorChangeLog.RedactionLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/redaction_log/) のレダクションログエントリを反復処理し、ステータスが *適用済み* 以外の項目の [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) プロパティを確認する必要があります:

```python
result = redactor.apply(redaction)
if result.status != RedactionStatus.FAILED:
    # デフォルトでは、レダクションされたドキュメントは PDF 形式で保存されます
    save_options = SaveOptions()
    save_options.add_suffix = True
    save_options.rasterize_to_pdf = True
    save_options.redacted_file_suffix = "redacted"
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}")
else:
    # 失敗またはスキップされたすべてのレダクションをダンプする
    print("Redaction failed!")
    for log_entry in result.redaction_log:
        if log_entry.result.status != RedactionStatus.APPLIED:
            print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")
```

## Apply multiple redactions

[Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) メソッドを1回呼び出すだけで、必要なだけ多くのレダクションを適用できます。このメソッドのオーバーロードはレダクションの配列とレダクションポリシーを受け取るためです。この場合、レダクションは配列に現れる順序で適用されます。コード内でレダクションセットを指定する代わりに、[here]() に記載されているようにレダクションポリシーを含む XML ファイルを作成することもできます。

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    RegexRedaction,
    ReplacementOptions,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def apply_multiple_redactions():
    # 赤字化ボックスの色を定義する
    color = Color.from_argb(255, 220, 20, 60)

    # 適用するレダクションのリストを順番通りに提供してください
    redaction_list = [
        ExactPhraseRedaction("John Doe", ReplacementOptions("[Client]")),
        RegexRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # レダクト対象のドキュメントをロードします
    with Redactor("./sample.docx") as redactor:
        # 赤字リストを適用する
        result = redactor.apply(redaction_list)

        if result.status != RedactionStatus.FAILED:
            # デフォルトでは、レダクションされたドキュメントは PDF 形式で保存されます
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)
        else:
            # 失敗またはスキップされたすべてのレダクションをダンプする
            print("Redaction failed!")
            for log_entry in result.redaction_log:
                if log_entry.result.status != RedactionStatus.APPLIED:
                    print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")

if __name__ == "__main__":
    apply_multiple_redactions()
```

`sample.docx` はこの例で使用されているサンプルファイルです。ダウンロードするには [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) をクリックしてください。

  
```text
Binary file (PDF, 1.2 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_multiple_redactions/sample_redacted.pdf)
