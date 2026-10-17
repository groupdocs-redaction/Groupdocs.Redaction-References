---
title: "레드액션 기본"
linkTitle: "Redaction basics"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "이 문서는 Python 개발자가 문서에 메타데이터, 이미지, 주석 및 텍스트 레드액션을 적용하는 방법을 보여줍니다. PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX 등 다양한 문서 형식을 지원합니다."
type: docs
url: /ko/python-net/guides/redaction-basics/
is_root: false
weight: 40
---


GroupDocs.Redaction은 효과적인 문서 레드액션 기능 세트를 지원합니다. 이를 통해 [text](), [metadata](), [annotations](), [images]()에 대한 레드액션을 적용할 수 있습니다.

PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX 등 다양한 문서 형식을 지원합니다. 전체 지원 형식 목록은 [supported document formats]() 기사에서 확인하십시오.

## Redaction types

GroupDocs.Redaction은 다음 레드액션 유형을 제공합니다:

| 유형 | 설명 | 클래스 |
| --- | --- | --- |
| [Text]() | Replaces or hides with color block a portion of text within document body | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) |
| [Metadata]() | Replace metadata values with empty ones or redacts metadata texts | [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/), [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) |
| [Annotations]() | Deletes annotations from document or redacts its texts | [DeleteAnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/), [AnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) |
| [Images]() | Replaces specific area of an image with a colored box | [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) |
| [Pages]() | Removes specific range of pages (slides, worksheets, etc.) | [RemovePageRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) |

## Apply redaction

문서에 레드랙션을 적용하는 것은 [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) 메서드를 통해 수행됩니다. 결과적으로 각 적용된 레드랙션에 대한 로그 항목을 포함하는 [RedactorChangeLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/) 인스턴스를 받게 됩니다. 해당 항목은 옵션, 작업 상태(아래 참조) 및 적용 가능한 경우 텍스트 설명을 포함하는 [Redacton](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redaction/) 인스턴스에 대한 참조를 포함합니다. 하나 이상의 레드랙션이 실패한 경우, [Status == RedactionStatus.Failed](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/)를 보게 됩니다:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def apply_redaction():
    # 편집 옵션을 지정합니다
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # 레드랙션할 문서를 로드합니다
    with Redactor("./sample.docx") as redactor:
        # 가리기를 적용합니다
        result = redactor.apply(ex_red)

        if result.status != RedactionStatus.FAILED:
            # 편집된 문서를 원본 파일 옆에 저장합니다
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    apply_redaction()
```

`sample.docx`는 이 예제에서 사용된 샘플 파일입니다. 다운로드하려면 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) 를 클릭하십시오.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_redaction/sample_redacted.docx)

[RedactionStatus](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) 열거형의 모든 가능한 상태가 이 표에 나열됩니다:

| 상태 | 설명 | 가능한 이유 |
| --- | --- | --- |
| *적용됨* | 레드랙션이 완전하고 성공적으로 적용되었습니다. | 레드랙션 프로세스 내의 모든 작업이 성공적으로 적용되었습니다. |
| *부분적으로 적용됨* | 레드랙션이 일치 항목의 일부에만 적용되었습니다. | 1) 교체에 대한 체험 제한이 초과되었습니다 2) 최소 하나의 변경이 사용자가 거부했습니다 |
| *건너뛰기* | 레드랙션이 건너뛰어졌습니다 (적용되지 않음). | 1) 레드랙션에 대한 체험 제한이 초과되었습니다 2) 이 유형의 문서에 레드랙션을 적용할 수 없습니다 3) 모든 교체가 사용자가 거부했으며 변경 사항이 없습니다. |
| *실패* | 레드랙션이 예외와 함께 실패했습니다. | 레드랙션 과정에서 예외가 발생했습니다. |

자세한 정보를 보려면 [RedactorChangeLog.RedactionLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/redaction_log/)의 레드랙션 로그 항목을 반복하고 *Applied*가 아닌 상태를 가진 항목의 [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) 속성을 확인해야 합니다:

```python
result = redactor.apply(redaction)
if result.status != RedactionStatus.FAILED:
    # 기본적으로 레드랙션된 문서는 PDF 형식으로 저장됩니다.
    save_options = SaveOptions()
    save_options.add_suffix = True
    save_options.rasterize_to_pdf = True
    save_options.redacted_file_suffix = "redacted"
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}")
else:
    # 실패하거나 건너뛴 모든 레드랙션을 덤프합니다.
    print("Redaction failed!")
    for log_entry in result.redaction_log:
        if log_entry.result.status != RedactionStatus.APPLIED:
            print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")
```

## Apply multiple redactions

[Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) 메서드를 한 번 호출하여 필요한 만큼 많은 레드랙션을 적용할 수 있습니다. 이 메서드의 오버로드는 레드랙션 배열과 레드랙션 정책을 받아들이기 때문입니다. 이 경우 레드랙션은 배열에 나타나는 순서대로 적용됩니다. 코드에서 레드랙션 세트를 지정하는 대신, [here]()에 설명된 대로 레드랙션 정책이 포함된 XML 파일을 만들 수 있습니다.

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    RegexRedaction,
    ReplacementOptions,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def apply_multiple_redactions():
    # 레드액션 상자의 색상 정의
    color = Color.from_argb(255, 220, 20, 60)

    # 적용할 레드랙션 목록을 순서대로 제공하십시오.
    redaction_list = [
        ExactPhraseRedaction("John Doe", ReplacementOptions("[Client]")),
        RegexRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # 레드랙션할 문서를 로드합니다
    with Redactor("./sample.docx") as redactor:
        # 편집 목록 적용
        result = redactor.apply(redaction_list)

        if result.status != RedactionStatus.FAILED:
            # 기본적으로 레드랙션된 문서는 PDF 형식으로 저장됩니다.
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)
        else:
            # 실패하거나 건너뛴 모든 레드랙션을 덤프합니다.
            print("Redaction failed!")
            for log_entry in result.redaction_log:
                if log_entry.result.status != RedactionStatus.APPLIED:
                    print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")

if __name__ == "__main__":
    apply_multiple_redactions()
```

`sample.docx`는 이 예제에서 사용된 샘플 파일입니다. 다운로드하려면 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) 를 클릭하십시오.

  
```text
Binary file (PDF, 1.2 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_multiple_redactions/sample_redacted.pdf)
