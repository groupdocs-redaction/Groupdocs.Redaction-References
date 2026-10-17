---
title: "load メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "XML ファイルから RedactionPolicy をロードします。"
type: docs
url: /ja/python-net/groupdocs.redaction/redactionpolicy/load/
is_root: false
weight: 1010
---


## load {#file_path}

XML ファイルから RedactionPolicy をロードします。

```python
def load(cls, file_path):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| file_path | `str` | XML ファイルへのパスです。 |

**Returns:** RedactionPolicy: The loaded redaction policy.

### 例

```python
from groupdocs.redaction import RedactionPolicy, Redactor

policy = RedactionPolicy.load("RedactionPolicy.xml")

with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

## load {#input}

XML 設定を含むストリームから RedactionPolicy インスタンスをロードします。

```python
def load(cls, input):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| input | `io.RawIOBase` | XML 設定を含むストリームです。 |

**Returns:** RedactionPolicy: The loaded redaction policy.

### 例

```python
from groupdocs.redaction import RedactionPolicy, Redactor

# XML ファイルからポリシーをロードする
with open("policy.xml", "rb") as stream:
    policy = RedactionPolicy.load(stream)

# ポリシーをドキュメントに適用します
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### 関連項目
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
