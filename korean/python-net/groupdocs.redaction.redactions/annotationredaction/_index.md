---
title: "AnnotationRedaction 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "주어진 정규식과 일치하는 주석 텍스트(댓글 등)를 교체하는 레드액션을 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/annotationredaction/
is_root: false
weight: 10
---


## AnnotationRedaction class

주어진 정규식과 일치하는 주석 텍스트(댓글 등)를 교체하는 레드액션을 나타냅니다.

자세히 알아보기

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

AnnotationRedaction 유형은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#pattern-replacement) | 정규식 패턴과 교체 텍스트를 사용하여 새로운 AnnotationRedaction을 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#regex-replacement) | 새 인스턴스를 초기화합니다 [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/). |

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to/#format_instance) | 주어진 포맷 인스턴스에 Redaction을 적용합니다. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to_document_format_instance/) |  |

### 속성
| 속성 | 설명 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/description/) | 가리기 설명으로, 가리기와 그 매개변수를 설명합니다. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/expression/) | 일치시킬 정규식입니다. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/replacement/) | 일치하는 텍스트에 대한 텍스트 교체. |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import AnnotationRedaction

with Redactor("document.pdf") as redactor:
    redactor.apply(AnnotationRedaction("(?i)approved", "[REVIEW]"))
    redactor.save()
```

### Guides
`AnnotationRedaction`를 사용하는 작업 가이드:

* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)

### 또 보기
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
