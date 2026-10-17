---
title: "DocumentFormatConfiguration 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "DocumentFormatInstance에서 파생된 클래스에 대한 유형 참조와 빠른 형식 감지를 위한 지원 파일 확장자 목록을 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction.configuration/documentformatconfiguration/
is_root: false
weight: 10
---


## DocumentFormatConfiguration class

빠른 형식 감지를 위한 지원 파일 확장자 목록과 [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)-파생 클래스에 대한 유형 참조를 나타냅니다.

자세히 알아보기

- More details about **GroupDocs.Redaction** configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

DocumentFormatConfiguration 유형은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/__init__/) | 새로운 DocumentFormatConfiguration 인스턴스를 초기화합니다. |

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [supports_extension](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/#file_extension) | 주어진 파일 확장자를 DocumentType으로 처리할 수 있는지 확인합니다. |
| [supports_extension_file](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_file/) |  |
| [supports_extension_string](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_string/) |  |

### 속성
| 속성 | 설명 |
| :- | :- |
| [document_type](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/document_type/) | [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)를 상속하는 클래스의 유형입니다. |
| [extension_filter](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/extension_filter/) | 쉼표로 구분된 파일 확장자 목록(예: ".pdf"), 대소문자를 구분하지 않습니다. |
| [initialization_data](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/initialization_data/) | [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) 초기화에 필요한 데이터입니다. |

### 예제

```python
from groupdocs.redaction import DocumentFormatConfiguration

# 사용자 지정 형식 구성을 생성합니다
config = DocumentFormatConfiguration()
config.ExtensionFilter = ".psd"
config.DocumentType = MyAdobePhotoshopFormatInstance
```

### 또 보기
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
