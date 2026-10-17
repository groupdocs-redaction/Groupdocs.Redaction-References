---
title: "Redactor クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "ドキュメントの編集プロセスを制御し、開く、編集する、保存することを可能にするメイン クラスを表します。"
type: docs
url: /ja/python-net/groupdocs.redaction/redactor/
is_root: false
weight: 150
---


## Redactor class

ドキュメントの編集プロセスを制御し、開く、編集する、保存することを可能にするメイン クラスを表します。

詳細を見る
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More advanced redaction topics: https://docs.groupdocs.com/redaction/net/advanced-usage/

Redactor 型は次のメンバーを公開します：

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path) | ファイルパスを使用して新しい Redactor インスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document) | ストリームを使用して[`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) の新しいインスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options) | パスを使用してパスワード保護されたドキュメント用に[`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) の新しいインスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options-settings) | パスと設定を使用して、パスワード保護されたドキュメント用の新しい Redactor インスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options) | ストリームを使用して、パスワード保護されたドキュメント用の新しい Redactor インスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options-settings) | ストリームと設定を使用して、パスワード保護されたドキュメント用に[`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) の新しいインスタンスを初期化します。 |

### メソッド
| メソッド | 説明 |
| :- | :- |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redaction) | ドキュメントにレダクションを適用します。 |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redactions) | ドキュメントにレダクションのセットを適用します。 |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#policy) | ドキュメントにレダクション ポリシーを適用します。 |
| [apply_redaction](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction/) |  |
| [apply_redaction_policy](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction_policy/) |  |
| [dispose](/redaction/python-net/groupdocs.redaction/redactor/dispose/) | リソースを解放します。 |
| [generate_preview](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#preview_options) | 指定された画像形式で特定のページのプレビュー画像を生成します。 |
| [generate_preview_preview_options](/redaction/python-net/groupdocs.redaction/redactor/generate_preview_preview_options/) |  |
| [get_document_info](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/) | サイズやページ数など、ドキュメントの一般情報を取得します。 |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/) | 次のオプションでドキュメントをファイルに保存します：AddSuffix = True、RasterizeToPDF = True。 |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#save_options) | ドキュメントをファイルに保存します。 |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#document-rasterization_options) | カスタムロケーションを含めて、ドキュメントをストリームに保存します。 |
| [save_save_options](/redaction/python-net/groupdocs.redaction/redactor/save_save_options/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactor/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactor/save_streams/) |  |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# ドキュメントを開き、最初のページを削除します
with Redactor("document.pdf") as redactor:
    redactor.apply(RemovePageRedaction(PageSeekOrigin.BEGIN, 0, 1))
    redactor.save()
```

### Guides
`Redactor` を使用するタスク ガイド:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [Get file info](/redaction/python-net/guides/get-file-info/)

### 関連項目
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
