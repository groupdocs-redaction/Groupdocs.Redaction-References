---
title: "DocumentFormatInstance 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "문서의 특정 형식을 나타내며, 사용자 정의 문서 유형을 추가하도록 구현될 수 있습니다."
type: docs
url: /ko/python-net/groupdocs.redaction.integration/documentformatinstance/
is_root: false
weight: 10
---


## DocumentFormatInstance class

문서의 특정 형식을 나타내며, 사용자 정의 문서 유형을 추가하도록 구현될 수 있습니다.

자세히 알아보기

- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

DocumentFormatInstance 유형은 다음 멤버를 노출합니다:

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [initialize](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/#config-settings) | 문서 형식 핸들러 인스턴스를 초기화합니다. |
| [initialize_document_format_configuration](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize_document_format_configuration/) |  |
| [is_redaction_accepted](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/#description) | [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) 구현을 확인하고, 지정된 경우 호출합니다. |
| [is_redaction_accepted_redaction_description](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted_redaction_description/) |  |
| [load](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load/#input) | 스트림에서 문서를 로드합니다. |
| [load_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_streams/) |  |
| [perform_binary_check](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/#input) | 주어진 스트림에 이 형식 인스턴스가 지원하는 문서가 포함되어 있는지 확인합니다. |
| [perform_binary_check_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_stream/) |  |
| [perform_binary_check_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_streams/) |  |
| [save](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save/#output) | 문서를 스트림에 저장합니다. |
| [save_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_streams/) |  |

### 속성
| 속성 | 설명 |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/password/) | 암호로 보호된 문서의 비밀번호. |

### 예제

```python
class DummyDocument(DocumentFormatInstance):
    def load(self, output: io.RawIOBase) -> None:
        # 파일 내용을 로드
        pass

    def save(self, output: io.RawIOBase) -> None:
        # 파일에 변경 사항을 저장
        pass
```

```python
class MyCustomHandler(DocumentFormatInstance):
    def __init__(self):
        self.my_property = None

    def initialize(self, config: DocumentFormatConfiguration) -> None:
        super().initialize(config)
        if "MyProperty" in config.initialization_data:
            self.my_property = config.initialization_data["MyProperty"]
```

### 또 보기
* module [`groupdocs.redaction.integration`](/redaction/python-net/groupdocs.redaction.integration/)
