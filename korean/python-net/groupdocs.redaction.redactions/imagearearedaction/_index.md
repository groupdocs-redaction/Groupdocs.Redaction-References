---
title: "ImageAreaRedaction 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "이미지 문서의 지정된 영역에 색상 사각형을 배치하는 편집을 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/imagearearedaction/
is_root: false
weight: 110
---


## ImageAreaRedaction class

이미지 문서의 지정된 영역에 색상 사각형을 배치하는 편집을 나타냅니다.

자세히 보기:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

ImageAreaRedaction 형식은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/#top_left-options) | 특정 사각형 영역을 가리기 위한 새 ImageAreaRedaction을 초기화합니다. |

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to/#format_instance) | 주어진 포맷 인스턴스에 Redaction을 적용합니다. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to_document_format_instance/) |  |

### 속성
| 속성 | 설명 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/description/) | Redaction의 설명으로, 이름과 매개변수를 포함합니다. |
| [options](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/options/) | 색상 및 영역 매개변수가 포함된 RegionReplacementOptions 옵션입니다. |
| [top_left](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/top_left/) | 제거할 영역의 왼쪽 위 위치입니다. |

### 예제

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

point = Point(516, 311)
size = Size(170, 35)
color = Color.from_argb(255, 0, 0, 255)  # blue
options = RegionReplacementOptions(color, size)
redaction = ImageAreaRedaction(point, options)

with Redactor("D:\\test.jpg") as redactor:
    result = redactor.apply(redaction)
    if result.status != RedactionStatus.FAILED:
        redactor.save()
```

### Guides
`ImageAreaRedaction`을 사용하는 작업 가이드:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### 또 보기
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
