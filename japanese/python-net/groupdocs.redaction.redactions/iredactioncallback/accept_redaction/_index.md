---
title: "accept_redaction メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "ドキュメントに対して削除を適用する直前にトリガーされ、ロギングや削除の禁止が可能です。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/
is_root: false
weight: 1010
---


## accept_redaction {#description}

ドキュメントに対して削除を適用する直前にトリガーされ、ロギングや削除の禁止が可能です。

```python
def accept_redaction(self, description):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| description | `RedactionDescription` | 特定のマッチタイプ、基準、テキスト、位置に関する情報を含みます。 |

**Returns:** bool: True to accept the redaction, False to decline it.

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.redaction.options import LoadOptions, RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

with Redactor("document.docx", LoadOptions(), RedactorSettings(callback=accept)) as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    redactor.save()
```

### 関連項目
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/)
