---
title: "find_format メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "指定されたファイル拡張子に対するフォーマット構成を検索します。"
type: docs
url: /ja/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/
is_root: false
weight: 1010
---


## find_format {#file_extension}

指定されたファイル拡張子に対するフォーマット構成を検索します。

```python
def find_format(self, file_extension):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| file_extension | `str` | ファイル拡張子、フォーマットは ".ext" です。 |

**Returns:** DocumentFormatConfiguration or None: If found, instance of DocumentFormatConfiguration, None otherwise.

### 例

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# シングルトン構成インスタンスを取得する
config = RedactorConfiguration.get_instance()

# 指定された拡張子のフォーマット設定を取得する
settings = config.find_format(".txt")
if settings:
    # 処理対象の拡張子リストを拡張し、例として .dump を追加します
    settings.extension_filter = settings.extension_filter + ",.dump"
```

### 関連項目
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
