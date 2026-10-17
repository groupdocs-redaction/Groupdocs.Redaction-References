---
title: "ReleasePageStream 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "CreatePageStream 대리자가 만든 스트림을 해제하는 메서드를 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction.options/releasepagestream/
is_root: false
weight: 100
---


## ReleasePageStream class

[`CreatePageStream`](/redaction/python-net/groupdocs.redaction.options/createpagestream/) 대리자가 만든 스트림을 해제하는 메서드를 나타냅니다.

ReleasePageStream 형식은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/releasepagestream/__init__/#object-method) |  |

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [begin_invoke](/redaction/python-net/groupdocs.redaction.options/releasepagestream/begin_invoke/#page_number-page_stream-callback-object) |  |
| [begin_invoke_int32](/redaction/python-net/groupdocs.redaction.options/releasepagestream/begin_invoke_int32/) |  |
| [begin_invoke_stream](/redaction/python-net/groupdocs.redaction.options/releasepagestream/begin_invoke_stream/) |  |
| [begin_invoke_streams](/redaction/python-net/groupdocs.redaction.options/releasepagestream/begin_invoke_streams/) |  |
| [end_invoke](/redaction/python-net/groupdocs.redaction.options/releasepagestream/end_invoke/#result) |  |
| [end_invoke_iasync_result](/redaction/python-net/groupdocs.redaction.options/releasepagestream/end_invoke_iasync_result/) |  |
| [invoke](/redaction/python-net/groupdocs.redaction.options/releasepagestream/invoke/#page_number-page_stream) |  |
| [invoke_int32](/redaction/python-net/groupdocs.redaction.options/releasepagestream/invoke_int32/) |  |
| [invoke_stream](/redaction/python-net/groupdocs.redaction.options/releasepagestream/invoke_stream/) |  |
| [invoke_streams](/redaction/python-net/groupdocs.redaction.options/releasepagestream/invoke_streams/) |  |

### 예제

```python
import os
import io
from GroupDocs.Redaction import Redactor
from GroupDocs.Redaction.Options import PreviewOptions

def create_delegate(page_number: int) -> io.RawIOBase:
    path = os.path.join(r"C:\Temp", f"page_{page_number}.png")
    return open(path, "wb")

def release_delegate(page_number: int, page_stream: io.RawIOBase) -> None:
    # 필요한 경우 스트림을 처리합니다
    page_stream.close()

preview_options = PreviewOptions(create_delegate, release_delegate)
preview_options.preview_format = preview_options.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor(r"C:\Temp\SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### 또 보기
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
