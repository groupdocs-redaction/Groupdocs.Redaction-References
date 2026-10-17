---
title: "DeleteAnnotationRedaction 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "주어진 정규식과 일치하는 경우 텍스트를 삭제하고, 선택적으로 모든 주석을 삭제하는 텍스트 레드액션을 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/deleteannotationredaction/
is_root: false
weight: 60
---


## DeleteAnnotationRedaction class

주어진 정규식과 일치하는 경우 텍스트를 삭제하고, 선택적으로 모든 주석을 삭제하는 텍스트 레드액션을 나타냅니다.

자세히 알아보기

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

DeleteAnnotationRedaction 유형은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/) | 모든 주석을 삭제하도록 설정된 DeleteAnnotationRedaction 클래스의 새 인스턴스를 초기화합니다(모두 일치). |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#pattern) | 주어진 표현식과 일치하는 주석을 삭제하는 DeleteAnnotationRedaction 클래스의 새 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#regex) | 주어진 표현식과 일치하는 주석을 삭제하는 DeleteAnnotationRedaction 클래스의 새 인스턴스를 초기화합니다. |

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to/#format_instance) | 주어진 포맷 인스턴스에 Redaction을 적용합니다. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to_document_format_instance/) |  |

### 속성
| 속성 | 설명 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/description/) | 삭제 작업의 설명으로, 삭제 이름과 매개변수를 포함합니다. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/expression/) | 일치시킬 정규식입니다. |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

with Redactor("document.pdf") as redactor:
    # 단어 "internal"이 포함된 주석을 삭제합니다(대소문자 구분 없음).
    redactor.apply(DeleteAnnotationRedaction("(?i)internal"))
    redactor.save()
```

### Guides
`DeleteAnnotationRedaction`를 사용하는 작업 가이드:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### 또 보기
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
