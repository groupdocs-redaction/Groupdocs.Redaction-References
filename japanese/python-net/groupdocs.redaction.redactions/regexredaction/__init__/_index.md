---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "RegexRedaction の新しいインスタンスを初期化します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/regexredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-options}

RegexRedaction の新しいインスタンスを初期化します。

```python
def __init__(self, pattern, options):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| pattern | `str` | 検索と置換に使用する正規表現。 |
| options | `ReplacementOptions` | 置換オプション（テキスト、色）。 |

### 例

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

## __init__ {#regex-options}

新しい RegexRedaction インスタンスを初期化します。

```python
def __init__(self, regex, options):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | 検索と置換に使用する正規表現。 |
| options | `ReplacementOptions` | 置換オプション（テキスト、色）。 |

### 例

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

### 関連項目
* class [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)
