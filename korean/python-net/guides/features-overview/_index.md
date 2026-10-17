---
title: "기능 개요"
linkTitle: "Features overview"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "GroupDocs.Redaction for Python via .NET은 단일 형식 독립 API를 통해 문서에서 텍스트, 메타데이터, 이미지 영역, 주석 및 전체 페이지와 같은 민감한 정보를 제거하고, 결과를 원본 형식이나 정제된 PDF로 저장합니다."
type: docs
url: /ko/python-net/guides/features-overview/
is_root: false
weight: 30
---


GroupDocs.Redaction for Python via .NET은 다양한 [supported document formats]()에서 민감한 정보를 제거하거나 영구적으로 가립니다. 모든 가리기는 동일한 워크플로를 따릅니다: [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)로 문서를 열고, `apply()`로 하나 이상 가리기를 적용한 뒤, `save()`로 정제된 결과를 원본 형식이나 정제된 PDF로 저장합니다. 아래 기능들은 단일 패스에서 자유롭게 결합할 수 있습니다.

## Text redaction

정확한 구문이나 정규식을 사용하여 텍스트를 찾고 교체할 수 있으며, 전체 단어와 이메일 주소, 전화번호, 주민등록번호와 같은 복잡한 패턴을 모두 다룹니다. 일치하는 텍스트는 대체 텍스트로 교체하거나 색상 상자로 가려 원본 내용을 복구할 수 없게 할 수 있습니다. 스프레드시트에서는 검색 범위를 단일 워크시트나 열로 좁힐 수 있습니다. See [Text Redactions]().

## Metadata redaction

문서 메타데이터—작성자, 제목, 회사, 주석 및 이미지의 EXIF 데이터—를 삭제하거나 다시 작성하여 민감한 세부 정보가 문서 속성을 통해 유출되지 않도록 합니다. 모든 메타데이터를 지우거나 특정 필드만 대상 지정하거나 값을 새 값으로 교체할 수 있습니다. See [Metadata Redactions]().

## Image-area redaction

임베드된 이미지나 스캔된 페이지의 사각형 영역을 채워진 상자를 그려 검은색으로 가릴 수 있습니다—서명, 사진, 헤더 또는 푸터와 같이 기밀 데이터가 나타날 수 있는 부분을 숨기는 데 유용합니다. See [Image Redactions]().

## Annotation redaction

주석, 코멘트 및 메모를 다시 작성하거나 삭제합니다. 모든 주석을 제거하거나 정규식을 사용해 민감한 텍스트가 포함된 주석만 매치할 수 있습니다. See [Annotation Redactions]().

## Page removal

PDF 문서의 전체 페이지, 프레젠테이션 슬라이드, 스프레드시트 워크시트를 제거합니다. 시작 페이지와 페이지 수, 그리고 시작점에 대한 방향을 지정합니다. See [Remove Page Redactions]().

## Rasterization to PDF

정리된 문서를 페이지가 래스터 이미지로 렌더링되는 PDF로 저장합니다. 결과 파일에는 검색 가능한 텍스트와 원본 메타데이터가 없으므로 제거된 내용을 복구할 수 없습니다. 제3자에게 문서를 전달하거나 PDF를 요구하는 규정을 준수해야 할 때 래스터화가 적합합니다. 특정 페이지를 선택하고 고급 래스터화 옵션을 통해 PDF/A 호환성을 요청할 수 있습니다. See [Save in Rasterized PDF]() and [Advanced Rasterization Options]().

## Redaction policies

여러 레드액션을 재사용 가능한 정책으로 그룹화하고 많은 문서에 동일한 규칙 집합을 일관되게 적용합니다—게시 전에 표준 필드 집합을 정리하는 반복 작업에 이상적입니다. See [Use Redaction Policies]().

## Loading and saving

로컬 경로나 스트림에서 문서를 로드할 수 있으며, 비밀번호로 보호된 파일도 포함하고, 필요에 따라 레드액션 전에 문서를 사전 래스터화할 수 있습니다. 저장 시 추가 편집을 위해 원본 형식을 유지하거나, 원본 파일을 덮어쓰거나, PDF로 래스터화하거나, 스트림에 쓸 수 있습니다. See [Loading Documents]() and [Saving Documents]().

## On-premise

GroupDocs.Redaction for Python via .NET은 완전히 자체 인프라에서 실행되며—문서가 환경을 떠나지 않습니다. 이 패키지는 모든 필요한 것을 포함하는 자체 포함 휠이며, 따라서 Microsoft Office, OpenOffice, Adobe Acrobat 또는 별도의 런타임을 설치할 필요가 없습니다. See [System Requirements]() for the supported platforms and native dependencies.
