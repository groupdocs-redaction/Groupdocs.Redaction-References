---
title: "com.groupdocs.redaction.options"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "이 패키지는 로드 및 저장 옵션 클래스를 제공합니다."
type: docs
weight: 15
url: /ko/java/com.groupdocs.redaction.options/
---

이 패키지는 로드 및 저장 옵션 클래스를 제공합니다.



## 클래스

| 클래스 | 설명 |
| --- | --- |
| [LoadOptions](../com.groupdocs.redaction.options/loadoptions) | 파일을 열 때 사용되는 옵션을 제공합니다. |
| [PreviewOptions](../com.groupdocs.redaction.options/previewoptions) | 미리보기 생성을 위한 요구 사항 및 스트림 대리자를 설정하는 옵션을 제공합니다. |
| [RasterizationOptions](../com.groupdocs.redaction.options/rasterizationoptions) | 파일을 PDF로 변환하기 위한 옵션을 제공합니다. |
| [RedactorSettings](../com.groupdocs.redaction.options/redactorsettings) | Redaction 설정을 나타내며, Redaction 프로세스를 사용자 정의할 수 있습니다. |
| [SaveOptions](../com.groupdocs.redaction.options/saveoptions) | 출력 파일 이름을 변경하고/또는 문서를 이미지 기반 PDF(래스터화)로 변환하는 옵션을 제공합니다. |
| [WordprocessingSaveOptions](../com.groupdocs.redaction.options/wordprocessingsaveoptions) | 워드 프로세싱 저장 옵션. |

## 인터페이스

| 인터페이스 | 설명 |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.redaction.options/icreatepagestream) | 페이지 미리보기 데이터를 쓰기 위한 스트림을 반환하는 메서드를 제공합니다. |
| [ILogger](../com.groupdocs.redaction.options/ilogger) | Redaction 과정에서 이벤트와 오류를 기록하는 데 사용할 수 있는 로거 인터페이스를 정의합니다. |
| [IReleasePageStream](../com.groupdocs.redaction.options/ireleasepagestream) | CreatePageStream 대리자가 만든 스트림을 해제하는 메서드를 나타냅니다. |

## 열거형

| 열거형 | 설명 |
| --- | --- |
| [AdvancedRasterizationOptions](../com.groupdocs.redaction.options/advancedrasterizationoptions) | 적용될 고급 래스터화 옵션을 관리하는 열거형입니다. |
| [PdfComplianceLevel](../com.groupdocs.redaction.options/pdfcompliancelevel) | 지원되는 PDF 호환성 수준 목록을 나타냅니다. |
| [PreviewFormats](../com.groupdocs.redaction.options/previewformats) | 지원되는 미리보기 형식을 나타냅니다. |
| [WordProcessingComplianceLevel](../com.groupdocs.redaction.options/wordprocessingcompliancelevel) | 워드 프로세싱 문서에 대한 OOXML 호환성 수준. |
