---
title: "RedactorSettings 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "삭제 프로세스를 사용자 정의할 수 있는 삭제 설정을 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction.options/redactorsettings/
is_root: false
weight: 90
---


## RedactorSettings class

삭제 프로세스를 사용자 정의할 수 있는 삭제 설정을 나타냅니다.

자세히 알아보기

- More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
- More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

RedactorSettings 형식은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/) | RedactorSettings 클래스의 새 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger) | 주어진 ILogger 인스턴스를 사용하여 새 RedactorSettings 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#callback) | 주어진 IRedactionCallback 인스턴스를 사용하여 RedactorSettings 클래스의 새 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#ocr_connector) | 지정된 IOcrConnector를 사용하여 새 RedactorSettings 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback) | 지정된 로거와 콜백을 사용하여 새 RedactorSettings 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback-ocr_connector) | 주어진 ILogger, IRedactionCallback 및 IOcrConnector 인스턴스를 사용하여 RedactorSettings 클래스의 새 인스턴스를 초기화합니다. |

### 속성
| 속성 | 설명 |
| :- | :- |
| [logger](/redaction/python-net/groupdocs.redaction.options/redactorsettings/logger/) | 이 로거는 이벤트와 오류를 기록하는 데 사용됩니다. [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/)을 구현하는 클래스의 인스턴스여야 합니다. |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.options/redactorsettings/ocr_connector/) | [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/)를 구현하는 OCR 커넥터 인스턴스입니다. |
| [redaction_callback](/redaction/python-net/groupdocs.redaction.options/redactorsettings/redaction_callback/) | 각 편집 설명을 평가하는 데 사용되는 편집 콜백입니다. |

### 예제

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

### 또 보기
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
