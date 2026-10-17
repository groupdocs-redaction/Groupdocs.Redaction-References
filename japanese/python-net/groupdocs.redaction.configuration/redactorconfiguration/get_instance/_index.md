---
title: "get_instance メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "組み込みフォーマットのデフォルト構成を持つシングルトンインスタンスを返します。"
type: docs
url: /ja/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/
is_root: false
weight: 1040
---


## get_instance

組み込みフォーマットのデフォルト構成を持つシングルトンインスタンスを返します。

```python
def get_instance(cls):
    ...
```

**Returns:** RedactorConfiguration: Configuration instance.

### 例

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# シングルトン構成を取得する
config = RedactorConfiguration.get_instance()

# プレーンテキスト形式のサポート対象拡張子を拡張する
txt_settings = config.find_format(".txt")
txt_settings.extension_filter += ",.dump"
```

### 関連項目
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
