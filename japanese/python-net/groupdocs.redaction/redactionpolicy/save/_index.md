---
title: "save メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "削除ポリシーをファイルに保存します。"
type: docs
url: /ja/python-net/groupdocs.redaction/redactionpolicy/save/
is_root: false
weight: 1060
---


## save {#file_path}

削除ポリシーをファイルに保存します。

```python
def save(self, file_path):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| file_path | `str` | ファイルへのパス。 |

### 例

```python
    policy = RedactionPolicy([
        ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
        RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
    ])
    policy.save("./sample_policy.xml")
    ```

## save {#output}

削除ポリシーをストリームに保存します。

```python
def save(self, output):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| output | `io.RawIOBase` | ポリシーを保存する対象ストリーム。 |

**Returns:** None.

### 関連項目
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
