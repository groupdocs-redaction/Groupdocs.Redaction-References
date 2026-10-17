---
title: "RedactionPolicy 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "적용할 특정 삭제 집합을 포함하는 정화 정책을 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction/redactionpolicy/
is_root: false
weight: 120
---


## RedactionPolicy class

적용할 특정 삭제 집합을 포함하는 정화 정책을 나타냅니다.

**Learn more**
- More details about policies: https://docs.groupdocs.com/redaction/net/use-redaction-policies/
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/

RedactionPolicy 타입은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/) | 새 RedactionPolicy 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/#redactions) | 특정 삭제 목록을 사용하여 새 RedactionPolicy를 초기화합니다. |

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#file_path) | XML 파일에서 RedactionPolicy를 로드합니다. |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#input) | XML 구성을 포함하는 스트림에서 RedactionPolicy 인스턴스를 로드합니다. |
| [load_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_file/) |  |
| [load_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_streams/) |  |
| [load_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_string/) |  |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#file_path) | 삭제 정책을 파일에 저장합니다. |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#output) | 삭제 정책을 스트림에 저장합니다. |
| [save_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_file/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_streams/) |  |
| [save_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_string/) |  |

### 속성
| 속성 | 설명 |
| :- | :- |
| [redactions](/redaction/python-net/groupdocs.redaction/redactionpolicy/redactions/) | 완전히 구성된 [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)-파생 클래스 목록입니다. |

### 예제

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

# 메모리 내에서 재사용 가능한 정책을 구축합니다
policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])

# 문서에 정책을 적용합니다
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Guides
`RedactionPolicy`를 사용하는 작업 가이드:

* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### 또 보기
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
