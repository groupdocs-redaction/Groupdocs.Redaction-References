---
title: "com.groupdocs.redaction.redactions"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "이 패키지는 다양한 유형의 삭제를 위한 클래스를 제공합니다."
type: docs
weight: 16
url: /ko/java/com.groupdocs.redaction.redactions/
---

이 패키지는 다양한 유형의 삭제를 위한 클래스를 제공합니다.



## 클래스

| 클래스 | 설명 |
| --- | --- |
| [AnnotationRedaction](../com.groupdocs.redaction.redactions/annotationredaction) | 주어진 정규식과 일치하는 주석 텍스트(댓글 등)를 교체하는 Redaction을 나타냅니다. |
| [CellColumnRedaction](../com.groupdocs.redaction.redactions/cellcolumnredaction) | 스프레드시트 문서(CSV, Excel 등)에서 텍스트를 교체하는 텍스트 Redaction을 나타냅니다. |
| [CellFilter](../com.groupdocs.redaction.redactions/cellfilter) | CellColumnRedaction의 범위를 워크시트와 열로 제한하는 옵션을 제공합니다. |
| [CustomRedactionContext](../com.groupdocs.redaction.redactions/customredactioncontext) | [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler)에 대한 입력 데이터를 제공합니다. |
| [CustomRedactionResult](../com.groupdocs.redaction.redactions/customredactionresult) | [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler)에 의해 반환되는 결과를 나타냅니다. |
| [DeleteAnnotationRedaction](../com.groupdocs.redaction.redactions/deleteannotationredaction) | 주어진 정규식과 일치하는 텍스트인 경우 주석을 삭제하는 텍스트 Redaction을 나타냅니다(옵션으로 모든 주석을 삭제할 수 있음). |
| [EraseMetadataRedaction](../com.groupdocs.redaction.redactions/erasemetadataredaction) | 문서에서 모든 메타데이터 또는 특정 MetadataFilters와 일치하는 메타데이터를 지우는 메타데이터 Redaction을 나타냅니다. |
| [ExactPhraseRedaction](../com.groupdocs.redaction.redactions/exactphraseredaction) | 문서 텍스트에서 정확한 구문을 교체하는 텍스트 Redaction을 나타냅니다. 기본적으로 대소문자를 구분하지 않습니다. |
| [ImageAreaRedaction](../com.groupdocs.redaction.redactions/imagearearedaction) | 이미지 문서의 지정된 영역에 색상 사각형을 배치하는 Redaction을 나타냅니다. |
| [MetadataFilters](../com.groupdocs.redaction.redactions/metadatafilters) | 가장 일반적인 문서 메타데이터 유형 목록을 나타냅니다. |
| [MetadataRedaction](../com.groupdocs.redaction.redactions/metadataredaction) | 문서 메타데이터 삭제를 위한 기본 추상 클래스를 나타냅니다. |
| [MetadataSearchRedaction](../com.groupdocs.redaction.redactions/metadatasearchredaction) | 정규식을 사용하여 메타데이터를 검색하고 삭제하며, 키 및/또는 값을 일치시키는 메타데이터 삭제를 나타냅니다. |
| [PageAreaFilter](../com.groupdocs.redaction.redactions/pageareafilter) | 문서 페이지 내에서 삭제를 적용할 영역을 설정하는 삭제 필터를 나타냅니다. |
| [PageAreaRedaction](../com.groupdocs.redaction.redactions/pagearearedaction) | 페이지 영역의 텍스트, 이미지 및 주석에 영향을 주는 복합 텍스트 삭제를 나타냅니다. |
| [PageRangeFilter](../com.groupdocs.redaction.redactions/pagerangefilter) | 문서 내에서 삭제를 적용할 페이지 범위를 설정하는 삭제 필터를 나타냅니다. |
| [RedactionDescription](../com.groupdocs.redaction.redactions/redactiondescription) | 삭제 과정 중 수행된 단일 변경 작업 정보를 나타냅니다. |
| [RedactionFilter](../com.groupdocs.redaction.redactions/redactionfilter) | 문서 내에서 삭제를 적용할 범위를 설정하는 삭제 필터를 나타냅니다. |
| [RedactionType](../com.groupdocs.redaction.redactions/redactiontype) | 삭제의 영향을 받는 문서 데이터 유형을 나타냅니다. |
| [RegexRedaction](../com.groupdocs.redaction.redactions/regexredaction) | 제공된 정규식을 일치시켜 문서의 텍스트를 검색하고 교체하는 텍스트 삭제를 나타냅니다. |
| [RegionReplacementOptions](../com.groupdocs.redaction.redactions/regionreplacementoptions) | 이미지 영역 교체를 위한 색상 및 영역 매개변수를 나타냅니다. |
| [RemovePageRedaction](../com.groupdocs.redaction.redactions/removepageredaction) | 문서에서 페이지(슬라이드, 워크시트 등)를 제거하는 삭제를 나타냅니다. |
| [ReplacementOptions](../com.groupdocs.redaction.redactions/replacementoptions) | 일치된 텍스트 교체 옵션을 나타냅니다. |
| [TextRedaction](../com.groupdocs.redaction.redactions/textredaction) | 문서 텍스트 삭제를 위한 기본 추상 클래스를 나타냅니다. |
| [TextReplacement](../com.groupdocs.redaction.redactions/textreplacement) | 텍스트 교체 정보를 나타냅니다. |

## 인터페이스

| 인터페이스 | 설명 |
| --- | --- |
| [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) | 사용자 정의 삭제 콜백을 정의합니다. |
| [IRedactionCallback](../com.groupdocs.redaction.redactions/iredactioncallback) | 각 삭제 변경에 대한 정보를 수신하고 선택적으로 이를 방지하기 위해 필요한 메서드를 정의합니다. |

## 열거형

| 열거형 | 설명 |
| --- | --- |
| [PageSeekOrigin](../com.groupdocs.redaction.redactions/pageseekorigin) | 문서 내에서 탐색을 위한 기준점을 나타내는 필드를 제공합니다. |
| [RedactionActionType](../com.groupdocs.redaction.redactions/redactionactiontype) | 삭제를 수행하기 위해 취할 수 있는 작업을 나타냅니다. |
| [ReplacementType](../com.groupdocs.redaction.redactions/replacementtype) | 일치된 텍스트에 대한 교체 유형을 나타냅니다. |
