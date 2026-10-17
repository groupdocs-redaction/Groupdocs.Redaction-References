---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "기본 설정으로 새 인스턴스를 초기화합니다: rasterizetopdf는 False이고 addsuffix는 False입니다."
type: docs
url: /ko/python-net/groupdocs.redaction.options/saveoptions/__init__/
is_root: false
weight: 10
---


## __init__

기본 설정으로 새 인스턴스를 초기화합니다: rasterize_to_pdf는 False이고 add_suffix는 False입니다.

```python
def __init__(self):
    ...
```

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

with Redactor("./sample.docx") as redactor:
    redactor.apply(ex_red)
    save_options = SaveOptions()  # defaults: rasterize_to_pdf=False, add_suffix=False
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}.")
```

## __init__ {#rasterize_to_pdf-suffix}

주어진 매개변수로 새 인스턴스를 초기화합니다.

```python
def __init__(self, rasterize_to_pdf, suffix):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| rasterize_to_pdf | `bool` | 문서의 모든 페이지를 이미지로 변환하여 단일 PDF 파일에 넣어야 하는 경우 True입니다. |
| suffix | `str` | 이 텍스트는 파일 이름 끝에 추가됩니다; 비어 있지 않으면 `add_suffix`를 True로 설정합니다. |

### 예제

```python
from groupdocs.redaction.options import SaveOptions

# 기본 설정으로 저장 옵션을 생성합니다
options = SaveOptions()
options.add_suffix = True
options.rasterize_to_pdf = True
options.redacted_file_suffix = "redacted"
```

### 또 보기
* class [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/)
