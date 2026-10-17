---
title: "RedactorConfiguration クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "組み込みおよびカスタムユーザー形式を含む、サポートされている形式の一覧へのアクセスを提供します。"
type: docs
url: /ja/python-net/groupdocs.redaction.configuration/redactorconfiguration/
is_root: false
weight: 20
---


## RedactorConfiguration class

組み込みおよびカスタムユーザー形式を含む、サポートされている形式の一覧へのアクセスを提供します。

詳しく読む：

- More details about GroupDocs.Redaction configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

RedactorConfiguration 型は次のメンバーを公開します:

### メソッド
| メソッド | 説明 |
| :- | :- |
| [find_format](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/#file_extension) | 指定されたファイル拡張子に対するフォーマット構成を検索します。 |
| [find_format_file](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_file/) |  |
| [find_format_string](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_string/) |  |
| [get_instance](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/) | 組み込みフォーマットのデフォルト構成を持つシングルトンインスタンスを返します。 |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [available_formats](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/available_formats/) | 認識されたフォーマットの一覧です。[`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/) を参照してください。 |

### 例

```python
# カスタムユーザーフォーマットハンドラを追加する
adobe_photoshop_settings = DocumentFormatConfiguration()
adobe_photoshop_settings.extension_filter = ".psd"
adobe_photoshop_settings.document_type = MyAdobePhotoshopFormatInstance

config = RedactorConfiguration.get_instance()
config.available_formats.add(adobe_photoshop_settings)
```

```python
# 組み込みまたはカスタムユーザーフォーマットハンドラを取得する
config = RedactorConfiguration.get_instance()
format_settings = config.find_format(".psd")
```

### 関連項目
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
