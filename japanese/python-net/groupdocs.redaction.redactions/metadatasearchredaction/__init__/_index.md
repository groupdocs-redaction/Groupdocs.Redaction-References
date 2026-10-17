---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "MetadataSearchRedaction クラスの新しいインスタンスを初期化し、値を使用して削除された項目と一致させます。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#value_pattern-replacement}

MetadataSearchRedaction クラスの新しいインスタンスを初期化し、値を使用して削除された項目と一致させます。

```python
def __init__(self, value_pattern, replacement):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| value_pattern | `str` | 検索と置換に使用する正規表現 |
| replacement | `str` | テキスト置換 |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    redactor.apply(MetadataSearchRedaction(".*@acme\\.com", "[EMAIL]"))
    redactor.save()
```

## __init__ {#value_pattern-replacement-key_pattern}

MetadataSearchRedaction の新しいインスタンスを初期化し、項目名と値を使用して削除された項目と一致させます。

```python
def __init__(self, value_pattern, replacement, key_pattern):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| value_pattern | `str` | メタデータ項目の値を検索・置換する正規表現です。 |
| replacement | `str` | テキスト置換。 |
| key_pattern | `str` | メタデータ項目の名前を検索・置換する正規表現です。 |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    # メタデータの値に見つかったメールアドレスをすべて置換
    redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement}

MetadataSearchRedaction クラスの新しいインスタンスを初期化し、値を使用して削除された項目と一致させます。

```python
def __init__(self, value_regex, replacement):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | 検索と置換に使用する正規表現。 |
| replacement | `str` | テキスト置換。 |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

# メタデータ内のメールアドレスをすべて編集
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement-key_regex}

MetadataSearchRedaction の新しいインスタンスを初期化し、項目名と値を使用して削除された項目と一致させます。

```python
def __init__(self, value_regex, replacement, key_regex):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | メタデータ項目の値を検索・置換する正規表現です。 |
| replacement | `str` | テキスト置換。 |
| key_regex | `System.Text.RegularExpressions.Regex` | メタデータ項目の名前を検索・置換する正規表現です。 |

### 例

```python
from groupdocs.redaction.redactions import MetadataSearchRedaction
from groupdocs.redaction import Redactor

# メタデータの値にあるメールアドレスを編集
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

### 関連項目
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/)
