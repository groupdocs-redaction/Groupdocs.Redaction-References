---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "すべてのアノテーション（すべてに一致）を削除する設定で、DeleteAnnotationRedaction クラスの新しいインスタンスを初期化します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/
is_root: false
weight: 10
---


## __init__

すべてのアノテーション（すべてに一致）を削除する設定で、DeleteAnnotationRedaction クラスの新しいインスタンスを初期化します。

```python
def __init__(self):
    ...
```

### 例

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# すべての注釈を削除
del_red = DeleteAnnotationRedaction()
```

## __init__ {#pattern}

指定された式に一致するアノテーションを削除する設定で、DeleteAnnotationRedaction クラスの新しいインスタンスを初期化します。

```python
def __init__(self, pattern):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| pattern | `str` | 正規表現。 |

### 例

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# 単語 "internal" を含むアノテーションを削除（大文字小文字を区別しない）
del_red = DeleteAnnotationRedaction(r"(?i)internal")
```

## __init__ {#regex}

指定された式に一致するアノテーションを削除する設定で、DeleteAnnotationRedaction クラスの新しいインスタンスを初期化します。

```python
def __init__(self, regex):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | 正規表現。 |

### 例

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# 正規表現と一致する内容の注釈を削除（大文字小文字を区別しない）
del_red = DeleteAnnotationRedaction("(?i)internal")
```

### 関連項目
* class [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/)
