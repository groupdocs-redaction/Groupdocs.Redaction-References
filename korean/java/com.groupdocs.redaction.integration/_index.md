---
title: "com.groupdocs.redaction.integration"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "이 패키지는 다양한 형식의 문서를 GroupDocs.Redactions와 통합하는 데 사용되는 인터페이스와 클래스를 제공합니다."
type: docs
weight: 13
url: /ko/java/com.groupdocs.redaction.integration/
---

이 패키지는 다양한 형식의 문서를 GroupDocs.Redactions와 통합하는 데 사용되는 인터페이스와 클래스를 제공합니다.



## 클래스

| 클래스 | 설명 |
| --- | --- |
| [DocumentFormatInstance](../com.groupdocs.redaction.integration/documentformatinstance) | 문서의 특정 형식을 나타냅니다. |
| [MetadataCollection](../com.groupdocs.redaction.integration/metadatacollection) | MetadataItem의 사전을 제목을 키로 나타냅니다. |
| [MetadataItem](../com.groupdocs.redaction.integration/metadataitem) | 모든 지원되는 형식에 공통이며 메타데이터 삭제에 사용되는 메타데이터 항목을 나타냅니다. |
| [RecognizedImage](../com.groupdocs.redaction.integration/recognizedimage) | 이미지에서 인식 과정을 통해 추출된 텍스트를 나타냅니다. |
| [RedactableImage](../com.groupdocs.redaction.integration/redactableimage) | 모든 래스터 이미지 삭제 작업에 대한 파사드를 제공합니다. |
| [TextFragment](../com.groupdocs.redaction.integration/textfragment) | OCR 엔진에 의해 추출된 인식된 텍스트(단어, 기호 등)의 일부를 나타냅니다. |
| [TextLine](../com.groupdocs.redaction.integration/textline) | 이미지에서 OCR 엔진이 추출한 텍스트 라인을 나타냅니다. |

## 인터페이스

| 인터페이스 | 설명 |
| --- | --- |
| [IAnnotatedDocument](../com.groupdocs.redaction.integration/iannotateddocument) | 주석(예: 댓글)에 접근하기 위해 필요한 메서드를 정의합니다. |
| [ICellularFormatInstance](../com.groupdocs.redaction.integration/icellularformatinstance) | 하나 이상의 워크시트를 가진 스프레드시트 형식에 접근하기 위해 필요한 메서드를 정의합니다. |
| [IFixedFormatDocument](../com.groupdocs.redaction.integration/ifixedformatdocument) | PDF 또는 프레젠테이션과 같은 고정 구조 형식에 접근하기 위해 필요한 메서드를 정의합니다. |
| [IImageFormatInstance](../com.groupdocs.redaction.integration/iimageformatinstance) | 래스터 이미지 형식 삭제를 위해 필요한 메서드를 정의합니다. |
| [IMetadataAccess](../com.groupdocs.redaction.integration/imetadataaccess) | 형식이 지원하는 경우 문서 메타데이터에 접근하기 위해 필요한 메서드를 정의합니다. |
| [IMultipleAreaRedactable](../com.groupdocs.redaction.integration/imultiplearearedactable) | 동일한 색상으로 여러 이미지 영역을 한 번에 삭제하기 위해 필요한 메서드를 정의합니다. |
| [IOcrConnector](../com.groupdocs.redaction.integration/iocrconnector) | 이미지 문서 및 포함된 이미지에 텍스트 삭제를 적용하기 위해 필요한 메서드를 정의합니다. |
| [IPaginatedDocument](../com.groupdocs.redaction.integration/ipaginateddocument) | 문서 페이지를 조작하기 위해 필요한 메서드를 정의합니다. |
| [IPreviewable](../com.groupdocs.redaction.integration/ipreviewable) | 문서 미리보기를 생성하기 위한 메서드를 정의합니다. |
| [IRasterizableDocument](../com.groupdocs.redaction.integration/irasterizabledocument) | 문서를 모든 바이너리 형태로 저장하기 위해 필요한 메서드를 정의합니다. |
| [ITextualFormatInstance](../com.groupdocs.redaction.integration/itextualformatinstance) | 텍스트를 포함하는 모든 문서에서 텍스트 데이터를 삭제하기 위해 필요한 메서드를 정의합니다. |
