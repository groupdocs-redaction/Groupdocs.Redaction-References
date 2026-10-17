---
title: "generate_preview 메서드"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "지정된 이미지 형식으로 특정 페이지의 미리보기 이미지를 생성합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.integration/ipreviewable/generate_preview/
is_root: false
weight: 1010
---


## generate_preview {#preview_options}

지정된 이미지 형식으로 특정 페이지의 미리보기 이미지를 생성합니다.

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

with Redactor("document.pdf") as redactor:
    options = PreviewOptions(
        format=PreviewFormats.PNG,
        start_page=1,
        end_page=5,
        create_page_stream=lambda page: open(f"page_{page}.png", "wb")
    )
    redactor.generate_preview(options)
```

### 또 보기
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
