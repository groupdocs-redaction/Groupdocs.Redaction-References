---
title: "RedactionDescription 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "편집 과정 중 수행된 단일 변경 작업 정보를 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/redactiondescription/
is_root: false
weight: 200
---


## RedactionDescription class

편집 과정 중 수행된 단일 변경 작업 정보를 나타냅니다.

자세히 알아보기

- More details about [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/) class and [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: Use redaction callback https://docs.groupdocs.com/redaction/net/use-redaction-callback/

RedactionDescription 유형은 다음 멤버를 제공합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#redaction_type-action_type-original_text) | RedactionDescription 클래스의 새 인스턴스를 교체 정보 없이 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#redaction_type-action_type-original_text-replacement) | RedactionDescription 클래스의 새 인스턴스를 교체 정보와 함께 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#redaction_type-action_type-image_area_replacement-image_details) | 이미지 영역 교체 정보를 사용하여 새 RedactionDescription을 초기화합니다. |

### 속성
| 속성 | 설명 |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/action_type/) | 레드액션 작업: 교체, 정리 또는 삭제. |
| [details](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/details/) | 레드액션 대상 항목에 대한 선택적 상세 정보입니다. |
| [image_area_replacement](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/image_area_replacement/) | 이미지 영역 레드액션에 대한 교체 정보이며, 텍스트 레드액션의 경우 None입니다. |
| [original_text](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/original_text/) | 표현식이 제공된 경우 일치하는 텍스트입니다. |
| [redaction_type](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/redaction_type/) | 문서 데이터 유형 – 텍스트, 메타데이터 또는 주석. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/replacement/) | 교체 정보이며, None일 수 있습니다. |

### 또 보기
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
