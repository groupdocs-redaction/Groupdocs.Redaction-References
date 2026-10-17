---
title: "groupdocs.redaction.redactions"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "groupdocs.redaction.redactions 아래의 유형들."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/
is_root: false
weight: 60
---


`groupdocs.redaction.redactions` 아래의 유형들.

### 클래스
| 클래스 | 설명 |
| :- | :- |
| [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) | 주어진 정규식과 일치하는 주석 텍스트(댓글 등)를 교체하는 레드액션을 나타냅니다. |
| [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/) | 스프레드시트 문서(CSV, Excel 등)에서 텍스트를 교체하는 텍스트 레드액션을 나타냅니다. |
| [`CellFilter`](/redaction/python-net/groupdocs.redaction.redactions/cellfilter/) | 워크시트와 열에 대한 범위를 제한하는 옵션을 [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/)에 제공합니다. |
| [`CustomRedactionContext`](/redaction/python-net/groupdocs.redaction.redactions/customredactioncontext/) | 맞춤 레드액션 처리를 위한 컨텍스트를 제공합니다. |
| [`CustomRedactionResult`](/redaction/python-net/groupdocs.redaction.redactions/customredactionresult/) | 맞춤 레드액션 작업의 결과를 나타냅니다. |
| [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/) | 주어진 정규식과 일치하는 경우 텍스트를 삭제하고, 선택적으로 모든 주석을 삭제하는 텍스트 레드액션을 나타냅니다. |
| [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/) | 문서에서 모든 메타데이터 또는 특정 MetadataFilters와 일치하는 메타데이터를 지우는 메타데이터 레드액션을 나타냅니다. |
| [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/) | 문서 텍스트에서 정확한 구문을 기본적으로 대소문자를 구분하지 않고 교체하는 텍스트 레드액션을 나타냅니다. |
| [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/) | 맞춤 레드액션 로직을 구현하기 위한 인터페이스를 제공합니다. |
| [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) | 각 편집 변경에 대한 정보를 수신하고 필요에 따라 방지하기 위해 필요한 메서드를 정의합니다. |
| [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) | 이미지 문서의 지정된 영역에 색상 사각형을 배치하는 편집을 나타냅니다. |
| [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) | 문서 메타데이터 편집을 위한 기본 추상 클래스를 나타냅니다. |
| [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) | 정규식을 사용하여 메타데이터를 검색하고 키 및/또는 값을 일치시켜 메타데이터를 편집하는 작업을 나타냅니다. |
| [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/) | 문서 페이지 내에서 편집을 적용할 영역을 설정하는 편집 필터를 나타냅니다. |
| [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/) | 페이지 영역의 텍스트, 이미지 및 주석에 영향을 주는 복합 텍스트 편집을 나타냅니다. |
| [`PageRangeFilter`](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/) | 문서 내 페이지 범위를 설정하여 편집을 적용하는 편집 필터를 나타냅니다. |
| [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/) | 편집 과정 중 수행된 단일 변경 작업 정보를 나타냅니다. |
| [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | 제공된 정규식을 일치시켜 문서의 텍스트를 검색하고 교체하는 텍스트 편집을 나타냅니다. |
| [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/) | 이미지 영역 교체를 위한 색상 및 영역 매개변수를 나타냅니다. |
| [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) | 문서에서 페이지(슬라이드, 워크시트 등)를 제거하는 편집을 나타냅니다. |
| [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) | 일치된 텍스트 교체 옵션을 나타냅니다. |
| [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) | 문서 텍스트 편집을 위한 기본 추상 클래스를 나타냅니다. |
| [`TextReplacement`](/redaction/python-net/groupdocs.redaction.redactions/textreplacement/) | 텍스트 교체 정보를 나타냅니다. |

### 열거형
| 열거형 | 설명 |
| :- | :- |
| [`MetadataFilters`](/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) |  |
| [`PageSeekOrigin`](/redaction/python-net/groupdocs.redaction.redactions/pageseekorigin/) |  |
| [`RedactionActionType`](/redaction/python-net/groupdocs.redaction.redactions/redactionactiontype/) |  |
| [`RedactionFilter`](/redaction/python-net/groupdocs.redaction.redactions/redactionfilter/) | 문서 내부 범위를 설정하여 편집을 적용하는 편집 필터를 나타냅니다. |
| [`RedactionType`](/redaction/python-net/groupdocs.redaction.redactions/redactiontype/) |  |
| [`ReplacementType`](/redaction/python-net/groupdocs.redaction.redactions/replacementtype/) |  |
