---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "置換情報なしで RedactionDescription クラスの新しいインスタンスを初期化します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/
is_root: false
weight: 10
---


## __init__ {#redaction_type-action_type-original_text}

置換情報なしで RedactionDescription クラスの新しいインスタンスを初期化します。

```python
def __init__(self, redaction_type, action_type, original_text):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| redaction_type | `RedactionType` | 削除対象データの種類です。 |
| action_type | `RedactionActionType` | これらのデータに対して実行されるアクションです。 |
| original_text | `str` | 一致したテキスト、コメント、または注釈本文です。 |

## __init__ {#redaction_type-action_type-original_text-replacement}

置換情報付きで RedactionDescription クラスの新しいインスタンスを初期化します。

```python
def __init__(self, redaction_type, action_type, original_text, replacement):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| redaction_type | `RedactionType` | 削除対象データの種類です。 |
| action_type | `RedactionActionType` | これらのデータに対して実行されるアクションです。 |
| original_text | `str` | 一致したテキスト、コメント、または注釈本文です。 |
| replacement | `TextReplacement` | 置換テキスト、一致したテキスト、および元の文字列内での位置です。 |

## __init__ {#redaction_type-action_type-image_area_replacement-image_details}

画像領域の置換情報を使用して新しい RedactionDescription を初期化します。

```python
def __init__(self, redaction_type, action_type, image_area_replacement, image_details):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| redaction_type | `RedactionType` | 削除対象データの種類です。 |
| action_type | `RedactionActionType` | これらのデータに対して実行されるアクションです。 |
| image_area_replacement | `RegionReplacementOptions` | 画像領域置換情報です。 |
| image_details | `str` | 画像のテキスト説明です。デフォルトでは空文字列です。 |

### 関連項目
* class [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/)
