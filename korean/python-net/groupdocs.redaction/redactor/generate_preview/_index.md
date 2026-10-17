---
title: "generate_preview 메서드"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "지정된 이미지 형식으로 특정 페이지의 미리보기 이미지를 생성합니다."
type: docs
url: /ko/python-net/groupdocs.redaction/redactor/generate_preview/
is_root: false
weight: 1050
---


## generate_preview {#preview_options}

지정된 이미지 형식으로 특정 페이지의 미리보기 이미지를 생성합니다.

`preview_options`에 정의된 설정에 따라 미리보기가 생성됩니다. 여기에는 이미지 형식, 차원, 페이지 범위 및 페이지 스트림을 생성하고 해제하는 콜백이 포함됩니다.

```python
def generate_preview(self, preview_options):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| preview_options | `PreviewOptions` | 이미지 속성 및 페이지 범위 설정. |

### 예제

```python
from groupdocs.redaction import Redactor, PreviewOptions, PreviewFormats

def create_page_stream(page_number):
    # 지정된 페이지의 미리보기 이미지에 대한 쓰기 가능한 파일 스트림을 반환합니다.
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")

def release_page_stream(page_number, page_stream):
    # 미리보기 이미지가 기록된 후에 호출됩니다.
    page_stream.close()

preview_options = PreviewOptions(
    create_page_stream=create_page_stream,
    release_page_stream=release_page_stream,
)
preview_options.preview_format = PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### 또 보기
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
