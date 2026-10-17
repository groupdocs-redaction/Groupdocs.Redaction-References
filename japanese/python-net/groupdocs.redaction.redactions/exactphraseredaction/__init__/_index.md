---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "大文字小文字を区別しないモードで ExactPhraseRedaction の新しいインスタンスを初期化します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#search_phrase-options}

大文字小文字を区別しないモードで ExactPhraseRedaction の新しいインスタンスを初期化します。

```python
def __init__(self, search_phrase, options):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| search_phrase | `str` | 検索および置換する文字列。 |
| options | `ReplacementOptions` | 置換オプション（テキスト、色）。 |

### 例

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# 「John Doe」の出現箇所を（大文字小文字を区別せずに）「[CUSTOMER]」に置き換える
redaction = ExactPhraseRedaction("John Doe", ReplacementOptions("[CUSTOMER]"))
```

## __init__ {#search_phrase-is_case_sensitive-options}

新しい ExactPhraseRedaction インスタンスを初期化します。

```python
def __init__(self, search_phrase, is_case_sensitive, options):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| search_phrase | `str` | 検索および置換する文字列。 |
| is_case_sensitive | `bool` | ケースセンシティブ検索が必要な場合は True。 |
| options | `ReplacementOptions` | 置換オプション（テキスト、色）。 |

### 例

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# 大文字小文字を区別しない正確なフレーズの編集
redaction = ExactPhraseRedaction("John Doe", False, ReplacementOptions("[CUSTOMER]"))

# 大文字小文字を区別する正確なフレーズの編集
redaction_cs = ExactPhraseRedaction("ACME", True, ReplacementOptions("[CO]"))
```

### 関連項目
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/)
