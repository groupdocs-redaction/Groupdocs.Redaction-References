---
title: "주석 편집"
linkTitle: "Annotation redactions"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "이 문서는 PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX 등 다양한 형식의 문서에 대한 주석 편집 구현 방법을 보여줍니다."
type: docs
url: /ko/python-net/guides/annotation-redactions/
is_root: false
weight: 80
---


GroupDocs.Redaction API를 사용하면 PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX 등 다양한 형식의 문서에 주석 편집을 적용할 수 있습니다. 전체 목록은 [지원 문서 형식]() 기사에서 확인하세요.

GroupDocs.Redactions는 주석 텍스트에서 민감한 데이터를 제거하거나 정규식을 사용해 주석을 완전히 제거할 수 있는 유연한 API를 제공합니다.

## Remove annotations (comments etc)

GroupDocs.Redaction을 사용하면 문서에서 모든 또는 특정 댓글 및 기타 주석을 제거할 수 있습니다. 예를 들어, 본문에 \"use\", \"show\", \"describe\"와 같은 텍스트가 포함된 모든 댓글을 제거할 수 있습니다:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

def remove_all_annotations():
    # 패턴에 일치하는 주석을 삭제하도록 편집 옵션을 지정합니다.
    a_red = DeleteAnnotationRedaction("(?im:(use|show|describe))")

    # 레드랙션할 문서를 로드합니다
    with Redactor("./annotated.xlsx") as redactor:
        # 가리기를 적용합니다
        result = redactor.apply(a_red)

        # 편집된 문서를 원본 파일 옆에 저장합니다
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    remove_all_annotations()
```

`annotated.xlsx`는 이 예제에 사용된 샘플 파일입니다. 다운로드하려면 [여기](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx)를 클릭하세요.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/remove_all_annotations/annotated_redacted.xlsx)

인자를 전달하지 않는 생성자를 사용하여 문서 내 모든 주석을 제거할 수 있습니다.

## Redact annotations

전체 또는 특정 주석을 제거하는 대신, 주석 텍스트에서 민감한 데이터를 제거할 수 있습니다. 예를 들어, 해당 문서에서 "John"에 대한 모든 언급을 제거할 수 있습니다, 예시:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import AnnotationRedaction

def redact_annotations():
    # 레드랙션 옵션을 지정하세요: 검색 패턴 및 교체 문자열
    a_red = AnnotationRedaction("(?im:john)", "[redacted]")

    # 레드랙션할 문서를 로드합니다
    with Redactor("./annotated.xlsx") as redactor:
        # 가리기를 적용합니다
        result = redactor.apply(a_red)

        # 편집된 문서를 원본 파일 옆에 저장합니다
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_annotations()
```

`annotated.xlsx`는 이 예제에 사용된 샘플 파일입니다. 다운로드하려면 [여기](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx)를 클릭하세요.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/redact_annotations/annotated_redacted.xlsx)
