---
title: "save 메서드"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "다음 옵션을 사용하여 문서를 파일에 저장합니다: AddSuffix = True, RasterizeToPDF = True."
type: docs
url: /ko/python-net/groupdocs.redaction/redactor/save/
is_root: false
weight: 1080
---


## save

다음 옵션을 사용하여 문서를 파일에 저장합니다: AddSuffix = True, RasterizeToPDF = True.

```python
def save(self):
    ...
```

**Returns:** str: Path to redacted document.

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("document.docx") as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    options = SaveOptions()
    options.add_suffix = True
    options.rasterize_to_pdf = True
    result_path = redactor.save(options)
    print(f"Saved to {result_path}")
```

## save {#save_options}

문서를 파일에 저장합니다.

```python
def save(self, save_options):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| save_options | `SaveOptions` | 접미사를 추가하거나 래스터화하는 옵션. |

**Returns:** Path to redacted document.

### 예제

```python
from datetime import datetime
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions


def save_in_original_format():
    # 편집 옵션을 지정합니다
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # 레드랙션할 문서를 로드합니다
    with Redactor("./sample.docx") as redactor:
        # 가리기를 적용합니다
        redactor.apply(ex_red)

        # 날짜 접미사를 붙여 원본 형식으로 편집된 문서를 저장합니다.
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = datetime.now().strftime("%Y-%m-%d %H-%M-%S")

        result_path = redactor.save(so)
        print(f"Document redacted successfully.\nCheck output in {result_path}.")


if __name__ == "__main__":
    save_in_original_format()
```

## save {#document-rasterization_options}

사용자 지정 위치를 포함하여 문서를 스트림에 저장합니다.

```python
def save(self, document, rasterization_options):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| document | `io.RawIOBase` | 대상 스트림. |
| rasterization_options | `RasterizationOptions` | 래스터화 여부와 래스터화할 페이지를 지정하는 옵션. |

### 예제

```python
import io
from groupdocs.redaction.options import RasterizationOptions
from groupdocs.redaction import Redactor

with Redactor("document.pptx") as redactor:
    # 첫 번째 슬라이드만 처리하도록 래스터화를 구성합니다.
    ro = RasterizationOptions()
    ro.page_index = 0
    ro.page_count = 1

    stream = io.BytesIO()
    redactor.save(stream, ro)

    # BytesIO 객체에 이제 저장된 문서가 포함됩니다.
    data = stream.getvalue()
```

### 또 보기
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
