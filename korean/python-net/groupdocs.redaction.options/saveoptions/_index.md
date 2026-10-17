---
title: "SaveOptions 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "출력 파일 이름을 변경하거나 문서를 이미지 기반 PDF(래스터화)로 변환하기 위한 옵션을 제공합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.options/saveoptions/
is_root: false
weight: 110
---


## SaveOptions class

출력 파일 이름을 변경하거나 문서를 이미지 기반 PDF(래스터화)로 변환하기 위한 옵션을 제공합니다.

자세히 보기:
- [Save with default options](https://docs.groupdocs.com/redaction/net/save-with-default-options/)
- [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
- [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)
- [Save in original format](https://docs.groupdocs.com/redaction/net/save-in-original-format/)
- [Save overwriting original file](https://docs.groupdocs.com/redaction/net/save-overwriting-original-file/)
- [Save to stream](https://docs.groupdocs.com/redaction/net/save-to-stream/)

SaveOptions 유형은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/) | 기본 설정으로 새 인스턴스를 초기화합니다: rasterize_to_pdf는 False이고 add_suffix는 False입니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/#rasterize_to_pdf-suffix) | 주어진 매개변수로 새 인스턴스를 초기화합니다. |

### 속성
| 속성 | 설명 |
| :- | :- |
| [add_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/add_suffix/) | add_suffix 속성은 저장하기 전에 파일 이름을 변경할지 여부를 나타냅니다. 기본값은 False입니다. |
| [rasterization](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterization/) | 래스터화 설정. |
| [rasterize_to_pdf](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterize_to_pdf/) | 문서의 모든 페이지를 이미지로 변환하고 단일 PDF 파일로 결합할지 여부를 나타내는 플래그. |
| [redacted_file_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/redacted_file_suffix/) | 출력 파일 이름에 대한 사용자 지정 접미사입니다. 지정하지 않으면 [`SaveOptions.SaveSuffix`](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/) 상수가 사용됩니다. |

### 필드
| 필드 | 설명 |
| :- | :- |
| [SAVE_SUFFIX](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/) | 기본 접미사 값인 "Redacted"를 나타냅니다. |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def save_with_default_options():
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    with Redactor("./sample.docx") as redactor:
        redactor.apply(ex_red)

        # 기본 옵션( PDF로 래스터화 및 접미사 추가)으로 문서를 저장합니다.
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"

        result_path = redactor.save(save_options)
        print(f"Document redacted successfully. Check output in {result_path}.")
```

### Guides
`SaveOptions`를 사용하는 작업 가이드:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### 또 보기
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
