---
title: "메타데이터 편집"
linkTitle: "Metadata redactions"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "이 문서는 Python 편집 API를 사용하여 필터 또는 정규식 검색으로 메타데이터를 교체하거나 제거하는 방법을 보여줍니다."
type: docs
url: /ko/python-net/guides/metadata-redactions/
is_root: false
weight: 70
---


GroupDocs.Redaction API를 사용하면 PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX 등 다양한 형식의 문서에 메타데이터 편집을 적용할 수 있습니다. 전체 목록은 [supported document formats]() 문서를 참조하십시오.

GroupDocs.Redactions는 필터 또는 정규식 검색을 사용하여 메타데이터를 교체하거나 제거할 수 있는 유연한 API를 제공합니다.

## Filter metadata

모든 편집의 기본 기능은 [MetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) 기반 클래스로부터 파생되며, 기본 클래스는 *metadata filtering*이며 메타데이터 편집에 필수입니다. 이 클래스는 가장 흔히 사용되는 메타데이터 항목을 포함하는 플래그 열거형 [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/)를 사용합니다. 필터를 *All*로 설정하거나 메타데이터의 조합을 선택할 수 있습니다. 예를 들어, 아래 예시는 필터를 *Author*, *Manager* 및 *NameOfApplication*으로 설정하여 텍스트 편집이나 해당 항목을 제거합니다:

```python
# MetadataRedaction에서 파생된 편집
redaction.filter = MetadataFilters.AUTHOR | MetadataFilters.MANAGER | MetadataFilters.NAME_OF_APPLICATION
```

아래는 [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) 항목의 전체 목록이 포함된 표입니다:

| 필터 | 숫자 값 | 설명 |
| --- | --- | --- |
| *None* | 0 | 빈 필터 설정으로, 메타데이터 항목과 일치하지 않습니다 |
| *Author* | 1 | 문서의 작성자 |
| *카테고리* | 2 | 문서의 카테고리 |
| *댓글* | 4 | 문서 댓글 |
| *회사* | 8 | 작성자의 회사 |
| *ContentStatus* | 16 | 콘텐츠 상태 |
| *CreatedTime* | 32 | 생성 시간 |
| *HyperlinkBase* | 64 | 하이퍼링크 기본 |
| *LastPrinted* | 128 | 마지막 인쇄 날짜 및 시간 |
| *LastSavedBy* | 256 | 사용자에 의해 마지막으로 저장됨 |
| *LastSavedTime* | 1024 | 마지막 저장 날짜 및 시간 |
| *NameOfApplication* | 2048 | 문서가 생성된 애플리케이션 이름 |
| *Manager* | 4096 | 작성자의 관리자 이름 |
| *RevisionNumber* | 8192 | 수정 번호 |
| *Subject* | 16384 | 문서의 주제 |
| *Template* | 32768 | 문서 템플릿 이름 |
| *Title* | 65536 | 문서 제목 |
| *TotalEditingTime* | 131072 | 총 편집 시간 |
| *버전* | 262144 | 문서 버전 |
| *설명* | 524288 | 문서 설명 |
| *키워드* | 1048576 | 문서 키워드 |
| *ContentType* | 2097152 | 콘텐츠 유형 |
| *전체* | 2147483647 | 메타데이터 항목의 모든 유형 |

## Clean metadata

문서의 모든 메타데이터 또는 특정 메타데이터를 빈(공백 또는 최소) 값으로 교체하려면 [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/) 클래스를 사용할 수 있습니다. 아래 예제는 문서의 모든 속성을 비웁니다:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_all_metadata():
    # 모든 메타데이터를 삭제하기 위한 레드랙션 옵션을 지정하세요
    met_red = EraseMetadataRedaction(MetadataFilters.ALL)

    # 레드랙션할 문서를 로드합니다
    with Redactor("./sample.docx") as redactor:
        # 가리기를 적용합니다
        result = redactor.apply(met_red)

        # 편집된 문서를 원본 파일 옆에 저장합니다
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_all_metadata()
```

`sample.docx`는 이 예제에서 사용된 샘플 파일입니다. 다운로드하려면 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx)를 클릭하세요.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/clean_all_metadata/sample_redacted.docx)

주어진 문서 내의 모든 메타데이터를 비우려면 [MetadataFilter.All](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/)을 지정하거나 기본 생성자를 사용할 수 있습니다. Custom - 모든 사용자 정의 메타데이터 항목을 삭제합니다.

## Redact metadata

정규식을 사용하여 문서 메타데이터에서 민감한 데이터를 제거하려면 [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/)을 사용할 수 있습니다. 예를 들어, \"Company Ltd.\"라는 언급을 모두 제거할 수 있습니다:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction

def redact_metadata():
    # 레드랙션 옵션을 지정하세요: 검색 패턴 및 교체 문자열
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # 레드랙션할 문서를 로드합니다
    with Redactor("./sample.docx") as redactor:
        # 가리기를 적용합니다
        result = redactor.apply(met_red)

        # 편집된 문서를 원본 파일 옆에 저장합니다
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata()
```

`sample.docx`는 이 예제에서 사용된 샘플 파일입니다. 다운로드하려면 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx)를 클릭하세요.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata/sample_redacted.docx)

첫 번째 인자는 정규식이고, 두 번째는 교체 문자열입니다. 필터를 설정하여 레드랙션 범위를 지정할 수도 있습니다(예: [MetadataFilter.Company](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/)). - 이렇게 하면 \"Company\" 속성을 제외한 모든 메타데이터 항목에서 정규식 매치가 적용되지 않습니다:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

def redact_metadata_with_filter():
    # 레드랙션 옵션을 지정하세요: 검색 패턴 및 교체 문자열
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # 레드랙션 범위를 Company 메타데이터 항목으로만 제한합니다
    met_red.filter = MetadataFilters.COMPANY

    # 레드랙션할 문서를 로드합니다
    with Redactor("./sample.docx") as redactor:
        # 가리기를 적용합니다
        result = redactor.apply(met_red)

        # 편집된 문서를 원본 파일 옆에 저장합니다
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata_with_filter()
```

`sample.docx`는 이 예제에서 사용된 샘플 파일입니다. 다운로드하려면 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx)를 클릭하세요.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata_with_filter/sample_redacted.docx)

## Metadata redaction status

모든 메타데이터 레드랙션은 각 메타데이터 항목에 개별적으로 적용되며, 메타데이터 항목 레드랙션이 실패하더라도 나머지 항목은 업데이트됩니다. 실패하거나 건너뛴(거부된) 메타데이터 항목 및 그 이유 목록은 [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) 속성의 [RedactorLogEntry.Result](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorlogentry/result/)에서 확인할 수 있습니다.
