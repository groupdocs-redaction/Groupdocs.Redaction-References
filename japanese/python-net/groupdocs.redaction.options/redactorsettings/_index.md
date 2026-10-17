---
title: "RedactorSettings クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "編集設定を表し、編集プロセスをカスタマイズできるようにします。"
type: docs
url: /ja/python-net/groupdocs.redaction.options/redactorsettings/
is_root: false
weight: 90
---


## RedactorSettings class

編集設定を表し、編集プロセスをカスタマイズできるようにします。

詳細を見る

- More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
- More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

RedactorSettings 型は次のメンバーを公開します：

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/) | RedactorSettings クラスの新しいインスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger) | 指定された ILogger インスタンスを使用して新しい RedactorSettings インスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#callback) | 指定された IRedactionCallback インスタンスを使用して RedactorSettings クラスの新しいインスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#ocr_connector) | 指定された IOcrConnector を使用して新しい RedactorSettings インスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback) | 指定されたロガーとコールバックを使用して新しい RedactorSettings インスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback-ocr_connector) | 指定された ILogger、IRedactionCallback、IOcrConnector のインスタンスを使用して RedactorSettings クラスの新しいインスタンスを初期化します。 |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [logger](/redaction/python-net/groupdocs.redaction.options/redactorsettings/logger/) | イベントとエラーを記録するために使用されるロガーです。[`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/) を実装したクラスのインスタンスである必要があります。 |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.options/redactorsettings/ocr_connector/) | `IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/) を実装した OCR コネクタ インスタンスです。 |
| [redaction_callback](/redaction/python-net/groupdocs.redaction.options/redactorsettings/redaction_callback/) | 各赤字記述を評価するために使用される赤字コールバックです。 |

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
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
