---
title: "안녕, 세상!"
linkTitle: "Hello, World!"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "간단한 예제를 만들고 실행하여 GroupDocs.Redaction for Python via .NET을 빠르게 시작하세요."
type: docs
url: /ko/python-net/guides/hello-world/
is_root: false
weight: 20
---


## Introduction
\"Hello, World!\" 예제는 GroupDocs.Redaction for Python via .NET을 탐색할 때 흔히 첫 번째 단계입니다. 이는 개발 환경이 올바르게 설정되었고 라이브러리가 예상대로 작동하는지 확인하는 간단한 테스트 역할을 합니다.

## Overview
GroupDocs.Redaction for Python via .NET을 사용하면 다양한 문서 형식에서 민감한 정보를 검색하고, 편집하며, 제거할 수 있습니다. 다양한 [지원 형식](https://docs.groupdocs.com/redaction/python-net/getting-started/supported-document-formats/)이 있어 여러 사용 사례에 유연하게 적용할 수 있습니다.

## How to redact a document
다음 단계에서는 GroupDocs.Redaction for Python via .NET을 사용하여 문서에서 민감한 정보를 편집하는 방법을 보여줍니다.

1. 필요한 `groupdocs.redaction` 클래스를 가져옵니다.
2. 편집을 설명합니다 (여기서는 색상 상자로 교체할 정확한 구문).
3. 샘플 문서 경로를 사용하여 [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)를 인스턴스화합니다.
4. 편집을 적용합니다.
5. 결과를 저장합니다.

## Complete example
아래 예제는 \"John Doe\" 구문이 나타나는 모든 위치를 반투명 빨간색 상자로 교체하고 편집된 문서를 저장합니다:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def hello_world():
    # \"John Doe\"가 나타나는 모든 위치에 반투명 빨간색 상자를 그립니다.
    options = ReplacementOptions(Color.from_argb(128, 255, 0, 0))
    redaction = ExactPhraseRedaction("John Doe", options)

    # 문서를 로드하고, 편집을 적용한 뒤 결과를 저장합니다.
    with Redactor("./sample.docx") as redactor:
        redactor.apply(redaction)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Document redacted successfully. Output saved to {result_path}.")

if __name__ == "__main__":
    hello_world()
```

`sample.docx`는 이 예제에 사용된 샘플 파일입니다. 다운로드하려면 [여기](https://docs.groupdocs.com/redaction/python-net/_sample_files/getting-started/hello-world/sample.docx)를 클릭하세요.

  
```text
Binary file (PDF, 1.0 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/getting-started/hello-world/hello_world/sample_redacted.pdf)

이 예제는 결과를 `sample_redacted.pdf`라는 PDF로 래스터화하므로 편집된 내용을 복구할 수 없습니다 (`save()`는 기본적으로 PDF로 래스터화합니다; `redacted_file_suffix` 옵션은 출력 이름만 제어합니다). 원본 형식을 유지하려면 `rasterize_to_pdf = False`로 설정하세요.

## Additional resources
이 데모는 GroupDocs.Redaction for Python via .NET [코드 샘플](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET/)을 참조합니다.
