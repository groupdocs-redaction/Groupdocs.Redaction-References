---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "RedactionDescription 클래스의 새 인스턴스를 교체 정보 없이 초기화합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/
is_root: false
weight: 10
---


## __init__ {#redaction_type-action_type-original_text}

RedactionDescription 클래스의 새 인스턴스를 교체 정보 없이 초기화합니다.

```python
def __init__(self, redaction_type, action_type, original_text):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| redaction_type | `RedactionType` | 삭제되는 데이터 유형. |
| action_type | `RedactionActionType` | 이 데이터에 수행될 작업. |
| original_text | `str` | 일치하는 텍스트, 주석 또는 애노테이션 본문. |

## __init__ {#redaction_type-action_type-original_text-replacement}

RedactionDescription 클래스의 새 인스턴스를 교체 정보와 함께 초기화합니다.

```python
def __init__(self, redaction_type, action_type, original_text, replacement):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| redaction_type | `RedactionType` | 삭제되는 데이터 유형. |
| action_type | `RedactionActionType` | 이 데이터에 수행될 작업. |
| original_text | `str` | 일치하는 텍스트, 주석 또는 애노테이션 본문. |
| replacement | `TextReplacement` | 대체 텍스트, 일치하는 텍스트 및 원본 문자열 내 위치. |

## __init__ {#redaction_type-action_type-image_area_replacement-image_details}

이미지 영역 교체 정보를 사용하여 새 RedactionDescription을 초기화합니다.

```python
def __init__(self, redaction_type, action_type, image_area_replacement, image_details):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| redaction_type | `RedactionType` | 삭제되는 데이터 유형. |
| action_type | `RedactionActionType` | 이 데이터에 수행될 작업. |
| image_area_replacement | `RegionReplacementOptions` | 이미지 영역 교체 정보. |
| image_details | `str` | 이미지 텍스트 설명, 기본값은 빈 문자열입니다. |

### 또 보기
* class [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/)
