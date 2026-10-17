---
title: "RasterizationOptions 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "파일을 PDF로 변환하기 위한 옵션을 제공합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.options/rasterizationoptions/
is_root: false
weight: 80
---


## RasterizationOptions class

파일을 PDF로 변환하기 위한 옵션을 제공합니다.

- More details about saving document as a rasterized PDF: https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/
- More details about rasterization options: https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/

RasterizationOptions 형식은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/__init__/) | 새 인스턴스를 초기화합니다. |

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type) | 적용할 고급 래스터화 옵션을 등록합니다. |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type-parameters) | 적용할 고급 래스터화 옵션을 등록합니다. |
| [add_advanced_option_advanced_rasterization_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option_advanced_rasterization_options/) |  |

### 속성
| 속성 | 설명 |
| :- | :- |
| [compliance](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/compliance/) | PDF 준수 수준입니다. |
| [enabled](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/enabled/) | 활성화 플래그는 문서의 모든 페이지가 이미지로 변환되어 단일 PDF 파일에 배치되는지를 나타냅니다. 기본값은 True이며, 래스터화를 방지하려면 False로 설정합니다. |
| [has_advanced_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/has_advanced_options/) | 고급 래스터화 옵션이 설정된 경우 이 표시기는 True입니다. |
| [page_count](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_count/) | PDF로 변환될 페이지 수입니다. |
| [page_index](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_index/) | PDF로 변환할 첫 번째 페이지의 인덱스(0부터 시작)입니다. |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import RasterizationOptions, PdfComplianceLevel

with Redactor("SomePresentation.pptx") as redactor:
    ro = RasterizationOptions()
    ro.page_index = 0          # first slide
    ro.page_count = 1
    ro.compliance = PdfComplianceLevel.PdfA1a
    redactor.save("PresentationFirstSlide.pdf", ro)
```

### 또 보기
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
