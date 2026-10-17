---
title: "メタデータのレダクション"
linkTitle: "Metadata redactions"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "この記事では、Python のレダクション API がフィルタや正規表現検索を使用してメタデータを置換または削除できる方法を示します。"
type: docs
url: /ja/python-net/guides/metadata-redactions/
is_root: false
weight: 70
---


GroupDocs.Redaction API を使用すると、PDF、DOC、DOCX、PPT、PPTX、XLS、XLSX などのさまざまな形式のドキュメントにメタデータのレダクションを適用できます。完全なリストは [サポートされているドキュメント形式]() 記事をご覧ください。

GroupDocs.Redactions は、フィルタや正規表現検索を使用してメタデータを置換または削除できる柔軟な API を提供します。

## Filter metadata

すべてのレダクションの基本機能は、[MetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) 基底クラスから派生しており、*metadata filtering* がメタデータレダクションに必須です。これは、最も頻繁に使用されるメタデータ項目を含むフラグ付き列挙体 [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) を使用します。フィルタを *All* に設定するか、メタデータの任意の組み合わせを指定できます。例えば、以下の例ではフィルタを *Author*、*Manager*、*NameOfApplication* に設定しています — テキストレダクションやそれらの除去のためです。

```python
# MetadataRedaction から派生したレダクション
redaction.filter = MetadataFilters.AUTHOR | MetadataFilters.MANAGER | MetadataFilters.NAME_OF_APPLICATION
```

以下は、[MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) 項目の完全なリストを示す表です。

| フィルタ | 数値 | 説明 |
| --- | --- | --- |
| *None* | 0 | 空のフィルタ設定で、メタデータ項目に一致しません |
| *Author* | 1 | ドキュメントの作成者 |
| *カテゴリ* | 2 | ドキュメントのカテゴリ |
| *コメント* | 4 | ドキュメントのコメント |
| *会社* | 8 | 作成者の会社 |
| *ContentStatus* | 16 | コンテンツのステータス |
| *CreatedTime* | 32 | 作成日時 |
| *HyperlinkBase* | 64 | ハイパーリンクのベース |
| *LastPrinted* | 128 | 最終印刷日時 |
| *LastSavedBy* | 256 | ユーザーによって最後に保存されました |
| *LastSavedTime* | 1024 | 最後に保存された日付と時刻 |
| *NameOfApplication* | 2048 | ドキュメントが作成されたアプリケーションの名前 |
| *Manager* | 4096 | 著者のマネージャー名 |
| *RevisionNumber* | 8192 | リビジョン番号 |
| *Subject* | 16384 | ドキュメントの件名 |
| *Template* | 32768 | ドキュメントテンプレート名 |
| *Title* | 65536 | ドキュメントのタイトル |
| *TotalEditingTime* | 131072 | 総編集時間 |
| *バージョン* | 262144 | ドキュメントのバージョン |
| *説明* | 524288 | ドキュメントの説明 |
| *キーワード* | 1048576 | ドキュメントのキーワード |
| *ContentType* | 2097152 | コンテンツタイプ |
| *すべて* | 2147483647 | すべてのメタデータ項目のタイプ |

## Clean metadata

ドキュメント内のすべてまたは特定のメタデータを空（ブランクまたは最小限）の値に置き換えるには、[EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/) クラスを使用します。以下の例はドキュメントのすべてのプロパティを空にします：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_all_metadata():
    # すべてのメタデータを削除するためのレダクションオプションを指定してください
    met_red = EraseMetadataRedaction(MetadataFilters.ALL)

    # レダクト対象のドキュメントをロードします
    with Redactor("./sample.docx") as redactor:
        # 赤字化を適用します
        result = redactor.apply(met_red)

        # マスクしたドキュメントを元ファイルの隣に保存する
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_all_metadata()
```

`sample.docx` はこの例で使用されるサンプルファイルです。ダウンロードするには [ここ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) をクリックしてください。

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/clean_all_metadata/sample_redacted.docx)

指定されたドキュメント内のすべてのメタデータを空にするには、[MetadataFilter.All](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) を指定するか、デフォルトコンストラクタを使用します。Custom はすべてのカスタムメタデータエントリをクリアします。

## Redact metadata

[MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) を使用して、正規表現でドキュメントのメタデータから機密データを削除できます。例えば、"Company Ltd." の記述をすべて削除できます：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction

def redact_metadata():
    # レダクションオプションを指定してください：検索パターンと置換文字列
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # レダクト対象のドキュメントをロードします
    with Redactor("./sample.docx") as redactor:
        # 赤字化を適用します
        result = redactor.apply(met_red)

        # マスクしたドキュメントを元ファイルの隣に保存する
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata()
```

`sample.docx` はこの例で使用されるサンプルファイルです。ダウンロードするには [ここ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) をクリックしてください。

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata/sample_redacted.docx)

最初の引数は正規表現、2番目は置換文字列です。フィルタを設定してレダクションのスコープを指定することもできます。例として [MetadataFilter.Company](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) を使用します。- これにより、"Company" プロパティを除くすべてのメタデータ項目で正規表現の一致がそのまま残ります：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

def redact_metadata_with_filter():
    # レダクションオプションを指定してください：検索パターンと置換文字列
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # レダクションのスコープを Company メタデータ項目のみに限定する
    met_red.filter = MetadataFilters.COMPANY

    # レダクト対象のドキュメントをロードします
    with Redactor("./sample.docx") as redactor:
        # 赤字化を適用します
        result = redactor.apply(met_red)

        # マスクしたドキュメントを元ファイルの隣に保存する
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata_with_filter()
```

`sample.docx` はこの例で使用されるサンプルファイルです。ダウンロードするには [ここ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) をクリックしてください。

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata_with_filter/sample_redacted.docx)

## Metadata redaction status

すべてのメタデータレダクションは各メタデータ項目に個別に適用され、メタデータ項目のレダクションが失敗しても、残りのメタデータ項目は更新されます。失敗した、スキップされた（拒否された）メタデータ項目とその理由の一覧は、[ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) プロパティおよび [RedactorLogEntry.Result](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorlogentry/result/) にあります。
