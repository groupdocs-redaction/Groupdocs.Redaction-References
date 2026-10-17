---
title: "EraseMetadataRedaction 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "문서에서 모든 메타데이터 또는 특정 MetadataFilters와 일치하는 메타데이터를 지우는 메타데이터 레드액션을 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/erasemetadataredaction/
is_root: false
weight: 70
---


## EraseMetadataRedaction class

문서에서 모든 메타데이터 또는 특정 MetadataFilters와 일치하는 메타데이터를 지우는 메타데이터 레드액션을 나타냅니다.

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document metadata redactions: https://docs.groupdocs.com/redaction/net/metadata-redactions/

EraseMetadataRedaction 형식은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/) | EraseMetadataRedaction 클래스의 새 인스턴스를 초기화하여 모든 메타데이터를 삭제합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/#filter) | EraseMetadataRedaction의 새 인스턴스를 초기화하고, 지정된 `MetadataFilters`와 일치하는 메타데이터를 지웁니다. |

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | 주어진 형식 인스턴스에 레드액션을 적용합니다. (상속됨: [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (상속됨: [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### 속성
| 속성 | 설명 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/description/) | 레드액션 및 해당 매개변수에 대한 설명입니다. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Author 또는 Company와 같은 모든 메타데이터 또는 특정 메타데이터를 선택하는 데 사용되는 필터입니다. (상속됨: [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # 모든 메타데이터 지우기
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # 작성자 필드만 지우기
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Guides
`EraseMetadataRedaction`를 사용하는 작업 가이드:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### 또 보기
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
