---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "すべてのメタデータを消去する EraseMetadataRedaction クラスの新しいインスタンスを初期化します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/
is_root: false
weight: 10
---


## __init__

すべてのメタデータを消去する EraseMetadataRedaction クラスの新しいインスタンスを初期化します。

```python
def __init__(self):
    ...
```

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    redactor.save()
```

## __init__ {#filter}

指定された `MetadataFilters` に一致するメタデータを消去する EraseMetadataRedaction の新しいインスタンスを初期化します。

```python
def __init__(self, filter):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| filter | `MetadataFilters` | 削除するメタデータのフィルタ。 |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # すべてのメタデータを消去する
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # author メタデータフィールドのみを削除する
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### 関連項目
* class [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/)
