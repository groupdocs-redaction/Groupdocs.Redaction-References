---
title: "set_license メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "現在のプロセスにライセンスを適用します。"
type: docs
url: /ja/python-net/groupdocs.redaction/license/set_license/
is_root: false
weight: 1010
---


## set_license {#license_source}

現在のプロセスにライセンスを適用します。

```python
def set_license(self, license_source):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| license_source |  | ``.lic`` ファイルへの文字列パスまたはライセンスバイトを生成する読み取り可能なファイルライクオブジェクトのいずれかです。ファイルライク入力は、一時ファイルに書き込まれた後、ブリッジに渡されます。 |

| 例外 | 説明 |
| :- | :- |
| `TypeError` | ``license_source`` が文字列パスでも読み取り可能なファイルライクオブジェクトでもない場合。 |

### 関連項目
* class [`License`](/redaction/python-net/groupdocs.redaction/license/)
