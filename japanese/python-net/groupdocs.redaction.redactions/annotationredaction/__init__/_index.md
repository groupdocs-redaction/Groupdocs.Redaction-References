---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "正規表現パターンと置換テキストを使用して新しい AnnotationRedaction を初期化します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-replacement}

正規表現パターンと置換テキストを使用して新しい AnnotationRedaction を初期化します。

```python
def __init__(self, pattern, replacement):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| pattern | `str` | 一致させる正規表現。 |
| replacement | `str` | 一致したテキストの文字列置換。 |

### 例

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# 注釈テキスト内の "approved" という単語をマスクする
redaction = AnnotationRedaction(r"(?i)approved", "[REVIEW]")
```

## __init__ {#regex-replacement}

[`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) の新しいインスタンスを初期化します。

```python
def __init__(self, regex, replacement):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | 一致させる正規表現。 |
| replacement | `str` | 一致したテキストの文字列置換。 |

### 例

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# 単語 "approved" を（大文字小文字を区別せずに）マスクし、"[REVIEW]" に置き換える
redaction = AnnotationRedaction("(?i)approved", "[REVIEW]")
```

### 関連項目
* class [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/)
