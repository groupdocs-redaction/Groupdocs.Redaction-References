---
title: "MetadataSearchRedaction 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "정규식을 사용하여 메타데이터를 검색하고 키 및/또는 값을 일치시켜 메타데이터를 편집하는 작업을 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/metadatasearchredaction/
is_root: false
weight: 140
---


## MetadataSearchRedaction class

정규식을 사용하여 메타데이터를 검색하고 키 및/또는 값을 일치시켜 메타데이터를 편집하는 작업을 나타냅니다.

- More details about applying redactions: <https://docs.groupdocs.com/redaction/net/redaction-basics/>
- More details about document metadata redactions: <https://docs.groupdocs.com/redaction/net/metadata-redactions/>

MetadataSearchRedaction 형식은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement) | 값을 사용하여 삭제된 항목을 일치시키는 MetadataSearchRedaction 클래스의 새 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement-key_pattern) | 항목 이름과 값을 사용하여 삭제된 항목을 일치시키는 MetadataSearchRedaction의 새 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement) | 값을 사용하여 삭제된 항목을 일치시키는 MetadataSearchRedaction 클래스의 새 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement-key_regex) | 항목 이름과 값을 사용하여 삭제된 항목을 일치시키는 MetadataSearchRedaction의 새 인스턴스를 초기화합니다. |

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | 주어진 형식 인스턴스에 레드액션을 적용합니다. (상속됨: [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (상속됨: [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### 속성
| 속성 | 설명 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/description/) | Redaction의 설명으로, 이름과 매개변수를 포함합니다. |
| [key_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/key_expression/) | 메타데이터 항목의 이름(키)을 일치시키는 정규식입니다. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/replacement/) | 텍스트 교체 값. |
| [value_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/value_expression/) | 메타데이터 항목의 값 텍스트를 일치시키는 정규식입니다. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Author 또는 Company와 같은 모든 메타데이터 또는 특정 메타데이터를 선택하는 데 사용되는 필터입니다. (상속됨: [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # 패턴과 일치하는 모든 메타데이터 값을 삭제합니다.
    redaction = MetadataSearchRedaction("Company Ltd.", "--company--")
    redaction.filter = MetadataFilters.COMPANY
    redactor.apply(redaction)
    redactor.save()
```

### Guides
`MetadataSearchRedaction`를 사용하는 작업 가이드:

* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)

### 또 보기
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
