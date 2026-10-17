---
title: "DocumentFormatConfiguration クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "DocumentFormatInstance 派生クラスへの型参照と、より高速なフォーマット検出のためのサポートされるファイル拡張子のリストを表します。"
type: docs
url: /ja/python-net/groupdocs.redaction.configuration/documentformatconfiguration/
is_root: false
weight: 10
---


## DocumentFormatConfiguration class

[`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) から派生したクラスの型参照と、より高速な形式検出のためにサポートされているファイル拡張子の一覧を表します。

詳細を見る

- More details about **GroupDocs.Redaction** configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

DocumentFormatConfiguration 型は次のメンバーを公開します:

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/__init__/) | DocumentFormatConfiguration の新しいインスタンスを初期化します。 |

### メソッド
| メソッド | 説明 |
| :- | :- |
| [supports_extension](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/#file_extension) | 指定されたファイル拡張子が DocumentType として処理できるかを確認します。 |
| [supports_extension_file](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_file/) |  |
| [supports_extension_string](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_string/) |  |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [document_type](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/document_type/) | [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) を継承するクラスの型です。 |
| [extension_filter](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/extension_filter/) | ファイル拡張子のカンマ区切りリスト（例: ".pdf"）で、大文字小文字を区別しません。 |
| [initialization_data](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/initialization_data/) | [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) の初期化に必要なデータです。 |

### 例

```python
from groupdocs.redaction import DocumentFormatConfiguration

# カスタム形式構成を作成する
config = DocumentFormatConfiguration()
config.ExtensionFilter = ".psd"
config.DocumentType = MyAdobePhotoshopFormatInstance
```

### 関連項目
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
