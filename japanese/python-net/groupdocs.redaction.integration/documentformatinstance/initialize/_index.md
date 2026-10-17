---
title: "initialize メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "ドキュメント形式ハンドラのインスタンスを初期化します。"
type: docs
url: /ja/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/
is_root: false
weight: 1010
---


## initialize {#config-settings}

ドキュメント形式ハンドラのインスタンスを初期化します。

```python
def initialize(self, config, settings):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| config | `DocumentFormatConfiguration` | フォーマット構成。 |
| settings | `RedactorSettings` | 赤字処理のデフォルト設定。 |

**Returns:** None.

### 例

```python
from groupdocs.redaction.integration import DocumentFormatInstance, DocumentFormatConfiguration, RedactorConfiguration

class MyCustomHandler(DocumentFormatInstance):
    def __init__(self):
        super().__init__()
        self.my_property = None

    def initialize(self, config, settings=None):
        super().initialize(config, settings)
        if "MyProperty" in config.initialization_data:
            self.my_property = config.initialization_data["MyProperty"]

# カスタムフォーマットを登録する
my_config = DocumentFormatConfiguration()
my_config.extension_filter = ".foo"
my_config.document_type = MyCustomHandler
my_config.initialization_data["MyProperty"] = "bar"

redactor_config = RedactorConfiguration.get_instance()
redactor_config.available_formats.append(my_config)
```

### 関連項目
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
