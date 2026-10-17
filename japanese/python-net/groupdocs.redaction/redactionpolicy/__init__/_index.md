---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "新しい RedactionPolicy インスタンスを初期化します。"
type: docs
url: /ja/python-net/groupdocs.redaction/redactionpolicy/__init__/
is_root: false
weight: 10
---


## __init__

新しい RedactionPolicy インスタンスを初期化します。

```python
def __init__(self):
    ...
```

### 例

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

## __init__ {#redactions}

特定の削除リストを使用して新しい RedactionPolicy を初期化します。

```python
def __init__(self, redactions):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| redactions | `list[Redaction]` | ポリシー用の redactions 配列。 |

### 例

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

### 関連項目
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
