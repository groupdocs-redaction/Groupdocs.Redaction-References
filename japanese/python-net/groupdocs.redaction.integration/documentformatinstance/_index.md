---
title: "DocumentFormatInstance クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "ドキュメントの特定のフォーマットを表し、カスタム ドキュメント タイプを追加するために実装できます。"
type: docs
url: /ja/python-net/groupdocs.redaction.integration/documentformatinstance/
is_root: false
weight: 10
---


## DocumentFormatInstance class

ドキュメントの特定のフォーマットを表し、カスタム ドキュメント タイプを追加するために実装できます。

詳細を見る

- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

DocumentFormatInstance 型は次のメンバーを公開します：

### メソッド
| メソッド | 説明 |
| :- | :- |
| [initialize](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/#config-settings) | ドキュメント形式ハンドラのインスタンスを初期化します。 |
| [initialize_document_format_configuration](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize_document_format_configuration/) |  |
| [is_redaction_accepted](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/#description) | 実装があるか [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) をチェックし、指定されていれば呼び出します。 |
| [is_redaction_accepted_redaction_description](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted_redaction_description/) |  |
| [load](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load/#input) | ストリームからドキュメントを読み込みます。 |
| [load_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_streams/) |  |
| [perform_binary_check](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/#input) | 指定されたストリームがこの形式インスタンスでサポートされるドキュメントを含んでいるか確認します。 |
| [perform_binary_check_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_stream/) |  |
| [perform_binary_check_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_streams/) |  |
| [save](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save/#output) | ドキュメントをストリームに保存します。 |
| [save_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_streams/) |  |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/password/) | パスワードで保護されたドキュメントのパスワードです。 |

### 例

```python
class DummyDocument(DocumentFormatInstance):
    def load(self, output: io.RawIOBase) -> None:
        # ファイル内容を読み込む
        pass

    def save(self, output: io.RawIOBase) -> None:
        # ファイルへの変更を保存する
        pass
```

```python
class MyCustomHandler(DocumentFormatInstance):
    def __init__(self):
        self.my_property = None

    def initialize(self, config: DocumentFormatConfiguration) -> None:
        super().initialize(config)
        if "MyProperty" in config.initialization_data:
            self.my_property = config.initialization_data["MyProperty"]
```

### 関連項目
* module [`groupdocs.redaction.integration`](/redaction/python-net/groupdocs.redaction.integration/)
