---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "指定された置換テキストで ReplacementOptions の新しいインスタンスを初期化します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#replacement}

指定された置換テキストで ReplacementOptions の新しいインスタンスを初期化します。

```python
def __init__(self, replacement):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| replacement | `str` | テキスト置換。 |

### 例

```python
from groupdocs.redaction.redactions import ReplacementOptions

# 一致したテキストを "[REDACTED]" に置換します
options = ReplacementOptions("[REDACTED]")
```

## __init__ {#color}

オプションとしてカラー矩形を使用して ReplacementOptions クラスの新しいインスタンスを初期化します。

```python
def __init__(self, color):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| color | `System.Drawing.Color` | 矩形の色です。 |

### 関連項目
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)
