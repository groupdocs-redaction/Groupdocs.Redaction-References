---
title: "RedactorConfiguration 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "내장 및 사용자 정의 형식을 포함한 지원 형식 목록에 대한 액세스를 제공합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.configuration/redactorconfiguration/
is_root: false
weight: 20
---


## RedactorConfiguration class

내장 및 사용자 정의 형식을 포함한 지원 형식 목록에 대한 액세스를 제공합니다.

자세히 보기:

- More details about GroupDocs.Redaction configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

RedactorConfiguration 유형은 다음 멤버를 노출합니다:

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [find_format](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/#file_extension) | 주어진 파일 확장자에 대한 형식 구성을 찾습니다. |
| [find_format_file](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_file/) |  |
| [find_format_string](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_string/) |  |
| [get_instance](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/) | 내장 형식의 기본 구성을 가진 싱글톤 인스턴스를 반환합니다. |

### 속성
| 속성 | 설명 |
| :- | :- |
| [available_formats](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/available_formats/) | 인식된 형식 목록은 [`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/)을 참조하십시오. |

### 예제

```python
# 사용자 정의 형식 핸들러를 추가합니다.
adobe_photoshop_settings = DocumentFormatConfiguration()
adobe_photoshop_settings.extension_filter = ".psd"
adobe_photoshop_settings.document_type = MyAdobePhotoshopFormatInstance

config = RedactorConfiguration.get_instance()
config.available_formats.add(adobe_photoshop_settings)
```

```python
# 내장 또는 사용자 정의 형식 핸들러를 검색합니다.
config = RedactorConfiguration.get_instance()
format_settings = config.find_format(".psd")
```

### 또 보기
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
