---
title: "Redactor 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "문서 삭제 프로세스를 제어하고 문서를 열고, 삭제하고, 저장할 수 있는 주요 클래스를 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction/redactor/
is_root: false
weight: 150
---


## Redactor class

문서 삭제 프로세스를 제어하고 문서를 열고, 삭제하고, 저장할 수 있는 주요 클래스를 나타냅니다.

자세히 알아보기
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More advanced redaction topics: https://docs.groupdocs.com/redaction/net/advanced-usage/

Redactor 유형은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path) | 파일 경로를 사용하여 새로운 Redactor 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document) | 스트림을 사용하여 새로운 [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options) | 경로를 사용하여 비밀번호로 보호된 문서에 대한 새로운 [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options-settings) | 경로와 설정을 사용하여 비밀번호로 보호된 문서에 대한 새로운 Redactor 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options) | 스트림을 사용하여 비밀번호로 보호된 문서에 대한 새로운 Redactor 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options-settings) | 스트림과 설정을 사용하여 비밀번호로 보호된 문서에 대한 새로운 [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) 인스턴스를 초기화합니다. |

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redaction) | 문서에 가리기 작업을 적용합니다. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redactions) | 문서에 일련의 가리기 작업을 적용합니다. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#policy) | 문서에 가리기 정책을 적용합니다. |
| [apply_redaction](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction/) |  |
| [apply_redaction_policy](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction_policy/) |  |
| [dispose](/redaction/python-net/groupdocs.redaction/redactor/dispose/) | 리소스를 해제합니다. |
| [generate_preview](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#preview_options) | 지정된 이미지 형식으로 특정 페이지의 미리보기 이미지를 생성합니다. |
| [generate_preview_preview_options](/redaction/python-net/groupdocs.redaction/redactor/generate_preview_preview_options/) |  |
| [get_document_info](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/) | 문서의 크기 및 페이지 수와 같은 일반 정보를 검색합니다. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/) | 다음 옵션을 사용하여 문서를 파일에 저장합니다: AddSuffix = True, RasterizeToPDF = True. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#save_options) | 문서를 파일에 저장합니다. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#document-rasterization_options) | 사용자 지정 위치를 포함하여 문서를 스트림에 저장합니다. |
| [save_save_options](/redaction/python-net/groupdocs.redaction/redactor/save_save_options/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactor/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactor/save_streams/) |  |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# 문서를 열고 첫 페이지를 제거합니다
with Redactor("document.pdf") as redactor:
    redactor.apply(RemovePageRedaction(PageSeekOrigin.BEGIN, 0, 1))
    redactor.save()
```

### Guides
`Redactor`를 사용하는 작업 가이드:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [Get file info](/redaction/python-net/guides/get-file-info/)

### 또 보기
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
