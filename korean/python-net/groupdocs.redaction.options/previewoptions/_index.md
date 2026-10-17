---
title: "PreviewOptions 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "미리보기 생성을 위한 요구 사항 및 스트림 대리자를 설정하는 옵션을 제공합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.options/previewoptions/
is_root: false
weight: 70
---


## PreviewOptions class

미리보기 생성을 위한 요구 사항 및 스트림 대리자를 설정하는 옵션을 제공합니다.

이 클래스는 미리보기 형식, 이미지 차원, 페이지 번호를 지정하고 각 생성된 페이지에 대한 스트림을 생성 및 선택적으로 해제하는 대리자를 허용합니다.

PreviewOptions 유형은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream) | 새 PreviewOptions 인스턴스를 초기화합니다. 출력 스트림은 사용 후 닫힙니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream-release_page_stream) | 새 PreviewOptions 인스턴스를 초기화하여 출력 스트림이 클라이언트에 반환되어 이후에 사용할 수 있도록 합니다. |

### 속성
| 속성 | 설명 |
| :- | :- |
| [create_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/create_page_stream/) | 페이지 스트림 생성 대리자. |
| [height](/redaction/python-net/groupdocs.redaction.options/previewoptions/height/) | 페이지 미리보기 높이. |
| [page_numbers](/redaction/python-net/groupdocs.redaction.options/previewoptions/page_numbers/) | 미리보기를 생성할 페이지 번호. |
| [preview_format](/redaction/python-net/groupdocs.redaction.options/previewoptions/preview_format/) | 미리보기 이미지 형식. |
| [release_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/release_page_stream/) | 페이지 미리보기 완료 대리자. |
| [width](/redaction/python-net/groupdocs.redaction.options/previewoptions/width/) | 페이지 미리보기 너비. |

### 예제

```python
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int):
    # 주어진 페이지의 미리보기 이미지를 위한 파일을 생성합니다.
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")  # returns a writable binary stream

preview_options = PreviewOptions(create_page_stream)
preview_options.preview_format = PreviewOptions.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### 또 보기
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
